# Challenge 2 — SAST Automation in CI/CD *(Basic)*

The goal: put **basic security into an automated pipeline** with minimal cost and complexity —
the entry point to DevSecOps. Static Application Security Testing (SAST) runs on every push and
pull request, so code is scanned before it ever merges.

**Tools:** GitHub · GitHub Actions · OWASP Juice Shop (target) · **Horusec** (SAST) · Docker · JSON reports.

## Steps

1. **Prepare the environment** — install Docker and Node.js.
2. **Clone the vulnerable project** — OWASP Juice Shop.
3. **Run it locally** — `npm install` then `npm start`.
4. **Access the app** — `http://localhost:3000`.
5. **Configure the CI/CD pipeline** — add a workflow at `.github/workflows/security.yml` that runs
   Horusec. (Ready-to-adapt file: [`../examples/github-actions-security.yml`](../examples/github-actions-security.yml).)

Now every push and pull request triggers an automatic SAST scan.

## Example result

Horusec flagged **hardcoded credentials** (`admin:admin123`) in `b2bOrder.spec.ts`.

- **Severity:** Critical (per Horusec) — high risk even in test code, because it exposes sensitive data.
- **Risk:** attackers could reuse those credentials to compromise systems, especially if the code is
  versioned publicly.
- **Fix / mitigation:**
  - Remove credentials from code.
  - Use environment variables or a secrets vault.
  - Apply least privilege.
  - Monitor and review for leaks with automated tooling.

## Why it matters

Catching a secret at commit time — before it reaches a shared branch — is the cheapest possible
place to fix it. That is the whole point of Shift Left: move the check as early as it will go.
