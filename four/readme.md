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

## 느낀점
군대 가기 전인 약 3년전에 마지막으로 react를 사용해보고 이번에 처음 다시 사용해봐서
너무 낯설게 느껴졌다. 굉장히 오랜 시간동안 계속 register 페이지로 넘어가지 않았고,
결국 끝까지 해결하지 못했지만, 문제를 해결하기 위해 link 등 이것저것 많이 시도해보면서
거의 하나도 모르다싶이 했던 react에 대해 조금 더 알게 되었다. 디자인도 오랜 시간 만졌는데,
후반부에 교수님이 알려주신 pico css로 빠르게 디자인하는걸 보면서 기술의 소중함을 느꼈다.
