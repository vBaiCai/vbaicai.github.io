---
layout: psot
title: SSH 配置
---

## 生成密钥
`ssh-keygen -A`
## 修改/etc/ssh/sshd_config
```
ListenAddress 0.0.0.0
PasswordAuthentication yes
PermitRootLogin yes
   
```


## 一条命令将公钥添加到服务器

```sh
ssh-copy-id username@server_address
```

## 私钥的权限
```sh
chmod 400 ~/.ssh/id_rsa
```