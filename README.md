# pineaoth

> 🛡️ Simple authenticator like `Google Authenticator`, but in `CLI` method

<div align="center">

  <img src="./icon/pineaoth_icon.png" alt="pineaoth icon by DiceBear" width="120" height="120" />

  <br><br>

  <img src="https://img.shields.io/pypi/v/pineoath?color=blue&label=PyPI&logo=pypi&style=flat-square" alt="PyPI" />
  <img src="https://img.shields.io/pypi/pyversions/pineoath?logo=python&label=Python&style=flat-square" alt="Python Versions" />
  <img src="https://img.shields.io/pypi/dm/pineoath?label=Downloads&style=flat-square&color=brightgreen" alt="Downloads" />
  <img src="https://img.shields.io/github/license/openpineapletools/pineaoth?style=flat-square&color=blueviolet" alt="License" />
  <img src="https://img.shields.io/github/repo-size/openpineapletools/pineaoth?style=flat-square&color=informational" alt="Repo Size" />
  <img src="https://img.shields.io/github/stars/openpineapletools/pineaoth?style=flat-square&color=yellow" alt="Stars" />
  <img src="https://img.shields.io/github/forks/openpineapletools/pineaoth?style=flat-square&color=orange" alt="Forks" />
  <img src="https://img.shields.io/github/last-commit/openpineapletools/pineaoth?style=flat-square&color=success" alt="Last Commit" />
  <img src="https://img.shields.io/github/issues/openpineapletools/pineaoth?style=flat-square" alt="Issues" />
  <img src="https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat-square&logo=github" alt="Contributions Welcome" />

</div>

---

## 🔰 Introduction

**@openpineaple** presents `pineaoth`, a lightweight CLI-based 2FA tool that works just like Google Authenticator — but right from your terminal. Easily manage your OTP secrets and get real-time tokens for any platform that supports 2FA.

---

## 📦 Installation

Install directly via PyPI:

```bash
pip install pineoath
```

---

## 🚀 Usage

Check available commands with:

```bash
pineaoth -h
```

<details>
<summary>📋 CLI Help Output</summary>

```text
usage: pineaoth [-h] [-v] {add,list,delete,live} ...

CLI 2FA Authenticator

positional arguments:
  {add,list,delete,live}
    add                 Tambah akun OTP
    list                Lihat semua akun
    delete              Hapus akun
    live                Live OTP

optional arguments:
  -h, --help            show this help message and exit
  -v, --version         show program's version number and exit

Contoh penggunaan:
  pineaoth add GitHub user123 ABCDEFGHIJKLMNOP
  pineaoth list
  pineaoth delete GitHub user123
  pineaoth live
```

</details>

---

## 📌 Example Commands

### ➕ Add an authenticator
```bash
pineaoth add GitHub user123 ABCDEFGHIJKLMNOP
```

### 📄 List all saved accounts
```bash
pineaoth list
```

### ❌ Delete an account
```bash
pineaoth delete GitHub user123
```

### ⏳ View live OTPs (auto-refreshing)
```bash
pineaoth live
```

---

## 🔧 Features

- ✅ Add/Delete multiple OTP accounts
- 🔁 Live auto-refresh OTP like Authy or Google Authenticator
- 🔐 Secret key-based OTP (TOTP)
- 💾 SQLite storage (local)
- ☁️ Upcoming: Cloud sync, QR code scan, and UI-based interaction
---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.

---

## 📜 License

This project is licensed under the terms of the **MIT License** – see the [LICENSE](./LICENSE) file for details.