## 🐋 로컬에서 Docker 로 빌드하기 🐋

1. Docker Desktop 실행
2. Build 하기 전 spotless 적용 ```./gradlew spotlessApply```
3. 정해진 컨벤션을 지키고 있는지 검사 (spotelesscheck) ```./gradlew spotlessCheck```
4. spring boot build ```./gradlew build```
5. Docker Desktop 실행중 인지 확인 ```docker info```
6. Docker로 빌드하기 ```docker build -t "본인 dockerhub repo 이름"/helfoome . ```
7. Docker Hub login(IDE terminal에서 실행) ```docker login```
8. Docker Image Tag ```docker tag "본인 dockerhub repo 이름"/helfoome "본인 dockerhub repo 이름"/helfoome:latest```
9. Docker Image Push ```docker push "본인 dockerhub repo 이름"/helfoome:latest```

### 🐋 Docker 실행중인 컨테이너 중지하기 🐋
1. 실행 중인 컨테이너 목록 확인 ```docker ps```
2. 컨테이너 중지 실행 중인 컨테이너의 CONTAINER ID를 찾아서 중지. ```docker stop <CONTAINER ID>```
3. 컨테이너의 삭제가 필요할 경우 ```docker rm <CONTAINER ID>```
4. 이미지 삭제가 필요할 경우 ```docker rmi <IMAGE ID or IMAGE NAME>```
