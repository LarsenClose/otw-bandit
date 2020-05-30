# Bandit

## Level 0

    ssh -p 2220  bandit0@bandit.labs.overthewire.org
    bandit0

## Level 0 -> 1
    cat readme

    ssh -p 2220  bandit1@bandit.labs.overthewire.org
    boJ9jbbUNNfktd78OOpsqOltutMc3MY1



## Level 1 -> 2


    ls
    cat < -

    ssh -p 2220  bandit2@bandit.labs.overthewire.org
    CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9


## Level 2 -> 3
    
    cat "spaces in this filename"
    ssh -p 2220  bandit3@bandit.labs.overthewire.org
    UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK

## Level 3 -> 4

    cd inhere
    ls -la

    cat .hidden
    ssh -p 2220  bandit4@bandit.labs.overthewire.org
    pIwrPrtPN36QITSp3EQaw936yaFoFgAB

## Level 4 -> 5

    file -- *
    cat < -file07
    ssh -p 2220  bandit5@bandit.labs.overthewire.org
    koReBOKuIDDepwhWk7jZC0RTdopnAYKh

## Level 5 -> 6

    find . -type f -readable -size 1033c ! -executable
    cat ./maybehere07/.file2
    ssh -p 2220  bandit6@bandit.labs.overthewire.org
    DXjZPULLxYr17uwoI01bNLQbtFemEgo7

## Level 6 -> 7

    cd /
    find . -size 33c 
    ls -Rl | grep 'bandit7 bandit6'
    find . -name bandit7.password
    cat ./var/lib/dpkg/info/bandit7.password
    ssh -p 2220  bandit7@bandit.labs.overthewire.org
    HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs

## Level 7 -> 8

    grep 'millionth' data.txt
    ssh -p 2220  bandit8@bandit.labs.overthewire.org
    cvX2JJa4CFALtqS87jk27qwqGhBM9plV

## Level 8 -> 9

    sort data.txt | uniq -u
    ssh -p 2220  bandit9@bandit.labs.overthewire.org
    UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR

## Level 9 -> 10

    strings -a data.txt | grep '==*'
    ssh -p 2220  bandit10@bandit.labs.overthewire.org
    truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk

## Level1 0 -> 11

    base64 -d data.txt
    ssh -p 2220  bandit11@bandit.labs.overthewire.org
    IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR

## Level 11 -> 12

    cat data.txt | python -c 'import sys; print sys.stdin.read().encode("rot13")'
    cat data.txt | tr 'n-za-mN-ZA-M' 'a-zA-Z'
    5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu

    ssh -p 2220  bandit12@bandit.labs.overthewire.org

## Level 12 -> 13

    mkdir /tmp/okay1
    cp data.txt /tmp/okay1
    cd /tmp/okay1
    xxd -r data.txt original.bin
    file original.bin
    mv original.bin original.bin.gz
    gzip -d original.bin.gz
    file original.bin
    mv original.bin original.bin.bz2
    bzip2 -d original.bin.bz2
    file original.bin
    mv original.bin original.bin.gz
    gzip -d original.bin.gz
    mv original.bin original.bin.tar
    tar -xf original.bin.tar
    file data5.bin
    tar -xr data5.bin
    tar -xf data6.bin
    tar -x data8.bin
    file data8.bin
    mv data8.bin data8.bin.gz
    gzip -d data8.bin.gz
    file data8.bin
    cat data8.bin
    The password is 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL

    ssh -p 2220  bandit13@bandit.labs.overthewire.org
    8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL

## Level 13 -> 14

_locally_
    cd Desktop
    vim bandit_key
    sudo chmod 700 bandit_key

    ssh -i ~/Desktop/bandit_key -p 2220  bandit14@bandit.labs.overthewire.org

## Level 14 -> 15

    cat /etc/bandit_pass/bandit14 | nc localhost 30000
    
