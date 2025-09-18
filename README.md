# Secure Note Locker – Reverse Engineering Challenge
## 📖 Overview

Secure Note Locker is a CTF-style reverse engineering challenge written in C.
It simulates a simple password-protected vault:

Users can add, list, and read notes.
Notes and secrets are XOR-obfuscated in memory.
Access requires a hidden master key, embedded in the binary.
The distributed binary is stripped (no source) to simulate a real-world RE exercise.

### This project is intentionally designed for educational purposes:
reverse engineers must analyze the binary to discover the master key and reveal the hidden secret.

## 🎯 Learning Objectives

By working with this challenge, participants will practice:
Static and dynamic binary analysis.
Reverse engineering of stripped C binaries.
XOR-based obfuscation and simple key-recovery techniques.
Using RE tools such as Ghidra, radare2, GDB, or xxd.

## 📂 Files in Repository

locker → Precompiled Linux binary (main challenge).
README.md → Documentation and instructions.

🔒 Note: Source code is excluded from the main branch to preserve the reverse engineering challenge.

## 🚀 Usage

1. Download / clone the repository
```bash
git clone https://github.com/yeabsira-mihret/secure-note-locker.git
cd secure-note-locker
```
2. Make the binary executable (Linux/MacOS):
```bash
chmod +x locker
```
3. Run the challenge
```bash
./locker
```
4. Explore features

Add and list notes (basic vault functionality).
Attempt to read notes or reveal the hidden secret.
You’ll be prompted for a master key.
Reverse Engineer the binary
Discover the obfuscated master key.
Unlock and reveal the hidden secret.

## 🕹 Example Run
```bash
Secure Note Locker
1. Add Note
2. List Notes
3. Read Note
4. Reveal Secret (RE Challenge)
5. Exit
Choice: 3
Enter note number: 1
Enter master key: <???>
```
The goal is to determine the correct master key via reverse engineering.

## 🧩 Challenge Tasks

Participants should:

1. Analyze the stripped binary.
2. Recover the XOR key.
3. Derive the master password.
4. Unlck the hidden secret.


## ⚠️ Disclaimer

This project is created solely for educational and training purposes.
It is a safe simulation not malware, not ransomware.
Any resemblance to malicious software is coincidental.

## 🛠 Skills Demonstrated

C programming (memory management, structs, obfuscation).
Reverse engineering challenge design.
Secure binary handling & stripping for RE.
Practical application of binary analysis techniques.

## 📌 About

l.Author: Yeabsira Mihret
l.Project Type: Reverse Engineering Challenge
l.Language: C
l.Focus: Binary analysis & RE practice
