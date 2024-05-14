### 1. 이미지 빌드

```shell
 docker buildx build -t amanecopse/krampoline-jenkins .
```

### 2. 컨테이너 실행 (윈도우 환경)

```shell
 docker run -d -p 8080:8080 -v C:\workspace\jenkins_home:/var/jenkins_home -v //var/run/docker.sock:/var/run/docker.sock --name jenkins -u root amanecopse/krampoline-jenkins
```

### 3. push

```shell
 docker push amanecopse/krampoline-jenkins
```

### 4. k8s

```shell
 kubectl apply -k ./k8s
```