Correct!
BfMYroe26WYalil77FoDi9qh59eK5xNr

    ssh -p 2220  bandit15@bandit.labs.overthewire.org
    BfMYroe26WYalil77FoDi9qh59eK5xNr

## Level 15 -> 16

    openssl s_client -connect localhost:30001 
    BfMYroe26WYalil77FoDi9qh59eK5xNr

BfMYroe26WYalil77FoDi9qh59eK5xNr
Correct!
cluFn7wTiGryunymYOu4RcffSxQluehd

    ssh -p 2220  bandit16@bandit.labs.overthewire.org
    cluFn7wTiGryunymYOu4RcffSxQluehd

## Level 16 -> 17

    nmap -A 127.0.0.1 -p 31000-32000

31790/tcp open  ssl/unknown

    openssl s_client -connect localhost:31790 
    cluFn7wTiGryunymYOu4RcffSxQluehd

-----BEGIN RSA PRIVATE KEY-----
MIIEogIBAAKCAQEAvmOkuifmMg6HL2YPIOjon6iWfbp7c3jx34YkYWqUH57SUdyJ
imZzeyGC0gtZPGujUSxiJSWI/oTqexh+cAMTSMlOJf7+BrJObArnxd9Y7YT2bRPQ
Ja6Lzb558YW3FZl87ORiO+rW4LCDCNd2lUvLE/GL2GWyuKN0K5iCd5TbtJzEkQTu
DSt2mcNn4rhAL+JFr56o4T6z8WWAW18BR6yGrMq7Q/kALHYW3OekePQAzL0VUYbW
JGTi65CxbCnzc/w4+mqQyvmzpWtMAzJTzAzQxNbkR2MBGySxDLrjg0LWN6sK7wNX
x0YVztz/zbIkPjfkU1jHS+9EbVNj+D1XFOJuaQIDAQABAoIBABagpxpM1aoLWfvD
KHcj10nqcoBc4oE11aFYQwik7xfW+24pRNuDE6SFthOar69jp5RlLwD1NhPx3iBl
J9nOM8OJ0VToum43UOS8YxF8WwhXriYGnc1sskbwpXOUDc9uX4+UESzH22P29ovd
d8WErY0gPxun8pbJLmxkAtWNhpMvfe0050vk9TL5wqbu9AlbssgTcCXkMQnPw9nC
YNN6DDP2lbcBrvgT9YCNL6C+ZKufD52yOQ9qOkwFTEQpjtF4uNtJom+asvlpmS8A
vLY9r60wYSvmZhNqBUrj7lyCtXMIu1kkd4w7F77k+DjHoAXyxcUp1DGL51sOmama
+TOWWgECgYEA8JtPxP0GRJ+IQkX262jM3dEIkza8ky5moIwUqYdsx0NxHgRRhORT
8c8hAuRBb2G82so8vUHk/fur85OEfc9TncnCY2crpoqsghifKLxrLgtT+qDpfZnx
SatLdt8GfQ85yA7hnWWJ2MxF3NaeSDm75Lsm+tBbAiyc9P2jGRNtMSkCgYEAypHd
HCctNi/FwjulhttFx/rHYKhLidZDFYeiE/v45bN4yFm8x7R/b0iE7KaszX+Exdvt
SghaTdcG0Knyw1bpJVyusavPzpaJMjdJ6tcFhVAbAjm7enCIvGCSx+X3l5SiWg0A
R57hJglezIiVjv3aGwHwvlZvtszK6zV6oXFAu0ECgYAbjo46T4hyP5tJi93V5HDi
Ttiek7xRVxUl+iU7rWkGAXFpMLFteQEsRr7PJ/lemmEY5eTDAFMLy9FL2m9oQWCg
R8VdwSk8r9FGLS+9aKcV5PI/WEKlwgXinB3OhYimtiG2Cg5JCqIZFHxD6MjEGOiu
L8ktHMPvodBwNsSBULpG0QKBgBAplTfC1HOnWiMGOU3KPwYWt0O6CdTkmJOmL8Ni
blh9elyZ9FsGxsgtRBXRsqXuz7wtsQAgLHxbdLq/ZJQ7YfzOKU4ZxEnabvXnvWkU
YOdjHdSOoKvDQNWu6ucyLRAWFuISeXw9a/9p7ftpxm0TSgyvmfLF2MIAEwyzRqaM
77pBAoGAMmjmIJdjp+Ez8duyn3ieo36yrttF5NSsJLAbxFpdlc1gvtGCWW+9Cq0b
dxviW8+TFVEBl1O4f7HVm6EpTscdDxU+bCXWkfjuRb7Dy9GOtt9JPsX8MBTakzh3
vBgsyi/sN3RqRBcGU40fOoZyfAMT8s1m/uYv52O6IgeuZ/ujbjY=
-----END RSA PRIVATE KEY-----

    vim bandit_key_17
    sudo chmod 700 bandit_key_17
    ssh -i ~/Desktop/bandit_key_17 -p 2220  bandit17@bandit.labs.overthewire.org

