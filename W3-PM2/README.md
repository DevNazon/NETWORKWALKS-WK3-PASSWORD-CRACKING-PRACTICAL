# Week 3 – PM2: Password Cracking with Networkwalks Tools

**Intern:** Nazon Abuga Orwaru  
**Batch:** B084H  
**Programme:** Networkwalks Cybersecurity Internship  
**Environment:** Kali Linux web browser  
**Status:** Completed

## Overview
This practical used the two browser-based Networkwalks tools specified in the Week 3 PM2 guide:
1. Networkwalks Hash Calculator
2. Networkwalks Password Cracker

The target was `My Locked PDF1 (for NW Tools Lab WK3-PM2).pdf`.

## Objectives
- Generate a PDF hash from the supplied locked PDF.
- Copy the complete hash beginning with `$pdf$`.
- Submit the hash to the Networkwalks Password Cracker.
- Verify the recovered password by opening the supplied PDF.

## Procedure

### 1. Generate the PDF hash
Open the [Networkwalks Hash Calculator](https://networkwalks.com/hash-calculator/). Select the **PDF** tab and upload `My Locked PDF1 (for NW Tools Lab WK3-PM2).pdf`. The calculator generates a PDF hash beginning with `$pdf$`. Copy the complete hash.

### 2. Submit the hash to the Password Cracker
Open the [Networkwalks Password Cracker](https://networkwalks.com/password-cracker/). Paste the complete PDF hash into the input field and start the attack. Wait for the tool to display the recovered password.

### 3. Verify the result
Open the same PM2 training PDF and enter the recovered password. The PDF opened successfully, confirming the result.

## Results

| Activity | Outcome |
|---|---|
| PDF hash generated | Successful |
| Complete hash submitted | Successful |
| Password recovered | Successful |
| PDF opened with recovered password | Successful |

## Evidence Screenshots
Place the six captured screenshots in `Screenshots/`:
- `01-Hash-Calculator-Opened.png`
- `02-PDF-Uploaded-Hash-Generated.png`
- `03-Password-Cracker-Opened.png`
- `04-Hash-Pasted-Into-Cracker.png`
- `05-Password-Cracked.png`
- `06-PDF-Unlocked.png`

## Folder Structure

```text
W3-PM2/
├── Screenshots/
│   ├── 01-Hash-Calculator-Opened.png
│   ├── 02-PDF-Uploaded-Hash-Generated.png
│   ├── 03-Password-Cracker-Opened.png
│   ├── 04-Hash-Pasted-Into-Cracker.png
│   ├── 05-Password-Cracked.png
│   └── 06-PDF-Unlocked.png
├── Files/
│   ├── pm2-hash.txt  # Optional, if downloaded
│   └── My Locked PDF1 (for NW Tools Lab WK3-PM2).pdf
├── W3-PM2-Practical-Report.docx
└── README.md
```

## Security and Ethical Use
This exercise was limited to the PDF supplied for the Networkwalks training task. Only use password-recovery tools on files you own or have explicit permission to assess. Do not reuse the recovered training password for personal accounts.

## Conclusion
The PM2 exercise was completed successfully using the Networkwalks Hash Calculator and Networkwalks Password Cracker. The generated PDF hash was submitted to the Password Cracker, the password was recovered, and the supplied PDF opened successfully with that password.

## References
- Networkwalks Week 3 PM2 practical guide.
- [Networkwalks Hash Calculator](https://networkwalks.com/hash-calculator/)
- [Networkwalks Password Cracker](https://networkwalks.com/password-cracker/)
