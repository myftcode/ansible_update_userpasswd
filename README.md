# 用户密码修改

# 使用方法
```
ansible-playbook -i tests/inventory tests/main.yml --private-key=/root/.ssh/id_rsa --key-file=/root/.ssh/id_rsa 
```

## 文件内容说明
```
自定义用户变量
defaultes/main.yml

定义用户和密码
userinfo:
- { name: 'test',passwd: 'passwd' }
- { ... }

定义root密码
rootpasswd: 'passwd'
```
