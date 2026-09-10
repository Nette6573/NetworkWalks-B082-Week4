# 🔎 M1 — Initial Access

## Objective

Retrieve three confidential patient laboratory-report PDFs from the restricted Patient Portal within the authorized training environment.

## Approach

The assessment began with reconnaissance and web application mapping. The Patient Portal was identified and its authentication behavior was examined through controlled testing.

Several approaches were tested. A constrained automated SQL injection check did not identify the successful condition. Further manual analysis of the authentication behavior led to identification and validation of an authentication-bypass SQL injection.

Following successful authentication, the three required PDF reports were retrieved.

## Evidence

- `M1-E01-Authenticated-Reports.png` — authenticated My Reports page showing three report downloads.
- `M1-E02-Three-PDF-Downloads.png` — local evidence showing the three retrieved PDF artifacts.
- `M1-E03-Login-Form.png` — Patient Portal authentication surface.
- `M1-E04-Username-Enumeration.png` — differentiated authentication response.
- `M1-E05-SQLMap-Check.png` — constrained automated SQLi check that did not identify the later successful condition.

## Result

**M1 — COMPLETED**

Credentials and reusable authentication material are intentionally excluded from the public repository.
