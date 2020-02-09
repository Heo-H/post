## 사용자 추가 방법

### 사용자 추가 및 설정
- {사용자명}: 생성할 사용자 이름
```command
$ sudo useradd {사용자명}  # 유저 추가
$ sudo passwd {사용자명}  # 패스워드 설정
$ sudo usermod -aG wheel {사용자명}  # sudo 권한 주기
```

### ssh key 복사
ssh key로 접속하는 경우, 현재 계정의 ssh key를 새로 생성한 사용자 디렉터리에 복사해줘야 접속이 가능하다.
- {사용자명}: 생성된 사용자 이름
```command
$ cd ~
$ sudo cp -r .ssh /home/{사용자명}/
$ sudo chown {사용자명}:{사용자명} -R /home/{사용자명}/.ssh
```
