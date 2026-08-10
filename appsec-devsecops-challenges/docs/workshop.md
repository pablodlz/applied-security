# Workshop & Talks

This material is not only a personal lab — it was prepared as teaching content and delivered to
audiences.

## Where it was shared

- **Presentation at IFPR** (Instituto Federal do Paraná) — presented the AppSec / DevSecOps approach
  and the progressive challenges.
- **Mini-course at FATEC Ourinhos** — delivered a hands-on mini-course walking students through the
  same practices: threat modeling, SAST/SCA/IaC automation in CI/CD, DAST, and the exploitation chain.

## Why teach it

The challenges were designed to be **progressive** (basic → intermediate → advanced) precisely so
they work as a learning path:

- Start with **why security belongs at design time** (threat modeling, Secure SDLC).
- Show that **automation is accessible** — a useful SAST gate is a short YAML file away.
- Build up to **broader coverage** (SCA, IaC) and **dynamic validation** (DAST).
- End with a **real exploitation chain**, so the audience sees the consequence of skipping the
  earlier controls.

Teaching the material end-to-end — and having to answer questions on it — is also what turned a set
of tool demos into a coherent story about **Shift Left** and **Security by Design**.

## Reusing this as a workshop

Anyone can re-run the path: each challenge in [`../README.md`](../README.md) is self-contained and
targets the public **OWASP Juice Shop**, so a session needs only Docker, Node.js and the tools
listed per challenge. The [SAST pipeline example](../examples/github-actions-security.yml) gives
attendees a working artefact to take home.
