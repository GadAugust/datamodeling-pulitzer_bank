# datamodeling_case-study1-pulitzer_bank
![pulitzer_bank](https://github.com/GadAugust/datamodeling_case-study1-pulitzer_bank/assets/81167692/e718d591-4711-4718-b3fc-4320abfc7030)


Pulitzer Bank, a conglomerate with numerous branches, faces a challenge in managing vast customer data spread across its network. Fragmented systems hinder a unified view of customer relationships, leading to inefficiencies in understanding customer behavior and preferences.

At the heart of the Bank’s operations lay a pivotal challenge: managing the vast array of
customer data across its extensive network. With customers holding multiple accounts
and loans across different branches, maintaining a unified view of customer relationships
proved to be a Herculean task. Data was scattered across disparate systems within each
branch, leading to fragmentation and inefficiencies in understanding customer behavior
and preferences.

## TASK OVERVIEW
I will get into the shoes of a Data Engineer at the Bank's headquarters.  Tasked with unraveling the
complexities of customer data to drive strategic decision-making and enhance customer
experiences.

The first task is to design a data model to visualize the intricate web of relationships in
the organization data.

## Tasks for Pulitzer Bank Data Model:
1. Identify all Entities for Pulitzer Bank
2. Find and show all relationships between Entities
3. Identify the key attributes for every Entity
4. Identify the Keys for each attribute (Select a Primary Key)
5. Identify other relevant attributes for each Entity
6. Draw a complete E-R Diagram with all Entities, attributes, and relationships showing Primary and Foreign Keys
7. Review your Data Model with your Stakeholders and Business users
   
# REQUIREMENT GATHERING

## Design Principles
The data model is designed to be scalable, efficient, and adaptable to the dynamic nature of customer relationships. It adheres to best practices in data modeling and database design, ensuring data integrity and accessibility.

## The Business Entities
- Bank:Banks in the conglomerate
- Customer: Represents individuals or entities holding accounts and loans with Pulitzer Bank.
- Account: Represents individual accounts held by customers
- Branch: Represents physical locations of Pulitzer Bank branches.
- Transaction: Represents financial transactions conducted by customers at branches.
- Loans: Represents individuals or entities holding loans/ loan accounts with Pulitzer Bank.
- Employee: Employees of pulitzer
- Grade_level: grades for Employees
- Account_types: including savings, checking, and loan accounts.

  ## The Entity Relations
- Bank to Branch(One_to_many relationship)
- Customers to Account(one_to_many relationship)
- Transaction to account(many_to_one relationship)
- Loan to account (many_to_one relationship)
- Branch to account(many_to _one relationship)
- Employee to bank(one_to_many relationship)

 ## The Entity Attributes
- Bank(bank_code(PK),name,ceo_id)
- Branch(branch_id, bank_code FK, address, manager_id(FK), GL_account,
- Transaction(transaction_ref_no(pk), account_no(FK), cust_no, related_account,transaction_date, transaction_type,
- customer(customer_no PK, name, address, email, date_of_birth,phone_no,gender
- Account(account_no(PK), customer_no(FK), account_name,account_type_id,account_officer_id(FK),is_active, is_blocked)
- Loan(loan_ref_no PK,settelement_account FK, customer_no, booking_date, due_date, branch_id, classifiaction)
- Employee(emp_id PK, name, address, email, date_of_birth, hire_date, gender,branch_id FK, is_active, grade_level_name)

  



