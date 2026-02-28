# 👋 Hi, I'm Bryam (@bryamzxz)

🇨🇴 Colombia · 2400m above sea level · where cosmic radiation kills hardware and makes you learn fast

---

## 🔍 What I actually do

I find bugs. I read source code, trace execution paths, and write reports that go upstream.

**Recent contributions:**
- 🐛 **Linux kernel / mt76** — Two patches submitted to `linux-wireless` for the MT7921U chip:
  - [`[PATCH 1/2]`](https://lore.kernel.org/linux-wireless/CANAPQzi_eC2n_mfxrcZ46tpCDB1_RkkbpnVd2Y=P=Ua4iPU2gQ@mail.gmail.com/T/#t) `mt76: connac: fix txpower_cur not updated in mt76_connac_mcu_set_rate_txpower()` — fixes `mt76_get_txpower()` always reporting 3 dBm because `txpower_cur` was never updated after sending the SKU table to firmware. Traces root cause to the zero-initialized value + 2-chain delta path in `mt76_get_txpower()`.
  - `[PATCH 2/2]` `mt76: mt7921u: add USB reset on SEFI chip recovery` — adds `usb_queue_reset_device()` in both `mt7921u_mac_reset()` and `mt792xu_init_reset()` so the chip recovers automatically from cosmic-radiation-induced SEFIs instead of hanging permanently. Tested at 2400m altitude, Bogotá, Colombia.
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
