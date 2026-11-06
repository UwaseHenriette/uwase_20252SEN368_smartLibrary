# Smart Library Circulation and Reservation System

## 1. Project Information

- Student Name: Uwase Henriette
- Student ID: 20252SEN368
- University: Adventist University of Central Africa (AUCA)
- Course: INSY 8311 – Database Development with PL/SQL
- Instructor: Eric Maniraguha
- Project: Smart Library Circulation and Reservation System

## 2. Project Overview

The Smart Library Circulation and Reservation System is a database-driven application designed to improve library operations by automating book borrowing, returns, reservations, and overdue fine management.

The system will use Oracle Database 21c, PL/SQL, and Oracle APEX to manage library records, monitor book availability, and generate useful reports.

## 3. Problem Statement

Many libraries face challenges managing book borrowing, returns, reservations, and overdue fines manually. These challenges can lead to inaccurate records, difficulties tracking book availability, delayed transactions, and poor management of library resources.

## 4. Proposed Solution

The proposed system will automate library circulation activities, maintain accurate book and member records, manage reservations, calculate overdue fines, and generate reports on book availability and borrowing trends.

## 5. Project Objectives

- Manage books, authors, categories, and book copies.
- Register and manage library members.
- Record book borrowing and returns.
- Manage book reservations.
- Calculate overdue fines automatically.
- Track available and borrowed books.
- Generate reports about library activities.
- Improve the accuracy and efficiency of library operations.

## 6. Technologies

- Database: Oracle Database 21c
- Programming Language: Oracle PL/SQL
- User Interface: Oracle APEX
- Version Control: Git and GitHub

## 7. Planned Database Tables

The proposed database will include:

1. BOOKS
2. AUTHORS
3. CATEGORIES
4. BOOK_COPIES
5. MEMBERS
6. LOANS
7. RESERVATIONS
8. FINES
9. PAYMENTS
10. INTERLIBRARY_LOANS

## 8. Planned PL/SQL Features

- Procedures: Book borrowing, returning, and reservation operations.
- Functions: Fine calculation and book availability checking.
- Triggers: Enforcing borrowing rules and updating overdue loan status.
- Cursors: Generating overdue book and popular book reports.
- Packages: Organizing library circulation and reservation operations.
- Exception Handling: Managing unavailable books, invalid transactions, and duplicate reservations.

## 9. Planned Innovation

An interactive Oracle APEX dashboard connected to Oracle Database 21c. It will support book circulation, reservations, overdue fine calculations, and real-time reports on book availability and borrowing trends.

## 10. Data Source

University of Illinois Library Interlibrary Loan Dataset:

https://databank.illinois.edu/datasets/IDB-6701059

This dataset will support lending and collection-utilization analysis. It contains interlibrary loan transactions and does not provide all the records required for ordinary library member borrowing and reservations. Additional appropriate sample or collected library records will be needed for those features.

## 11. Expected Results

The expected result is a functional library database application that improves book circulation, simplifies reservations, reduces manual record-keeping, and provides useful reports for library operations.

## 12. Project Status

Current Phase: Phase 0 – Research and Proposal

The project is currently in the planning and research stage. Database implementation and application development will follow in the subsequent phases.

## 13. Repository Structure

smartLibrary/
│
├── README.md
├── docs/
│   ├── research/
│   ├── proposal/
│   └── presentation/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── sql/
│   ├── tables/
│   ├── procedures/
│   ├── functions/
│   ├── triggers/
│   └── packages/
│
├── innovation/
└── screenshots/

## 14. References

- University of Illinois Library Interlibrary Loan Dataset: https://databank.illinois.edu/datasets/IDB-6701059
- Oracle Database Documentation: https://docs.oracle.com/en/database/
- Oracle APEX Documentation: https://docs.oracle.com/en/database/oracle/apex/

---

Developed by: Uwase Henriette
Student ID: 20252SEN368
Course: INSY 8311 – Database Development with PL/SQL
Academic Year: 2026–2027