## Level 17 -> 18

    diff passwords.new passwords.old

42c42
< kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd
---
> w0Yfolrc5bwjS4qw5mq1nnQi6mF03bii

    ssh -p 2220  bandit18@bandit.labs.overthewire.org
    kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd

## Level 18 -> 19

Byebye !
Connection to bandit.labs.overthewire.org closed.

Unfortunately, someone has modified .bashrc to log you out when you log in with SSH.

    scp -P 2220 bandit18@bandit.labs.overthewire.org:readme ~/Desktop/readme
    kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd

    cat Desktop/readme
    IueksS7Ubh8G3DCwVzrTd8rAVOwq3M5x

    ssh -p 2220  bandit19@bandit.labs.overthewire.org
    IueksS7Ubh8G3DCwVzrTd8rAVOwq3M5x

## Level 19 -> 20

    ./bandit20-do

Run a command as another user.
Example: ./bandit20-do id

    ./bandit20-do cat /etc/bandit_pass/bandit20

    ssh -p 2220  bandit20@bandit.labs.overthewire.org
    GbKksEFF4yrVs6il55v6gwY5aVje5f0j

## Level 20 -> 21

    echo "GbKksEFF4yrVs6il55v6gwY5aVje5f0j" | nc -lp 39999 &
    ./suconnect 39999

Read: GbKksEFF4yrVs6il55v6gwY5aVje5f0j
Password matches, sending next password
gE269g2h3mw3pwgrj0Ha9Uoqen1c9DGr

    ssh -p 2220  bandit21@bandit.labs.overthewire.org
    gE269g2h3mw3pwgrj0Ha9Uoqen1c9DGr



## Level 21 -> 22

    cd /etc/cron.d/
    cat cronjob_bandit*

    cat /usr/bin/cronjob_bandit22.sh

#!/bin/bash
chmod 644 /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
cat /etc/bandit_pass/bandit22 > /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv

    cat /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
    Yk7owGAcWjwMVRwrTesJEwB7WVOiILLI

    ssh -p 2220  bandit22@bandit.labs.overthewire.org
    Yk7owGAcWjwMVRwrTesJEwB7WVOiILLI

## Level 22 -> 23

    cd /etc/cron.d/
    cat cronjob_bandit23

* * * * * bandit23 /usr/bin/cronjob_bandit23.sh  &> /dev/null

    cat /usr/bin/cronjob_bandit23.sh

#!/bin/bash

myname=$(whoami)
mytarget=$(echo I am user $myname | md5sum | cut -d ' ' -f 1)

echo "Copying passwordfile /etc/bandit_pass/$myname to /tmp/$mytarget"

cat /etc/bandit_pass/$myname > /tmp/$mytarget

    echo I am user bandit23 | md5sum | cut -d ' ' -f 1

    ssh -p 2220  bandit23@bandit.labs.overthewire.org
    jc1udXuA1tiHqjIsL8yaapX5XIAI6i0n

