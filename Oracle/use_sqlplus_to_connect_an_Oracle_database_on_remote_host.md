##Use sqlplus to connect an Oracle database on remote host

I want to connect to an oracle database located on another host by using sqlplus.

Here is the command:

```
sqlplus user/pass@(DESCRIPTION=(ADDRESS=(PROTOCOL=TCP)(Host=hostname.network)(Port=1521))(CONNECT_DATA=(SID=remote_SID)))
```
