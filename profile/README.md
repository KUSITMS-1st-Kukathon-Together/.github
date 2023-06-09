
<img src="./profile/source/thumbnail.png">

##  **✨ 온길, Ongil**
**당신의 온길이, 온기가 되다**

## **📎** Github Links

- **Organization**: [KUSITMS-1st-Kukathon-Together](https://github.com/KUSITMS-1st-Kukathon-Together)

- **Frontend**: [GitHub - KUSITMS-1st-Kukathon-Together/AOS](https://github.com/KUSITMS-1st-Kukathon-Together/AOS)
<img src="https://file.notion.so/f/s/8562d8b9-416b-4668-9e28-b43d61a524ff/Untitled.png?table=block&id=ac0f78c8-dbf6-4a9b-9981-8e64921a5414&spaceId=a15e736d-1e85-48b0-a7fc-c3d9de9b90dd&expirationTimestamp=1679870994610&signature=x91X_UINcaY5ObOspibY4UHM2HYIXy5qwLSKZ2E5-Gg&downloadName=Untitled.png">

- **Backend**: [GitHub - KUSITMS-1st-Kukathon-Together/Server](https://github.com/KUSITMS-1st-Kukathon-Together/Server)
<img src="https://file.notion.so/f/s/8e2707f9-10e4-478f-b9fa-acb6e6d63b55/Untitled.png?table=block&id=ac306541-a689-4a75-b8c9-24ad77777d9a&spaceId=a15e736d-1e85-48b0-a7fc-c3d9de9b90dd&expirationTimestamp=1679871057003&signature=BvlibBRHJLHiS57G2_wt6FHdZQdR6i0lJQOlb8e2SIk&downloadName=Untitled.png">

## 👥 참여 학회원

| 분야 | 이름 | 프레임워크 |
| --- | --- | --- |
| 프론트엔드 | 김시연 | Android |
| 프론트엔드 | 정채현 | Android |
| 백엔드 | 김민근 | Spring Boot |
| 백엔드 | 정승연 | Spring Boot |

## ⚙️ 기술 스택

#### Frontend
<img src="https://img.shields.io/badge/Kotlin-F48E00?style=for-the-badge&logo=Kotlin&logoColor=white"/> <img src="https://img.shields.io/badge/Android Studio-3DDC84?style=for-the-badge&logo=Android Studio&logoColor=white">

#### Backend
<img src="https://img.shields.io/badge/java-007396?style=for-the-badge&logo=java&logoColor=white"> <img src="https://img.shields.io/badge/springboot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white"> <img src="https://img.shields.io/badge/Spring Security-6DB33F?style=for-the-badge&logo=Spring Security&logoColor=white"> <img src="https://img.shields.io/badge/mysql-4479A1?style=for-the-badge&logo=mysql&logoColor=white"> <img src="https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=JSON%20web%20tokens&logoColor=white" alt="icon" /> <img src="https://img.shields.io/badge/amazonaws-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white"> <img src="https://img.shields.io/badge/AWS RDS-527FFF?style=for-the-badge&logo=Amazon RDS&logoColor=white"> <img src="https://img.shields.io/badge/AWS EC2-FF9900?style=for-the-badge&logo=Amazon EC2&logoColor=white"> <img src="https://img.shields.io/badge/AWS S3-569A31?style=for-the-badge&logo=Amazon S3&logoColor=white"> <img src="https://img.shields.io/badge/GitHub Actions-2088FF?style=for-the-badge&logo=GitHub Actions&logoColor=white"> <img src="https://img.shields.io/badge/NGINX-009639?style=for-the-badge&logo=NGINX&logoColor=white"> <img src="https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=Postman&logoColor=white"/>

## 🔖 온길 기능명세서

| **대분류** | **소분류**                    | **할당**       | **설명**                                            | **수행** |
|---------|----------------------------|--------------|---------------------------------------------------|--------|
| 회원가입    | 회원가입 View                  | 프론트엔드        |                                                   | Yes    |
|         | 위치 조회 서비스                  | 프론트엔드        | "Google Maps 기반으로 위도, 경도, 상세 주소 제공"               | Yes    |
|         | ID 중복처리 API                | "백엔드, 프론트엔드" |                                                   | Yes    |
|         | 회원가입 API                   | "백엔드, 프론트엔드" | BCryptEncoder 사용                                  | Yes    |
|         | 회원가입 토큰 발행                 | 백엔드          | JWT 사용                                            | Yes    |
|         |                            |              |                                                   |      |
| 로그인     | 로그인 View                   | 프론트엔드        |                                                   | Yes    |
|         | 로그인 API                    | "백엔드, 프론트엔드" | BCryptEncoder 사용                                  | Yes    |
|         | 로그인 토큰 발행                  | 백엔드          | JWT 사용                                            | Yes    |
|         |                            |              |                                                   |      |
| 메인      | "메인 페이지 View (조심해요, 추천해요)" | 프론트엔드        |                                                   | Yes    |
|         | 현 위치 기반 2km 이내 게시글 조회      | 백엔드          | SQL 쿼리문 기반 위치 계산                                  | Yes    |
|         | 카테고리별 게시글 필터링 및 최신순 정렬     | 백엔드          |                                                   | Yes    |
|         | 게시글 제목 키워드 검색 및 최신순 정렬     | 백엔드          |                                                   | Yes    |
|         | 메인 페이지 게시글 목록 조회 API       | "백엔드, 프론트엔드" | 3개의 기능을 합쳐 API 하나로 구현                             | Yes    |
|         |                            |              |                                                   |      |
| 게시글 작성  | 게시글 작성 View                | 프론트엔드        |                                                   | Yes    |
|         | 위치 조회 서비스                  | 프론트엔드        | "Google Maps 기반으로 위도, 경도, 상세 주소 제공"               | Yes    |
|         | 게시글 작성 API                 | "백엔드, 프론트엔드" |                                                   | Yes    |
|         |                            |              |                                                   |      |
| 게시글 상세  | 게시글 상세 View                | 프론트엔드        |                                                   | Yes    |
|         | 게시글 댓글 작성                  | "백엔드, 프론트엔드" |                                                   | Yes    |
|         | 게시글 대댓글 작성                 | "백엔드, 프론트엔드" | 순환관계 테이블 구성                                       | Yes    |
|         | 게시글 좋아요 / 좋아요 취소           | "백엔드, 프론트엔드" |                                                   | Yes    |
|         | 댓글 작성 View                 | 프론트엔드        |                                                   | Yes    |
|         |                            |              |                                                   |      |
| API 서버  | 무중단 CI/CD 서버 구축            | 백엔드          | Github Actions + EC2 + S3 + CodeDeploy / nginx 사용 | Yes    |
|         | JWT 필터 구현                  | 백엔드          | Spring Security 사용                                | Yes     |
|         | DB 서버 구축                   | 백엔드          | RDS 사용                                            | Yes     |
|         |                            |              |                                                   |      |


## 🧩 시스템 아키텍쳐

<img src="./profile/source/Untitled.png">

## 💿 ER Diagram

<img src="./profile/source/Untitled 1.png">

## 📚 API 문서

| **메소드** | **URI**                       | **설명**       | **구현** | **메모** |
|---------|-------------------------------|--------------|--------|--------|
| GET     | /health                       | 서버 생존 여부 체크  | Yes    |        |
| POST    | /api/auth/sign-up             | 회원가입         | Yes    |        |
| POST    | /api/auth/login               | 로그인          | Yes    |        |
| POST    | /api/auth/verify              | ID 중복 체크     | Yes    |        |
| GET     | /api/main                     | 메인페이지 조회     | Yes    |        |
| GET     | /api/post/{postId}            | 게시글 상세 정보 조회 | Yes    |        |
| POST    | /api/post                     | 게시글 작성       | Yes    |        |
| POST    | /api/post/{postId}/comment    | 댓글 작성        | Yes    |        |
| POST    | /api/post/{postId}like        | 게시글 좋아요      | Yes    |        |
| POST    | /api/search?keyword={keyword} | 제목기반 검색      | Yes    |        |문서](Github%E1%84%8B%E1%85%A6%20%E1%84%8B%E1%85%A9%E1%86%AF%E1%84%85%E1%85%B5%E1%86%AF%20README%20827a95ea93f74fa3b5674e53ce451f5d/API%20%E1%84%86%E1%85%AE%E1%86%AB%E1%84%89%E1%85%A5%2084d6162273574fc2a2950a76e85f989c.md)
