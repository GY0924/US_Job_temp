# How to create fake github profile

## Download online repositories

## Update commit info.

How to replace old author info in past git commits?\
https://stackoverflow.com/questions/750172/how-do-i-change-the-author-and-committer-name-email-for-multiple-commits

Proven method:

```
git filter-repo --commit-callback '
    if commit.author_name == b"Ido Shemesh":
        commit.author_name = b"eric-barros"
        commit.author_email = b"e.mhz.barros@gmail.com"
        commit.committer_name = b"eric-barros"
        commit.committer_email = b"e.mhz.barros@gmail.com"
'
```



## Upload fake repositories.