# Bryam Vargas · `@bryamzxz`

Independent security researcher in Colombia. Source-first: read the code, trace input to sink, reproduce in an isolated lab, disclose in coordination with the maintainers.

**[bryamzxz.github.io](https://bryamzxz.github.io)**: write-ups and disclosure policy.

## Disclosures

- **Dolibarr ERP/CRM**: CVE-2026-37711, CVE-2026-37712, CVE-2026-37713 (CVSS 9.1 / 9.1 / 8.1). PHP code injection through `dol_eval()` and OS command execution through the cron scheduler. [Write-up](https://bryamzxz.github.io/2026/05/25/dol_eval-five-years/)

## Projects

- **[tinylink](https://github.com/bryamzxz/tinylink)**: a clean-room, Tailscale-compatible node for the bare ESP32 (no PSRAM, ~741 KiB, pure C). It implements the ts2021 control plane, WireGuard from scratch, DISCO/STUN NAT traversal and a DERP fallback.

## Upstream reports

- `espressif/esp-idf` [#18574](https://github.com/espressif/esp-idf/issues/18574): the DHCP client callback panics on custom netifs.
- `pop-os/cosmic-comp` [#2146](https://github.com/pop-os/cosmic-comp/issues/2146): a tiled sibling window shrinks when another window goes fullscreen.
- `frappe/frappe` [#37799](https://github.com/frappe/frappe/issues/37799): `remove_orphan_doctypes()` deletes custom-app DocTypes on migrate.
- `Dolibarr/dolibarr` [#37227](https://github.com/Dolibarr/dolibarr/issues/37227) and [#37266](https://github.com/Dolibarr/dolibarr/issues/37266).

## Focus

PHP web applications · Linux kernel drivers · embedded (ESP32 / ESP-IDF) · WireGuard and Tailscale · Colombian e-invoicing (UBL 2.1, XAdES)

`C` · `PHP` · `Python` · `Rust` · `Bash`

---

Vulnerability identification is human-driven. AI assistance is limited to documentation and is disclosed when used. The default disclosure window is 90 days; [details here](https://bryamzxz.github.io/about/).
Open to application security and vulnerability research work.
