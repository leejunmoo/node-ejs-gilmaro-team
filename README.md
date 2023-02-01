# 쇼핑몰 길마로🖲

## 팀프로젝트: GILMARO 스마트 웹앱 구현 
by)김선민(조장/피그마 디자인 시안/프론트엔드),  
   권동환(팀원/백엔드/프론트엔드),      
   이준무(팀원/피그마 디자인 시안/ 프론트엔드/백엔드)    
       - Header & Footer 틀 제작    
       - 제품상세소개 , 주문제작의뢰 , 관리자전용페이지 제작    
       - 주문제작의뢰에 이용되는 DB 제작    
       - 디자인 시안 참여 ( 제작된 메인틀에 맡은 페이지제작 추가 )    
       - 로그인 기능 , 회원정보 DB 제작 참여 / 회원수정기능제작 참여    
   
### 기존 길마로 홈페이지를 참고하여 프로젝트를 진행 하였음
#### 프로젝트 기간 : 2023.01.09~2023.01.18
#### 기본 업체 홈페이지 : www.gilmaro.co.kr/
#### 피그마 시안 : https://www.figma.com/file/cO0KZkw8EqCr8mfsko14dx/GILMARO-%EB%B8%8C%EB%9E%9C%EB%93%9C%EC%83%B5-%EC%A0%9C%EC%9E%91-%EC%BD%98%EC%85%89%ED%8A%B8?node-id=140%3A298&t=Ycu9sTc6UErOXXao-1
#### 배포 : https://port-0-node-ejs-gilmaro-team-fyyf25lboho2ya.gksl2.cloudtype.app/
##### 📌개발환경 : 운영체제 윈도우10 chrome
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

***

### logo 및 검색,장바구니 구현

***


✅ 검색: 클릭시 검색창이 따로 나타나며 실제 검색기능까지 구현 완료.   
✅ 장바구니: 제품상세페이지에서 장바구니담기 클릭시 이 장바구니로 정보 이동    
실제로 수량,금액,색상등 변경가능  + 로그인 필요   
✅ 구매기능은 미구현


</details>
<details>
<summary>장바구니</summary>    

![image](https://user-images.githubusercontent.com/113665599/213632702-5e1cd3d0-9a9f-4241-8ecc-46f40ae26b5c.png)   

***

### 실제 담은 상품, 삭제, 수량 및 색상 변경 금액 합산 기능 구현     

***

✅ 상품정보: 이름, 금액 등 실제DB 정보를 불러옴 ( session+storage 활용 )   
  장바구니에담기를 눌렀던 제품을 session 에 저장 후 장바구니(결제) 페이지 이동시 session 에 저장된 정보를 DB에서 찾아 제품을 불러옴     
✅ 수량 및 색상 변경: 변경시 밑에 합산 금액 실시간 변경 및 합산금액 자동 산출 ( ejs 문법 활용 )


</details>
<details>
<summary>footer</summary>   

![image](https://user-images.githubusercontent.com/113665599/213643685-5b69c6fc-d1bd-455e-b3d9-5e3faa841564.png)
![image](https://user-images.githubusercontent.com/113665599/213643845-27f4b2bc-181b-472d-a0e5-26db5aecea91.png)
![image](https://user-images.githubusercontent.com/113665599/213644060-118bcd69-b3ef-42bb-a9a9-2b787860f710.png)



***

### 찜목록, 로그인 + 로그아웃, 기능 구현

***

✅ 홈: 메인화면 이동   
✅ 사이트맵   
✅ 찜목록: 제품옆에 ♡ 모양 클릭시 색이채워지면서 찜목록에 담김 (재클릭시 취소)   
✅ 로그인: 각각의 상태에 따라 icon 모양 자동변경 / 로그인이 필요할 경우 입력창 등장 /   
로그아웃이 필요할 경우 누르면 로그아웃 창 등장

</details>

</details>
<details>
<summary>메인</summary>


![image](https://user-images.githubusercontent.com/113665619/213124879-0cbb4815-38ab-4fdb-b7ad-cc4bfaedbc54.png)


</details>
<details>
<summary>제품소개</summary>

![image](https://user-images.githubusercontent.com/113665599/213646863-5ad5bf5e-a0b8-4271-897b-77f6aaff846f.png)

***

### lnb - 브랜드 클릭시 제품군에따른 분류기능

***





</details>
<details>
<summary>제품 상세소개</summary>

![image](https://user-images.githubusercontent.com/113665599/214778126-c016bc78-22ef-4403-9a6b-309e6213349d.png)

***

### 제품상세소개 에서만 나오는 하단 btn-box / 제품이름, 가격, 브랜드 등 모두 DB에서 가져옴

***

✅ 장바구니담기: 찜목록과는 별개로 사용됨 클릭시 장바구니(결제)홈페이지에 제품이 담김   
✅ 바로구매하기: 실제 결제 기능은 미구현. 클릭시 장바구니(결제)홈페이지로 이동 ( 로그인 필요 )


</details>
<details>
<summary>주문제작의뢰</summary>

![image](https://user-images.githubusercontent.com/113665599/214778957-081e412e-68eb-4d89-ac03-9b4b2966df63.png)
![image](https://user-images.githubusercontent.com/113665599/214779561-a45ff1a8-feef-4fa0-a478-46e35d0fc4be.png)
![image](https://user-images.githubusercontent.com/113665599/214779574-16f61a61-d939-438a-93e9-5a30ece187e4.png)


***

### 주문제작 버튼: 모든 페이지에서 하단nav 처럼 떠다니게 만듬 클릭시 주문제작의뢰서로 이동

***

✅ 이름, 이메일, 연락처 : 빈값 금지 설정 및 규격(패턴)에 맞게 입력값 설정   
✅ 입력한 내용이 그대로 DB에 저장되서 관리자전용페이지에서 확인할수 있음



</details>
<details>
<summary>관리자전용페이지</summary>

![image](https://user-images.githubusercontent.com/113665599/214780357-5d786fd0-83fe-4409-865c-fd63fdb77492.png)
![image](https://user-images.githubusercontent.com/113665599/214780405-964d86d8-aebe-447c-88bf-6686458653ce.png)


***

### 관리자전용아이디로 로그인필요( cookie 활용 관리자전용아이디 인가? 판별후 페이지 로딩 아닐경우 경고창 등장 )   
### 저장된 DB를 Table 형식으로 보여줌

***

✅ 순번, 이름, 이메일주소, 연락처: 실제 저장된 DB에서 정보를 불러와 보여줌   
✅ 관리자(주문제작상세내역): 이 페이지또한 실제 저장된 DB에서 정보를 불러와 보여줌


</details>
<details>
<summary>내정보</summary>

![image](https://user-images.githubusercontent.com/113665599/214781289-65d10f6b-5c0b-4732-9c8e-e2ea1919da87.png)

***

### 실제 정보 수정 및 회원탈퇴 가능 input 박스를 이용해   
### 따로 수정버튼 을 누르고 수정하는 방식x 바로입력후 밑 수정버튼 클릭

***

</details>



