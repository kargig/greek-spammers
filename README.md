greek-spammers
========================

Greek Spammers Email Addresses Blacklist

Collection of e-mail addresses of well-known spammers who send spam
messages either in Greek language or of Greek interest.

How to use
----------
```
$ git clone https://github.com/kargig/greek-spammers.git
$ sudo ln -rsf greek-spammers/grrbl_blacklist.cf /etc/spamassassin/
```

You should add a cron entry to perform a git pull every day in order to always have the latest version of the blacklist.

License
------
Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International
