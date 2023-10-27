## AppWrite를 이용한 Login 페이지 구현

pm2 kill 후 pm2 status로 확인 <br>
pm2 serve build --name login --port 2308 --spa <br>
pm2 restart 0 --watch <br>
-> 아직 빌드 안된 상태 <br>
npm run <br>

## Login 페이지 메인화면
![Login_main](https://github.com/ChamChiii7/EcoleProject/assets/126247047/3858356c-88f6-4828-8365-b63de7faee99)

## 사용자에게 email,password,name 입력 받아서 계정 생성
![create](https://github.com/ChamChiii7/EcoleProject/assets/126247047/1eb50230-ba4b-40d8-93f0-60806175c3ed)

## 사용자에게 email,password 입력 받아서 로그인
![login](https://github.com/ChamChiii7/EcoleProject/assets/126247047/7ea94873-3a18-40d0-835e-da6f9bfad28c)

## react 렌더링이 안되고 있는 관계로 register 화면은 현재는 구현 X
현재 화면의 Logout 버튼 삭제 후 이미 로그인을 한 유저들의 화면에만 Logout 구현. <br>
register 버튼 삭제하고 링크 형식으로 register 렌더링 예정. <br>
register 화면에서는 사용자의 email, password, name 입력 받아서 계정 생성. <br>
