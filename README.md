<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=00B2DF&height=150&section=header&text=applied-security&fontColor=ffffff&fontSize=38&desc=Hands-on%20offensive%20%26%20AppSec%2FDevSecOps%20work&descSize=15&descAlignY=72" width="100%" alt="applied-security" />

![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-00B2DF?style=flat-square)
![Offensive](https://img.shields.io/badge/-Offensive%20Security-d64545?style=flat-square&logo=hackthebox&logoColor=white)
![AppSec](https://img.shields.io/badge/-AppSec%20%2F%20DevSecOps-2b6cb0?style=flat-square&logo=owasp&logoColor=white)
![Projects](https://img.shields.io/badge/projects-3-47A141?style=flat-square)

**Things I built and broke.** The practical counterpart to my
[`research`](https://github.com/pablodlz/research) — hands-on work across both sides of the
discipline: offensive (penetration testing) and defensive (Application Security / DevSecOps).

</div>

---

## 🔴 Offensive Security

<table>
<tr>
<td width="50%" valign="top">

### [🌐→🖥️ internal-network-pentest](internal-network-pentest/)

One exposed service → privileged access on **5 hosts** (Linux + Windows). Network pivoting,
RCE, Pass-the-Hash, and a cracked KeePass vault. **Postgraduate capstone · 13 findings.**

![Hosts](https://img.shields.io/badge/hosts-5%2F5-d64545?style=flat-square)
![Findings](https://img.shields.io/badge/findings-13-orange?style=flat-square)

</td>
<td width="50%" valign="top">

### [🕸️ full-chain-web-pentest](full-chain-web-pentest/)

A complete pentest — **recon → RCE → root** — against a vulnerable web app and its host.
Kill-chain diagram and a remediation guide. **18 findings.**

![Chain](https://img.shields.io/badge/chain-recon%E2%86%92root-d64545?style=flat-square)
![Findings](https://img.shields.io/badge/findings-18-orange?style=flat-square)

</td>
</tr>
</table>

## 🔵 AppSec / DevSecOps

<table>
<tr>
<td width="50%" valign="top">

### [🛡️ appsec-devsecops-challenges](appsec-devsecops-challenges/)

An AppSec/DevSecOps journey in progressive challenges — threat modeling, SAST/SCA/IaC/DAST,
exploitation — on OWASP Juice Shop. **Presented at IFPR & taught at FATEC Ourinhos.**

![Shift Left](https://img.shields.io/badge/-Shift%20Left-2b6cb0?style=flat-square)
![Tools](https://img.shields.io/badge/tools-Horusec%20·%20ZAP%20·%20Snyk-2b6cb0?style=flat-square)

</td>
<td width="50%" valign="top">

<br/>

> *More hands-on projects (pentests, CTFs, AppSec labs) will be added here over time.*

</td>
</tr>
</table>

---

## 🗂️ Repository layout

```text
applied-security/
├── README.md · LICENSE · SECURITY.md
├── internal-network-pentest/       # 5-host capstone (offensive)
├── full-chain-web-pentest/         # web engagement report (offensive)
└── appsec-devsecops-challenges/    # AppSec / DevSecOps challenges
```

Each project reads on its own; shared licence and security policy live at the root. Local-only
publication drafts (`social/`) are git-ignored.

## ⚠️ Scope

Everything here targets **deliberately vulnerable, authorised practice environments** (lab VMs,
OWASP Juice Shop). Use the techniques only against systems you own or are authorised to test —
a permissive licence is not authorisation.

---

<div align="center">

**License:** written content **CC BY 4.0**, snippets **MIT** — see [LICENSE](LICENSE).

Maintained by [pablodlz](https://github.com/pablodlz) · [portfolio](https://pablodlz.github.io/portfolio/)

<img src="https://capsule-render.vercel.app/api?type=waving&color=00B2DF&height=90&section=footer" width="100%" alt="" />

</div>
