# networkwalks-B082-week3

# Week 3 Cybersecurity Project: Password Cracking

## Project Overview

For Week 3 of my cybersecurity training, I worked on a password-cracking lab designed to help me understand how password-protected files can be analyzed and how password strength affects security.

The project was divided into two modules. In the first module, I used **John the Ripper (JTR)** and **Johnny GUI** to crack the password of a protected PDF. In the second module, I used the **NetworkWalks Hash Calculator** and **NetworkWalks Password Cracker** to perform the same type of password-recovery process through web-based tools.

The main goal was not just to recover the password, but to understand the process behind password cracking, including hash extraction, password recovery, and the importance of strong passwords.

> **Note:** This project was carried out in a controlled training environment for educational and ethical hacking purposes. Password-cracking techniques should only be used on systems or files where permission has been granted.

---

## Objectives

During this project, I worked on the following:

* Understanding how password cracking works.
* Understanding the role of hashes in password security.
* Extracting a password hash from a protected PDF.
* Using John the Ripper to perform password recovery.
* Using Johnny as the graphical interface for John the Ripper.
* Using the NetworkWalks Hash Calculator.
* Using the NetworkWalks Password Cracker.
* Understanding why password complexity is important.

---

# Module 1: Password Cracking with John the Ripper

### What I Used

* John the Ripper (JTR)
* Johnny GUI
* Windows PC
* Protected PDF
* PDF hash extraction tool
* Notepad

John the Ripper is a password-cracking tool commonly used by security professionals to test password strength. It can work with different password hashes and password-protected file types, including PDF, ZIP, and Office documents. Johnny provides a graphical interface that makes it easier to work with John the Ripper.

### My Approach

I started by setting up John the Ripper and Johnny on my computer. After configuring Johnny to use the `john.exe` file, I obtained the protected PDF used for the lab.

The next step was to extract the password hash from the PDF. The extracted value started with `$pdf$`, and I saved the hash in a text file called `hash1.txt`.

I then opened Johnny and loaded the hash file. From there, I started a new password-cracking attack and waited for the tool to recover the password.

Once the password was recovered, I used it to open the protected PDF and confirm that the password worked.

### Workflow

```text
Protected PDF
      ↓
Extract PDF Hash
      ↓
Save Hash as hash1.txt
      ↓
Load Hash into Johnny
      ↓
Start Password Attack
      ↓
Password Recovered
      ↓
Open Protected PDF
```

### Screenshots

The screenshots below document the process:

```text
screenshots/
├── 01-john-installation.png
├── 02-johnny-configuration.png
├── 03-pdf-hash-extraction.png
├── 04-hash-file.png
├── 05-johnny-attack.png
└── 06-password-recovered.png
```

---

# Module 2: Password Cracking with NetworkWalks Tools

The second part of the project used two browser-based tools provided by NetworkWalks:

* **Hash Calculator**
* **Password Cracker**

Unlike the first module, these tools did not require a local installation. The lab explains that the Hash Calculator extracts the hash from the protected PDF, while the Password Cracker uses that hash to attempt password recovery.

### My Approach

I first opened the NetworkWalks Hash Calculator and uploaded the protected PDF. The tool generated a hash beginning with `$pdf$`.

I copied the complete hash and then opened the NetworkWalks Password Cracker. I pasted the hash into the tool and started the password-cracking process.

After waiting for the process to complete, the recovered password was displayed. I then used the password to open the protected PDF and confirm the result.

### Workflow

```text
Protected PDF
      ↓
NetworkWalks Hash Calculator
      ↓
Extract $pdf$ Hash
      ↓
Copy Complete Hash
      ↓
NetworkWalks Password Cracker
      ↓
Password Recovered
      ↓
Open Protected PDF
```

### Screenshots

```text
screenshots/
├── 07-networkwalks-hash-calculator.png
├── 08-extracted-pdf-hash.png
├── 09-networkwalks-password-cracker.png
├── 10-cracking-process.png
└── 11-password-recovered.png
```

---

# What I Learned

One of the main things I learned from this project is that password cracking is not simply about guessing a password. There is a process involved, starting with obtaining the protected data or hash and then using an appropriate tool to attempt password recovery.

I also gained a better understanding of the role of **hashes** in password security. A hash represents the password in a scrambled form, and password-cracking tools can attempt different passwords until they find one that matches the hash.

Another important concept I learned was the difference between **encryption and hashing**. The project material explains encryption as a two-way function that can be reversed with the proper key, while hashing is described as a one-way process that produces a message digest.

The project also showed me why password complexity matters. The time required to recover a password can depend on how simple or complex the password is.

---

# Tools Comparison

|                   | John the Ripper           | NetworkWalks Tools                 |
| ----------------- | ------------------------- | ---------------------------------- |
| Platform          | Local computer            | Web browser                        |
| Main Tools        | JTR & Johnny              | Hash Calculator & Password Cracker |
| Hash Extraction   | Separate extraction step  | Built-in Hash Calculator           |
| Password Recovery | John the Ripper           | Password Cracker                   |
| Installation      | Required                  | Not required                       |
| Purpose           | Password security testing | Password security testing          |

---

# Project Structure

```text
Week-3-Password-Cracking/
│
├── README.md
│
├── JTR/
│   └── hash1.txt
│
├── NetworkWalks/
│
└── screenshots/
    ├── 01-john-installation.png
    ├── 02-johnny-configuration.png
    ├── 03-pdf-hash-extraction.png
    ├── 04-hash-file.png
    ├── 05-johnny-attack.png
    ├── 06-password-recovered.png
    ├── 07-networkwalks-hash-calculator.png
    ├── 08-extracted-pdf-hash.png
    ├── 09-networkwalks-password-cracker.png
    ├── 10-cracking-process.png
    └── 11-password-recovered.png
```

---

# Conclusion

This Week 3 project gave me practical experience with password-cracking techniques and helped me understand how password-protected files can be analyzed in a controlled cybersecurity environment.

Working with both **John the Ripper** and **NetworkWalks tools** allowed me to see two different approaches to password recovery. More importantly, the exercise helped me understand the relationship between password strength, hashing, and security.

The overall process can be summarized as:

**Protected File → Hash Extraction → Password Cracking → Password Recovery → Verification**

This was a valuable hands-on exercise and another step in building my practical cybersecurity skills.

---

# Author

**Oluwagbenga Atanda**

---

## Training

**NetworkWalks — Cybersecurity & Ethical Hacking Project**

**Week 3 — Project Module 1 & Module 2**

* Password Cracking with John the Ripper
* Password Cracking with NetworkWalks Tools
