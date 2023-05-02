# aflk
MSA(Micro Service Architecture)로 구성된 프로젝트 입니다.


## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

What things you need to install the software and how to install them

```
Give examples
```

### Installing

A step by step series of examples that tell you how to get a development env running

Say what the step will be

```
Give the example
```

And repeat

```
until finished
```

End with an example of getting some data out of the system or using it for a little demo

## Running the tests

Explain how to run the automated tests for this system

### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```


## 구성
* [discovery](https://github.com/jaebum7396/discovery) -- 로드밸런싱을 위한 디스커버리 서비스 netflix eureka
* [gateway](https://github.com/jaebum7396/gateway) -- jwt 인증 및 각 서비스 라우팅을 위한 게이트웨이 서비스
* [user](https://github.com/jaebum7396/user) -- 회원가입 및 유저정보 서비스([swagger](http://52.79.162.165:8000/user/swagger-ui/))
* [auth](https://github.com/jaebum7396/auth) -- 권한(로그인) 서비스([swagger](http://52.79.162.165:8000/auth/swagger-ui/))
