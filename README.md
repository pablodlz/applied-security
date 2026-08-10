# applied-security

Hands-on, applied security work by **Pablo Galerani** ([pablodlz](https://github.com/pablodlz)) —
the practical counterpart to my [`research`](https://github.com/pablodlz/research) (academic papers).

This repository collects **things I built and broke**, across both sides of the discipline:
offensive (penetration testing) and defensive (Application Security / DevSecOps). Each project is
self-contained, with its own README, methodology and documentation.

## Projects

### 🔴 Offensive Security

| Project | What it is |
| --- | --- |
| [**internal-network-pentest**](internal-network-pentest/) | A full internal-network pentest — one exposed service → privileged access on **5 hosts** (Linux + Windows), with network pivoting, RCE, Pass-the-Hash and a cracked KeePass vault. Postgraduate capstone; 13 findings. |
| [**full-chain-web-pentest**](full-chain-web-pentest/) | A complete penetration test — recon → RCE → root — against a deliberately vulnerable web app and its Linux host. 18 findings, kill-chain diagram, remediation guide. |

### 🔵 AppSec / DevSecOps

| Project | What it is |
| --- | --- |
| [**appsec-devsecops-challenges**](appsec-devsecops-challenges/) | An AppSec/DevSecOps journey in progressive challenges (threat modeling, SAST/SCA/IaC/DAST, exploitation) on OWASP Juice Shop. Presented at IFPR and taught at FATEC Ourinhos. |

*More hands-on projects (pentests, CTFs, AppSec labs) will be added here over time.*

## How this repo is organised

```text
applied-security/
├── README.md                       # this index
├── LICENSE                         # CC BY 4.0 (prose) + MIT (code snippets)
├── SECURITY.md
├── full-chain-web-pentest/         # offensive engagement report
└── appsec-devsecops-challenges/    # AppSec / DevSecOps challenges
```

Each project reads on its own. Shared licence and security policy live here at the root. Local-only
publication drafts (`social/`) are git-ignored.

## A note on scope

Everything here targets **deliberately vulnerable, authorised practice environments** (lab VMs, OWASP
Juice Shop). The techniques are documented for learning and defence. Use them only against systems
you own or are explicitly authorised to test — a permissive licence is not authorisation.

## License

Written content: **CC BY 4.0**. Code/pipeline snippets: **MIT**. See [LICENSE](LICENSE).

---

*Maintained by [pablodlz](https://github.com/pablodlz) · [portfolio](https://pablodlz.github.io/portfolio/)*
