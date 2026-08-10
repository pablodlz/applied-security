# Security

This repository documents **hands-on security practice** — offensive penetration testing and
AppSec/DevSecOps work — performed against **deliberately vulnerable, authorised practice
environments** (lab VMs and OWASP Juice Shop). It is educational material, not an attack toolkit.

## Design commitments

- **No real targets.** Every engagement here uses a disposable lab VM (RFC1918 host-only network)
  or a public, intentionally-vulnerable app. Clients are fictitious.
- **No raw evidence / screenshots committed.** Findings are reconstructed as prose (see
  `.gitignore`), so nothing sensitive is redistributed.
- **No secrets.** No credentials, tokens or keys are stored here. Pipeline examples reference
  secrets via environment variables / CI secrets, never hardcoded.

## Reporting a problem

Found something that should be redacted, or a factual error? Email **pablogalerani@gmail.com**
rather than opening a public issue, and I will take the content down first and discuss afterwards.

## Scope

Everything here describes **authorised** testing in controlled labs or on public practice apps. Use
the techniques only against systems you own or are explicitly authorised to test. A permissive
licence is not authorisation.
