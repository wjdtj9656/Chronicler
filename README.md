# Chronicler
 - 비지니스 목적을 위한 자동 회의록 작성 서비스

# 팀원을 소개합니다!
        김정서          김영진          나예인          송상훈          조선송

![kimjeongseo jpg](https://user-images.githubusercontent.com/63994962/187566676-4b167d52-01b5-4845-8096-9d26ebe5cd9b.png) ![김영진 jpg](https://user-images.githubusercontent.com/63994962/187566679-0fbab3f4-627e-4483-9a06-912b6a29f5d0.jpg) ![jenkins-logo](https://user-images.githubusercontent.com/63994962/187566675-a38857c0-faf1-4d28-8dd0-363c73f10c58.png) ![송상훈](https://user-images.githubusercontent.com/63994962/187566682-5afcdd4b-5b77-44f3-97d0-d1e97c76ea19.jpg) ![조선송__2_](https://user-images.githubusercontent.com/63994962/187566691-822625b8-a78e-4d5c-ac6b-c030c089d251.jpg)

# 팀원 역할
송상훈 : 팀장, Backend <br> 
김영진 : Backend, Server <br>
나예인 : Backend, Docker <br>
김정서 : Frontend <br>
조선송 : Frontend

<hr>

## 프로젝트 기간 : 2022.07.11 ~ 2022.08.19

## Chronicler 로고
![logo](https://user-images.githubusercontent.com/63994962/187566677-314a37b0-9833-43da-b438-c825f4aa3317.png)
<hr>

## 개발환경

- [ ]  협업툴
- Notion
- Jira
- Mattermost
- GitLab
- Webex
----------------------------- 
- [ ]  Frontend
- React 18.2.0
- React Router 6.3.0
- Recoil 0.7.4
- Material UI 5.9.1
- Axios 0.27.2
- Typescript 4.7.4
- sweetalert2 11.4.24
---
- [ ]  Backend
- openjdk 1.8.0_192
- Java Zulu 8.33.0.1
- eclipse 4.16.0 (2020-06)
- Spring Boot 2.7.1
- Spring Data JPA
- Spring Security 5.6.6
- JWT 0.11.2
- AWS EC2
- MySQL 5.7.37
---
- [ ]  WebRTC
- Openvidu
---
- [ ]  STT(Speech-to-Text)
- JavaScript window 객체
---
- [ ]  CI/CD
- Docker version 20.10.17, build 100c701
- NGINX
- AWS EC2
---
- [ ]  Docx file API
- Aspose words 22.7
---
- [ ]  Email
- Spring Java MailSender
---
- [ ]  형태소 분석
- KOMORAN 3.3.4

<hr>

# Chronicler의 모토
간편하고 쉽게 이용하는 자동 서기관 시스템

<hr>

# Chronicler 서비스 화면 
- 메인 페이지
![main](https://user-images.githubusercontent.com/63994962/187566678-ef5a0fcf-8cd5-4aa3-955e-14cd9d7d4b21.png)

- 회의실 실시간 자막 
![회의_자막](https://user-images.githubusercontent.com/63994962/187566694-9ef8b7b1-fe85-40db-aedc-3a7b856f534c.png)

- 회의 종료 후 메일 발송
![크로니클러_메일왔을때](https://user-images.githubusercontent.com/63994962/187566692-be2ea56d-16c2-4835-8380-8e3824b38250.png)

- 회의록

![회의록1](https://user-images.githubusercontent.com/63994962/187566666-32c5f792-2790-485b-8f86-4e23baf2ff48.png)  ![회의록2](https://user-images.githubusercontent.com/63994962/187566669-4b613543-f47b-46de-849a-5cc4a0e4f96d.png)

![회의록3](https://user-images.githubusercontent.com/63994962/187566670-7f87a684-0d89-44e4-8750-f4eee346b229.png)  ![회의록4](https://user-images.githubusercontent.com/63994962/187566672-8d91bbc6-5289-4019-a717-6ee113504409.png)

<hr>

# 서비스 설명
회의에서 사용자들이 대화한 데이터를 수집, 자동으로 회의록을 docx 파일로 제작해주는 서비스

# 주요 기능
- webRTC를 통한 화상 채팅 기능
- STT를 활용한 실시간 자막 제공
- 대화 data를 분석하여 형태소 처리 이후 관련 데이터 차트 제공
- 회의 종료 시 해당 회의에 대한 회의록 작성
- 방장의 이메일로 회의록 docx파일로 송신
<hr>

# 시스템 아키텍쳐
![시스템아키텍처](https://user-images.githubusercontent.com/63994962/187566685-a64fe765-d49c-4d67-aff1-83232f32d1f9.PNG)
<hr>

# CI/CD 구축 및 SSL 인증서 적용
프론트엔드 React.js는 Nginx와 함께 docker를 사용하여 빌드 및 배포하였고, 백엔드, openvidu도 docker container를 통해 배포하였습니다. 
<br>
Nginx와 letsencrypt를 이용하여 SSL 인증서를 적용하고, 프론트엔드는 https의 기본값 443을 통해 분기, 백엔드는 /api의 경로로 프록시를 걸어주었습니다.

# 기술 특이점
- WebRTC
- STT(Speech-To-Text)
- Aspose
<hr>

# 요구사항 정의서
![요구사항정의서](https://user-images.githubusercontent.com/63994962/187566688-ab140feb-2abd-4ed7-a94f-c5726d85100c.PNG)
<hr>

# Git 컨벤션

```
FEAT:    새로운 기능을 추가할 경우
FIX:     버그를 고친 경우
STYLE:   코드 포맷 변경, 간단한 수정, 코드 변경이 없는 경우
REFATOR: 프로덕션 코드 리팩토링
DOCS:    문서를 수정한 경우(ex> Swagger)
Rename:  파일 혹은 폴더명 수정 및 이동
Remove:  파일 삭제
```

<hr>

# Git Flow 브랜치 전략
- 사용 브랜치
master - 배포
devleop - 개발
feature - 기능

- 진행 방식
feature의 기능이 완성되면 develop에 merge
배포 준비가 완료되면 develop 브랜치를 master에 merge

<hr>

# Jira
Jira를 통해서 매주 진행 예상되는 업무를 sprint에 넣어서 관리했습니다. 팀원 개개인이 어떤 일을 하고 있는지에 대한 확인할 때에도 backlog를 통해서 확인하였고, 스프린트는 일주일 단위로 진행하였습니다. 
- story : 디테일한 부분까지 상세하게 기술
- epic : BACKEND, FRONTEND, SERVER, DOCKER 등으로 구성하였습니다.

Mattermost와 연동하여 업무에 대한 변동사항을 실시간으로 파악할 수 있도록 했습니다. 

<hr>

# Notion
FRONTEND, BACKEND, FREEDOM, 회의록, 일정관리 카테고리로 나누어 FRONT에게 필요한 정보, BACK에게 필요한 정보 모두가 함께 알아야 할 정보로 나누어 관리했습니다.
<br> 
매일 회의한 내용을 회의록 카테고리에 작성했고, 일정에 대한 부분도 기술하였습니다. 

<hr>

# ER Diagram
![erd](https://user-images.githubusercontent.com/63994962/187566674-e41562e8-34fb-4687-87fb-9ecff8ae5763.png)

<hr>

# EC2 포트 정리
|443 | HTTPS|
|-|-|
|80 | HTTP -> HTTPS로 Redirect|
|3306 | MySQL|
|8080 | Spring Boot |
|3000 | React |
|4443 | Openvidu|

<hr>


# Docker command

DB :

```docker
docker pull yeinrah/mysql:5.7.37
```

```docker
docker run -d -p 3306:3306 --name mysql --network chronicler -e MYSQL_ROOT_PASSWORD=ssafy -e MYSQL_DATABASE=chronicler -e MYSQL_USER=A301 -e MYSQL_PASSWORD=SSAFY0707 yeinrah/mysql:5.7.37
```

BE : 

```docker
docker pull yeinrah/chronicler-back
```

```docker
docker run -d -p 8080:8080 --name chronicler-back --network chronicler yeinrah/chronicler-back
```

FE :
```docker
docker pull yeinrah/chronicler-front
```

```docker
docker run -d -p 3000:80 --name chronicler-front --network chronicler yeinrah/chronicler-front
```

<hr>



# 개발 후 회고
<hr>

송상훈 : 6주 동안의 시간이 정말 빠르게 흘러갔습니다. 사용자 입장에서 고민 많이 했습니다. 실시간 자막 및 회의록 자동생성(빈도분석포함) 기능에 집중한 CHRONICLER 다들 사랑해주세요! <br>

김영진 : 혼자 해결하려고 했다면 하루 종일도 걸렸을 에러가 함께 고민하니 금방 해결돼버리는 기이한 현상을 봤습니다. 협업의 중요성! <br>

나예인 : 저희가 만든 서비스를 직접 빌드 및 배포해보면서 1학기와는 또 다른 것들을 많이 배울 수 있는 시간이었습니다. 다음 프로젝트에서는 반드시 젠킨스를 도입해서 생산성을 높여보고 싶습니다. 다들 수고하셨습니다! <br>

김정서 : 코딩이 막힐 때, 스트레스 받아도 좋은 팀원이 있어서 스트레스가 덜 했던 것 같습니다. 저 또한 좋은 팀원이 되기위해 노력 해야겠습니다. <br>

조선송 : 팀원들이 모두 정말 좋아서 프로젝트를 즐겁게 마칠 수 있었습니다. <br>