## Level 23 -> 24

    cat /etc/cron.d/cronjob_bandit24

@reboot bandit24 /usr/bin/cronjob_bandit24.sh &> /dev/null
* * * * * bandit24 /usr/bin/cronjob_bandit24.sh &> /dev/null
  


#!/bin/bash

myname=$(whoami)

cd /var/spool/$myname
echo "Executing and deleting all scripts in /var/spool/$myname:"
for i in * .*;
do
    if [ "$i" != "." -a "$i" != ".." ];
    then
        echo "Handling $i"
        owner="$(stat --format "%U" ./$i)"
        if [ "${owner}" = "bandit23" ]; then
            timeout -s 9 60 ./$i
        fi
        rm -f ./$i
    fi
done

    mkdir /tmp/pass24
    cd /tmp/pass24
    nano password.sh

#!/bin/bash
cat /etc/bandit_pass/bandit24 > /tmp/pass24/password.txt

    chmod 777 password.sh
    touch password.txt
    chmod 777 password.txt
    cp password.sh /var/spool/bandit24/
    cat password.txt

    ssh -p 2220  bandit24@bandit.labs.overthewire.org
    UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ

## Level 24 -> 25

Attempts:

#! python3
import socket

connSock=socket(AF_INET, SOCK_STREAM)
connSock.connect(("127.0.0.1", 30002))
connSock.send(str.encode("UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ"))


for pin in itertools.permutations(range(4)): 
    print("UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ", pin)



python3 interpreter
brute_force = lambda: [print("UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ " + str(number)) for number in range(10000)]
brute_force()

#! python3
import os
import sys

os.system("nc localhost 30002")



brute_force = lambda: [print("UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ " + str(number)) for number in range(10000)]
brute_force()

#### brute.py

brute_force = lambda: [print("UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ " + str(number)) for number in range(10000)]

brute_force()

    python3 ./brute.py | nc localhost 30002

Correct!
The password of user bandit25 is uNG9O58gUE7snukf3bvZ0rxhtnjzSGzG

    ssh -p 2220  bandit25@bandit.labs.overthewire.org
    uNG9O58gUE7snukf3bvZ0rxhtnjzSGzG

## Level 25 -> 26

    echo $SHELL
    ls
    cat bandit26.sshkey

