README.md안에내요을 배포 시 빌드 (React)

bash
복사
편집
cd client
npm run build이렇게 안에있는것처럼 한번에줘
ChatGPT의 말:
ChatGPT
아래 내용을 README.md 파일에 복사하여 사용하세요.

markdown
복사
편집
# 🚀 MRT 프로젝트 (React + Node.js + MongoDB)

이 프로젝트는 **React(프론트엔드)**, **Node.js(백엔드)**, **MongoDB(데이터베이스)**를 활용하여 인증 및 상태 관리를 포함한 웹 애플리케이션입니다. JWT + Refresh Token + 소셜 로그인을 통해 보안을 강화했습니다.

---

## 📂 프로젝트 폴더 구조

MRT/ │-- client/ # React 프론트엔드 │ ├── node_modules/ # 패키지 종속성 │ ├── public/ # 정적 파일 (favicon, index.html) │ ├── src/ # 소스 코드 │ │ ├── api/ # API 호출 관리 (axios) │ │ ├── components/ # 재사용 가능한 컴포넌트 │ │ ├── pages/ # 주요 페이지 컴포넌트 │ │ ├── styles/ # CSS 및 스타일링 │ │ ├── App.js # 메인 애플리케이션 파일 │ │ ├── index.js # React 진입점 │ │ └── setupTests.js # 테스트 설정 │ ├── .env # 환경 변수 설정 │ ├── package.json # 프론트엔드 의존성 및 설정 │ ├── README.md # 프로젝트 설명 파일 │-- server/ # Node.js 백엔드 │ ├── config/ # 환경 설정 (DB 연결) │ ├── controllers/ # 라우트 핸들링 로직 │ ├── middleware/ # 인증 미들웨어 │ ├── models/ # 데이터베이스 모델 (MongoDB) │ ├── routes/ # 라우트 설정 │ ├── utils/ # JWT 유틸리티 │ ├── .env # 환경 변수 설정 │ ├── server.js # 서버 진입점 │ ├── package.json # 백엔드 의존성 및 설정 │ ├── README.md # 프로젝트 설명 파일 └── README.md # 전체 프로젝트 설명 파일

yaml
복사
편집

---

## 📦 필수 패키지 설치 및 설정

### 🔹 클라이언트 (React)

```bash
cd client
npm install axios react-router-dom bootstrap jwt-decode react-cookie redux react-redux redux-thunk react-hook-form yup react-icons @mui/material @mui/icons-material
프로젝트 실행 방법
bash
복사
편집
npm start
.env 파일 설정
bash
복사
편집
REACT_APP_API_URL=http://localhost:5000/api
🔹 백엔드 (Node.js + Express + MongoDB)
bash
복사
편집
cd server
npm install express mongoose dotenv jsonwebtoken bcryptjs cors morgan cookie-parser
서버 실행 방법
bash
복사
편집
node server.js
.env 파일 설정
makefile
복사
편집
MONGO_URI=mongodb://localhost:27017/mrt
JWT_SECRET=your_jwt_secret_key
PORT=5000
🔐 인증 및 보안 기능
JWT 인증: 로그인 시 JWT 발급 및 보관
Refresh Token: JWT 토큰 갱신 처리
소셜 로그인: Google, Facebook, Naver OAuth 연동 가능
비밀번호 암호화: bcrypt를 사용한 보안 강화
CORS 설정: React 프론트엔드와 연동을 위한 보안 조정
🚀 주요 기능
회원가입 및 로그인

JWT 기반의 로그인 및 인증
소셜 로그인 (구글, 페이스북, 네이버)
프로필 조회 및 수정

JWT를 통한 유저 정보 보호
비밀번호 재설정

이메일 인증 후 비밀번호 변경
🛠 개발 및 배포
개발 모드 실행
bash
복사
편집
# 클라이언트 실행
cd client
npm start

# 서버 실행
cd server
node server.js
배포 시 빌드 (React)
bash
복사
편집
cd client
npm run build
🔍 API 엔드포인트
HTTP Method	Endpoint	설명
POST	/api/auth/register	회원가입
POST	/api/auth/login	로그인
GET	/api/auth/profile	사용자 프로필 조회
PUT	/api/auth/update-profile	프로필 수정
POST	/api/auth/reset-password	비밀번호 재설정 요청
📜 라이센스
이 프로젝트는 자유롭게 사용하실 수 있습니다.

go
복사
편집

이제 `README.md` 파일에 복사하여 프로젝트에 적용하세요. 🚀





