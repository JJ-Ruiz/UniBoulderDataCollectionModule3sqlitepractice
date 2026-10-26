# UniBoulderDataCollectionModule3sqlitepractice
Connecting to a SQLite Database, Fetching Its Data, and Loading It into a Pandas DataFrame
```markdown
# Connecting to a SQLite Database, Fetching Its Data, and Loading It into a Pandas DataFrame

A short practice exercise on collecting data from a SQLite database with Python.

## Dataset

`bike_rentals.sqlite` is a dummy dataset of city bike rentals (2021 to 2023). It contains one table, `bike_rentals_data`, with 15,482 rows and 10 columns:

| Column | Description |
|---|---|
| `rental_id` | Unique rental identifier |
| `user_id` | Customer identifier |
| `gender` | Female / Male |
| `age` | Customer age |
| `bike_type` | City, Mountain, Electric, Road or Cargo |
| `duration_minutes` | Length of the rental |
| `fare` | Price paid |
| `payment_method` | Credit Card, Debit Card, Mobile App, Cash or Subscription |
| `rental_date` | Date of the rental (dd/mm/yyyy, stored as text) |
| `station` | Rental station |

## Tasks

1. Establish the connection (`sqlite3.connect`, `connection.cursor`)
2. Find the table name through `sqlite_master`
3. Preview the data with `LIMIT 3` and check the types of the result and of each row
4. Fetch all records with `fetchall()` and count them with `len()`
5. Add the column names and create a pandas DataFrame
6. Check the first rows with `df.head()`
7. Save the DataFrame to `bike_rentals.csv` and close the connection
