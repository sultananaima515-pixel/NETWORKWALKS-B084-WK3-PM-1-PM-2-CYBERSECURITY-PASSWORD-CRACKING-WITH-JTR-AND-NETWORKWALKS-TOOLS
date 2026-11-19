# NetworkWalks Cybersecurity Internship – Week 3

## Password Cracking with John the Ripper and NetworkWalks Tools

**Program:** Cybersecurity Internship – NetworkWalks  
**Batch:** B084  
**Week:** 03  
**Practical Modules:**
- W3-PM1: Password Cracking with John the Ripper (JTR)
- W3-PM2: Password Cracking with NetworkWalks Tools

---

## Overview

This repository documents the practical activities completed during Week 3 of the NetworkWalks Cybersecurity Internship.

The main focus was learning about password security, password hash extraction, dictionary-based password auditing, and practical password-cracking tools.

All exercises were performed for educational purposes using training files and authorized lab materials.

## Learning Objectives

- Understand password hashing and password security.
- Learn the basic working principles of John the Ripper.
- Understand dictionary-based password auditing.
- Learn how to extract password hashes from password-protected PDF files.
- Use wordlists such as RockYou for authorized password auditing.
- Explore the password-cracking tools introduced by NetworkWalks.
- Understand the importance of strong passwords and secure password storage.

---

## W3-PM1: Password Cracking with John the Ripper

### 1. Introduction

John the Ripper is an open-source password security auditing tool. It tests candidate passwords against extracted password hashes to determine whether a password can be recovered.

### 2. Tools Used

| Tool | Purpose |
|---|---|
| Kali Linux | Security testing environment |
| John the Ripper | Password auditing |
| pdf2john | Extracting password hashes from PDF files |
| RockYou | Dictionary wordlist |
| Terminal | Executing commands |

### 3. Practical Steps

**Step 1: Verify John the Ripper**

```bash
john --version
```

**Step 2: Locate the PDF training file**

```bash
ls -lh /media/sf_Shared_file/
```

**Step 3: Extract the PDF hash**

```bash
pdf2john "/media/sf_Shared_file/My Locked PDF1.pdf" > ~/W3-PM1/pdf_hash.txt
```

**Step 4: Verify the extracted hash**

```bash
cat ~/W3-PM1/pdf_hash.txt
```

**Step 5: Check the RockYou wordlist**

```bash
ls -lh /usr/share/wordlists/rockyou.txt
```

**Step 6: Perform dictionary-based password auditing**

```bash
john --wordlist=/usr/share/wordlists/rockyou.txt ~/W3-PM1/pdf_hash.txt
```

**Step 7: Display the result**

```bash
john --show ~/W3-PM1/pdf_hash.txt
```

### 4. Evidence – W3-PM1

| Screenshot | Description |
|---|---|
| [Screenshot 1](Module1/1.Screenshot(PDF1).png) | PDF 1 practical evidence |
| [Screenshot 2](./2.Screenshot%28PDF1%29.png) | PDF 1 additional evidence |
| [Screenshot 3](./3.Screenshot%28PDF2%29.png) | PDF 2 practical evidence |
| [Screenshot 4](./4.Screenshot%28PDF2%29.png) | PDF 2 additional evidence |
| [Screenshot 5](./5.Screenshot%28PDF3%29.png) | PDF 3 practical evidence |
| [Output 1](./1.Output%20of%20PDF%201.png) | PDF 1 output |
| [Output 2](./2.Output%20of%20PDF2.png) | PDF 2 output |
| [Output 3](./3.Output%20of%20PDF3.png) | PDF 3 output |

---

## W3-PM2: Password Cracking with NetworkWalks Tools

### 1. Introduction

This practical module focuses on learning and using the password-cracking tools introduced by NetworkWalks.

The exercise provides practical exposure to password auditing and helps develop an understanding of password security.

### 2. Practical Activities

The following screenshots document the practical work:

| Screenshot | Description |
|---|---|
| [Screenshot 6](./6.screenshot%28NW%20Tools%29.png) | NetworkWalks Tools practical evidence |
| [Screenshot 7](./7.Screenhot%28NW%20Tools%29.png) | Additional practical evidence |
| [Screenshot 8](./8.screenshot%28NW%20tools%29.png) | Practical output |

*Add the exact tool names, commands, and observations here after documenting the corresponding exercise.*

---

## Key Learning Outcomes

Through these practical exercises, I gained experience in:

1. Understanding password hashes and password auditing.
2. Using John the Ripper in Kali Linux.
3. Extracting PDF password hashes using pdf2john.
4. Working with the RockYou wordlist.
5. Performing dictionary-based password auditing.
6. Understanding the importance of password complexity.
7. Documenting cybersecurity practical activities with terminal evidence.

---

## Tools and Technologies

- Kali Linux
- John the Ripper
- pdf2john
- RockYou Wordlist
- NetworkWalks Password-Cracking Tools

---

## Disclaimer

This repository is intended for educational purposes as part of the NetworkWalks Cybersecurity Internship.

All practical activities should be performed only on authorized training materials, systems, and files.

Training PDFs, extracted hashes, and recovered passwords should not be redistributed or published without explicit permission from their owner.

---

**Cybersecurity Internship – NetworkWalks | Batch B084 | Week 03**
