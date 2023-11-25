ignasiusadhitia@DESKTOP-276I4SF MINGW64 ~
$ ssh-keygen
Generating public/private rsa key pair.
Enter file in which to save the key (/c/Users/ignas/.ssh/id_rsa):
Created directory '/c/Users/ignas/.ssh'.
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in /c/Users/ignas/.ssh/id_rsa
Your public key has been saved in /c/Users/ignas/.ssh/id_rsa.pub
The key fingerprint is:
SHA256:qATTqC7d/ItAewHRLARTvRj4O/icw9NU3pSPE3fU3qo ignasiusadhitia@DESKTOP-276I4SF
The key's randomart image is:
+---[RSA 3072]----+
|o=++ . |
|..o++ . . |
| .=+.. . . . . |
| .o+. ..+ . . . .|
|....oo.oS= . . |
|ooo=.o. + . . |
|.=+== . . |
|. Bo.o E |
| o. o. |
+----[SHA256]-----+

ignasiusadhitia@DESKTOP-276I4SF MINGW64 ~
$ cd .ssh

ignasiusadhitia@DESKTOP-276I4SF MINGW64 ~/.ssh
$ ls -l
total 5
-rw-r--r-- 1 ignasiusadhitia 197609 2622 Nov 25 09:21 id_rsa
-rw-r--r-- 1 ignasiusadhitia 197609 585 Nov 25 09:21 id_rsa.pub

ignasiusadhitia@DESKTOP-276I4SF MINGW64 ~/.ssh
$ cat id_rsa.pub
ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQDZI5a8OG2uUUr681NNrWC+jKBMniKF6NQuJLWGiPToyQaLfd6CWxjyvyhFbNoVeiHORkGJ5ghOX5t77kThAnRMustak+3qdwowiQBCAlaziZ9H0poKflWZfNWpLakcVwh2OnsJcyO8Ow+NshdccUg/KhyrluaFCm6yVnI3NH5gdxD8sQJ9k+G+tS1HSprwt/ZCKs1m9E3BljWbaxLUtoHhpUz4D2k2n0uRovcBRUoOxfRDqhzpy5WmpSso3azqmIHNCgnHq8nYgiE4dflG4yMoI6ZYw5Yb5r8nDOmhaMyu8juSCA1gX5u9O+n5aSafDRzEA1+eUqhmA6x0PMimdsnD9EgWsQdw4hnHoiDzJZ1HwyOFRmWFWp1nwCGQiL+h9ILG1CMr7w5NHayGvipT2hN86osaOqEs8ERuo0EI73FgzTK1q1DeQ2cTOwdPYSfi0JCF2+bzYs1QVOCI0GxZ5dagpL3MjxBoTJOac1WTPCIVvp4/8Gr+Zh1i9Pop/T5EaDk= ignasiusadhitia@DESKTOP-276I4SF

ignasiusadhitia@DESKTOP-276I4SF MINGW64 ~/.ssh
$ ssh -T git@github.com
The authenticity of host 'github.com (20.205.243.166)' can't be established.
ED25519 key fingerprint is SHA256:+DiY3wvvV6TuJJhbpZisF/zLDA0zPMSvHdkr4UvCOqU.
This key is not known by any other names.
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added 'github.com' (ED25519) to the list of known hosts.
Hi ignasiusadhitia! You've successfully authenticated, but GitHub does not provide shell access.

ignasiusadhitia@DESKTOP-276I4SF MINGW64 ~/.ssh
$ ssh -T git@github.com
Hi ignasiusadhitia! You've successfully authenticated, but GitHub does not provide shell access.

ignasiusadhitia@DESKTOP-276I4SF MINGW64 ~/.ssh
$ git clone ssh.git@github.com:ignasiusadhitia/git-github-basic.git
Cloning into 'git-github-basic'...
ssh.git@github.com: Permission denied (publickey).
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

ignasiusadhitia@DESKTOP-276I4SF MINGW64 ~/.ssh
$
