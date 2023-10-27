## AppWrite를 이용한 Login 페이지 구현

pm2 kill 후
pm2 status로 확인

 pm2 serve build --name login --port 2308 --spa
pm2 restart 0 --watch
-> 아직 빌드 안된 상태
npm run 

## Login 페이지 메인화면
![Login](https://github.com/ChamChiii7/EcoleProject/assets/126247047/29ee1156-9491-48a3-b82f-2b2014ace887)

## react 렌더링이 안되고 있는 관계로 register 화면은 현재는 구현 X
현재 화면의 Logout 버튼 삭제 후 이미 로그인을 한 유저들의 화면에만 Logout 구현.
register 버튼 삭제하고 링크 형식으로 register 렌더링 예정.
register 화면에서는 사용자의 email, password, name 입력 받아서 계정 생성.
