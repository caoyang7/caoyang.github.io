caoya@DESKTOP-EUP3RV2 MINGW64 ~
$ ssh-keygen -t rsa -C "caoyang529_7@163.com"
Generating public/private rsa key pair.
Enter file in which to save the key (/c/Users/caoya/.ssh/id_rsa):
Created directory '/c/Users/caoya/.ssh'.
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in /c/Users/caoya/.ssh/id_rsa.
Your public key has been saved in /c/Users/caoya/.ssh/id_rsa.pub.
The key fingerprint is:
SHA256:BNVKOKxAnWxDNXhUVY0nqfYmbkkggvsunF/9RfS52yQ caoyang529_7@163.com
The key's randomart image is:
+---[RSA 3072]----+
| ..+.*=+oo...+   |
|  . B =o. . + o  |
|   + + o.. ..o   |
|  . o ..o o. . . |
|   . . .So .. o  |
|  .    .  o.o  . |
| . o  . .o +. E .|
|  + ..   .+.   = |
|   +o    ..   . .|
+----[SHA256]-----+

caoya@DESKTOP-EUP3RV2 MINGW64 ~
$ ssh -T git@github.com
The authenticity of host 'github.com (13.229.188.59)' can't be established.
RSA key fingerprint is SHA256:nThbg6kXUpJWGl7E1IGOCspRomTxdCARLviKw6E5SY8.
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added 'github.com,13.229.188.59' (RSA) to the list of known hosts.
Hi caoyang7/caoyang7.github.io! You've successfully authenticated, but GitHub does not provide shell access.

caoya@DESKTOP-EUP3RV2 MINGW64 ~
$ git config --global user.name "caoyang7"

caoya@DESKTOP-EUP3RV2 MINGW64 ~
$ git config --global user.email "caoyang529_7@163.com"