-----BEGIN RSA PRIVATE KEY-----
MIIEpQIBAAKCAQEApis2AuoooEqeYWamtwX2k5z9uU1Afl2F8VyXQqbv/LTrIwdW
pTfaeRHXzr0Y0a5Oe3GB/+W2+PReif+bPZlzTY1XFwpk+DiHk1kmL0moEW8HJuT9
/5XbnpjSzn0eEAfFax2OcopjrzVqdBJQerkj0puv3UXY07AskgkyD5XepwGAlJOG
xZsMq1oZqQ0W29aBtfykuGie2bxroRjuAPrYM4o3MMmtlNE5fC4G9Ihq0eq73MDi
1ze6d2jIGce873qxn308BA2qhRPJNEbnPev5gI+5tU+UxebW8KLbk0EhoXB953Ix
3lgOIrT9Y6skRjsMSFmC6WN/O7ovu8QzGqxdywIDAQABAoIBAAaXoETtVT9GtpHW
qLaKHgYtLEO1tOFOhInWyolyZgL4inuRRva3CIvVEWK6TcnDyIlNL4MfcerehwGi
il4fQFvLR7E6UFcopvhJiSJHIcvPQ9FfNFR3dYcNOQ/IFvE73bEqMwSISPwiel6w
e1DjF3C7jHaS1s9PJfWFN982aublL/yLbJP+ou3ifdljS7QzjWZA8NRiMwmBGPIh
Yq8weR3jIVQl3ndEYxO7Cr/wXXebZwlP6CPZb67rBy0jg+366mxQbDZIwZYEaUME
zY5izFclr/kKj4s7NTRkC76Yx+rTNP5+BX+JT+rgz5aoQq8ghMw43NYwxjXym/MX
c8X8g0ECgYEA1crBUAR1gSkM+5mGjjoFLJKrFP+IhUHFh25qGI4Dcxxh1f3M53le
wF1rkp5SJnHRFm9IW3gM1JoF0PQxI5aXHRGHphwPeKnsQ/xQBRWCeYpqTme9amJV
tD3aDHkpIhYxkNxqol5gDCAt6tdFSxqPaNfdfsfaAOXiKGrQESUjIBcCgYEAxvmI
2ROJsBXaiM4Iyg9hUpjZIn8TW2UlH76pojFG6/KBd1NcnW3fu0ZUU790wAu7QbbU
i7pieeqCqSYcZsmkhnOvbdx54A6NNCR2btc+si6pDOe1jdsGdXISDRHFb9QxjZCj
6xzWMNvb5n1yUb9w9nfN1PZzATfUsOV+Fy8CbG0CgYEAifkTLwfhqZyLk2huTSWm
pzB0ltWfDpj22MNqVzR3h3d+sHLeJVjPzIe9396rF8KGdNsWsGlWpnJMZKDjgZsz
JQBmMc6UMYRARVP1dIKANN4eY0FSHfEebHcqXLho0mXOUTXe37DWfZza5V9Oify3
JquBd8uUptW1Ue41H4t/ErsCgYEArc5FYtF1QXIlfcDz3oUGz16itUZpgzlb71nd
1cbTm8EupCwWR5I1j+IEQU+JTUQyI1nwWcnKwZI+5kBbKNJUu/mLsRyY/UXYxEZh
ibrNklm94373kV1US/0DlZUDcQba7jz9Yp/C3dT/RlwoIw5mP3UxQCizFspNKOSe
euPeaxUCgYEAntklXwBbokgdDup/u/3ms5Lb/bm22zDOCg2HrlWQCqKEkWkAO6R5
/Wwyqhp/wTl8VXjxWo+W+DmewGdPHGQQ5fFdqgpuQpGUq24YZS8m66v5ANBwd76t
IZdtF5HXs2S5CADTwniUS5mX1HO9l5gUkk+h0cH5JnPtsMCnAUM+BRY=
-----END RSA PRIVATE KEY-----

    ssh -i ~/Desktop/bandit26 -p 2220  bandit26@bandit.labs.overthewire.org

    ssh -p 2220  bandit25@bandit.labs.overthewire.org

    cd /
    cd /home/bandit26
    ls -la
    cat text.txt

    cd ../etc
    cat shells

/etc/shells: valid login shells
/bin/sh
/bin/dash
/bin/bash
/bin/rbash
/usr/bin/screen
/usr/bin/tmux
/usr/bin/showtext

    cat passwd

bandit26:x:11026:11026:bandit level 26:/home/bandit26:/usr/bin/showtext

    /usr/bin/showtext

more: stat of /home/bandit25/text.txt failed: No such file or directory

    more /usr/bin/showtext

#!/bin/sh

export TERM=linux

more ~/text.txt
exit 0

## Level 26 -> 27

    more /home/bandit26/text.txt

    scp -P 2220 bandit26@bandit.labs.overthewire.org:/etc/bandit_pass/bandit26 ~/Desktop/banditpass

    ssh -i ~/Desktop/bandit26 -p 2220  bandit26@bandit.labs.overthewire.org

#### Resize shell - got help from Nicholas

    v
    shift + : set shell=/bin/bash
    :shell
    ls
    ./bandit27-do
    
    ./bandit27-do cat /etc/bandit_pass/bandit27

3ba3118a22e93127a4ed485be72ef5ea

    ssh -p 2220  bandit27@bandit.labs.overthewire.org
    3ba3118a22e93127a4ed485be72ef5ea

## Level 27 -> 28

