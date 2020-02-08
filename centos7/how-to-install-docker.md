## 도커 설치하기

### docker 설치

```command
# 도커 설치
$ sudo yum install -y docker

# 권한 설정
$ sudo groupadd docker
$ sudo usermod -aG docker $USER

# 도커 자동 시작 설정 및 시작
$ sudo systemctl enable docker.service
$ sudo systemctl start docker.service
```

위 명령어 입력 후 ssh 세션을 재접속한다.

### docker-compose 설치

[docker-compose 설치 매뉴얼](https://docs.docker.com/compose/install/#install-using-pip) 참고
```command
$ sudo curl -L "https://github.com/docker/compose/releases/download/1.25.3/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
$ sudo chmod +x /usr/local/bin/docker-compose
```
