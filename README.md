React 초기 설정 <br>
1. 작업 폴더 생성 (이름은 아무거나(React) <br><br>
2. 폴더 우클릭 후 터미널 실행 (관리자 X) <br><br>
3. Git 사용자 정보 설정 입력 <br><br>
git config --global user.name "이름" <br>
git config --global user.email "이름@gmail.com" <br><br>
4. React 앱 생성 <br><br>
npx create-react-app my-app / npm create-react-app 프로젝트명 (npx,npm 차이가 npx가 매번 최신 버전) <br><br>

React 배포 방법 <br><br>
1. GitHub 리포지토리 생성 (React-dev) <br><br>
2. React 프로젝트 생성 (npx create-react-app React-dev) <br><br>
3. gh-pages 패키지 설치 (터미널 -> npm install gh-pages --save-dev) <br><br>
4. package.json 파일 수정 <br><br>
"homepage": "https://your-username.github.io/apps",<br> <br>
"scripts": { <br>
  "predeploy": "npm run build", <br>
  "deploy": "gh-pages -d build" <br>
} 
<br>
5. Git 초기화 및 커밋 <br><br>
   git init <br>
   git add . <br>
   git commit -m "커밋하고 남길 메세지" <br><br>
6. 원격 저장소 추가 <br>
     터미널 -> git remote add origin https://github.com/<your-username>/apps.git <br>
   git branch -M main <br>
   git push -u origin main <br><br>
7. 배포 (터미널 -> npm run deploy)
