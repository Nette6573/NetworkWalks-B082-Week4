# 🔐 M2 — PDF Password Recovery

## Objective

Recover access to all three protected PDF reports retrieved during M1 and validate successful access.

## Approach

Each PDF was assessed individually. The NetworkWalks Hash Calculator was used to extract crackable PDF hashes, followed by dictionary-based password recovery using the NetworkWalks Password Cracker.

Successful recovery was achieved for all three documents, and each PDF was subsequently opened and validated.

## Evidence

- `M2-E01-PDF1-Successful-Recovery.png` — successful password recovery for PDF 1.
- `M2-E02-PDF2-Successful-Recovery.png` — successful password recovery for PDF 2.
- `M2-E03-PDF3-Successful-Recovery.png` — successful password recovery for PDF 3.
- `M2-E04-PDF1-Opened.png` — PDF 1 opened after recovery.
- `M2-E05-PDF2-Opened.png` — PDF 2 opened after recovery.
- `M2-E06-PDF3-Opened.png` — PDF 3 opened after recovery.

## Result

**M2 — COMPLETED**

Recovered passwords, hashes, patient identities, identifiers, dates of birth, clinical results and other sensitive information are redacted or omitted.
