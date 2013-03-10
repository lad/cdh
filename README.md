Bash CD History Utility
-----------------------

```
~> cd
~> cdh
0:/home/louis
~> cd /tmp
/tmp> cdh
0:/home/louis 1:/tmp
/tmp> cd /usr/local
0:/home/louis 1:/tmp 2:/usr/local
/usr/local> cdcl 0
0:/tmp 1:/usr/local
/usr/local> cd 0
/tmp> cd 1
/usr/local> cdcl
<empty>
/usr/local> cdh
<empty>
```
