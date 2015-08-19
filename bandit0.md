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

```


## Bandit 16 to 17
Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit16"** and the above password **UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK** 


## Bandit 17 to 18
Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit17"** and the above password **UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK** 


## Bandit 18 to 19
Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit218"** and the above password **UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK** 


## Bandit 19 to 20
Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit19"** and the above password **UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK** 


## Bandit 20 to 21
Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit20"** and the above password **UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK** 


## Bandit 21 to 22
Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit21"** and the above password **UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK** 


## Bandit 22 to 23
Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit22"** and the above password **UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK** 


## Bandit 23 to 24
Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit23"** and the above password **UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK** 


## Bandit 24 to 25
Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit24"** and the above password **UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK** 


## Bandit 25 to 26
Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit25"** and the above password **UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK** 


## Bandit 26 to 27
Open a SSH session to bandit.labs.overthewire.org using putty.
Use the user name as **"bandit26"** and the above password **UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK** 


