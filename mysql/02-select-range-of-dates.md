# Select rows from a range of dates

If you need to select rows from a MySQL database table in a date range, you need to use a command like this:

```sh
SELECT * FROM [table] WHERE [date_column] >= '2017-01-01' AND [date_column] <= '2017-03-01';
```

Another way is to use this command:

```sh
SELECT * FROM [table] WHERE [date_column] BETWEEN >= '2017-01-01' AND '2017-03-01';
```

Change the [table] and [date_column] to meet your needs.
