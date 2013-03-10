Bash CD History Utility
-----------------------

Replacement for the **cd** command which maintains a history of the directories
visited to allow easy recall. In addition the command **cdh** show the cd
history and **cdcl** clears one or more entries from the history.

Entries in a cd history list can be access by their index in the list:

```
# cdh
0: /tmp
1: /usr
2: /etc
# cd 0
# pwd
/tmp
```

Negative numbers index from the end of the history list:

```
# cdh
0: /tmp
1: /usr
2: /etc
# cd -2
# pwd
/usr
```

**cdcl** without arguments will clear the history list or an index can be
supplied to remove a single element. As with **cd** a postive or negative
index can be supplied

```
# cdh
0: /tmp
1: /usr
2: /etc
3: /usr/local/bin
# cdcl 0
0: /usr
1: /etc
2: /usr/local/bin
# cdcl -2
0: /usr
1: /usr/local/bin
# cdcl
<empty>


If **cd <index>** is used in a directory that contains a directory that matches
"<index>" exactly it cd's into that directory and behaves as the bash builtin
would behave.
