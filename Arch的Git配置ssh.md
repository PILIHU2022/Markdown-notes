# arch的Git，配置ssh
```
ssh-keygen -t rsa#生成秘钥
```
## 查看秘钥内容
```
cat ~/.ssh/    使用tab键补全
```
将查看到的内容复制，打开GitHub，点击头像，settting > SSH and GPG keys > new ssh key，然后填入刚刚查看到的值，从ssh-rsa到结尾
## 使用以下命令查看是否成功
```
ssh -vT git@github.com
```
若显示`Exit status 1`则为成功