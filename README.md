# 🏢 Codernic Sovereign Enterprise Mock Dataset (v2.0)

[![Standard](https://img.shields.io/badge/Standard-ISO%2FIEC%2017025-blue.svg)](https://www.iso.org/standard/67193.html)
[![Compliance](https://img.shields.io/badge/Compliance-Swiss%20nLPD%20%26%20GDPR-green.svg)](https://www.fedlex.admin.ch/eli/cc/2022/491/fr)
[![Integrity](https://img.shields.io/badge/Integrity-ALCOA%2B%20Verified-purple.svg)](#)

A canonical, high-fidelity synthetic benchmark corpus designed to stress-test **Enterprise Security Gateways (SWG)**, **Data Loss Prevention (DLP)** engines, **Format-Preserving Encryption (FPE)**, and **Isometric Document Redaction** across real-world business formats (PDF, DOCX, XLSX, PPTX, XML, CSV).

---

## 📂 Architecture & Directory Organization

The dataset is organized by enterprise departmental domains and specialized torture test chambers:

```
enterprise_mock_data/
├── dataset_manifest.json               # Full JSON inventory & schema definition
├── golden_corpus/                      # Curated baseline across 6 business domains
│   ├── 01_legal_contracts/             # M&A, NDAs, Share Purchase Agreements
│   ├── 02_financial_models/            # Excel budgets, payroll spreadsheets, P&L
│   ├── 03_executive_slides/            # Board presentations, strategy decks (.pptx)
│   ├── 04_scanned_documents/           # OCR-battered scanned invoices & receipts
│   ├── 05_corporate_emails/            # Internal CEO/CFO correspondence (.eml, .txt)
│   └── 06_cloud_devops/                # Terraform state, .env files, API configs
│
├── torture_chamber/                    # Stress-testing & adversarial corner-cases
│   ├── 01_pdf_complex_enterprise/     # Swiss Ultimate Challenge, SEC 10-K filings, CMap traps
│   ├── 02_docx_enterprise/             # Multi-run Word formatting, track changes
│   ├── 03_xlsx_enterprise/             # Shared strings table, formulas, pivot tables
│   ├── 04_pptx_presentations/          # Vector shapes, master slide metadata
│   └── 05_legacy_office/               # Binary legacy Office documents (.doc, .xls, .ppt)
│
├── Executive_Board_and_Strategy/       # Minutes, acquisition roadmaps, board resolutions
├── Finance_Accounting_and_Tax/         # Swiss VAT (TVA/MWST), ledger exports, tax filings
├── Human_Resources_and_Payroll/        # Swiss AVS/AHV payroll records, employee salary slips
├── Legal_Contracts/                    # Commercial SLAs, licensing, vendor terms
├── Operations_Logistics_and_ISO/       # ISO-27001 audit trails, SOC-2 reports, supply chain
├── Patient_Archives/                   # Synthetic healthcare & clinical trial records
└── Sales_CRM_and_Marketing/            # Proposal decks, enterprise CRM pipeline exports
```

---

## 🛡️ Synthetic PII & Compliance Vectors Covered

| Category | Formats & Standards | Examples |
| :--- | :--- | :--- |
| **Swiss National ID** | Swiss AVS / AHV 13-digit | `756.9217.0769.85`, `756.3314.9812.19` |
| **Swiss Company UID** | Swiss IDE / UID / TVA | `CHE-109.876.543 TVA`, `CHE-441.209.818 HR` |
| **Banking & IBAN** | Swiss QR-IBAN, SEPA | `CH93 0076 2011 6238 5295 7`, `CH44 3000...` |
| **Financial Amounts** | Swiss thousands apostrophe | `CHF 14'850'200.50`, `EUR 4'230'100.00` |
| **Named Entities** | Multi-lingual ambiguous names | `Pierre Genève`, `Hans Zürich-Meier` |
| **Healthcare** | HIPAA / Patient Identifiers | MRN, ICD-10 diagnoses, medical consents |
| **DevOps Secrets** | Synthetic mock tokens | `sk_test_mock_...`, `ghp_...`, `AKIAIOSFODNN7EXAMPLE` |

---

## 📜 Licensing & Usage

All documents in this repository are **100% synthetic or derived from public domain regulatory filings (SEC EDGAR, GovDocs)**.  
No real personal data or proprietary commercial secrets are contained within this repository.

Distributed under the **Apache-2.0 License**. See [LICENSE](LICENSE) for details.
