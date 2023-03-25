## **📎** Github Links

- **Organization**: [KUSITMS-1st-Kukathon-Together](https://github.com/KUSITMS-1st-Kukathon-Together)

- **Frontend**: [GitHub - KUSITMS-1st-Kukathon-Together/AOS](https://github.com/KUSITMS-1st-Kukathon-Together/AOS)

- **Backend**: [GitHub - KUSITMS-1st-Kukathon-Together/Server](https://github.com/KUSITMS-1st-Kukathon-Together/Server)
<img src="https://file.notion.so/f/s/1201acd9-3b24-40a0-aa31-adf7d63c4cc3/Untitled.png?table=block&id=4f521471-537a-4c5e-89d1-254eacc3f3cc&spaceId=a15e736d-1e85-48b0-a7fc-c3d9de9b90dd&expirationTimestamp=1679868552750&signature=qTSfCHAcM1U0OToaOrPPr1u3jTbSKUoH8lPFtnxJKbs&downloadName=Untitled.png">

## 👥 참여 학회원

| 분야 | 이름 | 프레임워크 |
| --- | --- | --- |
| 프론트엔드 | 김시연 | Android |
| 프론트엔드 | 정채현 | Android |
| 백엔드 | 김민근 | Spring Boot |
| 백엔드 | 정승연 | Spring Boot |

## ⚙️ 기술 스택

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

<img src="./source/Untitled.png">

## 💿 ER Diagram

<img src="./source/Untitled 1.png">

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
