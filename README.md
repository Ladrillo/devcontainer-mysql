# MySQL DevContainer

1. Create an `.env` file and place it inside the `.devcontainer` folder.

    ```text
    MYSQL_ROOT_PASSWORD=1234
    MYSQL_PASSWORD=1234
    MYSQL_USER=ladygaga
    MYSQL_DATABASE=gagadb
    ```

    Replace `ladygaga`, `gagadb`, and `1234` with desired values.

2. Reopen the project in a dev container.

3. Run the following in order to connect (replacing `ladygaga` with the actual user):

    ```bash
    mysql -u ladygaga -p -h mysql
    ```

4. Set up your database, (replacing `gagadb` and `/the/path/` with the real thing):

    ```sql
    USE gagadb;
    SOURCE /the/path/northwind_ddl.sql;
    SOURCE /the/path/northwind_data.sql;
    ```
