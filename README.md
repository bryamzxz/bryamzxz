# Bryam Vargas — `@bryamzxz`

Independent security researcher based in Bogotá, Colombia.
Source-level vulnerability research in PHP web applications, Linux kernel drivers, and FOSS infrastructure.

---

## Current work

Active vulnerability research projects in coordinated disclosure with upstream maintainers and MITRE. Findings will be made public as their disclosure timelines complete.

---

## Open source

- **Linux kernel — `mt76` / MT7921U wireless subsystem.** Active interest in driver-level recovery and power management. Earlier submissions to `linux-wireless` are being revisited and refined.
- **`pop-os/cosmic-comp`** (Wayland compositor, Rust) — identified tiling geometry bug triggered by fullscreen requests from tiled windows. Root cause traced to `update_positions()` in `tiling/mod.rs` after ruling out PR #2099 as a fix. Filed as [issue #2146](https://github.com/pop-os/cosmic-comp/issues/2146).

---

## Methodology

Source-first: read the codebase, trace data flows, reproduce in isolated lab, document. All vulnerability identification is human-driven. AI assistance is limited to documentation drafting and is disclosed when used. Per-finding audit trails (grep histories, taintability notes, lab reproduction logs) available on request.

Disclosure follows coordinated standards: vendor-first contact, 90-day default timeline, CERT/CC escalation when needed, MITRE Primary assignment when the CNA chain fails. Comfortable navigating adversarial coordination — see Dolibarr 2026 case for a documented MITRE Primary override after vendor-CNA refused assignment.

---

## Areas of focus

- PHP web application security (ERP/CRM, large legacy codebases, eval-injection patterns)
- Linux kernel drivers (mt76 / wireless / USB recovery)
- Embedded firmware and network appliances

## Stack

`PHP` · `Python` · `Rust` · `C` · `Bash` · Linux kernel (mt76, USB, networking) · Podman Quadlets · libvirtd · Tailscale · MariaDB · SQLite · UBL 2.1 / XAdES-BES (DIAN compliance research).

---

## Contact

- GitHub — [@bryamzxz](https://github.com/bryamzxz)

Open to remote positions in application security, vulnerability research, and FOSS audit. Particularly interested in boutiques where research output is valued over volume metrics.

<!---
bryamzxz/bryamzxz is a special repository because its README.md appears on the GitHub profile.
--->
