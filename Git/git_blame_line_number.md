## Git blame command accepts a commit which specifies the starting point of the search.

so you can do following:

```
git blame -L6,+3 "04038dee^" app/views/another_view_folder/_a_random_file_name.haml
```

Check [Here](http://zsoltfabok.com/blog/2012/02/git-blame-line-history/) more a real world use case example :)
