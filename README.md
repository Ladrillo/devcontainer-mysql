# MySQL DevContainer

1. Create an `.env` file and place it inside the `.devcontainer` folder.

    ```text
    MYSQL_ROOT_PASSWORD=1234
    MYSQL_PASSWORD=1234
    MYSQL_USER=user
    MYSQL_DATABASE=name
    ```

    Replace `user`, `name`, and `1234` with desired values.

2. Reopen the project in a dev container.

3. Run the following in order to connect (replacing `user` with actual user):

    ```bash
    mysql -u user -p -h mysql
    ```

4. Set up your database, (replacing `/the/path/` with the actual path to the sql files):

    ```sql
    SOURCE /the/path/northwind_ddl.sql;
    SOURCE /the/path/northwind_data.sql;
    ```
