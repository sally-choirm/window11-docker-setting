### 문제

```
  error during connect: this error may indicate that the docker daemon is not running.:
  get "http://%2f%2f.%2fpipe%2fdocker_engine/v1.24/containers/json": 
  open //./pipe/docker_engine: the system cannot find the file specified.
```

1. google에 오류를 치면 나오는 해결책이 안먹음 

```
cd C:\Program Files\Docker\Docker
DockerCli.exe -SwitchDaemon
```

2. Docker Desktop 이 ENGINE STOPED 되어 있음

### 문제의 원인

윈도우 11 부터 사용할수 있는 wls을 설치 해야 했다.

### 해결책

사용해야 docker desktop이 정상 작동

[https://docs.microsoft.com/ko-kr/windows/wsl/install-manual#step-4---download-the-linux-kernel-update-package](https://docs.microsoft.com/ko-kr/windows/wsl/install-manual#step-4---download-the-linux-kernel-update-package)

1,3,4,5단계 했는데 docker 정상 작동
