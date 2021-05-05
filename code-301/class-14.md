# DataBase Normalization:
- Database normalization is a process used to organize a database into tables and columns. The idea is that a table should be about a specific topic and that only those columns which support that topic are included. For example, a spreadsheet containing information about sales people and customers serves several purposes:
    - Identify sales people in your organization
    - List all customers your company calls upon to sell product
    - Identify which sales people call on specific customers
- Reasons for Normalization:
- There are three main reasons to normalize a database. The first is to minimize duplicate data, the second is to minimize or avoid data modification issues, and the third is to simplify queries. As we go through the various states of normalization, we’ll discuss how each form addresses these issues, but to start, let’s look at some data which hasn’t been normalized and discuss some potential pitfalls. Once these are understood, I think you’ll better appreciate the reason to normalize the data.
- Data Duplication and Modification Anomalies:
- Notice that for each SalesPerson, we have listed both the SalesOffice and OfficeNumber. This information is duplicated for each SalesPerson. Duplicated information presents two problems:

- It increases storage and decreases performance.
- It becomes more difficult to maintain data changes.
- For example: Consider if we move the Chicago office to Evanston, IL. To properly reflect this in our table, we need to update the entries for all the SalesPersons currently in Chicago. Our table is a small example, but you can see if it were larger, that potentially this could involve hundreds of updates.
- Also consider what would happen if John Hunt quits. If we remove his entry, then we lose the information for New York.
- Normalization:
    - here are three common forms of normalization: 1st, 2nd, and 3rd normal form. There are several additional forms, such as BCNF, but I consider those advanced, and not too necessary to learn in the beginning. The forms are progressive, meaning that to qualify for 3rd normal form, a table must first satisfy the rules for 2nd normal form, and 2nd normal form must adhere to those for 1st normal form. Before we discuss the various forms and rules in details, let’s summarize the various forms:

    - First Normal Form – The information is stored in a relational table and each column contains atomic values, and there are not repeating groups of columns.
    - Second Normal Form – The table is in first normal form and all the columns depend on the table’s primary key.
    - Third Normal Form – The table is in second normal form and all of its columns are not transitively dependent on the primary key.