ssh://bandit27-git@localhost/home/bandit27-git/repo

    mkdir /tmp/git11 && cd /tmp/git11
    git clone ssh://bandit27-git@localhost/home/bandit27-git/repo
    cd repo
    cat README

The password to the next level is: 0ef186ac70e04ea33b4c1853d2526fa2

    rm -rf /tmp/git11
    ssh -p 2220  bandit28@bandit.labs.overthewire.org
    0ef186ac70e04ea33b4c1853d2526fa2

## Level 28 -> 29

    mkdir /tmp/git11 && cd /tmp/git11
    git clone ssh://bandit28-git@localhost/home/bandit28-git/repo
    cd repo/
    cat README.md
    
    git branch
    git log
    git log -p

-- username: bandit29
-- password: <TBD>
+- password: bbc96594b4e001778eee9975372716b2

    ssh -p 2220  bandit29@bandit.labs.overthewire.org
    bbc96594b4e001778eee9975372716b2

## Level 29 -> 30

    cd /tmp/git11
    git clone ssh://bandit29-git@localhost/home/bandit29-git/repo
    bbc96594b4e001778eee9975372716b2

    cd repo
    git branch -r
    git checkout dev
    git log -p

-- username: bandit30
-- password: <no passwords in production!>
+- password: 5b90576bedb2cc04c86a9e924ce42faf

    ssh -p 2220  bandit30@bandit.labs.overthewire.org
    5b90576bedb2cc04c86a9e924ce42faf

## Level 30 -> 31

    mkdir /tmp/git13 && cd /tmp/git13

    git clone ssh://bandit30-git@localhost/home/bandit30-git/repo
    cat README.md

just an epmty file... muahaha

    git branch -r
    git log -p
    ls -la

    cd .git
    cat *

3aefa229469b7ba1cc08203e5d8fa299354c496b refs/remotes/origin/master
f17132340e8ee6c159e0a4a6bc6f80e1da3b1aea refs/tags/secret

    git show secret

47e603bb428404d265f59c42920d81e5

    ssh -p 2220  bandit31@bandit.labs.overthewire.org
    47e603bb428404d265f59c42920d81e5

## Level 31 -> 32

    mkdir /tmp/git && cd /tmp/git
    git clone ssh://bandit31-git@localhost/home/bandit31-git/repo
    47e603bb428404d265f59c42920d81e5

This time your task is to push a file to the remote repository.

Details:
File name: key.txt
Content: 'May I come in?'
Branch: master

    vim key.txt 'May I come in?'
    git add key.txt
    git add -f key.txt
    git commit
    git push (fails)
    vim .gitignore
    git commit
    git push ((fails))
    rm key.txt
    git add .
    git commit
    vim key.txt May I come in?

remote: Well done! Here is the password for the next level:
remote: 56a9bf19c63d650ce78e6ec0354ee45e

    ssh -p 2220  bandit32@bandit.labs.overthewire.org
    56a9bf19c63d650ce78e6ec0354ee45e

## Level 32 -> 33

WELCOME TO THE UPPERCASE SHELL
>>

    ls
    cd
    ls | sh
    echo $shell
    echo $PATH
    #!/bin/sh echo ls >
    $PATH ./usr/bin/sh sh
    $@
    $0
    ls
    cat uppershell
    ls -la
    cat /etc/bandit_pass/bandit33

c9c3199ddf4121b10cf581a98d51caee

    ssh -p 2220  bandit33@bandit.labs.overthewire.org
    c9c3199ddf4121b10cf581a98d51caee

## Level 32 -> 33

    cat README.txt

# The flag!

Congratulations on solving the last level of this game!

At this moment, there are no more levels to play in this game. However, we are constantly working
on new levels and will most likely expand this game with more levels soon.
Keep an eye out for an announcement on our usual communication channels!
In the meantime, you could play some of our other wargames.

If you have an idea for an awesome new level, please let us know!

