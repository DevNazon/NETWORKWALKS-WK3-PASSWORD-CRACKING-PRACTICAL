# Week 3 – PM1: Password Cracking with John the Ripper

**Intern:** Nazon Abuga Orwaru  
**Batch:** B084H  
**Programme:** Networkwalks Cybersecurity Internship  
**Environment:** Kali Linux running in Oracle VirtualBox  
**Status:** Completed

## Overview

This practical demonstrates password recovery on the PDF training document supplied for Week 3 PM1. The task was completed using both John the Ripper in the Kali terminal and Johnny, its graphical interface.

> **Scope note:** Testing was limited to the training PDF supplied for this exercise. Only use these techniques on files you own or have explicit permission to assess.

## Objectives

- Extract a password hash from the supplied PDF using `pdf2john`.
- Recover the PDF password using John the Ripper.
- Repeat the recovery using the Johnny graphical interface.
- Verify the recovered password by opening the supplied PDF.

## Tools

- Kali Linux
- John the Ripper
- `pdf2john`
- Johnny GUI

## Procedure

### 1. Extract the PDF hash

From the directory containing `My Locked PDF1.pdf`, run:

```bash
pdf2john "My Locked PDF1.pdf" > hash1.txt
```

The resulting `hash1.txt` contains the PDF hash in a John-compatible format. The extracted hash begins with `$pdf$`.

### 2. Crack with John the Ripper

```bash
john --format=PDF hash1.txt
```

**Result:** John loaded one PDF hash and successfully recovered the training document password.

### 3. Crack with Johnny

1. Launch Johnny.
2. Open the existing password file `hash1.txt`.
3. Start the password recovery attack.
4. Confirm that Johnny reports a successful recovery.

**Result:** The password was successfully recovered through the graphical interface as well.

### 4. Verify the result

Open `My Locked PDF1.pdf` and enter the recovered training password. The document opened successfully.

## Results

| Activity | Outcome |
|---|---|
| PDF hash extraction | Successful |
| John terminal recovery | Successful |
| Johnny GUI recovery | Successful |
| PDF password verification | Successful |

## Folder Structure

```text
W3-PM1/
├── Screenshots/
│   ├── 01-John-Version.png
│   ├── 02-PDF-Hash-Extracted.png
│   ├── 03-John-Terminal-Cracked.png
│   ├── 04-Johnny-Loaded-Hash.png
│   ├── 05-Johnny-Cracked.png
│   └── 06-PDF-Unlocked.png
├── Files/
│   ├── hash1.txt
│   └── My Locked PDF1.pdf
├── W3-PM1-Practical-Report.docx
└── README.md
```

The filenames above are the recommended organisation. Place your actual screenshots and working files in the corresponding folders before packaging the submission.

## Conclusion

The PM1 task was completed using both the John the Ripper command-line tool and Johnny GUI. The extracted PDF hash was successfully tested, the password was recovered, and the original training PDF was opened to verify the result.

## References

- Networkwalks Week 3 – PM1 practical guide.
- [John the Ripper](https://www.openwall.com/john/)
- [Kali Linux – John the Ripper](https://www.kali.org/tools/john/)
