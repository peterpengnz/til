## List Files With Full Path

Sometimes we have few files that have some name, so file path would help us
to find out which file is which.

On Ubuntu we could use `readlink` command: 

`readlink - print resolved symbolic links or canonical file names`

Command:

`readlink -f views/*/_detail*.haml`
