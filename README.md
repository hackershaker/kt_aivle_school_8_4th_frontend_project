## 📌 KT AIVLE School 8기 4차 미니프로젝트 – Backend

  React + vite 기반 프론트엔드 프로젝트입니다.<br>
  백엔드(Spring Boot)와 연동되며, REST API를 요청하고 유저 인터페이스를 제공하는 역할을 수행합니다.

## 👥 Team Structure

  PM : 조유송 <br>
  Backend : 나도요, 나성곤, 정성호<br>
  Frontend : 이정민, 이동규, 조유송<br>

## Skills

    React
    Vite
    Fetch
    axios
    


## Project Structure 
  components.book.BookCard - 메인 카드 목록 기술 - 사용X
  components.book.ui.Test - 서버 연결 상태 확인 - 테스트 용
  
  pagesㅡㅡBDPage - 상세 페이지 (요청 : axios , UI : CSS)
        |ㅡ MainPage - 메인 페이지 (요청 : axios, UI : CSS)
        |ㅡ NewBookCoverPage - AI 이미지 생성 페이지 (요청 : fetch , UI : MUI)
        |ㅡ NewBookPage - 새로운 책 등록 페이지 (요청 : fetch , UI : MUI)
        ㄴ  RevisePage - 기존 책 수정 페이지 (요청 : axios , UI : MUI)
  App - 페이지 경로 설정 
    

## Start 
  1. backEnd Server 생성 > `https://github.com/nsg716/kt_aivle_school_8_4th_backend_project` ->bootWar 빌드 ->java -jar (servername).war 

  2. front 파일중 public, src, eslint.config.js, index.html, package.json, package-lock.json, vite.config.js 파일 복제 후 새 폴더에 생성 

  3. 폴더 위치에서 CMD 명령어로 1. npm install 2. npm run build 수행 

  4. 폴더 위치에서 npm run preview 
  


## Project Requirements
  페이지 경로 설정 : App.jsx에 명시 
      import {Route, Routes} from "react-router-dom";
      import MainPage from "./pages/MainPage.jsx";
      ...
      <Routes>
        {/* 메인 페이지 */}
        <Route path="/" element={<MainPage/>}/>
  MUI 컴포넌트 :  NewBookCoverPage.jsx, NewBookPage.jsx, RevisePage.jsx 에서 사용
  fetch 요청 : NewBookCoverPage.jsx, NewBookPage.jsx 에서 적용
  
## 각 페이지별 주소 
  기본 주소 : http://localhost:5173
  주소                         |    페이지
  ㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡ
  /                            |  MainPage.jsx
  /detail/{bookID}             |  BDPage.jsx
  /edit/{bookID}               |  RevisePage.jsx
  /register                    |  NewBookPage.jsx
  /detail/{bookID}/updateCover |  NewBookCoverPage.jsx

## 차후 계획 

  Back : UserDTO추가 및 Login, SigUp 요청 구현
  Front: 로그인, 회원가입 페이지 생성, 기존 메인화면에 내 작품보기 버튼 생성, 내 작품일 경우에만 수정가능
  
