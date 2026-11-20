# 🔐 Networkwalks Cybersecurity Internship — Week 3: Password Cracking

![Status](https://img.shields.io/badge/status-completed-brightgreen)
![Batch](https://img.shields.io/badge/batch-B084-blue)
![Week](https://img.shields.io/badge/week-03-orange)

**Intern:** Yash Krishna Patil
**Week:** 03
**Project Modules:** PM1 & PM2
**Topic:** PDF Password Cracking using John the Ripper and Networkwalks Tools

---

## 📌 Project Overview

This repository documents the practical work completed for **Week 3, Project Modules 1 and 2** of the **Networkwalks Cybersecurity Internship (Batch B084)**.

The goal was to recover the password of a protected PDF file (`My Locked PDF1.pdf`) using two different cracking approaches:

1. **John the Ripper (JTR)** with the **Johnny GUI**
2. **Networkwalks Hash Calculator** and **Password Cracker** (browser-based)

Both methods show how password hashes can be extracted from a PDF and tested against dictionary-based attacks.

---

## 🛠️ WK3-PM1: Password Cracking Using John the Ripper

### 🎯 Objective
Extract the password hash of a protected PDF and recover its password using **John the Ripper** and its GUI front-end, **Johnny**.

### 🔧 Tools Used
- John the Ripper (JTR)
- Johnny GUI
- Online HashCrack PDF Hash Extractor
- Password-protected PDF file

### ⚙️ Steps Performed

**Step 1 — Extract PDF Hash**
Uploaded the protected PDF to the Online HashCrack PDF Hash Extractor and generated its password hash in `$pdf$...` format.

![Hash Extraction](PM1/Hash-Extract.png)

**Step 2 — Configure Johnny**
Opened Johnny, pointed it to the John the Ripper executable, and loaded the hash file via **Open Password File**.

![Johnny Configuration](PM1/JTR-PM1-Setup.png)

**Step 3 — Perform Password Cracking**
Started the cracking process in Johnny. The tool successfully recovered the password.

![JTR Password Cracking Result](PM1/JTR-PM1.png)

**Step 4 — Verify the Password**
Opened the protected PDF with the recovered password to confirm success.

![Unlocked PDF](PM1/W3-PM1-file-unlocked.png)

### ✅ PM1 Result
Successfully recovered and verified the PDF password: **`good-luck`**

---

## 🌐 WK3-PM2: Password Cracking Using Networkwalks Tools

### 🎯 Objective
Recover the password of the same protected PDF using Networkwalks' browser-based **Hash Calculator** and **Password Cracker**.

### 🔧 Tools Used
- Networkwalks Hash Calculator
- Networkwalks Password Cracker
- Web Browser
- Password-protected PDF file

### ⚙️ Steps Performed

**Step 1 — Generate PDF Hash**
Uploaded the protected PDF to the Networkwalks Hash Calculator, which extracted the password hash in `$pdf$...` format.

![Hash Calculator](PM2/Hash-Calculator.png)

**Step 2 — Perform Dictionary Attack**
Pasted the hash into the Networkwalks Password Cracker, selected the dictionary attack method, and ran the crack.

![Password Cracker Result](PM2/Cracked.png)

**Step 3 — Verify the Password**
Used the recovered password to open and confirm the unlocked PDF.

![Unlocked PDF](PM2/W3-PM2-File-Unlocked.png)

### ✅ PM2 Result
Successfully recovered and verified the PDF password: **`password1`**

---

## 📊 Comparison: PM1 vs PM2

| Feature | PM1 – John the Ripper | PM2 – Networkwalks |
|---|---|---|
| Tools | John the Ripper & Johnny | Networkwalks Online Tools |
| Interface | Desktop GUI | Web-based |
| Hash Extraction | Online HashCrack | Hash Calculator |
| Attack Method | Dictionary-based cracking | Dictionary attack |
| Installation | Required | Not required |
| Recovered Password | `good-luck` | `password1` |

---

## 💡 Key Learnings

- How to extract password hashes from protected PDF files
- How PDF password hashes are represented in `$pdf$...` format
- How to configure and use John the Ripper with the Johnny GUI
- How to perform dictionary-based password attacks
- How to use browser-based password-cracking tools
- How to verify recovered passwords by opening protected files
- Why short, predictable passwords are vulnerable to dictionary attacks

## 🔐 Security Takeaway

Weak, predictable passwords can be recovered quickly with publicly available cracking tools. Using long, unique, and complex passwords significantly reduces the risk of unauthorized access.

---

## 📁 Repository Structure

```
.
├── PM1/
│   ├── .gitkeep
│   ├── Hash-Extract.png
│   ├── JTR-PM1-Setup.png
│   ├── JTR-PM1.png
│   └── W3-PM1-file-unlocked.png
├── PM2/
│   ├── .gitkeep
│   ├── Cracked.png
│   ├── Hash-Calculator.png
│   └── W3-PM2-File-Unlocked.png
└── README.md
```

---

## ⚠️ Disclaimer

This project was conducted strictly for **educational and cybersecurity training purposes** as part of the Networkwalks Cybersecurity Internship. The target PDF and lab materials were provided by Networkwalks, and password recovery was performed only on the authorized training file.

**For educational purposes only.** Always obtain proper authorization before conducting password recovery or security testing.

---

⭐ If you find this project useful, feel free to explore and star the repository!
