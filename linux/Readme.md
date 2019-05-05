```
Command to listout client IP of current ssh connections?
]#pinky
 or
]# echo $SSH_CLIENT
  or
]# echo $SSH_CONNECTION
```

```
Check out Client IPs connected to specific app using specific port
eg:(jenkins:8080)
]# lsof -i :8080
```
```
ADD a new with "Its begining" line in the begining of file and at end "Its End!"
awk 'BEGIN {print "Its begining"}
{print $0}
'END {print "Its End!"}' myfile.txt
```
```
awk 'BEGIN{FS=":"; OFS="-"} {print $1,$6,$7}' /etc/passwd
*FS     Specifies the field separator.
*OFS  Specifies the Output separator.
```
```
Print Last field of a file
awk 'BEGIN{FS=":"; OFS=":"} {print $1,$NF}' /etc/passwd
```
```
awk 'BEGIN {FS=","}
> {print $1,"FNR="FNR,"NR="NR}
> END{print "Total",NR,"processed lines"}' db.txt db.txt

John FNR=1 NR=1
Barbi FNR=2 NR=2
Mitch FNR=3 NR=3
Tim FNR=4 NR=4
Lisa FNR=5 NR=5
John FNR=1 NR=6
Barbi FNR=2 NR=7
Mitch FNR=3 NR=8
Tim FNR=4 NR=9
Lisa FNR=5 NR=10
*NR    Retrieves total count of processed records.
*FNR     The record which is processed.
```
