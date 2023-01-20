# 쇼핑몰 길마로🖲

# 팀프로젝트 : GILMARO 스마트 웹앱 구현 
by)김선민(조장/피그마 디자인 시안/프론트엔드),  
   권동환(팀원/백엔드/프론트엔드),      
   이준무(팀원/피그마 디자인 시안/ 프론트엔드/백엔드)
### 기존 길마로 홈페이지를 참고하여 프로젝트를 진행 하였음
#### 프로젝트 기간 : 2023.01.09~2023.01.18
#### 기본 업체 홈페이지 : www.gilmaro.co.kr/
#### 피그마 시안 : https://www.figma.com/file/cO0KZkw8EqCr8mfsko14dx/GILMARO-%EB%B8%8C%EB%9E%9C%EB%93%9C%EC%83%B5-%EC%A0%9C%EC%9E%91-%EC%BD%98%EC%85%89%ED%8A%B8?node-id=140%3A298&t=Ycu9sTc6UErOXXao-1
#### 배포 : https://port-0-node-ejs-gilmaro-19k5ygi525lcsucitd.gksl2.cloudtype.app/
#### 서버운영 : https://cloudtype.io
##### 📌개발환경 : 운영체제 윈도우10 chrome✅
##### 📌사용 코드에디터 : vs code
##### 📌개발언어: HTML, CSS, JavaScript 
##### 📌사용 모듈: node.js, express, sqlite3, sequelize, cookie-parse 활용 

# 제작 목표📑
#### 1. 기존 홈페이지를 참고하되. 상품의 간결화
#### 2. 실제 회원가입, 로그인 정보수정 등 기능 구현
#### 3. 장바구니, 찜목록등 session 과 cookie 등 브라우저의 기능 활용

# 사이트 메인 페이지📰
![image](https://user-images.githubusercontent.com/113665619/213124879-0cbb4815-38ab-4fdb-b7ad-cc4bfaedbc54.png)

# 페이지별 소개
<details>
<summary>공통사항</summary>




<details>
<summary>header</summary>
![image](https://user-images.githubusercontent.com/113665599/213631073-4e97bbed-aad9-4170-88b7-c58b2c18c213.png)
![image](https://user-images.githubusercontent.com/113665599/213631229-9baf86c1-eaa8-4d2e-ad85-53048d758e27.png)


### logo 및 검색,장바구니 구현   
✅ 검색: 클릭시 검색창이 따로 나타나며 실제 검색기능까지 구현 완료.   
✅ 장바구니: 제품상세페이지에서 장바구니담기 클릭시 이 장바구니로 정보 이동    
실제로 수량,금액,색상등 변경가능  + 로그인 필요
✅ 구매기능은 미구현


</details>

## 장바구니     
![image](https://user-images.githubusercontent.com/113665599/213632702-5e1cd3d0-9a9f-4241-8ecc-46f40ae26b5c.png)   

### 실제 담은 상품, 삭제, 수량 및 색상 변경 금액 합산 기능 구현     
✅ 상품정보: 이름, 금액 등 실제 존재하는 정보를 불러옴 ( session 활용 )      
✅ 수량 및 색상 변경: 변경시 밑에 합산 금액 실시간 변경 및 합산금액 자동 산출 ( ejs 문법 활용 )






</details>
<details>
<summary>메인</summary>


![image](https://user-images.githubusercontent.com/113665619/213124879-0cbb4815-38ab-4fdb-b7ad-cc4bfaedbc54.png)


</details>
<details>
<summary>제품소개</summary>




</details>
<details>
<summary>제품 상세소개</summary>




</details>
<details>
<summary>주문제작의뢰</summary>




</details>
<details>
<summary>관리자전용페이지</summary>




</details>
<details>
<summary>내정보</summary>




</details>



