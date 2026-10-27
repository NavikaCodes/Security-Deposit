# FDR Sentinel (SIH 2026 prototype)

Security Deposit & FDR Management Portal for AICTE. Demonstration prototype with fictional data.

## Run
Requires Node.js 18+.

```bash
npm install
npm run dev        # http://localhost:5173
```

Other commands: `npm run build` (output in `dist/`), `npm run preview` (serve the build).
Data is saved in the browser's localStorage. Settings > Reset demo data (Admin) restores the seed.

## Demo roles
Institution, Scrutiny Officer, Accounts Officer, Competent Authority, Administrator, Auditor (one-click login).

## Demo walkthrough
1. Institution: New FDR (try a duplicate number, or upload a file named mismatch.pdf).
2. Scrutiny: Verification > open case > Start review > Simulated bank check > Mark complete.
3. Change the Demo date in the header > Maturity & Alerts > Run reminder check.
4. Institution: open an Active FDR > Renew / replace; Scrutiny completes it.
5. Institution: Request release > Scrutiny > Accounts > Competent Authority approves.
6. Auditor: Audit Trail; Reports > CSV (opens a copy box).

## Simulated / not implemented
Simulated: bank verification, OCR, email/SMS, login.
Not implemented: React/Node/PostgreSQL backend, real OCR, document preview, PDF export, encryption, real authentication.
