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
Use the user name as **"bandit2"** and the above password **UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK**  

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

password for bandit 3 is **"pIwrPrtPN36QITSp3EQaw936yaFoFgAB"**
