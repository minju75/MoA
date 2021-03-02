# 펀딩 시스템을 도입한 프로젝트 팀 구성 서비스 "MoA"



![logo](images/logo.png)

MoA'로 'Make Of teAm'의 스펠링을 따서 팀을 구성한다라는 의미와 한글 발음으로는 '모아'로 모으다 라는 의미를 함축적인 의미를 가진 '모아 프로젝트'를 진행하게 되었습니다. 

아이콘의 문어는 여러개의 다리로 구성된 문어가 프로젝트 팀 구성원들의 조직을 떠올린다고 생각하여 선정하게 되었습니다. 



## 기획배경

자신이 원하는 주제로 프로젝트로 개발해보고 싶지만 혼자서 하기에는 버거울때, 지인들로만 팀을 구성하기에는 한계가 있을 때, 더불어 팀을 구성할 때 교육적으로 도움을 주며 이끌어줄 수 있는 멘토가 필요할 때! 

이러한 문제를 겪는 사람들이 많을 것이라고 생각하여 프로젝트를 함꼐할 팀원을 모으고 멘토를 구할 수 있는 웹서비스 "MoA"를 기획하게 되었습니다. 



## 핵심기능

 ### 회원가입 & 로그인

 * 멘토와 멘티를 구분한 회원가입을 진행하여 차별화된 서비스를 제공
 * 세션이 유지되는 로그인을 지원

### 마이 페이지

* 회원 가입 시 입력한 정보를 확인할 수 있으며, 수정 및 탈퇴 가능
* 펀딩을 관심 목록에 추가하면 마이페이지에서 확인 가능(카카오톡 공유 가능)

### 메인 화면

* 펀딩을 검색할 수 있으며, 최신순, 마감 임박 순 등으로 모집중인 펀딩을 확인할 수 있음
* 관심사에 따라 추천 프로젝트를 우선으로 보여줌(카테고리 별 확인 가능)

### Q&A

* Q&A 서비스를 통해서 MoA Web Page 사용에서 문의하고 싶은 내용 등을 문의 가능
* 24시간 답변을 위해서 챗봇 시스템 도입

### 펀딩 서비스

* 진행하고 싶은 프로젝트를 멘토 및 멘티가 펀딩을 열 수 있음
* 오픈 채팅방을 통해 실시간으로 문의가 가능하며, 카카오톡 문의하기 기능을 제공

### 일정 관리 서비스

* Jira의 협업 일정 관리 서비스와 유사한 기능을 제공
* 사용에 편리한 UI/UX로 구성하여 서비스 제공

### 멘토 및 멘티 평가 서비스

* 협조적이지 않은 팀원 및 멘토를 방지하기 위해 프로젝트 종료 후 의무적으로 평가를 통해 기록이 남도록 함
* 문제를 일으키게 되면 다른 프로젝트 참여에 문제가 될 수 있도록 함

### 멘토 랭킹 & 멘티 능력치

* 평가를 기반으로 멘토들은 랭킹을 통해 경력을 보여줄 수 있음
* 랭킹에 따라 포인트 환급 수수료를 줄여줘 보다 열정적으로 임할 수 있게 하려는 의도
* 멘티들은 능력치를 부여 받아 성취감을 더욱 높이고자 함



## 사용기술 스택

![techStack](images/techStack.png)

백엔드에서는 spring과 MySQL을 핵심적으로 이용해 개발을 진행하였고 프론트엔드에서는 Vue를 기반으로 Vuetify, Node.js, HTML, CSS를 이용해 개발을 진행하였습니다. 



## 프로젝트 구성원 소개

![team_members](images/team_members.png)





## MoA 개발일정

![개발일정](images/개발일정.JPG)

저희 팀은 많은 회의를 거쳐 서비스를 기획하였으며 개발에 앞서 와이어프레임을 제작하여 
제공하고자 하는 서비스를 보다 명확하게 진행할 수 있도록 하고자 하였습니다. 이렇게 제작한 와이어프레임을 기반으로 보다 효율적인 데이터베이스를 설계할 수 있었습니다. 후에 본격적으로 db에 맞게 백엔드를 구현하였고 스웨거를 통해서 프론트엔드와 유연하게 연동하였습니다. 그리고 최종적으로 사용자 측면에서 불편함을 최소화하기 위해서최적화를 거친 후 편의성을 극대화 할 수 있는 UI, UX를 구축하였습니다. 



## MoA 와이어프레임

frammer를 이용해서 페이지 제작전의 기본적인 틀을 구성하였습니다. 헤더와 푸터의 고정사이즈, 각 카테고리의 사이즈 등을 대략적으로 정해놓았습다. 밑의 사진들은 저희 MoA 웹서비스의 와이어프레임입니다. 

#### 로그인

먼저 로그인 페이지입니다, 모든 사이트의 필수 기능인 로그인은 간단하게 구현하였습니다.

로그인 밑에는 비밀번호 찾기와 회원가입 버튼을 구성해놓아 언제 어디서나 회원가입, 비밀번호 찾기가 가능하게 하였습니다. 

![로그인](images/wireframe/로그인.png)



#### 비밀번호 찾기

비밀번호 찾기 페이지는 ID 를 입력하면 핸드폰 인증이나 이메일 인증으로 비밀번호를 찾을 수 있도록 설정해두었습니다. 

![비밀번호찾기](images/wireframe/비밀번호찾기.png)



