# Challenge 3 — SAST + SCA + IaC in CI/CD *(Intermediate)*

A more complete security pipeline that covers **source code, dependencies and infrastructure**,
in a more customisable, corporate-style setup. This is where DevSecOps coverage broadens beyond
"just SAST".

**Tools:** GitHub · **Jenkins** (CI/CD) · OWASP Juice Shop (target) · **Snyk** (SAST + SCA + IaC) ·
Docker · **NGROK** (localhost tunnelling) · Snyk reports.

## What each layer adds

- **SAST** — analyses the application's own source code for insecure patterns.
- **SCA** — Software Composition Analysis: finds known-vulnerable third-party dependencies (a huge
  share of real risk lives in libraries you didn't write).
- **IaC** — scans infrastructure-as-code definitions for insecure configuration before deploy.

## Steps

1. **Prepare the environment** — Docker, Node.js, JDK 17, Jenkins, Snyk, NGROK.
2. **Configure Jenkins** — install the required plugins.
3. **Create a pipeline** — a `Jenkinsfile` describing the build + security stages.
4. **Configure Snyk** — wire the Snyk tool and credentials into Jenkins (token via Jenkins
   Credentials, never hardcoded).
5. **Automate with a webhook** — trigger the pipeline on push; NGROK exposes the local Jenkins so
   the webhook can reach it.

After a push, Snyk produces detailed results with a **"how to fix"** for each issue.

## Why Jenkins here

Jenkins running locally / on your own infrastructure makes it straightforward to reach services on
`localhost` and to integrate tools like Snyk and (in the next challenge) a DAST scanner — something
that is more awkward when the runner is an external, isolated VM. This is the trade-off that pushes
teams toward self-hosted CI for certain security stages.
