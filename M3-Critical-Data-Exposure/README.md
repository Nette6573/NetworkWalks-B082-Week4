# 🚨 M3 — Critical Data Exposure

## Objective

Identify employee salary information and shareholder details within the authorized training environment.

## Finding

An SQL database backup was found in a web-accessible location. The resource returned successfully over HTTP, was retrieved locally, and was examined within the authorized Kali evidence environment.

Schema analysis identified staff and shareholder structures. The staff data model included identity, employment, contact, national-identification and salary-related fields. The shareholder structure included shareholder identity, ownership percentage, shares held and share class.

## Evidence

- `M3-E01-SQL-Backup-HTTP-200.png` — evidence that the SQL backup was directly retrievable over HTTP.
- `M3-E02-Backup-Downloaded.png` — local acquisition of the exposed backup.
- `M3-E03-Staff-Shareholder-Schema.png` — evidence of staff and shareholder database structures.
- `M3-E04-Database-Fields.png` — evidence of sensitive field/record structure.

## Result

**M3 — COMPLETED**

Actual employee records, salary figures, national identifiers, contact details and shareholder values are not included in this public repository.
