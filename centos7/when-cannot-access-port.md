## 특정 포트에 접근할 수 없을 때
방화벽을 풀어줘야한다.
```command
$ sudo firewall-cmd --permanent --zone=public --add-port=8000/tcp
$ sudo firewall-cmd --permanent --zone=public --add-port=3000/tcp
$ sudo firewall-cmd --permanent --zone=public --add-port=80/tcp
$ sudo firewall-cmd --reload
```
