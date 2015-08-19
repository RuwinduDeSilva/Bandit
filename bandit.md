**Name** - Ruwindu De Silva  
**SLIIT ID** - IT12044528  
**Curtin ID** - 18297188  
## Bandit 0 to 1
  
Open a SSH session to bandit.labs.overthewire.org using putty.  
Both the user name and the password is **"bandit0"**  
  
```
bandit0@melinda:~$ ls
readme
bandit0@melinda:~$ cat readme
```
readme file has the password to bandit1 and it is
```
boJ9jbbUNNfktd78OOpsqOltutMc3MY1
```  
## Bandit 1 to 2

Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit1"** and the above password **boJ9jbbUNNfktd78OOpsqOltutMc3MY1**

```
bandit1@melinda:~$ ls
-
bandit1@melinda:~$ cat ./-
```
File name **"-"** has the bandit2 password and it is
```
CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9
```

## Bandit 2 to 3

Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit2"** and the above password **CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9**  

```
bandit2@melinda:~$ ls
spaces in this filename
bandit2@melinda:~$ cat spaces\ in\ this\ filename
UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK
```
password for bandit 3 is **"UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK"**

## Bandit 3 to 4

Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit3"** and the above password **UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK**  

```
bandit3@melinda:~$ ls
inhere
bandit3@melinda:~$ cd inhere/
bandit3@melinda:~/inhere$ ls
bandit3@melinda:~/inhere$ ls -a
.  ..  .hidden
bandit3@melinda:~/inhere$ cat ./.hidden
pIwrPrtPN36QITSp3EQaw936yaFoFgAB
bandit3@melinda:~/inhere$
```

password for bandit 4 is **"pIwrPrtPN36QITSp3EQaw936yaFoFgAB"**  


## Bandit 4 to 5
Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit4"** and the above password **pIwrPrtPN36QITSp3EQaw936yaFoFgAB** 

```
bandit4@melinda:~$ ls
inhere
bandit4@melinda:~$ cd inhere/
bandit4@melinda:~/inhere$ ls -h
-file00  -file02  -file04  -file06  -file08
-file01  -file03  -file05  -file07  -file09
bandit4@melinda:~/inhere$ cat ./-file00
;▒-▒(▒▒z▒▒У▒▒ޘ▒▒8鑾bandit4@melinda:~/inhere$


bandit4@melinda:~/inhere$ cat ./-file01
?▒@c
    O8▒L▒c▒Ч7▒zb~▒▒ף▒▒U▒bandit4@melinda:~/inhere$
.
.
.
bandit4@melinda:~/inhere$ cat ./-file07
koReBOKuIDDepwhWk7jZC0RTdopnAYKh
```
-file07 contains the password for the next level.

password for bandit 5 is **"koReBOKuIDDepwhWk7jZC0RTdopnAYKh"**

## Bandit 5 to 6
Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit5"** and the above password **koReBOKuIDDepwhWk7jZC0RTdopnAYKh** 

```
bandit5@melinda:~$ ls
inhere
bandit5@melinda:~$ cd inhere/
bandit5@melinda:~/inhere$ ls
maybehere00  maybehere04  maybehere08  maybehere12  maybehere16
maybehere01  maybehere05  maybehere09  maybehere13  maybehere17
maybehere02  maybehere06  maybehere10  maybehere14  maybehere18
maybehere03  maybehere07  maybehere11  maybehere15  maybehere19

bandit5@melinda:~/inhere$ find -readable -size 1033c ! -executable
./maybehere07/.file2
bandit5@melinda:~/inhere$ cat ./maybehere07/.file2
DXjZPULLxYr17uwoI01bNLQbtFemEgo7
```
password for bandit 6 is **"DXjZPULLxYr17uwoI01bNLQbtFemEgo7"**


## Bandit 6 to 7
Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit6"** and the above password **DXjZPULLxYr17uwoI01bNLQbtFemEgo7** 

```
bandit6@melinda:/$ find / -user bandit7 -group bandit6 -size 33c 2>&1 | grep -v -F Permission
find: `/proc/29160/task/29160/fd/5': No such file or directory
find: `/proc/29160/task/29160/fdinfo/5': No such file or directory
find: `/proc/29160/fd/5': No such file or directory
find: `/proc/29160/fdinfo/5': No such file or directory
/var/lib/dpkg/info/bandit7.password
bandit6@melinda:/$ cat /var/lib/dpkg/info/bandit7.password
HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs
```

