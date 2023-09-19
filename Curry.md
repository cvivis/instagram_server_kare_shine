### 20221029 개발 일지
- ERD 1차 작성완료
- API 명세서 1차 완성

### 20221030 개발 일지
- RDS 테이블 세팅

### 20221031 개발 일지
- DB 연결
- 빌드 실행/확인
- Post 전체조회 (80%) (최근 날짜 정렬로 변경)

### 1101 
- 개발 서버 세팅, gradle build 에러 
- 2.1 게시물 목록 조회(홈화면) (follow 연동 X)
- 2.2 특정 게시물 조회
- 2.3 특정 유저 게시물 조회
- 2.4 게시물 탐색 

### 1102 
- 2.5 게시물 생성
- img_id/ img_url을 위한 로직 변경

### 1103 
- 1차 피드백 
- 샤인님 디비 연결 확인, api 확인 
- git 연결문제 발생 merge X (build 파일 permission 문제)

### 1104
- 인텔리제이 jdk 초기화 문제 
- git merge문제 해결X -> 해결도중 stash도 안되짐 (Problem 1) <br>
- img_id/ img_url가 한 포스트당 이미지별로 결과를 받아옴 (/app/posts 만 수정) <br>
ㄴ img_id와 img_url을 List로 받기위해 Post 타입 명시 

#### ㄴ 해결사항 
1. git merge 문제 
2. img_id와 img_url 다른 포스트 API 처리
### 1105 
- 모든 Post관련 img_id/ img_url 출력 변경 
- 문제 2 관련 급한 불 해결 <br>
  ㄴ 현재 작업중인 branch, origin에 push후 다시 클론

#### ㄴ 해결사항
1. 조회시 날짜 -> 몇일전으로 표시하기

### 1106
- Post 이미지 관련 validation 추가
- 작업 중 branch에서 파일 삭제가 되었는데 삭제가 안되어있는 문제 발생 <br>
  ㄴ 그 전 커밋으로 돌린 후 작업했던 branch closed 후 새 branch 생

#### ㄴ 해결사항
1. 조회시 날짜 -> 몇일전으로 표시하기

### 1107
- follow 작업 중 response 수정 필요성
- response 관련 로직 처리

#### ㄴ 해결사항
1. 조회시 날짜 -> 몇일전으로 표시하기

### 1108
- like 작업 중 response 수정 필요성
- response 관련 로직 처리

#### ㄴ 해결사항
1. 조회시 날짜 -> 몇일전으로 표시하기
2. 둘이 비슷한 로직 사용으로 가능할듯 

### 1108
- follow Api 작성 및 response 수정
- follow userlist로 가독성 좋게 리스트로 받아와짐
- userJwt로 userid 받아오기

#### ㄴ 해결사항
1. 조회시 날짜 -> 몇일전으로 표시하기 

### 1109
- like Api 작성 및 response 수정
- likeCount 빼고 구현
- 멘토님 피드백 -> validation 추가 ,트랜잭션 처리 추후 공부 방향

#### ㄴ 해결사항
1. 조회시 날짜 -> 몇일전으로 표시하기
2. likeCount 구현
3. follow - post연동해서 보여주기
4. 트랜잭션
5. validation 추가 
   <br> ㄴ userJwt로 userid 유효성검사
   <br> ㄴ postId없으면 포스트 접근 x 

### 1109
- llikeCount 구현
- follow - post연동해서 보여주기
- validation 추가
   <br> ㄴ postId 없으면 포스트 접근 x

#### ㄴ 해결사항
1. 조회시 날짜 -> 몇일전으로 표시하기
2. 트랜잭션 
3. validation 추가
   <br> ㄴ userJwt로 userid 유효성검사

### 1110
- 조회시 날짜 -> 몇일전으로 표시하기 진행
- 트랜잭션 진행
- validation 추가 진행
   <br> ㄴ userJwt로 userid 유효성검사

### 1111
- 시연영상 찍기 
- 조회시 날짜 -> 몇일전으로 표시하기 
- 트랜잭션 
- validation 추가 
  <br> ㄴ userJwt로 userid 유효성검사
