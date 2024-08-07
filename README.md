# 위캔필라테스 Admin

- 위캔필라테스 상담예약 관리
- 위캔필라테스 회원 / 회원권 관리
- 위캔필라테스 강사 관리
- 지점 당 매출 관리
- 회원님의 출석율에 따른 케어 문자 발송 및 관리

<br>

### 개발 환경

- Front-end : Flutter
- Back-end : AWS를 활용한 node.js
- 버전 및 이슈관리 : Github, CodePipeline, Elastic Beanstalk
- 협업 툴 : Github, Notion, Slack
- 서비스 배포 환경 : AWS
- DB : MySQL, AWS RDS, S3

<br>


### 마일스톤
- **2023년 5월 - 2023년 11월**
    - 기존 웹 UI 대규모 리뉴얼
    - 회원님의 출석율에 따른 케어 문자 발송 기능 구현
    - 지점이 늘어감에 따른 디버깅

<br>

## 화면구성


| 로그인 | 상담예약 |
|:--:|:--:|
|![login](https://github.com/user-attachments/assets/e4246a21-86bd-4647-9a19-9ee32e2261c1)|![councel](https://github.com/user-attachments/assets/07f0bdca-b50c-4719-b7e0-ece11a984e92)|
| 회원목록 | 회원정보 |
|![member](https://github.com/user-attachments/assets/bd2c583c-593d-4567-92a0-661dcf0f1ec8)|![info](https://github.com/user-attachments/assets/1f993436-3c6a-4b65-bb03-5a391c4435cd)|
| 회원권 | 회원권 정보 |
|![ticket](https://github.com/user-attachments/assets/436136e5-62a5-4d77-9e49-4d7c2a40444c)|![ticket-regi](https://github.com/user-attachments/assets/682dfc99-6701-4190-9552-386486f366d9)|

### 로그인
- 로그인이 되어 있지 않은 경우 : 로그인 페이지
- 로그인이 되어 있는 경우 : 상담예약 페이지
- 관리자가 1명이라 자동로그인 기능은 사용되지 않았음

### 상담예약
- 캘린더에 상담현황 표시
- 어제 / 오늘의 상담 실적 표시
- 상담 마쳤을 시 메모 기능

### 회원 / 회원권
- 상담문의 / 방문상담 / 회원등록(결제) / 만료예정 / 재등록 탭으로 나누어 관리
- 회원등록 / 수정 시 상태에 따라 각 탭에 맞추어 등록 / 수정됨
- 해당 회원의 회원권을 모두 표시(만료된 회원권까지)
- 특정 기간 안에 해당하는 회원권 표시
- 회원권 마다 색으로 구분
- pt강의 일 때 고정수업 / 담당 강사 등록
- 결제 정보까지 회원권에 함께 등록

<br><br>

| 강사목록 | 강사 정보 | 강사 개인PT |
|:--:|:--:|:--:|
|![director](https://github.com/user-attachments/assets/2ff84fb2-1b61-4729-a453-0791469d0cdd)|![director-info](https://github.com/user-attachments/assets/70746779-4bfa-4d9e-8517-71422ce56186)|![director-pt](https://github.com/user-attachments/assets/25ce8de2-f977-44d4-acf3-10677dde198f)|

### 강사
- 강사 / 강사정보 / 강사별 개인PT 정보 관리

<br><br>

| 매출현황 | 출석율 | 문자내역 |
|:--:|:--:|:--:|
|![money](https://github.com/user-attachments/assets/e916c15e-2858-46b1-addf-7ca17b5a5c94)|![coaching](https://github.com/user-attachments/assets/02c913c3-da56-4910-9858-cc86b57fb3c6)|![sms](https://github.com/user-attachments/assets/b0d56ada-317f-4b6c-8b4e-1bf064d47069)|

### [매출현황]
- 매장별 매출 현황 표시
- 단체수업에 따라 매출율 따로 표시

### [출석율]
- 출석률을 양호 / 보통 / 미흡으로 나누어 관리
- 미흡일 시 개별 / 단체로 문자 발송

### [문자내역]
- 문자 발송 내역 확인