#### 회원가입

회원가입 페이지에서는 이름, 나이, 전공과 같은 기초적인 정보들을 입력해야하며 이는 추후에 추가할 부분입니다. 

![회원가입](images/wireframe/회원가입.png)



#### 메인페이지

사이트의 핵심이 되는 메인페이지입니다. 메인페이지에서는 프로젝트의 카테고리를 선택할 수 있는 카테고리 목록이 들어가며 원하는 프로젝트나 카테고리의 키워드를 검색할 수 있는 검색창 또한 들어갈 수 있도록 구성하였습니다. 카테고리의 밑에는 현재 진행중인 펀딩들의 목록이 뜨고 그 밑으로는 분야별 멘토들의 랭킹을 확인할 수 있도록 구성하였습니다. 

![메인페이지](images/wireframe/메인페이지.png)



#### 프로젝트 오픈 페이지

프로젝트 오픈 페이지에서는 자신이 진행하고자 하는 프로젝트를 열어서 팀원과 멘토를 구할 수 있도록 구성하였습니다. 이 페이지에서는 자신이 진행해보고 싶은 프로젝트의 상세설명을 적을 수 있고 참여로 필요한 인원과 카테고리 또한 설정 할 수 있습니다.

![프로젝트오픈페이지](C:\Users\multicampus\Desktop\포트폴리오\images\wireframe\프로젝트오픈페이지.png)



#### 프로젝트 세부정보 페이지

프로젝트를 생성 후 프로젝트 목록에서 진행중 인 프로젝트를 클릭할 시 해당 프로젝트의 세부정보를 확인할 수 있는 페이지입니다. 이 페이지에서는 프로젝트의 이미지, 세부정보, 공유하기, 관심등록 등이 가능하며 가장 하단에는 일정에 대한 설명을 쓸 수 있는 달력을 담아뒀습니다. 이 달력의 우측 상단 버튼을 클릭하면 일정관리 페이지로 넘어갈 수 있습니다. 

![프로젝트 세부 정보 페이지](C:\Users\multicampus\Desktop\포트폴리오\images\wireframe\프로젝트 세부 정보 페이지.png)



#### 일정관리 페이지

일정관리 페이지는 할일, 진행중, 완료 3가지로 일을 나누었으며 drag & drop으로 일정을 수정하거나 변경할 수 있습니다.

![일정관리 페이지](C:\Users\multicampus\Desktop\포트폴리오\images\wireframe\일정관리 페이지.png)



#### 마이페이지

마이페이지에서는 현재 진행중인 프로젝트 부터 내가 관심등록한 프로젝트까지 전부 확인이 가능하며 종료된 프로젝트는 팀원을 평가할 수 있습니다.

![마이페이지](C:\Users\multicampus\Desktop\포트폴리오\images\wireframe\마이페이지.png)



✔이 외에도 개발을 진행하면서 페이지는 더 추가되었으며 임시적으로 만들어 놓은 와이어프레임입니다.



## MoA의 ERD

![MOA ERD](C:\Users\multicampus\Desktop\포트폴리오\images\MOA ERD.png)

MoA의 ERD입니다. 





## MoA 웹서비스 실행화면

모아 웹페이지는 전부 반응형으로 구현하였기 때문에 언제 어디서나 모바일 기기로 편하게 접속이 가능합니다. 

#### 메인페이지(로그인전)

![로그인 전 메인 페이지](C:\Users\multicampus\Desktop\포트폴리오\images\모아 사이트 스크린 캡쳐\로그인 전 메인 페이지.JPG)





#### 회원가입 페이지

![회원가입 폼](C:\Users\multicampus\Desktop\포트폴리오\images\모아 사이트 스크린 캡쳐\회원가입 폼.JPG)

회원가입페이지입니다. 회원가입 페이지에서는 자신의 선호 카테고리를 설정할 수 있으며 전공, 휴대폰번호, 자기소개를 작성할 수 있도록 되어있습니다. 



#### 로그인 페이지

![로그인 폼](C:\Users\multicampus\Desktop\포트폴리오\images\모아 사이트 스크린 캡쳐\로그인 폼.JPG)

로그인 페이지입니다.



#### 메인페이지(로그인후)

![로그인 후 메인 페이지](C:\Users\multicampus\Desktop\포트폴리오\images\모아 사이트 스크린 캡쳐\로그인 후 메인 페이지.JPG)

로그인 후에 메인페이지에 들어가면 헤더의 카테고리들이 펀딩오픈, 마이페이지, 로그아웃으로 바뀌어있습니다. 

메인페이지에는 디자인, IT, 번역, 영상, 운세, 마케팅 6가지의 카테고리로 구분되어 있습니다. 



#### 메인페이지의 펀딩목록과 멘토 랭킹

![00.메인페이지02-w](C:\Users\multicampus\Desktop\포트폴리오\images\모아 사이트 스크린 캡쳐\모아 웹서비스 시연 사진\00.메인페이지\00.메인페이지02-w.jpg)

또한 메인페이지에서는 모집 중인 펀딩을 최신순으로 확인할 수 있으며

![메인페이지 멘토랭킹 리스트](C:\Users\multicampus\Desktop\포트폴리오\images\모아 사이트 스크린 캡쳐\메인페이지 멘토랭킹 리스트.JPG)

하단에는 멘토의 랭킹을 전부 확인할 수 있습니다. 
