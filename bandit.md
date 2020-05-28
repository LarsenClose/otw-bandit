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

    *locally*
    cd Desktop
    vim bandit_key
    sudo chmod 700 bandit_key

    ssh -i /Users/lclose/Desktop/bandit_key -p 2220  bandit14@bandit.labs.overthewire.org

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
    ssh -i /Users/lclose/Desktop/bandit_key_17 -p 2220  bandit17@bandit.labs.overthewire.org

## Level 17 -> 18


