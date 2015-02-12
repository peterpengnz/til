## Check database connection information in console

1. show current connected database

```
ActiveRecord::Base.connection.current_database
```

2. check the connection information

```
Connection.current
```

3. switch to different database schema for current connection

```
Connection.schema_name!
```

Replace the `schema_name` with the real name.
To list different schema, you search search for `!`

```
Connection.methods.grep /!/
```
