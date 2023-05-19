# AFLK([http://www.aflk-chat.com](http://www.aflk-chat.com/chat/login)) <-- UI 바로가기
  <p align="center">
    <img src = 'https://github.com/jaebum7396/aflk/assets/38182229/6fb9f5a9-751e-411b-a586-86aa38094fe3' style='width:60%;' />  
  </p>
  
  스프링 클라우드를 이용해 MSA(Micro Service Architecture)로 구성한 프로젝트 입니다.  
  EC2, docker, jenkins를 통해 CICD를 구축하였고  
  각 서비스는 스프링부트, 그래들을 이용하여 구현하였습니다.  

### 구현방법
```
Java, Spring Boot, 스프링 시큐리티, 스프링 클라우드, Jenkins, JPA, mysql, Gradle, Docker, redis
```
### 프로젝트 구성

#### devops
* [discovery](https://github.com/jaebum7396/discovery) : 로드밸런싱을 위한 디스커버리 서비스 netflix eureka
* [gateway](https://github.com/jaebum7396/gateway) : jwt 인증 및 각 서비스 라우팅을 위한 게이트웨이 서비스

#### FE
* [client](http://www.aflk-chat.com/chat/login) : 프로젝트 ui

#### service
* [user](https://github.com/jaebum7396/user) : 회원가입 및 유저정보 API - ([swagger](http://www.aflk-chat.com:8000/user/swagger-ui/))
* [chat](https://github.com/jaebum7396/chat) : 채팅 API - ([swagger](http://www.aflk-chat.com:8000/chat/swagger-ui/))
* [socket-streamer](https://github.com/jaebum7396/socket-streamer) : 웹 소켓 서버
* [file-storage](https://github.com/jaebum7396/file-storage.git) : 파일 처리 서버 
  
* [auth](https://github.com/jaebum7396/auth) : 권한(로그인) 서비스([swagger](http://52.79.162.165:8000/auth/swagger-ui/)) -- 삭제 예정(설계상 user와 상당부분 겹침)
