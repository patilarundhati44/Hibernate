## Hibernate CRUD Project (Regions & Countries)

This is a simple Java console application that demonstrates how to perform CRUD operations using Hibernate Native API (Session) on a PostgreSQL database.

It covers:
- Hibernate configuration
- `Region` and `Country` entities
- Insert, Read, Update, Delete (CRUD) using Hibernate

---


##  Technologies Used

- Java 17+
- Hibernate ORM 6+
- PostgreSQL
- Maven (build tool)
- Eclipse IDE

---

##  Database Tables

Before running the project, create the following tables in PostgreSQL:

```sql
CREATE TABLE regions (
    region_id SERIAL PRIMARY KEY,
    region_name VARCHAR(25)
);

CREATE TABLE countries (
    country_id CHAR(2) PRIMARY KEY,
    country_name VARCHAR(40),
    region_id INT NOT NULL REFERENCES regions(region_id)
);
```

## Author

Name : Arundati Anand Patil

Email : patilarundati44@gmail.com
