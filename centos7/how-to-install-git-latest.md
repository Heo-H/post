## git 2.x 버전 설치하기

CentOS 7에서 그냥 git을 설치할 경우 낮은 버전(1.8)이 설치된다.
다른 앱들과의 호환성을 위해 2.x 버전을 설치해보자.

```command
$ sudo rpm -Uvh http://opensource.wandisco.com/centos/7/git/x86_64/wandisco-git-release-7-2.noarch.rpm  # 저장소 추가
$ sudo yum install -y git
```
