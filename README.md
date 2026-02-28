# 👋 Hi, I'm Bryam (@bryamzxz)

🇨🇴 Colombia · 2400m above sea level · where cosmic radiation kills hardware and makes you learn fast

---

## 🔍 What I actually do

I find bugs. I read source code, trace execution paths, and write reports that go upstream.

**Recent contributions:**
- 🐛 **Linux kernel / mt76** — Identified and reported driver bugs in the MT7921 WiFi chip, including TX power reporting issues and USB reset behavior for SEFI recovery at high altitude. Patches submitted to the mt76 project.
- 🔒 **Dolibarr ERP** — Security research and vulnerability reporting. Analyzed root causes in the codebase and submitted findings through responsible disclosure.
- 🖥️ **cosmic-comp** — Forensic analysis of the Wayland compositor source (Rust). Identified a tiling geometry bug triggered by fullscreen requests from tiled windows, traced to `update_positions()` in `tiling/mod.rs`. Filed as [issue #2146](https://github.com/pop-os/cosmic-comp/issues/2146) after ruling out PR #2099 as a fix.

I don't run exploits. I read the code, find the root cause, and report it. **Gray/White team.**

---

## 🏗️ What I run

A production homelab in Bogotá serving real businesses — 6 to 12 users daily.

```
Minisforum NAB9 · i9-12900H · dual Intel I226-V · MT7921 WiFi
Ubuntu Server · Podman Quadlets · libvirtd · Tailscale · dnsmasq · Cockpit (compiled from source)
```

**Services in production:**
- 📄 Colombian e-invoicing compliance (DIAN) — custom modules for ERPNext and Dolibarr, UBL 2.1, XAdES-BES/EPES, production use · *private, active development*
- 🐦 **ERPNext** via podman-compose for furniture business management
- 🗄️ **[Dolibarr](https://github.com/bryamzxz/dolibarr)** fork + Quadlet pod (MariaDB + app container)
- 📡 **[sensor_app](https://github.com/bryamzxz/sensor_app)** — Arduino (TMP117+BME680) → SQLite + Telegram alerts
- 📦 **[cockpit-sensors](https://github.com/bryamzxz/cockpit-sensors)** — lm-sensors module for Cockpit
- 🔐 Zero-trust network via Tailscale MagicDNS + iptables

**Infrastructure I've built:**
- WiFi SEFI recovery automation (cosmic radiation induced Single Event Functional Interrupts)
- USB power cycling for MT7921 resets without rebooting
- Cockpit 354+ compiled from source with custom modules
- Rootless Podman Quadlets for security isolation

---

## 🧠 How I work

- Read source before touching config
- `journalctl` and kernel logs before guessing
- Reproduce → isolate → root cause → report
- Everything through git: `servidor1-scripts` repo → GitHub → `git pull` on server

---

## 🌱 Building

- **Colombian e-invoicing (DIAN)** — open-source compliance modules for ERPNext and Dolibarr · releasing when stable
- **Linux driver contributions** — mt76 / MT7921 upstream patches
- **Security research** — ERP and compositor-level vulnerability analysis

---

## 📫 Find me

> If you're working on mt76, cosmic-comp, ERPNext, Dolibarr, or Colombian tax compliance — let's talk.

<!---
bryamzxz/bryamzxz is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
--->
