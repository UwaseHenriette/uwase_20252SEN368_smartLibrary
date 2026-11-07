

# Smart Library Circulation and Reservation System

Student: Uwase Henriette 
Student ID: 20252SEN368 
Institution: Adventist University of Central Africa (AUCA)
Course: INSY 8311 – Database Development with PL/SQL
Instructor: Eric Maniraguha
Research log started: 6 November 2026

---

## 1. Purpose of the Research

The purpose of this research is to understand library circulation and resource-sharing processes, review existing library-management solutions, identify relevant technical approaches, and assess whether the selected public dataset can support the proposed project.

The project proposes a database-driven system for managing book records, physical copies, members, loans, returns, reservations, overdue fines, and reports. The system is planned around Oracle Database 21c and PL/SQL, with an interactive user interface planned for the innovation component.

## 2. Research Sources and Notes

Source 1 — Research Paper: Circulation Methods in Academic Libraries

Reference (APA 7):

Kharat, S., & Nagarkar, S. (2023). A systematic literature review (SLR) of circulation methods in academic libraries: Proposing QR codes for self-issue/return method. Global Knowledge, Memory and Communication, 74(3–4), 845–863.

https://doi.org/10.1108/GKMC-08-2022-0188

Type: Peer-reviewed research paper.

Notes:

- The paper reviews circulation methods used in academic libraries, including manual, mechanized, automated, and networked approaches.
- It discusses a QR-code-based self-check-in and self-check-out model.
- It provides background for considering how circulation transactions can be recorded and made easier for library users.

Relevance to this project:

Supports the research rationale for automating check-out and return processes. It may also inform a future improvement such as barcode or QR-code-assisted circulation.

Follow-up: Read the full paper and record any useful design details.

Source 2 — Research Paper: Smart Library Environments

Reference (APA 7):

Adewojo, A. A., & Monjolaoluwa, O. P. (2025). Smart library environments: IoT and automation for next-generation services. Business Information Review, 42(4), 232–237.

https://doi.org/10.1177/02663821251384884

Type: Peer-reviewed research article.

Notes:

- The article reviews the use of Internet of Things (IoT) and automation in library operations.
- It discusses circulation, inventory management, interactive services, and data-driven decision-making.
- It identifies implementation concerns such as integration with existing systems, cost, maintenance, and privacy.

Relevance to this project:

Helps identify possible future enhancements and practical implementation considerations. The current project will focus on database-backed circulation and reservations rather than claiming to implement a full IoT/RFID environment.

Follow-up: Read the full article and verify which recommendations are applicable to this project.

Source 3 — Report and Library Statistics

Reference (APA 7):

Association of College and Research Libraries. (2024). The state of U.S. academic libraries: Findings from the ACRL 2023 annual survey. American Library Association.

https://www.ala.org/sites/default/files/2024-10/2023%20State%20of%20Academic%20Libraries%20Report.pdf

Type: Professional association report and statistics.

Notes:

- The report summarizes responses from 1,414 academic-library institutions in the 2023 survey.
- It covers library staffing, expenditures, collections, circulation, and information services.
- Its executive summary reports that digital materials accounted for 98.4% of total reported circulation in the responding institutions.

Relevance to this project:

Shows why library systems need to manage and report on different kinds of resources and circulation activity. This statistic describes the surveyed U.S. academic libraries, not AUCA or Rwandan libraries.

Follow-up: Read the report methodology and detailed tables before using additional figures.

Source 4 — Existing Library Management System

Reference (APA 7):

Koha Community. (n.d.). Koha manual: Circulation.

https://koha-community.org/manual/22.05/en/html/circulation.html

Type: Existing library-management system documentation.

Notes:

- Koha is an existing integrated library system.
- Its circulation documentation describes check-outs, holds (reservations), overdue reports, and overdue fines.
- The manual distinguishes a hold in a queue from a date-specific booking.

Relevance to this project:

Provides a practical reference for expected circulation and reservation functions. The proposed system can implement a smaller set of similar functions using Oracle tables and PL/SQL business rules.

