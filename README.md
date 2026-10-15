# 🦉 OCookieX

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OWeb-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0.0-cyan?style=flat-square"/>
</p>

> **OCookieX** — Cookie Security Analyzer & Session Auditor

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

Cookie security analyzer & session auditor

---

## ✨ Features

- URL fetch with per-hop Set-Cookie capture across the full redirect chain (stdlib urllib, TLS verify toggle)
- Importers — raw Set-Cookie blocks, curl -i output, Netscape cookies.txt, browser JSON exports, Cookie: request headers (auto-detected)
- Per-cookie deep audit — Secure, HttpOnly, SameSite (Lax / Strict / None+Secure), Path & Domain scope, Max-Age / Expires lifetime, __Host- / __Secure- prefix enforcement, session vs persistent class
- Session risk engine — session/auth name detection, Shannon entropy & charset bit-strength estimate, predictable / sequential / short ID detection, Base64 / hex / JWT shape detection + JWT decoding (alg=none, exp / nbf / iat, sensitive claims)
- Scope & fixation risks — parent-domain cookies, public-suffix scoping, broad Path, HTTP-set cookies reused on HTTPS, duplicate-name shadowing
- Jar diff — before/after login comparison, rotation check (session fixation indicator)
- Tracker heuristics + third-party detection in batch
- Remediation — secure Set-Cookie, Express, Django, Flask, Laravel, Spring, PHP, ASP.NET, Nginx snippets
- Batch mode (threaded) with worst-cookie summary
- Export TXT / CSV / JSON, save chooser, clipboard
- Full CLI mode (-u, --file, --jwt-inspect, --json ...)

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OCookieX
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
