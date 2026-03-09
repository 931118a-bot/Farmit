## 프로젝트 개요
Farmit - 소셜·일반 로그인 통합 인증 구조를 구현한 
         농산물 통합 판매 서비스 프로젝트

## 구현한 기능 (회원 + 소셜 로그인)
- 로그인 / 로그아웃 / 소셜로그인 기능

로그인 실패 및 탈퇴 계정 예외 처리
로그인 시 마지막 로그인 시간 업데이트
로그아웃 시 세션 무효화 처리
네이버 OAuth 2.0 로그인 연동
소셜 로그인 시 기존 회원과 소셜 계정 자동 연동 처리 
탈퇴 처리 중 계정 소셜 로그인 차단
소셜 계정 탈퇴 시 연동 해제 처리

- 회원가입 기능
아이디 중복 확인 (AJAX) 분기별 구분 처리 / 전화번호 중복 검사
생년월일 유효성 검증
비밀번호 암호화 저장
회원가입 완료 후 자동 로그인 처리
탈퇴 회원 재가입 7일 유예 처리(연락처 기준)

- 비밀번호 찾기 / 임시 비밀번호 발급
아이디 + 이름 + 이메일 검증
임시 비밀번호 랜덤 생성
비밀번호 암호화 후 DB 저장
이메일 발송 처리
임시 비밀번호 로그인 시 강제 변경 처리

- 마이페이지 기능
회원 정보 조회 (이메일/전화번호 마스킹 처리)
최근 주문 3건 조회
회원 정보 수정 기능
수정 전 비밀번호 재확인 기능 
소셜 회원 재인증(회원 정보 수정/탈퇴 시)

- 비밀번호 변경 기능
현재 비밀번호 검증
새 비밀번호 일치 검증
기존 비밀번호와 동일 여부 검사
임시 비밀번호 상태 해제 처리

- 회원 탈퇴 기능
장바구니 상품 존재 시 탈퇴 제한
논리 삭제 처리 (7일 후 자동 삭제 스케줄 처리)
소셜 로그인 계정 연동 해제 후 탈퇴

## 기술 스택
Language - Spring, Spring Boot, JSP/Servlet, Java, JSON, XML, HTML/CSS, JavaScript(ES 5+), Ajax, React, jQuery, Bootstrap, Python, Pandas, Django
Server - Apache Tomcat, Linux Ubuntu, AWS 
Tool - STS/Eclipse, VSCode, DBeaver, UML, Notion, Git/Github
DataBase - Oracle, MySQL/MariaDB, Sqlite3, myBatis, JPA, NoSQL(MongoDB)
API - Rest API, 소셜 로그인(Naver, Kakao), SMTP(ID/비밀번호 찾기), 간편 결제(Kakao Pay), OAuth, BCrypt, Daum Postcode API

## 발표 자료
- farmit_이승민.pptx
