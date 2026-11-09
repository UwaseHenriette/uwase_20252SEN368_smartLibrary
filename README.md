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

## 15. ### Phase I: Business Process Modeling

This phase focuses on modeling the university library's book borrowing process using BPMN 2.0. The diagram illustrates how students submit borrowing requests, how librarians verify eligibility, and how the library system checks book availability and records borrowing transactions. It also shows the possible outcomes, including successful borrowing, rejected requests, and unavailable books.
[View the book borrowing process diagram](https://viewer.diagrams.net/?tags=%7B%7D&lightbox=1&highlight=0000ff&edit=_blank&layers=1&nav=1&title=business_process_diagram.drawio&dark=auto#R%3Cmxfile%3E%3Cdiagram%20id%3D%22prtHgNgQTEPvFCAcTncT%22%20name%3D%22Page-1%22%3E7Vxbc9o4FP41PCbjGwYem1vT2bTbWbq7zdOOsAVWIywqywH661eyJXyNcYwvsLOZ6QQdZNn%2BvnPT0UlH5u1695GCjfeZuBCPDM3djcy7kWHoujnlv4RkH0vsqRULVhS5clIimKNfUAo1KQ2RC4PMREYIZmiTFTrE96HDMjJAKdlmpy0Jzt51A1awIJg7ABelfyOXebF0akwS%2BSNEK0%2FdWbdn8TdroCbLNwk84JJtSmTej8xbSgiLP613txAL8BQu8XUPb3x7eDAKfVbnAvfLbv%2Flt4kzmS6etq%2BBCz8%2Fjq%2F0WXEZuXLA9gqEYIvWGPh8dOOxNeZCnX90PITdJ7AnobgwYMB5UaMbCgNO5Ve1qp4TfQZCQTSxHqHoF%2FEZwFLA16FM6oGRnTEXt5DT4md8BTiUz%2Finj14hDRDbczlGCwroXk6ClMFd6t0kPh8hWUMmZmleikJ7LAnbJnzPlEwuY8vhXimrHAOpbavD0gkh%2FIPk5B38KD2DbkFNE8IqmQ1ISB1YdQurwLe421wOCWUeWREf4PtEekNJ6LvQlWQkc54I2Ui%2Bf0DG9pJIEDKSVR7oux%2BEefKhTyLN4pIHhHGGX64LK1j1loZdUIRyhinEgHENyTqItukyx93TNR2YLgeDIEBOhjG9PmOmNShB0%2B4Jsi%2BcIPtEgqJL%2BcOAfWrChiCfBamVvwpB4lH1adalmlYumuXmW1rlfP4hfoJEVQ6vcoI31t6rLMdiaEW0eyvQzVnoirs3iW2HZCQd28xsbDM6i2WNneMhhTpqe%2BYQtlc3VllnFasUVvXRT4GKMU%2FABXhbDzE434CIli3fA5RBk9FervAj80O0nlRkzYfQDcQ78n8LQl4a6fakRLWzmm1lXUZ3im41RzarjEfQXXJH8QDWCIs3eoT4FTLkAPmFVFfdkONbggmNbmJq0Q%2BXA4xWvggZ%2FDkhLeULAup40c6JCqx8VzwvxGKvdSJh0yJhes4X6bOcl%2B%2BKMtPs3DeZJWZ0UXmBcVbuy6wbiy%2FAyCh0oABMGJMgC%2FmruKSxRHTNsST%2BwfQoZCEVQxcw2JrZ6TlHafRldsYQMeieIxlFoNh1aRJ%2Bty04Z%2FliwbinuPPuvUwH6elTVHpBwG%2BE5kHVaiSoCs7u8Jw1DgqqhvZf3yyqasSZBAUFZ32Czjco%2FFEaFCj8GcKAHeKB40HnJZNMQ74yWiDMGpY%2FiwY4zSVlHUQH7fGvn%2FOru3%2FmwHnSbj%2Bufkwfb6%2Ba52S1zW%2BYYtoOse%2Bpz89iqeuxHN2p0ng02KuBzxH9nh6krhLD5LJopK5z4RKEmD2BBcQ3wHlZRU%2BvNDI%2B%2FSjxB9885NfwCaW0vaFkrXuA0psrDyDPg8BC8VqSLlYpXU4jIvyyLBYsWBgadwL4g%2FxijVw3Vhhx8iGfRHAia2F88fHNaHzHJcj3IEXsG9yp05JavBV8xpffa9t8KR3ykivtmueEetbK3yYsV6FTU8hyGUBWYLSNOtz0BDfvkfUiDM7CxX8SRQ%2FmwRL%2FLR73oS0HbucSqHFfDrxVD%2F62s%2Bnbgb%2FDOI96y%2BG21VV4dp5AFV6awh9xTak022lgByXHuPnykjnJGcK4K1Rr11qLsB4BMot6AVYUBCFMtrpck1O%2Bph1UjRyqY6snVOtXD0q8RN3qQeCBDfzkB8iFKvAHm7jTZIl2AviKAkOSrcfq3bDGMDtaYzBzhVLd6sqn6z2coA7SkdAwU268cx6sc6Gc1sa1jjPvXGgYqyt6F86GM5WTN97rlNQBL2iz83w%2Fr%2B1Nj%2Bx2TNuevE1S%2F%2FubuoGt%2B0KuAC%2FYBwyuG0UuQ3t3Pdcad3ba0LiZThFy%2FJBv6Ga6Vpp%2Fzqaea9Y%2BSTcKuJ9bPVdVamUmDl4BwmCBMOqsUNtFw0NpHGl%2BTlLbrgY5J2lznz%2FYQUn51ml8Yurwf%2BYgM4eshQ2TRJQndz1Eu4u3Sv28dmEq3jXP6CeXbJftHV9oE9vIWOaxfuU%2B03uz9il1SVZzRscXKDm%2ByCY1uFlnklXMaKxcmcvu6eRCN9p0nlUJwQX7Tv2sfGftM8GiUdUwpTILKby%2BQ2HUlZc7w3AIdRsZREmKf2i%2BUK16feX4%2BrsNoH18w42r8CVx0wtgYeSEyAH0hiX2GlDbvUF9QnxoC2qJcOif5tJrwGoafR1dWI2delmNu9JK%2Bq7%2FqOaga3tmjjINQjN7MqpuEYpGX3kCx1EWgb5%2B31DdQGEOGResVv8ms%2FJ4d5g2sqR17HmU6hw70kZ2PdWnaU3Re9SSiob%2B9rWED5M%2Fso9T%2BOS%2FKjDv%2FwU%3D%3C%2Fdiagram%3E%3C%2Fmxfile%3E#%7B%22pageId%22%3A%22prtHgNgQTEPvFCAcTncT%22%7D)

---

Developed by: Uwase Henriette
Student ID: 20252SEN368
Course: INSY 8311 – Database Development with PL/SQL
Academic Year: 2026–2027
