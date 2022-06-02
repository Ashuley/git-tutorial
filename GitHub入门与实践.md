1. 初始设置							

```shell
git config --global user.name "Firstname Lastname"
git config --global user.email "your_email@example.com"
git config --global color.ui auto
cat ~/.gitconfig	# 该命令可以查看上面的设置
```

2. 设置SSH Key

```shell
ssh-keygen -t rsa -C "your_email@example.com"
# 跳出的待回复可以设置密码
# 下面是查看公钥，可以把显示的公钥粘贴到GitHub的个人账户
$ cat ~/.ssh/id_rsa.pub
$ ssh -T git@github.com
The authenticity of host 'github.com (20.205.243.166)' can't be established.
ED25519 key fingerprint is SHA256:+DiY3wvvV6TuJJhbpZisF/zLDA0zPMSvHdkr4UvCOqU.
This key is not known by any other names
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added 'github.com' (ED25519) to the list of known hosts.
Enter passphrase for key '/c/Users/Owen/.ssh/id_rsa':
Hi Ashuley! You've successfully authenticated, but GitHub does not provide shell access.

```

3. Get Clone

```shell
git clone git@github.com:DuGuQiuBai/Java.git
```

