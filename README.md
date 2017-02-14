# Database_Basics
Android_Assignment_7.1


a. What is the use of SQLite open helper class inSQLite?
Answer -> A helper class to manage database creation and version management.

b. What is the use of OnUpgrade function in SQLiteOpenHelper class?
Answer -> onUpgrade is basically for handling new db changes(could be new columns addition,table addition) for any new version of your app.
Droping the table is not always necessary in onUpgrade it all depends on what your use case is. If the requirment is to not to persists the data from your older version of app then drop should help,but if its like changing schema then it should only have alter scripts.

c. How to show SQLite database table information in Android application what is the best
way to do it?
Answer -> Use table layout with cursor
