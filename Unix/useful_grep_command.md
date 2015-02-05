##Useful grep command

I used to use `find` command in the past for searching through files on unix system.

Here is the command:

```
find . -type f -exec grep -H -n "search_query" {} \;
```

it uses `grep` command in the `find` command, so why not using grep directly?

```
grep -RHin "search_query" .
```
