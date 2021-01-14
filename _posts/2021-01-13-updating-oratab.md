*** Updating /etc/oratab
Starting with Oracle 12c Oct 2019 PSU, the PSU patching removes any entries in /etc/oratab with the keyword "added by Agent".
Oracle 19c installer does not update /etc/oratab at all. Since many of the home grown scripts depend on /etc/oratab to locate Oracle software home,
I came up with [this](https://gist.github.com/vinayakrk/123ac9519df06d4c7bed4a21e9d900c0) simple script to update /etc/oratab in a RAC environment.
