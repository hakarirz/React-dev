React 초기 설정
1. 작업 폴더 생성 (이름은 아무거나(React)
2. 폴더 우클릭 후 터미널 실행 (관리자 X)
3. Git 사용자 정보 설정 입력 (git config --global user.name "이름" / git config --global user.email "이름@gmail.com")
4. React 앱 생성 npx create-react-app my-app / npm create-react-app 프로젝트명 (npx,npm 차이가 npx가 매번 최신 버전)

React 배포 방법
1. GitHub 리포지토리 생성 (React-dev)
2. React 프로젝트 생성 (npx create-react-app React-dev)
3. gh-pages 패키지 설치 (터미널 -> npm install gh-pages --save-dev)
4. package.json 파일 수정 (
"homepage": "https://your-username.github.io/apps",
"scripts": {
  "predeploy": "npm run build",
  "deploy": "gh-pages -d build"
}
)
5. Git 초기화 및 커밋 (
   git init
   git add .
   git commit -m "커밋하고 남길 메세지"
6. 원격 저장소 추가 (
   터미널 -> git remote add origin https://github.com/<your-username>/apps.git
   git branch -M main
   git push -u origin main
7. 배포 (터미널 -> npm run deploy)
