# AFLK([http://www.aflk-chat.com](http://www.aflk-chat.com/chat/login)) <-- UI 바로가기
  <p align="center">
    <img src = 'https://github.com/jaebum7396/aflk/assets/38182229/6fb9f5a9-751e-411b-a586-86aa38094fe3' style='width:60%;' />  
  </p>
  스프링 클라우드를 이용해 MSA(Micro Service Architecture)로 구성한 프로젝트 입니다.  
  EC2, docker, jenkins를 통해 CICD를 구축하였고  
  각 서비스는 스프링부트, 그래들을 이용하여 구현하였습니다.  

### 구현기능
* 회원가입, 로그인, 프로필이미지 변경
* 친구추가, 채팅방 오픈, 채팅메시지 송수신
* 읽음 메시지 표시(1 표시) -- 채팅방 참여 + 어플리케이션 포커스 일시 1 사라지도록
* 타이핑 시 상대방에게 타이핑 중입니다 표시
* 내 정보 창 UI 추가

### 구현예정
* 이미지, 동영상, 링크 전송
* 내 정보 변경
* 챗 GPT 활용한 내 정보 도움 기능
* 단체 채팅
* 친구찾기 기능(랜덤 세션 매칭-- 가칭 아바타모드)
* 이상형 월드컵 기능

### 구현방법
```
Java, Spring Boot, 스프링 시큐리티, 스프링 클라우드, Jenkins, JPA, mysql, Gradle, Docker, redis
```
### 프로젝트 구성
<img src = 'https://github.com/jaebum7396/AFLK/assets/38182229/56b15140-616c-48cc-8ead-0c11424c5be6' style='width:100%' />

#### devops
* [discovery](https://github.com/jaebum7396/discovery) : 로드밸런싱을 위한 디스커버리 netflix eureka
* [gateway](https://github.com/jaebum7396/gateway) : jwt 인증 및 각 서비스 라우팅을 위한 게이트웨이

#### fe
* [client](http://www.aflk-chat.com/chat/login) : 프로젝트 ui

#### service
* [user](https://github.com/jaebum7396/user) : 회원가입 및 유저정보 API - ([swagger](http://www.aflk-chat.com:8000/user/swagger-ui/))
* [chat](https://github.com/jaebum7396/chat) : 채팅 API - ([swagger](http://www.aflk-chat.com:8000/chat/swagger-ui/))
* [socket-streamer](https://github.com/jaebum7396/socket-streamer) : 웹 소켓 서버
* [file-storage](https://github.com/jaebum7396/file-storage.git) : 파일 처리 서버 

UI 아이콘 디자인 도움 thanks to thdus12
