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

The main focus is password security, password hash extraction, dictionary-based password auditing, and practical password-cracking tools.

All exercises were performed for educational purposes using authorized training materials.

## Learning Objectives

- Understand password hashing and password security.
- Learn the working principles of John the Ripper.
- Understand dictionary-based password auditing.
- Extract password hashes from password-protected PDF files.
- Use wordlists such as RockYou for authorized password auditing.
- Learn to use the NetworkWalks Hash Calculator and Password Cracker.
- Understand the importance of strong passwords and secure password storage.

---

# W3-PM1: Password Cracking with John the Ripper

## 1. Introduction

John the Ripper (JTR) is an open-source password security auditing tool. It tests candidate passwords against extracted password hashes to determine whether a password can be recovered.

## 2. Tools Used

| Tool | Purpose |
|---|---|
| Kali Linux | Security testing environment |
| John the Ripper | Password auditing |
| pdf2john | Extracting password hashes from PDF files |
| RockYou | Dictionary wordlist |
| Terminal | Executing commands |

## 3. Practical Steps

**Step 1: Verify John the Ripper**

```bash
john --version
```

**Step 2: Create a working directory**

```bash
mkdir -p ~/W3-PM1
cd ~/W3-PM1
```

**Step 3: Locate the PDF training files**

```bash
ls -lh /media/sf_Shared_file/
```

**Step 4: Extract the PDF hash**

```bash
pdf2john "/media/sf_Shared_file/My Locked PDF1.pdf" > ~/W3-PM1/pdf_hash.txt
```

**Step 5: Verify the extracted hash**

```bash
ls -lh ~/W3-PM1/pdf_hash.txt
cat ~/W3-PM1/pdf_hash.txt
```

**Step 6: Check the RockYou wordlist**

```bash
ls -lh /usr/share/wordlists/rockyou.txt
```

**Step 7: Perform dictionary-based password auditing**

```bash
john --wordlist=/usr/share/wordlists/rockyou.txt ~/W3-PM1/pdf_hash.txt
```

**Step 8: Display the result**

```bash
john --show ~/W3-PM1/pdf_hash.txt
```

## 4. Evidence – W3-PM1

| Screenshot | Description |
|---|---|
| [Screenshot 1](Module1/1.Screenshot%28PDF1%29.png) | PDF 1 practical evidence |
| [Screenshot 2](Module1/2.Screenshot%28PDF1%29.png) | PDF 1 additional evidence |
| [Screenshot 3](Module1/3.Screenshot%28PDF2%29.png) | PDF 2 practical evidence |
| [Screenshot 4](Module1/4.Screenshot%28PDF2%29.png) | PDF 2 additional evidence |
| [Screenshot 5](Module1/5.Screenshot%28PDF3%29.png) | PDF 3 practical evidence |
| [Output 1](OUTPUT/1.Output%20of%20PDF%201.png) | PDF 1 output |
| [Output 2](OUTPUT/2.Output%20of%20PDF2.png) | PDF 2 output |
| [Output 3](OUTPUT/3.Output%20of%20PDF3.png) | PDF 3 output |

---

# W3-PM2: Password Cracking with NetworkWalks Tools

## 1. Introduction

This practical module focuses on using the NetworkWalks Hash Calculator and Password Cracker tools to perform password-cracking exercises on a password-protected PDF file.

The task was performed on a Windows laptop using the training PDF provided for the internship.

## 2. Tools Used

| Tool | Purpose |
|---|---|
| Windows Laptop | Environment for running NetworkWalks tools |
| NetworkWalks Hash Calculator | Calculating the hash value of the provided PDF file |
| NetworkWalks Password Cracker | Performing password-cracking exercises |
| My Locked PDF1.pdf | Password-protected training file |

## 3. Practical Task

**Task:** Crack the password of the provided PDF file (`My Locked PDF1.pdf`) using the NetworkWalks Hash Calculator and Password Cracker tools on a Windows laptop.

## 4. Practical Workflow

1. Open the NetworkWalks Hash Calculator on Windows.
2. Select the provided `My Locked PDF1.pdf` file.
3. Calculate and obtain the required hash value.
4. Open the NetworkWalks Password Cracker.
5. Provide the required hash or input according to the tool's instructions.
6. Select the appropriate password-cracking method and start the process.
7. Observe the result and record whether the password was recovered.
8. Capture screenshots as practical evidence.

## 5. Evidence – W3-PM2

| Screenshot | Description |
|---|---|
| [Screenshot 6](Module2/6.screenshot%28NW%20Tools%29.png) | NetworkWalks Tools practical evidence |
| [Screenshot 7](Module2/7.Screenhot%28NW%20Tools%29.png) | Additional practical evidence |
| [Screenshot 8](Module2/8.screenshot%28NW%20tools%29.png) | Password-cracking output |

---

## Key Learning Outcomes

Through these practical exercises, I gained experience in:

1. Understanding password hashes and password auditing.
2. Using John the Ripper in Kali Linux.
3. Extracting PDF password hashes using pdf2john.
4. Working with the RockYou wordlist.
5. Performing dictionary-based password auditing.
6. Using the NetworkWalks Hash Calculator.
7. Understanding the workflow of the NetworkWalks Password Cracker.
8. Learning the importance of password complexity and secure password storage.
9. Documenting cybersecurity practical activities with screenshots and terminal evidence.

---

## Tools and Technologies

- Kali Linux
- Windows 11
- John the Ripper (JTR)
- pdf2john
- RockYou Wordlist
- NetworkWalks Hash Calculator
- NetworkWalks Password Cracker

---

## Disclaimer

This repository is intended for educational purposes as part of the NetworkWalks Cybersecurity Internship.

All practical activities should be performed only on authorized training materials, systems, and files.

Training PDFs, extracted hashes, and recovered passwords should not be redistributed or published without explicit permission from their owner.

---

**Cybersecurity Internship – NetworkWalks | Batch B084 | Week 03**
