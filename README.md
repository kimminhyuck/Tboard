📋 React 프로젝트 설정 가이드
📦 필수 패키지 설치
아래 명령어를 실행하여 프로젝트에 필요한 필수 패키지를 설치하세요.

bash
복사
편집
npm install axios react-router-dom bootstrap jwt-decode react-cookie redux react-redux redux-thunk react-hook-form yup react-icons @mui/material @mui/icons-material
📄 패키지 설명
패키지명	설명
axios	백엔드와의 HTTP 통신을 위한 라이브러리 (Spring Boot 연동)
react-router-dom	클라이언트 사이드 라우팅을 위한 라이브러리
bootstrap	반응형 UI 스타일링을 위한 Bootstrap 5 지원
jwt-decode	JWT 토큰 디코딩 및 사용자 정보 추출
react-cookie	쿠키 기반의 인증 및 상태 관리
redux	전역 상태 관리 라이브러리
react-redux	React와 Redux를 연동하는 라이브러리
redux-thunk	비동기 작업을 처리하기 위한 Redux 미들웨어
react-hook-form	React에서 폼을 쉽게 관리하기 위한 라이브러리
yup	폼 유효성 검사를 위한 스키마 기반 라이브러리
react-icons	다양한 아이콘(FontAwesome, Material 등) 지원
@mui/material	Material-UI 컴포넌트 라이브러리
@mui/icons-material	Material-UI 아이콘 라이브러리
🛠 프로젝트 실행 방법
패키지 설치

bash
복사
편집
npm install
개발 서버 실행

bash
복사
편집
npm start
React 애플리케이션 접속

브라우저에서 http://localhost:3000에 접속
📂 프로젝트 폴더 구조
csharp
복사
편집
react_board/
│-- node_modules/         # 패키지 종속성
│-- public/               # 정적 파일 (favicon, index.html)
│-- src/                   # 소스 코드
│   ├── api/               # API 호출 관리 (axios)
│   ├── components/        # 재사용 가능한 컴포넌트
│   ├── pages/             # 주요 페이지 컴포넌트
│   ├── styles/            # CSS 및 스타일링
│   ├── App.js             # 메인 애플리케이션 파일
│   ├── index.js           # React 진입점
│   └── setupTests.js      # 테스트 설정
│-- .gitignore             # Git 무시 파일
│-- package.json           # 프로젝트 의존성 및 설정
│-- README.md              # 프로젝트 설명 파일
