Certainly! Here's a cheatsheet for SQLite command line commands:

1. **Open/Create Database**:
   ```
   sqlite3 [database_name]
   ```

2. **Exit SQLite**:
   ```
   .exit
   ```

3. **Show Tables**:
   ```
   .tables
   ```

4. **Show Table Schema**:
   ```
   .schema [table_name]
   ```

5. **Execute SQL Query**:
   ```
   SELECT * FROM [table_name];
   ```

6. **Display Column Headers**:
   ```
   .header on
   ```

7. **Display Query Output in Column Format**:
   ```
   .mode column
   ```

8. **Display Query Output in List Format**:
   ```
   .mode list
   ```

9. **Display Query Output in CSV Format**:
   ```
   .mode csv
   ```

10. **Save Query Results to a File**:
    ```
    .output [file_name]
    ```

11. **Import Data from CSV File**:
    ```
    .import [file_name.csv] [table_name]
    ```

12. **Execute SQL Commands from a File**:
    ```
    .read [file_name.sql]
    ```

13. **Show Current Settings**:
    ```
    .show
    ```

14. **Toggle Display of Query Execution Time**:
    ```
    .timer on
    ```

15. **Run SQLite in Interactive Mode** (Similar to Command Line, but within SQLite shell):
    ```
    sqlite3
    ```

16. **Execute SQL Commands Without Entering Interactive Mode** (Useful for scripting):
    ```
    sqlite3 [database_name] "SQL_COMMAND;"
    ```

These commands should cover most basic interactions with SQLite via the command line interface.