Follow-up: Review the sections on check-outs, returns, holds, circulation rules, and fines.

Source 5 — Registered Dataset

Reference (APA 7):

Teper, T., Lenkart, J., Thacker, M., & Coskun, E. (2018). University of Illinois at Urbana-Champaign Library Interlibrary Loan Lending Data 2009–2013 [Data set]. University of Illinois at Urbana-Champaign.

https://doi.org/10.13012/B2IDB-6701059_V1

Type: Public dataset.

Dataset page: https://databank.illinois.edu/datasets/IDB-6701059

Licence shown on the dataset page: CC0.

Notes:

- The dataset describes five years of interlibrary-loan transactions (2009–2013) for materials lent by the University of Illinois at Urbana-Champaign Library to other institutions.
- The published dataset description reports 169,890 transactions.
- The downloaded Excel workbook contains one worksheet, 169,890 data rows (plus the header row), and 51 columns.
- The inspected columns include ILL Record Number, ILL Date, ILL Year, Borrower Code, Library Type, borrower location fields, Format, Title, Author, ISBN, circulation counts, OCLC holdings, and lender/borrower transaction dates.

Relevance to this project:

The dataset can support analysis of interlibrary lending, material formats, publication information, and resource-sharing activity.

Important limitation:

This is institution-to-institution interlibrary-loan data. It does not provide a complete set of individual library-member accounts, ordinary item-level member check-outs, member reservations, or member fine/payment records.

Those parts of the proposed application must be supported by separately identified and appropriately sourced sample data or project test records. Such records must not be described as if they came from the Illinois dataset.

Source 6 — Technical Documentation: Oracle PL/SQL

Reference (APA 7):

Oracle. (2024). Oracle Database PL/SQL language reference, 21c.

https://docs.oracle.com/en/database/oracle/oracle-database/21/lnpls/

Type: Official technical documentation.

Notes:

- The documentation covers PL/SQL fundamentals, data types, control statements, records and collections, subprograms, triggers, packages, and error handling.
- These are the core programming features expected to be used in the database project.

Relevance to this project:

Provides the official technical reference for implementing procedures, functions, triggers, packages, and exception handling in Oracle Database 21c.

Follow-up: Consult the relevant chapters while implementing and testing each PL/SQL feature.

---

## 3. Initial Findings

1. Library circulation systems commonly support check-out, return, reservation/hold, overdue monitoring, and fine-related processes.
2. Existing systems such as Koha provide a useful functional reference, but this project will implement a smaller scope suitable for the course.
3. The selected Illinois dataset is publicly available under the CC0 licence stated on its dataset page.
4. The downloaded workbook has 169,890 data records and 51 columns. Its focus is interlibrary lending between institutions, not individual member circulation.
5. The Illinois dataset can be used for resource-sharing analysis, but it cannot by itself populate every planned application function. Any supplementary or synthetic records must be labelled honestly.
6. Oracle Database 21c PL/SQL documentation provides the technical basis for the planned stored-program features.

## 4. Initial Project Implications

The project database is expected to include entities such as:

- BOOKS
- AUTHORS
- CATEGORIES
- BOOK_COPIES
- MEMBERS
- LOANS
- RESERVATIONS
- FINES
- PAYMENTS
- INTERLIBRARY_LOANS

The final table structure must be confirmed during the later data modelling and normalization phase.

The Illinois dataset should be retained unchanged in the raw-data folder. A separate processed copy may be created later after data profiling, cleaning decisions, and documentation.

## 5. Research Status and Next Actions

- [x] Identify the registered dataset and open its official repository page.
- [x] Download the original Excel workbook.
- [x] Confirm the workbook sheet, row count, column count, and sample fields.
- [x] Identify six initial sources across the required source categories.
- [ ] Read both research papers in full and add useful findings.
- [ ] Read the ACRL report methodology and relevant tables.
- [ ] Review Koha circulation, holds, and fines documentation in more detail.
- [ ] Record further data-cleaning and data-quality findings.
- [ ] Finalize the research log after verifying all references and notes.

Last updated: 6 November 2026
