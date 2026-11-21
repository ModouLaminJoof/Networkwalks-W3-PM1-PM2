# Networkwalks W3 PM1 & PM2

Documentation and evidence from a Networkwalks Academy cybersecurity exercise focused on password recovery and persistence.

## Overview

This walkthrough demonstrates how a password-protected PDF can be analyzed and recovered in an authorized lab environment. The exercise covers:

- Extracting and recognizing a PDF password hash
- Loading the hash into **Johnny**, the graphical interface for John the Ripper
- Running a wordlist-based password attack
- Verifying the recovered password by opening the protected PDF
- Capturing the first flag and the persistence flag

## Walkthrough

### 1. Identify the protected PDF hash

The exercise provides a PDF hash in `$pdf$` format. This hash is used as the input for the password-recovery tool.

### 2. Run a wordlist attack

The hash is loaded into Johnny and tested against a wordlist. Johnny displays each candidate password and reports a successful match when the correct password is found.

### 3. Verify the recovered password

After the password is recovered, it can be used to unlock the PDF. The recovered value should always be verified against the original protected file.

### 4. Capture the flags

The exercise includes two milestones:

- **First flag:** confirms the initial password-recovery objective
- **Persistence flag:** confirms completion of the later challenge objective

## Evidence

### Password recovery result

![Password recovery result](Screenshot%202026-11-21%20012433.png)

![Wordlist attack progress](Screenshot%202026-11-21%20012908.png)

### First flag

![First flag captured](Screenshot%202026-11-21%20012633.png)

### Persistence flag

![Persistence flag captured](Screenshot%202026-11-21%20012814.png)

### Johnny verification

![Johnny verification](Screenshot%202026-11-21%20014725.png)

## Tools and concepts

- **Johnny** - graphical interface for John the Ripper
- **John the Ripper** - password auditing and recovery tool
- **Wordlists** - candidate-password collections used during authorized testing
- **PDF hash formats** - representations of protected PDF credentials for auditing

## Responsible use

Only perform password recovery or security testing against files, systems, and accounts that you own or are explicitly authorized to assess. Do not use these techniques to access another person’s data or bypass access controls.

## Credits

This exercise was completed as part of the Networkwalks Academy cybersecurity learning journey.
