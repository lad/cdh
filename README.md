Bash CD History Utility
-----------------------

```
~> cd
~> cdh
<empty>
~> cd /tmp
/tmp> cdh
0:/tmp
/tmp> cd /usr/local
0:/tmp
1:/usr/local
/usr/local> cd /etc
/etc> cdh
0:/tmp
1:/usr/local
2:/etc
/etc> cdcl 0
0:/usr/local
1:/etc
/etc> cd 0
/usr/local> cd 1
/etc> cdcl
<empty>
/usr/local> cd
~> cdh
<empty>
```