password for bandit 7 is **"HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs"**


## Bandit 7 to 8
Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit7"** and the above password **HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs**

```
bandit7@melinda:~$ ls
data.txt
bandit7@melinda:~$ grep -e 'millionth' data.txt
millionth       cvX2JJa4CFALtqS87jk27qwqGhBM9plV
```

password for bandit 8 is **"cvX2JJa4CFALtqS87jk27qwqGhBM9plV"**


## Bandit 8 to 9
Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit8"** and the above password **cvX2JJa4CFALtqS87jk27qwqGhBM9plVK** 

```
bandit8@melinda:~$ ls
data.txt
bandit8@melinda:~$ sort data.txt | uniq -u
UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR
```

password for bandit 9 is **"UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR"**

## Bandit 9 to 10
Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit9"** and the above password **UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK** 

```
bandit9@melinda:~$ ls
data.txt
bandit9@melinda:~$ strings data.txt | grep "="
epr~F=K
7?YD=
?M=HqAH
/(Ne=
C=_"
I========== the6
z5Y=
`h(8=`
n\H=;
========== password
========== ism
N$=&
l/a=L)
f=C(
========== truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk
ie)=5e
bandit9@melinda:~$
```
password for bandit 10 is **"truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk"**


## Bandit 10 to 11
Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit10"** and the above password **truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk** 

```
bandit10@melinda:~$ ls
data.txt
bandit10@melinda:~$ base64 -d data.txt
The password is IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR
bandit10@melinda:~$
```
password for bandit 11 is **"IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR"**


## Bandit 11 to 12
Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit11"** and the above password **IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR**

```
bandit11@melinda:~$ ls
data.txt
bandit11@melinda:~$ cat data.txt | tr a-zA-Z n-za-mN-ZA-M
The password is 5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu
bandit11@melinda:~$
```

password for bandit 12 is **"5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu"**



## Bandit 12 to 13
Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit12"** and the above password **5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu** 

```
bandit12@melinda:~$ cd ..
bandit12@melinda:/home$ cd ..
bandit12@melinda:/$ cd tmp
bandit12@melinda:/tmp$ mkdir arp
bandit12@melinda:/tmp$ cp /home/bandit12/data.txt /tmp/arp
bandit12@melinda:/tmp$ cd arp
bandit12@melinda:/tmp/arp$ ls
data.txt
bandit12@melinda:/tmp/arp$ file data.txt
data.txt: ASCII text
bandit12@melinda:/tmp/arp$ xxd -r data.txt >bandit
bandit12@melinda:/tmp/arp$ ls
bandit  data.txt
bandit12@melinda:/tmp/arp$ file bandit
bandit: gzip compressed data, was "data2.bin", from Unix, last modified: Fri Nov 14 10:32:20 2014, max compression
bandit12@melinda:/tmp/arp$ mv bandit bandit.gz
bandit12@melinda:/tmp/arp$ ls
bandit.gz  data.txt
bandit12@melinda:/tmp/arp$ file bandit.gz
bandit.gz: gzip compressed data, was "data2.bin", from Unix, last modified: Fri Nov 14 10:32:20 2014, max compression
bandit12@melinda:/tmp/arp$ gzip -d bandit.gz
bandit12@melinda:/tmp/arp$ ls
bandit  data.txt
bandit12@melinda:/tmp/arp$ file bandit
bandit: bzip2 compressed data, block size = 900k
bandit12@melinda:/tmp/arp$ mv bandit bandit.bz2
bandit12@melinda:/tmp/arp$ ls
bandit.bz2  data.txt
bandit12@melinda:/tmp/arp$ bzip2 -d bandit.bz2
bandit12@melinda:/tmp/arp$ ls
bandit  data.txt
bandit12@melinda:/tmp/arp$ file bandit
bandit: gzip compressed data, was "data4.bin", from Unix, last modified: Fri Nov 14 10:32:20 2014, max compression
bandit12@melinda:/tmp/arp$ mv bandit bandit.gz
bandit12@melinda:/tmp/arp$ ls
bandit.gz  data.txt
bandit12@melinda:/tmp/arp$ gzip -d bandit.gz
bandit12@melinda:/tmp/arp$ ls
bandit  data.txt
bandit12@melinda:/tmp/arp$ file bandit
bandit: POSIX tar archive (GNU)
bandit12@melinda:/tmp/arp$ tar -xvf bandit
data5.bin
bandit12@melinda:/tmp/arp$ file data5.bin
data5.bin: POSIX tar archive (GNU)
bandit12@melinda:/tmp/arp$ tar -xvf data5.bin
data6.bin
bandit12@melinda:/tmp/arp$ file data6.bin
data6.bin: bzip2 compressed data, block size = 900k
bandit12@melinda:/tmp/arp$ mv data6.bin bandit.bz2
bandit12@melinda:/tmp/arp$ ls
bandit  bandit.bz2  data.txt  data5.bin
bandit12@melinda:/tmp/arp$ bzip2 -d bandit.bz2
bzip2: Output file bandit already exists.
bandit12@melinda:/tmp/arp$ rm bandit
bandit12@melinda:/tmp/arp$ bzip2 -d bandit.bz2
bandit12@melinda:/tmp/arp$ ls
bandit  data.txt  data5.bin
bandit12@melinda:/tmp/arp$ file bandit
bandit: POSIX tar archive (GNU)
bandit12@melinda:/tmp/arp$ tar -xvf bandit
data8.bin
bandit12@melinda:/tmp/arp$ file data8.bin
data8.bin: gzip compressed data, was "data9.bin", from Unix, last modified: Fri Nov 14 10:32:20 2014, max compression
bandit12@melinda:/tmp/arp$ mv data8.bin data8.gz ; gzip -d data8.gz
bandit12@melinda:/tmp/arp$ file data8
data8: ASCII text
bandit12@melinda:/tmp/arp$ cat data8

The password is 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL
```

password for bandit 13 is **"8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL"**



## Bandit 13 to 14
Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit13"** and the above password **8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL** 

```
bandit13@melinda:~$ ls
sshkey.private
bandit13@melinda:~$ man ssh
bandit13@melinda:~$ ssh sshkey.privat bandit14@localhost
ssh: Could not resolve hostname sshkey.privat: Name or service not known
bandit13@melinda:~$ man ssh
bandit13@melinda:~$ ssh -i sshkey.private bandit14@localhost
Could not create directory '/home/bandit13/.ssh'.
The authenticity of host 'localhost (127.0.0.1)' can't be established.
ECDSA key fingerprint is 05:3a:1c:25:35:0a:ed:2f:cd:87:1c:f6:fe:69:e4:f6.
Are you sure you want to continue connecting (yes/no)? yes
```
This will log to the bandit14 through secure shell.

```
bandit14@melinda:~$ ls
bandit14@melinda:~$ cat  /etc/bandit_pass/bandit14
4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e
bandit14@melinda:~$
```

password for bandit 14 is **"4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e"**


## Bandit 14 to 15
Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit14"** and the above password **4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e** 

```
bandit14@melinda:~$ man nc
bandit14@melinda:~$ echo 4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e | nc -v localhost 30000
Connection to localhost 30000 port [tcp/*] succeeded!
Correct!
BfMYroe26WYalil77FoDi9qh59eK5xNr

bandit14@melinda:~$
```

password for bandit 15 is **"BfMYroe26WYalil77FoDi9qh59eK5xNr"**


## Bandit 15 to 16
Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit15"** and the above password **BfMYroe26WYalil77FoDi9qh59eK5xNr** 

```
bandit15@melinda:~$ man openssl
bandit15@melinda:~$ echo BfMYroe26WYalil77FoDi9qh59eK5xNr | openssl s_client -quiet -connect localhost:30001depth=0 CN = li190-250.members.linode.com
verify error:num=18:self signed certificate
verify return:1
depth=0 CN = li190-250.members.linode.com
verify return:1
Correct!
cluFn7wTiGryunymYOu4RcffSxQluehd

read:errno=0
bandit15@melinda:~$
```

password for bandit 16 is **"cluFn7wTiGryunymYOu4RcffSxQluehd"**


## Bandit 16 to 17
Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit16"** and the above password **cluFn7wTiGryunymYOu4RcffSxQluehd**

Find the listening ports.
```
bandit16@melinda:~$ nmap -p 31000-32000 localhost

Starting Nmap 6.40 ( http://nmap.org ) at 2015-08-19 18:20 UTC
Nmap scan report for localhost (127.0.0.1)
Host is up (0.0014s latency).
Not shown: 996 closed ports
PORT      STATE SERVICE
31046/tcp open  unknown
31518/tcp open  unknown
31691/tcp open  unknown
31790/tcp open  unknown
31960/tcp open  unknown

Nmap done: 1 IP address (1 host up) scanned in 0.09 seconds
```
Find correct port among other listening ports
```
bandit16@melinda:~$ echo cluFn7wTiGryunymYOu4RcffSxQluehd | openssl s_client -quiet -connect localhost:31790
depth=0 CN = li190-250.members.linode.com
verify error:num=18:self signed certificate
verify return:1
depth=0 CN = li190-250.members.linode.com
verify return:1
Correct!
```
Get the password
```
bandit16@melinda:~$ mkdir -p /tmp/key/
bandit16@melinda:~$ cd /tmp/key
bandit16@melinda:/tmp/key$ touch sshkey.private
bandit16@melinda:/tmp/key$ vim sshkey.private
bandit16@melinda:/tmp/key$ ssh -i ./sshkey.private bandit17@localhost
Could not create directory '/home/bandit16/.ssh'.
The authenticity of host 'localhost (127.0.0.1)' can't be established.
ECDSA key fingerprint is 05:3a:1c:25:35:0a:ed:2f:cd:87:1c:f6:fe:69:e4:f6.
Are you sure you want to continue connecting (yes/no)? yes
.
.
.
bandit17@melinda:~$
```  
Now we are in the bandit17


## Bandit 17 to 18
This continues with the bandit 16 to 17.  
Enter following commands...

```
bandit17@melinda:~$ ls
passwords.new  passwords.old
bandit17@melinda:~$ diff passwords.new passwords.old
42c42
< kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd
---
> BS8bqB1kqkinKJjuxL6k072Qq9NRwQpR
```

password for bandit 18 is **"kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd"**



## Bandit 18 to 19
Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit218"** and the above password **kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd**   
This will close the terminal bt prompting **"Byebye!"**  
connect to the bandit18 by using following command...

```
ssh -t bandit18@bandit.labs.overthewire.org /bin/sh
```
password is **kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd** 

```
ls
cat readme
IueksS7Ubh8G3DCwVzrTd8rAVOwq3M5x
```
password for bandit 19 is **"IueksS7Ubh8G3DCwVzrTd8rAVOwq3M5x"**

## Bandit 19 to 20
Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit19"** and the above password **IueksS7Ubh8G3DCwVzrTd8rAVOwq3M5x** 

```
bandit19@melinda:~$ ls
bandit20-do
bandit19@melinda:~$ ll
total 28
drwxr-xr-x   2 root     root     4096 Nov 14  2014 ./
drwxr-xr-x 167 root     root     4096 Jul  9 16:27 ../
-rw-r--r--   1 root     root      220 Apr  9  2014 .bash_logout
-rw-r--r--   1 root     root     3637 Apr  9  2014 .bashrc
-rw-r--r--   1 root     root      675 Apr  9  2014 .profile
-rwsr-x---   1 bandit20 bandit19 7370 Nov 14  2014 bandit20-do*
bandit19@melinda:~$ ./bandit20-do --help
Usage: env [OPTION]... [-] [NAME=VALUE]... [COMMAND [ARG]...]
Set each NAME to VALUE in the environment and run COMMAND.

Mandatory arguments to long options are mandatory for short options too.
  -i, --ignore-environment  start with an empty environment
  -0, --null           end each output line with 0 byte rather than newline
  -u, --unset=NAME     remove variable from the environment
      --help     display this help and exit
      --version  output version information and exit

A mere - implies -i.  If no COMMAND, print the resulting environment.

Report env bugs to bug-coreutils@gnu.org
GNU coreutils home page: <http://www.gnu.org/software/coreutils/>
General help using GNU software: <http://www.gnu.org/gethelp/>
Report env translation bugs to <http://translationproject.org/team/>
For complete documentation, run: info coreutils 'env invocation'
bandit19@melinda:~$ ./bandit20-do cat /etc/bandit_pass/bandit20
GbKksEFF4yrVs6il55v6gwY5aVje5f0j
```
password for bandit 20 is **"GbKksEFF4yrVs6il55v6gwY5aVje5f0j"**


## Bandit 20 to 21
Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit20"** and the above password **GbKksEFF4yrVs6il55v6gwY5aVje5f0j** 

```
bandit20@melinda:~$ ls
suconnect
bandit20@melinda:~$ ./suconnect
Usage: ./suconnect <portnumber>
This program will connect to the given port on localhost using TCP. If it receives the correct password from the other side, the next password is transmitted back.
bandit20@melinda:~$ nc -l 32123 < /etc/bandit_pass/bandit20
gE269g2h3mw3pwgrj0Ha9Uoqen1c9DGr
bandit20@melinda:~$
```  
Then start another ssh session and enter the following commands...
```
bandit20@melinda:~$ ./suconnect 32123
Read: GbKksEFF4yrVs6il55v6gwY5aVje5f0j
Password matches, sending next password
bandit20@melinda:~$
```
password for bandit 21 is **"gE269g2h3mw3pwgrj0Ha9Uoqen1c9DGr"**

## Bandit 21 to 22
Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit21"** and the above password **gE269g2h3mw3pwgrj0Ha9Uoqen1c9DGr** 
```
bandit21@melinda:~$ cd /etc/cron.d
bandit21@melinda:/etc/cron.d$ ls
behemoth4_cleanup      leviathan5_cleanup     natas25_cleanup~  semtex0-ppc
cron-apt               manpage3_resetpw_job   natas26_cleanup   semtex5
cronjob_bandit22       melinda-stats          natas27_cleanup   sysstat
cronjob_bandit23       natas-session-toucher  php5              vortex0
cronjob_bandit24       natas-stats            semtex0-32        vortex20
cronjob_bandit24_root  natas25_cleanup        semtex0-64
bandit21@melinda:/etc/cron.d$ cat cronjob_bandit22
* * * * * bandit22 /usr/bin/cronjob_bandit22.sh &> /dev/null
bandit21@melinda:/etc/cron.d$
bandit21@melinda:/etc/cron.d$
bandit21@melinda:/etc/cron.d$
bandit21@melinda:/etc/cron.d$
bandit21@melinda:/etc/cron.d$  cat /usr/bin/cronjob_bandit22.sh
#!/bin/bash
chmod 644 /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
cat /etc/bandit_pass/bandit22 > /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
bandit21@melinda:/etc/cron.d$
bandit21@melinda:/etc/cron.d$
bandit21@melinda:/etc/cron.d$
bandit21@melinda:/etc/cron.d$ cat /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
Yk7owGAcWjwMVRwrTesJEwB7WVOiILLI
bandit21@melinda:/etc/cron.d$
```
password for bandit 22 is **"Yk7owGAcWjwMVRwrTesJEwB7WVOiILLI"**


## Bandit 22 to 23
Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit22"** and the above password **Yk7owGAcWjwMVRwrTesJEwB7WVOiILLI** 
```
bandit22@melinda:~$ cd /etc/cron.d/
bandit22@melinda:/etc/cron.d$
bandit22@melinda:/etc/cron.d$
bandit22@melinda:/etc/cron.d$ ls
behemoth4_cleanup      leviathan5_cleanup     natas25_cleanup~  semtex0-ppc
cron-apt               manpage3_resetpw_job   natas26_cleanup   semtex5
cronjob_bandit22       melinda-stats          natas27_cleanup   sysstat
cronjob_bandit23       natas-session-toucher  php5              vortex0
cronjob_bandit24       natas-stats            semtex0-32        vortex20
cronjob_bandit24_root  natas25_cleanup        semtex0-64
bandit22@melinda:/etc/cron.d$
bandit22@melinda:/etc/cron.d$
bandit22@melinda:/etc/cron.d$
bandit22@melinda:/etc/cron.d$  cat cronjob_bandit23
* * * * * bandit23 /usr/bin/cronjob_bandit23.sh  &> /dev/null
bandit22@melinda:/etc/cron.d$
bandit22@melinda:/etc/cron.d$
bandit22@melinda:/etc/cron.d$
bandit22@melinda:/etc/cron.d$ cat /usr/bin/cronjob_bandit23.sh
#!/bin/bash

myname=$(whoami)
mytarget=$(echo I am user $myname | md5sum | cut -d ' ' -f 1)

echo "Copying passwordfile /etc/bandit_pass/$myname to /tmp/$mytarget"

cat /etc/bandit_pass/$myname > /tmp/$mytarget
bandit22@melinda:/etc/cron.d$
bandit22@melinda:/etc/cron.d$
bandit22@melinda:/etc/cron.d$
bandit22@melinda:/etc/cron.d$  /usr/bin/cronjob_bandit23.sh
Copying passwordfile /etc/bandit_pass/bandit22 to /tmp/8169b67bd894ddbb4412f9157          3b38db3
bandit22@melinda:/etc/cron.d$ echo I am user bandit23 | md5sum | cut -d ' ' -f 1          8ca319486bfbbc3663ea0fbe81326349
bandit22@melinda:/etc/cron.d$
bandit22@melinda:/etc/cron.d$ cat /tmp/8ca319486bfbbc3663ea0fbe81326349
jc1udXuA1tiHqjIsL8yaapX5XIAI6i0n
bandit22@melinda:/etc/cron.d$
```
password for bandit 23 is **"jc1udXuA1tiHqjIsL8yaapX5XIAI6i0n"**


## Bandit 23 to 24
Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit23"** and the above password **jc1udXuA1tiHqjIsL8yaapX5XIAI6i0n** 
```

bandit23@melinda:~$ cd /etc/cron.d
bandit23@melinda:/etc/cron.d$ ls
behemoth4_cleanup      leviathan5_cleanup     natas25_cleanup~  semtex0-ppc
cron-apt               manpage3_resetpw_job   natas26_cleanup   semtex5
cronjob_bandit22       melinda-stats          natas27_cleanup   sysstat
cronjob_bandit23       natas-session-toucher  php5              vortex0
cronjob_bandit24       natas-stats            semtex0-32        vortex20
cronjob_bandit24_root  natas25_cleanup        semtex0-64
bandit23@melinda:/etc/cron.d$ cat cronjob_bandit24
* * * * * bandit24 /usr/bin/cronjob_bandit24.sh &> /dev/null
bandit23@melinda:/etc/cron.d$ cat /usr/bin/cronjob_bandit24.sh
#!/bin/bash

myname=$(whoami)

cd /var/spool/$myname
echo "Executing and deleting all scripts in /var/spool/$myname:"
for i in * .*;
do
    if [ "$i" != "." -a "$i" != ".." ];
    then
        echo "Handling $i"
        timeout -s 9 60 "./$i"
        rm -f "./$i"
    fi
done


bandit23@melinda:/etc/cron.d$ mkdir -p /tmp/level24
bandit23@melinda:/etc/cron.d$ cd /tmp/level24
bandit23@melinda:/tmp/level24$ vim sp.sh
bandit23@melinda:/tmp/level24$ chmod 777 sp.sh
bandit23@melinda:/tmp/level24$ cp sp.sh /var/spool/bandit24/
bandit23@melinda:/tmp/level24$ ls
bandit24  ok  sp.sh
bandit23@melinda:/tmp/level24$ cat bandit24
UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ
```
password for bandit 24 is **"UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ"**


## Bandit 24 to 25
Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit24"** and the above password **UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ**   
  
  Create following script to make a bruteforce...
```
#!/bin/bash
passwd="UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ"

for a in {0..9}{0..9}{0..9}{0..9}
do
    echo $passwd' '$a | nc localhost 30002 >> result &
done
```  
Enter following commands
```
$ sort result | uniq -u
Correct!
The password of user bandit25 is uNG9O58gUE7snukf3bvZ0rxhtnjzSGzG
```  
password for bandit 25 is **"uNG9O58gUE7snukf3bvZ0rxhtnjzSGzG"**

