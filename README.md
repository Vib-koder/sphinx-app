# sphinx-app
A secure message and file encryptor for Windows
# 🦁 Sphinx — Secure Message & File Encryptor

*"I keep secrets. That is what I do."*

Sphinx is a lightweight, standalone Windows application for encrypting and decrypting messages and files. No installation required. No cloud. No nonsense. Just you, your passcode, and an ancient guardian who takes privacy very seriously.

---

## ✨ What It Does

- **Encode** any text message with a passcode — turn it into an unreadable cipher
- **Decode** it back — but only if you know the passcode
- **Encrypt files** of any type (up to 20 MB) — the output is a `.sphinx` file with a scrambled filename
- **Decrypt files** — restore the original file, name and all
- Wrong passcode? The Sphinx will let you know. Loudly.

---

## 🔐 How It Works

Sphinx uses **PBKDF2-SHA256** (200,000 rounds) combined with **HMAC-SHA256** to derive a keystream from your passcode and a hidden master key embedded in the app. Each message is salted with 16 random bytes, so no two encryptions are alike — even for the same text.

In short: it is not trivial to crack.

---

## 🚀 Getting Started

1. Download `Sphinx.exe` from the [Releases](../../releases) page
2. Double-click to run — no installation, no Python needed
3. Type your message (or load a file), enter a passcode, and hit **Encode**
4. Share the encoded result with whoever needs it
5. They open Sphinx, paste it in the Decode tab, enter the same passcode — done

---

## 📋 Requirements

- Windows 10 or 11
- Nothing else. Seriously.

---

## ⚠️ A Word of Warning

Sphinx encodes and decodes using a **shared passcode**. If you lose the passcode, the message is gone. The Sphinx does not do password recovery. The Sphinx does not negotiate.

---

## 👤 Author

Made with care (and a healthy respect for ancient mysteries) by **Akhenaton**.
Version 1.1

---

*"What has four legs in the morning, two at noon, and three in the evening? I already know. Do you?"*
