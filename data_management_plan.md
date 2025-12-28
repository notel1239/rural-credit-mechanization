# Data Management Plan

## 1. Data Collection
- Primary data will be collected via face‑to‑face interviews using a structured questionnaire.
- The target population is farmers in selected rural districts.
- Sampling will be stratified by farm size and credit access to ensure representativeness.
- Data collection will be conducted by trained enumerators using digital forms (e.g., ODK, KoboToolbox) to minimize entry errors.

## 2. Data Storage & Security
- Raw data files (CSV/Excel) will be stored in a dedicated `data/raw/` directory in this repository.
- Personal identifiers (names, phone numbers, exact addresses) will be **removed** before storage. A unique anonymized ID will be assigned to each respondent.
- The repository will **not** contain any personally identifiable information (PII).
- Backup copies of anonymized data will be kept in a secure cloud storage (password‑protected) separate from the repository.

## 3. Data Cleaning
- A cleaning script (R or Python) will be placed in `scripts/clean_data.R` (or `.py`).
- The script will:
  - Check for missing values and implausible entries.
  - Recode categorical variables consistently.
  - Create derived variables (e.g., binary indicators for credit access).
  - Produce a clean dataset saved as `data/clean/farmer_survey_clean.csv`.
- A log of cleaning decisions will be maintained in `data/clean/cleaning_log.md`.

## 4. Version Control
- All data files will be versioned using Git LFS (Large File Storage) if size exceeds 100 MB.
- Each survey round will be tagged with a version number (e.g., `v1.0‑survey‑2025`).
- The `data/raw/` directory will be read‑only after each round to preserve original records.

## 5. Documentation
- A data dictionary (`data/documentation/data_dictionary.md`) will describe each variable, its source, allowed values, and any transformations.
- Questionnaire versions will be stored in `questionnaire/` as PDF and source files.

## 6. Access & Sharing
- Anonymized clean datasets will be made publicly available under a CC‑BY‑4.0 license.
- Researchers wishing to access the raw (identifiable) data must sign a data‑use agreement and obtain ethics approval.
- All published results will reference the dataset’s DOI (to be obtained from a repository such as Zenodo).

## 7. Ethics & Compliance
- Informed consent will be obtained from all participants before the interview.
- The study protocol will be reviewed and approved by the relevant institutional ethics committee.
- Data will be stored and processed in accordance with GDPR/ local data‑protection regulations.