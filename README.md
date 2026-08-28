<!DOCTYPE html>

<html lang="ko">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>대광고등학교 큰빛축제</title>

<style>
*{box-sizing:border-box}
html,body{margin:0;padding:0}

body{
  font-family:"Malgun Gothic","Noto Sans KR",sans-serif;
  background:#f7eef1;
  color:#24151b;
  user-select:none;
  overflow-x:hidden;
}

input,textarea,button{font:inherit}
input,textarea{user-select:text}

/* =========================
   배경 로고
========================= */

#floatingLogos{
  position:fixed;
  inset:0;
  z-index:0;
  pointer-events:none;
  overflow:hidden;
}

.logo-float{
  position:absolute;
  left:0;
  top:0;
  pointer-events:none;
  opacity:.10;
  filter:blur(.2px);
}

.logo-float:nth-child(1){width:64px;height:64px;animation:move1 17s linear infinite}
.logo-float:nth-child(2){width:56px;height:56px;animation:move2 20s linear infinite}
.logo-float:nth-child(3){width:48px;height:48px;animation:move3 18s linear infinite}
.logo-float:nth-child(4){width:60px;height:60px;animation:move4 21s linear infinite}
.logo-float:nth-child(5){width:52px;height:52px;animation:move5 16s linear infinite}
.logo-float:nth-child(6){width:68px;height:68px;animation:move6 23s linear infinite}
.logo-float:nth-child(7){width:50px;height:50px;animation:move7 19s linear infinite}
.logo-float:nth-child(8){width:58px;height:58px;animation:move8 22s linear infinite}
.logo-float:nth-child(9){width:44px;height:44px;animation:move9 17s linear infinite}
.logo-float:nth-child(10){width:62px;height:62px;animation:move10 24s linear infinite}
.logo-float:nth-child(11){width:54px;height:54px;animation:move11 20s linear infinite}
.logo-float:nth-child(12){width:46px;height:46px;animation:move12 18s linear infinite}

@keyframes move1{
  0%{transform:translate3d(2vw,118vh,0)}
  100%{transform:translate3d(82vw,-18vh,0)}
}
@keyframes move2{
  0%{transform:translate3d(18vw,120vh,0)}
  100%{transform:translate3d(103vw,-18vh,0)}
}
@keyframes move3{
  0%{transform:translate3d(35vw,120vh,0)}
  100%{transform:translate3d(118vw,-16vh,0)}
}
@keyframes move4{
  0%{transform:translate3d(-7vw,117vh,0)}
  100%{transform:translate3d(74vw,-18vh,0)}
}
@keyframes move5{
  0%{transform:translate3d(49vw,121vh,0)}
  100%{transform:translate3d(126vw,-15vh,0)}
}
@keyframes move6{
  0%{transform:translate3d(7vw,120vh,0)}
  100%{transform:translate3d(96vw,-20vh,0)}
}
@keyframes move7{
  0%{transform:translate3d(66vw,121vh,0)}
  100%{transform:translate3d(129vw,-14vh,0)}
}
@keyframes move8{
  0%{transform:translate3d(26vw,122vh,0)}
  100%{transform:translate3d(110vw,-19vh,0)}
}
@keyframes move9{
  0%{transform:translate3d(-4vw,119vh,0)}
  100%{transform:translate3d(87vw,-18vh,0)}
}
@keyframes move10{
  0%{transform:translate3d(43vw,121vh,0)}
  100%{transform:translate3d(120vw,-17vh,0)}
}
@keyframes move11{
  0%{transform:translate3d(72vw,120vh,0)}
  100%{transform:translate3d(132vw,-15vh,0)}
}
@keyframes move12{
  0%{transform:translate3d(11vw,123vh,0)}
  100%{transform:translate3d(105vw,-21vh,0)}
}

/* =========================
   헤더
========================= */

.hero{
  background:linear-gradient(135deg,#64152f,#8f2948);
  color:#fff;
  padding:28px 18px 34px;
  box-shadow:0 4px 16px #0002;
  position:relative;
  z-index:10;
}

.top{
  max-width:1050px;
  margin:auto;
  display:flex;
  align-items:center;
  gap:18px;
}

.logo{
  width:78px;
  height:78px;
  border:3px solid #fff;
  border-radius:50%;
  background:#fff;
  display:grid;
  place-items:center;
  flex:none;
  box-shadow:0 3px 10px #0004;
}

.mark{
  color:#741b38;
  font-weight:900;
  font-size:25px;
  line-height:1;
  text-align:center;
}

.mark small{
  display:block;
  font-size:8px;
  letter-spacing:1px;
  margin-top:3px;
}

h1{margin:0;font-size:30px}
.sub{margin-top:7px;opacity:.9}

/* =========================
   공통
========================= */

main{
  max-width:1050px;
  margin:24px auto;
  padding:0 14px;
  position:relative;
  z-index:5;
}

.page{
  display:none;
  position:relative;
  z-index:5;
}

.page.active{display:block}

.panel{
  background:#fff;
  border-radius:18px;
  padding:20px;
  box-shadow:0 4px 18px #6d203714;
  margin-bottom:20px;
  position:relative;
  z-index:5;
}

.panel h2{
  margin:0 0 15px;
  font-size:20px;
}

.grid{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:12px;
}

input,textarea{
  width:100%;
  border:1px solid #dccbd1;
  border-radius:10px;
  padding:12px;
  outline:none;
  background:#fff;
}

input:disabled{
  background:#f1edef;
  color:#8f858a;
  cursor:not-allowed;
}

textarea{
  min-height:105px;
  resize:none;
}

input:focus,textarea:focus{
  border-color:#8a2947;
  box-shadow:0 0 0 3px #8a29471a;
}

.full{grid-column:1/-1}

button{
  border:0;
  border-radius:10px;
  padding:11px 18px;
  cursor:pointer;
  background:#741b38;
  color:#fff;
  font-weight:700;
  position:relative;
  z-index:1;
}

button:disabled{
  cursor:not-allowed;
}

button.secondary{
  background:#f1e5e9;
  color:#5d1930;
}

button.danger{
  background:#b73550;
}

.actions{
  display:flex;
  gap:8px;
  justify-content:flex-end;
  margin-top:12px;
  flex-wrap:wrap;
}

.hint{
  font-size:13px;
  color:#76636b;
  margin-top:8px;
}

.entry{
  border:1px solid #ead6dc;
  border-radius:15px;
  padding:17px;
  margin-top:12px;
  background:#fffafb;
  position:relative;
  z-index:5;
}

.entry-head{
  display:flex;
  justify-content:space-between;
  gap:10px;
  align-items:center;
}

.name{
  font-weight:800;
  font-size:17px;
}

.time{
  font-size:12px;
  color:#7d6c74;
  text-align:right;
}

.content{
  white-space:pre-wrap;
  line-height:1.65;
  margin:12px 0;
}

.tag{
  display:inline-block;
  background:#f3e3e8;
  color:#741b38;
  border-radius:999px;
  padding:4px 9px;
  font-size:12px;
}

.empty{
  text-align:center;
  color:#8b7b82;
  padding:35px 10px;
}

.back-btn{margin-bottom:16px}

/* =========================
   메뉴
========================= */

.menu-wrap{
  min-height:calc(100vh - 150px);
  display:flex;
  align-items:center;
  justify-content:center;
  padding:25px 0 40px;
  position:relative;
  z-index:6;
}

.menu{
  width:min(760px,100%);
  position:relative;
  z-index:7;
}

.menu-title{
  text-align:center;
  margin-bottom:28px;
  position:relative;
  z-index:7;
}

.menu-title h2{
  margin:0;
  color:#741b38;
  font-size:31px;
}

.menu-title p{
  margin:10px 0 0;
  color:#806d76;
}

.menu-grid{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:18px;
  position:relative;
  z-index:8;
}

.menu-card{
  background:#fff;
  border:1px solid #ead6dc;
  border-radius:22px;
  padding:32px 20px;
  text-align:center;
  box-shadow:0 8px 28px #6d203725;
  cursor:pointer;
  transition:.2s;
  position:relative;
  z-index:9;
}

.menu-card:hover{
  transform:translateY(-5px);
  box-shadow:0 12px 32px #6d203735;
}

.menu-icon{
  font-size:50px;
  margin-bottom:14px;
  position:relative;
  z-index:2;
}

.menu-card h3,
.menu-card p{
  position:relative;
  z-index:2;
}

.menu-card h3{
  margin:0;
  color:#741b38;
  font-size:22px;
}

.menu-card p{
  color:#806d76;
  margin:9px 0 0;
  font-size:14px;
}

/* =========================
   좋아요
========================= */

.like-area{
  display:flex;
  align-items:center;
  gap:7px;
  flex-wrap:wrap;
}

.like-btn{
  background:#fff;
  color:#8a2947;
  border:1px solid #ead6dc;
  padding:9px 14px;
  border-radius:10px;
  font-weight:700;
}

.like-count{
  min-width:28px;
  text-align:center;
  color:#8a2947;
  font-size:14px;
  font-weight:800;
}

.cancel-like{
  background:#f1e5e9;
  color:#5d1930;
  border:0;
  padding:9px 14px;
  border-radius:10px;
  font-weight:700;
}

.cancel-like:disabled{
  background:#f3f1f2;
  color:#aaa0a5;
  cursor:not-allowed;
}

/* =========================
   모달
========================= */

.modal{
  position:fixed;
  inset:0;
  background:#2b0d1799;
  display:none;
  align-items:center;
  justify-content:center;
  padding:18px;
  z-index:100;
}

.modal.show{display:flex}

.modal-card{
  background:#fff;
  border-radius:17px;
  padding:22px;
  width:min(430px,100%);
  box-shadow:0 15px 50px #0005;
}

.modal-card h3{margin-top:0}

.error{
  color:#b73550;
  font-size:13px;
  margin-top:8px;
  min-height:18px;
}

/* =========================
   게임
========================= */

.game-box{
  background:#fff;
  border-radius:18px;
  padding:20px;
  box-shadow:0 4px 18px #6d203714;
  margin-bottom:20px;
  position:relative;
  z-index:5;
}

.game-title{
  text-align:center;
  color:#741b38;
  margin:0 0 8px;
  font-size:25px;
}

.game-description{
  text-align:center;
  color:#806d76;
  margin:0 0 18px;
  font-size:14px;
}

.game-status{
  display:grid;
  grid-template-columns:repeat(4,1fr);
  gap:10px;
  margin-bottom:18px;
}

.status-box{
  background:#f8eff2;
  border:1px solid #ead6dc;
  border-radius:12px;
  padding:12px;
  text-align:center;
}

.status-label{
  display:block;
  color:#806d76;
  font-size:12px;
  margin-bottom:4px;
}

.status-value{
  color:#741b38;
  font-weight:900;
  font-size:18px;
}

.nickname-row{
  display:flex;
  gap:8px;
  margin-bottom:16px;
}

.nickname-row input{flex:1}

.game-screen{
  border:1px solid #ead6dc;
  border-radius:16px;
  padding:22px;
  background:linear-gradient(180deg,#fffafb,#f6e9ed);
}

.difficulty{
  display:inline-block;
  padding:6px 11px;
  border-radius:999px;
  background:#f1dce3;
  color:#741b38;
  font-size:12px;
  font-weight:800;
  margin-bottom:10px;
}

.question-timer-wrap{
  width:100%;
  height:8px;
  background:#eadde1;
  border-radius:999px;
  overflow:hidden;
  margin-bottom:12px;
}

#questionTimerBar{
  height:100%;
  width:100%;
  background:#8a2947;
  transition:width 1s linear;
}

.question{
  min-height:115px;
  display:flex;
  align-items:center;
  justify-content:center;
  text-align:center;
  font-size:24px;
  font-weight:900;
  color:#24151b;
  line-height:1.55;
  padding:8px;
  word-break:break-word;
}

.choices{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:10px;
  margin-top:16px;
}

.choice-btn{
  background:#fff;
  color:#5d1930;
  border:1px solid #dccbd1;
  padding:14px 12px;
  min-height:54px;
  transition:.15s;
  text-align:center;
}

.choice-btn:hover{
  background:#f8edf1;
  border-color:#b86b85;
}

.choice-btn.correct{
  background:#dff3e5;
  color:#176b32;
  border-color:#77ba8b;
}

.choice-btn.wrong{
  background:#fde2e2;
  color:#a12831;
  border-color:#d9888f;
}

.game-message{
  text-align:center;
  color:#806d76;
  min-height:23px;
  margin-top:14px;
  font-size:14px;
}

.game-start-wrap{
  text-align:center;
  margin-top:16px;
}

.big-btn{
  padding:14px 25px;
  font-size:16px;
}

.result{
  display:none;
  text-align:center;
  padding:12px 0 2px;
}

.result.show{display:block}

.result-score{
  color:#741b38;
  font-size:31px;
  font-weight:900;
  margin-bottom:6px;
}

.result-info{
  color:#806d76;
  font-size:14px;
}

/* =========================
   랭킹
========================= */

.ranking-box{
  margin-top:20px;
  border-top:1px solid #ead6dc;
  padding-top:20px;
}

.ranking-title{
  color:#741b38;
  font-size:20px;
  font-weight:900;
  margin-bottom:12px;
}

.ranking-table{
  width:100%;
  border-collapse:collapse;
}

.ranking-table th,
.ranking-table td{
  padding:10px 8px;
  text-align:center;
  border-bottom:1px solid #eee1e5;
  font-size:14px;
}

.ranking-table th{
  background:#f4e6ea;
  color:#741b38;
}

.ranking-table tr:last-child td{
  border-bottom:0;
}

/* =========================
   모바일
========================= */

@media(max-width:650px){

  .grid{grid-template-columns:1fr}
  .full{grid-column:auto}
  h1{font-size:23px}
  .logo{width:65px;height:65px}
  .menu-grid{grid-template-columns:1fr}
  .menu-title h2{font-size:26px}
  .game-status{grid-template-columns:1fr 1fr}
  .choices{grid-template-columns:1fr}
  .question{font-size:21px}
  .nickname-row{flex-direction:column}
  .logo-float{opacity:.07}

}
</style>

</head>

<body>

<div id="floatingLogos"></div>

<header class="hero">
  <div class="top">

```
<div class="logo">
  <div class="mark">
    大光
    <small>DAE KWANG</small>
  </div>
</div>

<div>
  <h1>대광고등학교 큰빛축제</h1>
  <div class="sub">우리들의 축제, 우리들의 기록</div>
</div>
```

  </div>
</header>

<!-- =========================
     메뉴
========================= -->

<section id="menuPage" class="page active">

  <div class="menu-wrap">

```
<div class="menu">

  <div class="menu-title">
    <h2>🎉 큰빛축제</h2>
    <p>대광고등학교 큰빛축제를 즐겨보세요!</p>
  </div>

  <div class="menu-grid">

    <div class="menu-card" onclick="showPage('guestbookPage')">
      <div class="menu-icon">📖</div>
      <h3>방문록</h3>
      <p>축제에서 느낀 점과 추억을 남겨보세요</p>
    </div>

    <div class="menu-card" onclick="showPage('gamePage')">
      <div class="menu-icon">🎮</div>
      <h3>수학 미니게임</h3>
      <p>고등학교 수학부터 대학 수학까지 도전!</p>
    </div>

  </div>

</div>
```

  </div>

</section>

<!-- =========================
     방문록
========================= -->

<section id="guestbookPage" class="page">

  <main>

```
<button class="secondary back-btn" onclick="showPage('menuPage')">
  ← 메뉴로 돌아가기
</button>

<section class="panel">

  <h2>✍️ 방문록 남기기</h2>

  <div class="grid">

    <input id="name" maxlength="30" placeholder="이름 또는 닉네임">

    <input
      id="password"
      type="password"
      maxlength="30"
      placeholder="수정·삭제용 비밀번호"
    >

    <textarea
      id="message"
      class="full"
      maxlength="1000"
      placeholder="큰빛축제에서 느낀 점을 남겨보세요."
    ></textarea>

  </div>

  <div class="actions">
    <button onclick="addEntry()">방문록 등록</button>
  </div>

  <div class="hint">
    ※ 작성할 때 입력한 비밀번호로 본인 글을 수정·삭제할 수 있습니다.
  </div>

</section>


<section class="panel">

  <h2>
    📖 큰빛축제 방문록
    <span id="count" class="tag">0개</span>
  </h2>

  <div id="entries"></div>

</section>
```

  </main>

</section>

<!-- =========================
     수학게임
========================= -->

<section id="gamePage" class="page">

  <main>

```
<button class="secondary back-btn" onclick="showPage('menuPage')">
  ← 메뉴로 돌아가기
</button>

<section class="game-box">

  <h2 class="game-title">🎮 랜덤 수학 미니게임</h2>

  <p class="game-description">
    고등학교 1학년 이상의 문제가 랜덤으로 출제됩니다.
    문제마다 20초의 제한시간이 있으며 5번 연속 오답이면 종료됩니다.
  </p>


  <div class="nickname-row">

    <input
      id="gameNickname"
      maxlength="20"
      placeholder="랭킹에 표시할 닉네임"
    >

  </div>


  <div class="game-status">

    <div class="status-box">
      <span class="status-label">점수</span>
      <span id="gameScore" class="status-value">0</span>
    </div>

    <div class="status-box">
      <span class="status-label">문제 시간</span>
      <span id="questionTime" class="status-value">20</span>
    </div>

    <div class="status-box">
      <span class="status-label">맞힌 문제</span>
      <span id="gameSolved" class="status-value">0</span>
    </div>

    <div class="status-box">
      <span class="status-label">연속 오답</span>
      <span id="wrongStreak" class="status-value">0 / 5</span>
    </div>

  </div>


  <div class="game-screen">

    <div id="difficulty" class="difficulty">
      게임을 시작해주세요
    </div>

    <div class="question-timer-wrap">
      <div id="questionTimerBar"></div>
    </div>

    <div id="question" class="question">
      랜덤 수학문제 5지선다
    </div>

    <div id="choices" class="choices"></div>

    <div id="gameMessage" class="game-message">
      닉네임을 입력한 뒤 게임 시작을 눌러주세요.
    </div>

  </div>


  <div class="game-start-wrap">

    <button
      id="startGameBtn"
      class="big-btn"
      onclick="startMathGame()"
    >
      게임 시작
    </button>

  </div>


  <div id="result" class="result">

    <div id="resultScore" class="result-score">0점</div>

    <div id="resultInfo" class="result-info"></div>

  </div>


  <div class="ranking-box">

    <div class="ranking-title">
      🏆 큰빛축제 수학게임 랭킹
    </div>

    <table class="ranking-table">

      <thead>
        <tr>
          <th>순위</th>
          <th>닉네임</th>
          <th>점수</th>
        </tr>
      </thead>

      <tbody id="rankingBody"></tbody>

    </table>

  </div>

</section>
```

  </main>

</section>

<!-- =========================
     비밀번호
========================= -->

<div id="modal" class="modal">

  <div class="modal-card">

```
<h3 id="modalTitle">비밀번호 확인</h3>

<input
  id="checkPw"
  type="password"
  placeholder="비밀번호"
>

<div id="pwError" class="error"></div>

<div class="actions">

  <button class="secondary" onclick="closeModal()">
    취소
  </button>

  <button onclick="confirmPassword()">
    확인
  </button>

</div>
```

  </div>

</div>

<script>
/* =====================================================
   배경 로고
===================================================== */

function createLogoSVG(){
  return `
    <svg
      viewBox="0 0 200 200"
      width="100%"
      height="100%"
      xmlns="http://www.w3.org/2000/svg"
    >
      <circle cx="100" cy="100" r="94" fill="#8a2340"/>
      <circle cx="100" cy="100" r="76" fill="none" stroke="#fff" stroke-width="8"/>

      <path
        d="M58 63 Q100 42 142 63
           L136 118 Q132 146 100 163
           Q68 146 64 118 Z"
        fill="#8a2340"
        stroke="#fff"
        stroke-width="3"
      />

      <path
        d="M74 72 L88 61 L100 72
           L112 61 L126 72
           L126 83 L74 83 Z"
        fill="#fff"
      />

      <text
        x="100"
        y="101"
        text-anchor="middle"
        fill="#fff"
        font-family="Georgia"
        font-size="13"
        font-weight="700"
      >LUX ET SAL</text>

      <text
        x="100"
        y="128"
        text-anchor="middle"
        fill="#fff"
        font-family="serif"
        font-size="27"
        font-weight="700"
      >大光</text>

      <text
        x="100"
        y="28"
        text-anchor="middle"
        fill="#fff"
        font-family="Georgia"
        font-size="9"
        font-weight="700"
      >DAE GWANG HIGH SCHOOL</text>

      <text
        x="100"
        y="185"
        text-anchor="middle"
        fill="#fff"
        font-family="serif"
        font-size="9"
        font-weight="700"
      >대 광 고 등 학 교</text>
    </svg>
  `;
}

const floatingLogos=document.getElementById("floatingLogos");

for(let i=0;i<12;i++){
  const item=document.createElement("div");
  item.className="logo-float";
  item.innerHTML=createLogoSVG();
  item.style.animationDelay=`${-(i*1.7)}s`;
  floatingLogos.appendChild(item);
}


/* =====================================================
   페이지 상태
===================================================== */

const PAGE_KEY="daekwang_bigbit_current_page_final";

function showPage(pageId){

  document.querySelectorAll(".page").forEach(page=>{
    page.classList.remove("active");
  });

  const target=document.getElementById(pageId);

  if(!target){
    return;
  }

  target.classList.add("active");

  sessionStorage.setItem(PAGE_KEY,pageId);

  window.scrollTo(0,0);
}

function restorePage(){

  const saved=sessionStorage.getItem(PAGE_KEY);

  const valid=[
    "menuPage",
    "guestbookPage",
    "gamePage"
  ];

  if(saved && valid.includes(saved)){
    showPage(saved);
  }else{
    showPage("menuPage");
  }
}


/* =====================================================
   방문록
===================================================== */

const STORAGE_KEY="daekwang_bigbit_festival_guestbook_v2";
const LIKE_KEY="daekwang_bigbit_festival_likes_v3";
const MASTER_PASSWORD="20100806";
const LIKE_CANCEL_DELAY=7000;

let entries=loadJSON(STORAGE_KEY,[]);
let likes=loadJSON(LIKE_KEY,{});
let pending=null;

function loadJSON(key,fallback){

  try{
    const value=localStorage.getItem(key);

    if(value===null){
      return fallback;
    }

    const parsed=JSON.parse(value);

    return parsed;
  }catch(error){
    return fallback;
  }
}

function save(){
  localStorage.setItem(
    STORAGE_KEY,
    JSON.stringify(entries)
  );
}

function saveLikes(){
  localStorage.setItem(
    LIKE_KEY,
    JSON.stringify(likes)
  );
}

function escapeHTML(text){

  return String(text).replace(
    /[&<>"']/g,
    char=>({
      "&":"&amp;",
      "<":"&lt;",
      ">":"&gt;",
      '"':"&quot;",
      "'":"&#039;"
    }[char])
  );
}

function formatDate(iso){

  const d=new Date(iso);

  const p=n=>String(n).padStart(2,"0");

  return `${d.getFullYear()}년 ${p(d.getMonth()+1)}월 ${p(d.getDate())}일 ${p(d.getHours())}시 ${p(d.getMinutes())}분 ${p(d.getSeconds())}초`;
}

function addEntry(){

  const name=document.getElementById("name").value.trim();
  const password=document.getElementById("password").value;
  const message=document.getElementById("message").value.trim();

  if(!name || !password || !message){
    alert("이름(닉네임), 비밀번호, 내용을 모두 입력해주세요.");
    return;
  }

  const id=
    window.crypto && typeof crypto.randomUUID==="function"
    ? crypto.randomUUID()
    : `${Date.now()}_${Math.random()}`;

  entries.unshift({
    id:id,
    name:name,
    message:message,
    password:password,
    createdAt:new Date().toISOString()
  });

  save();
  render();

  document.getElementById("name").value="";
  document.getElementById("password").value="";
  document.getElementById("message").value="";
}


/* =====================================================
   좋아요
===================================================== */

function normalizeLikes(id){

  if(!likes[id]){
    likes[id]={
      count:0,
      times:[]
    };
  }

  if(typeof likes[id]==="number"){
    likes[id]={
      count:likes[id],
      times:[]
    };
  }

  if(!Array.isArray(likes[id].times)){
    likes[id].times=[];
  }

  if(typeof likes[id].count!=="number"){
    likes[id].count=0;
  }

  return likes[id];
}

function addLike(id){

  const data=normalizeLikes(id);

  data.count++;
  data.times.push(Date.now());

  saveLikes();
  render();
}

function getCancelableIndex(id){

  const data=likes[id];

  if(!data || !Array.isArray(data.times)){
    return -1;
  }

  const now=Date.now();

  return data.times.findIndex(
    timestamp=>now-timestamp>=LIKE_CANCEL_DELAY
  );
}

function cancelLike(id){

  const data=likes[id];

  if(!data){
    return;
  }

  const index=getCancelableIndex(id);

  if(index===-1){
    alert("좋아요를 누른 후 7초가 지나야 취소할 수 있습니다.");
    return;
  }

  data.times.splice(index,1);
  data.count=Math.max(0,data.count-1);

  saveLikes();
  render();
}

function getCancelText(id){

  const data=likes[id];

  if(!data || !data.times.length){
    return "좋아요 취소";
  }

  const now=Date.now();

  const available=data.times.some(
    timestamp=>now-timestamp>=LIKE_CANCEL_DELAY
  );

  if(available){
    return "좋아요 취소";
  }

  const earliest=Math.min(...data.times);

  const remain=Math.max(
    0,
    Math.ceil(
      (LIKE_CANCEL_DELAY-(now-earliest))/1000
    )
  );

  return `${remain}초 후 취소`;
}


/* =====================================================
   방문록 렌더
===================================================== */

function render(){

  const entriesBox=document.getElementById("entries");
  const countBox=document.getElementById("count");

  if(!entriesBox || !countBox){
    return;
  }

  countBox.textContent=`${entries.length}개`;

  if(entries.length===0){

    entriesBox.innerHTML=`
      <div class="empty">
        아직 등록된 방문록이 없습니다.<br>
        첫 번째 기록을 남겨보세요!
      </div>
    `;

    return;
  }

  entriesBox.innerHTML=entries.map(entry=>{

    const data=normalizeLikes(entry.id);
    const cancelAvailable=getCancelableIndex(entry.id)!==-1;

    return `
      <article class="entry">

        <div class="entry-head">

          <div class="name">
            ${escapeHTML(entry.name)}
          </div>

          <div class="time">
            작성: ${formatDate(entry.createdAt)}
            ${
              entry.updatedAt
              ? `<br>수정: ${formatDate(entry.updatedAt)}`
              : ""
            }
          </div>

        </div>

        <div class="content">
          ${escapeHTML(entry.message)}
        </div>

        <div class="actions">

          <div class="like-area">

            <button
              class="like-btn"
              onclick="addLike('${entry.id}')"
            >
              ❤️ 좋아요
            </button>

            <span class="like-count">
              ${data.count}
            </span>

            <button
              class="cancel-like"
              onclick="cancelLike('${entry.id}')"
              ${cancelAvailable ? "" : "disabled"}
            >
              ${getCancelText(entry.id)}
            </button>

          </div>

          <button
            class="secondary"
            onclick="requestAction('edit','${entry.id}')"
          >
            수정
          </button>

          <button
            class="danger"
            onclick="requestAction('delete','${entry.id}')"
          >
            삭제
          </button>

        </div>

      </article>
    `;

  }).join("");
}


/* =====================================================
   수정 / 삭제
===================================================== */

function requestAction(action,id){

  pending={
    action:action,
    id:id
  };

  document.getElementById("checkPw").value="";
  document.getElementById("pwError").textContent="";

  document.getElementById("modalTitle").textContent=
    action==="edit"
    ? "수정을 위한 비밀번호 확인"
    : "삭제를 위한 비밀번호 확인";

  document.getElementById("modal").classList.add("show");

  setTimeout(()=>{
    document.getElementById("checkPw").focus();
  },50);
}

function closeModal(){

  pending=null;

  document.getElementById("modal")
    .classList.remove("show");
}

function confirmPassword(){

  if(!pending){
    return;
  }

  const entry=entries.find(
    item=>item.id===pending.id
  );

  const password=
    document.getElementById("checkPw").value;

  if(
    !entry ||
    !(
      password===entry.password ||
      password===MASTER_PASSWORD
    )
  ){

    document.getElementById("pwError")
      .textContent="비밀번호가 올바르지 않습니다.";

    return;
  }

  const action=pending.action;
  const id=pending.id;

  closeModal();

  if(action==="delete"){

    if(confirm("이 방문록을 삭제할까요?")){

      entries=entries.filter(
        item=>item.id!==id
      );

      delete likes[id];

      save();
      saveLikes();
      render();
    }

    return;
  }

  const target=entries.find(
    item=>item.id===id
  );

  if(!target){
    return;
  }

  const newName=prompt(
    "이름 또는 닉네임",
    target.name
  );

  if(newName===null){
    return;
  }

  const newMessage=prompt(
    "방문록 내용",
    target.message
  );

  if(newMessage===null){
    return;
  }

  if(!newName.trim() || !newMessage.trim()){

    alert("내용을 비워둘 수 없습니다.");
    return;
  }

  target.name=newName.trim();
  target.message=newMessage.trim();
  target.updatedAt=new Date().toISOString();

  save();
  render();
}

document.getElementById("modal").addEventListener(
  "click",
  event=>{
    if(event.target.id==="modal"){
      closeModal();
    }
  }
);

document.addEventListener(
  "keydown",
  event=>{
    if(event.key==="Escape"){
      closeModal();
    }
  }
);


/* =====================================================
   수학게임
===================================================== */

const QUESTION_TIME=20;
const MAX_WRONG_STREAK=5;

const RANKING_KEY=
  "daekwang_bigbit_math_ranking_final";

const BEST_KEY=
  "daekwang_bigbit_math_best_final";

const difficultyConfig={

  high:{
    label:"🟠 고등학교",
    score:8,
    weight:70
  },

  university:{
    label:"🔴 대학",
    score:12,
    weight:23
  },

  universityHard:{
    label:"🔴 대학 심화",
    score:16,
    weight:7
  }

};

let gameRunning=false;
let gameScore=0;
let questionTime=QUESTION_TIME;
let gameSolved=0;
let wrongStreak=0;
let questionTimer=null;
let currentQuestion=null;
let usedQuestionKeys=new Set();
let lastQuestionType=null;

let bestGameScore=
  Number(
    localStorage.getItem(BEST_KEY) || 0
  );


function randInt(min,max){

  return Math.floor(
    Math.random()*(max-min+1)
  )+min;
}

function randomChoice(array){

  return array[
    Math.floor(
      Math.random()*array.length
    )
  ];
}

function sameAnswer(a,b){

  if(
    typeof a==="number" &&
    typeof b==="number"
  ){
    return Math.abs(a-b)<0.000001;
  }

  return String(a)===String(b);
}

function formatNumber(value){

  if(typeof value!=="number"){
    return String(value);
  }

  if(!Number.isFinite(value)){
    return "∞";
  }

  if(
    Math.abs(
      value-Math.round(value)
    )<0.000001
  ){
    return String(Math.round(value));
  }

  return String(
    Math.round(value*100)/100
  );
}

function combination(n,r){

  if(r<0 || r>n){
    return 0;
  }

  r=Math.min(r,n-r);

  let result=1;

  for(let i=1;i<=r;i++){
    result=result*(n-r+i)/i;
  }

  return Math.round(result);
}

function chooseDifficulty(){

  const keys=Object.keys(
    difficultyConfig
  );

  let total=0;

  keys.forEach(
    key=>{
      total+=difficultyConfig[key].weight;
    }
  );

  let random=Math.random()*total;

  for(const key of keys){

    random-=difficultyConfig[key].weight;

    if(random<=0){
      return key;
    }
  }

  return "high";
}

function chooseType(types){

  let pool=types.filter(
    type=>type!==lastQuestionType
  );

  if(pool.length===0){
    pool=types;
  }

  return randomChoice(pool);
}


/* =====================================================
   고등학교
===================================================== */

function generateHigh(){

  const types=[

    "quadratic",
    "logarithm",
    "exponent",
    "trigonometry",
    "arithmetic_sequence",
    "geometric_sequence",
    "derivative",
    "probability",
    "combination",
    "triangle_area",
    "triangle_angle",
    "pythagoras",
    "coordinate_distance",
    "coordinate_midpoint",
    "circle_area",
    "circle_circumference",
    "circle_sector",
    "circle_arc",
    "circle_equation",
    "circle_chord",
    "parabola"

  ];

  const type=chooseType(types);


  if(type==="quadratic"){

    const r1=randInt(-9,9);
    const r2=randInt(-9,9);

    const B=-(r1+r2);
    const C=r1*r2;

    return {
      type:type,
      question:
        `x² ${B>=0?"+ "+B:"- "+Math.abs(B)}x ${C>=0?"+ "+C:"- "+Math.abs(C)} = 0의 한 근은?`,
      answer:r1
    };
  }


  if(type==="logarithm"){

    const base=randomChoice([2,3,4,5]);
    const exponent=randInt(2,6);
    const value=Math.pow(base,exponent);

    return {
      type:type,
      question:`log_${base}(${value}) = ?`,
      answer:exponent
    };
  }


  if(type==="exponent"){

    const base=randomChoice([2,3,5]);
    const a=randInt(2,6);
    const b=randInt(1,4);

    return {
      type:type,
      question:`${base}^${a} × ${base}^${b} = ?`,
      answer:Math.pow(base,a+b)
    };
  }


  if(type==="trigonometry"){

    const data=randomChoice([

      {q:"sin 30°",a:0.5},
      {q:"cos 60°",a:0.5},
      {q:"sin 90°",a:1},
      {q:"cos 0°",a:1},
      {q:"tan 45°",a:1}

    ]);

    return {
      type:type,
      question:`${data.q} = ?`,
      answer:data.a
    };
  }


  if(type==="arithmetic_sequence"){

    const first=randInt(1,20);
    const d=randInt(2,10);
    const n=randInt(5,15);

    return {
      type:type,
      question:
        `등차수열의 첫째항이 ${first}, 공차가 ${d}일 때 ${n}번째 항은?`,
      answer:first+(n-1)*d
    };
  }


  if(type==="geometric_sequence"){

    const first=randInt(1,5);
    const ratio=randomChoice([2,3,-2]);
    const n=randInt(3,6);

    return {
      type:type,
      question:
        `등비수열의 첫째항이 ${first}, 공비가 ${ratio}일 때 ${n}번째 항은?`,
      answer:first*Math.pow(ratio,n-1)
    };
  }


  if(type==="derivative"){

    const n=randInt(2,6);
    const x=randInt(1,8);

    return {
      type:type,
      question:`f(x)=x^${n}일 때 f'(${x})는?`,
      answer:n*Math.pow(x,n-1)
    };
  }


  if(type==="probability"){

    const n=randInt(3,6);
    const success=randInt(0,n);

    return {
      type:type,
      question:
        `동전을 ${n}번 던질 때 앞면이 정확히 ${success}번 나올 확률은?`,
      answer:
        combination(n,success)*Math.pow(0.5,n)
    };
  }


  if(type==="combination"){

    const n=randInt(5,12);
    const r=randInt(2,n-2);

    return {
      type:type,
      question:`C(${n}, ${r}) = ?`,
      answer:combination(n,r)
    };
  }


  if(type==="triangle_area"){

    const base=randInt(5,20);
    const height=randInt(5,20);

    return {
      type:type,
      question:
        `밑변 ${base}, 높이 ${height}인 삼각형의 넓이는?`,
      answer:base*height/2
    };
  }


  if(type==="triangle_angle"){

    const a=randInt(30,80);
    const b=randInt(20,70);
    const c=180-a-b;

    if(c<=10){
      return generateHigh();
    }

    return {
      type:type,
      question:
        `삼각형의 두 내각이 ${a}°, ${b}°일 때 나머지 한 각은?`,
      answer:c
    };
  }


  if(type==="pythagoras"){

    const triples=[
      [3,4,5],
      [5,12,13],
      [6,8,10],
      [7,24,25],
      [8,15,17]
    ];

    const triple=randomChoice(triples);
    const multiple=randInt(1,3);

    const a=triple[0]*multiple;
    const b=triple[1]*multiple;
    const c=triple[2]*multiple;

    return {
      type:type,
      question:
        `직각삼각형의 두 직각변의 길이가 ${a}, ${b}일 때 빗변의 길이는?`,
      answer:c
    };
  }


  if(type==="coordinate_distance"){

    const x1=randInt(-8,8);
    const y1=randInt(-8,8);
    const x2=randInt(-8,8);
    const y2=randInt(-8,8);

    return {
      type:type,
      question:
        `두 점 (${x1},${y1}), (${x2},${y2}) 사이의 거리는?`,
      answer:
        Math.sqrt(
          Math.pow(x2-x1,2)+
          Math.pow(y2-y1,2)
        )
    };
  }


  if(type==="coordinate_midpoint"){

    const x1=randInt(-10,10);
    const x2=randInt(-10,10);

    return {
      type:type,
      question:
        `두 점 (${x1},0), (${x2},0)의 중점의 x좌표는?`,
      answer:(x1+x2)/2
    };
  }


  if(type==="circle_area"){

    const r=randInt(2,12);

    return {
      type:type,
      question:
        `반지름 ${r}cm인 원의 넓이는? (π로 나타내세요)`,
      answer:`${r*r}π`
    };
  }


  if(type==="circle_circumference"){

    const r=randInt(2,12);

    return {
      type:type,
      question:
        `반지름 ${r}cm인 원의 둘레는? (π로 나타내세요)`,
      answer:`${2*r}π`
    };
  }


  if(type==="circle_sector"){

    const r=randInt(2,10);
    const angle=randomChoice([30,45,60,90,120,180]);
    const coefficient=r*r*angle/360;

    return {
      type:type,
      question:
        `반지름 ${r}, 중심각 ${angle}°인 부채꼴의 넓이는? (π로 나타내세요)`,
      answer:`${coefficient}π`
    };
  }


  if(type==="circle_arc"){

    const r=randInt(2,10);
    const angle=randomChoice([30,45,60,90,120,180]);
    const coefficient=2*r*angle/360;

    return {
      type:type,
      question:
        `반지름 ${r}, 중심각 ${angle}°인 호의 길이는? (π로 나타내세요)`,
      answer:`${coefficient}π`
    };
  }


  if(type==="circle_equation"){

    const r=randInt(2,10);

    return {
      type:type,
      question:
        `중심이 원점이고 반지름이 ${r}인 원의 방정식은?`,
      answer:`x²+y²=${r*r}`
    };
  }


  if(type==="circle_chord"){

    const r=randInt(5,12);
    const distance=randInt(1,r-1);

    const chord=
      2*Math.sqrt(
        r*r-distance*distance
      );

    return {
      type:type,
      question:
        `반지름이 ${r}인 원의 중심에서 현까지의 거리가 ${distance}일 때 현의 길이는?`,
      answer:chord
    };
  }


  const a=randInt(2,8);
  const x=randInt(-5,8);

  return {
    type:type,
    question:`f(x)=${a}x²일 때 f(${x})는?`,
    answer:a*x*x
  };
}


/* =====================================================
   대학
===================================================== */

function generateUniversity(){

  const types=[
    "integral",
    "integral_linear",
    "derivative",
    "matrix_trace",
    "determinant",
    "probability",
    "complex",
    "limit",
    "vector",
    "circle_integral",
    "circle_sector"
  ];

  const type=chooseType(types);


  if(type==="integral"){

    const n=randInt(2,8);

    return {
      type:type,
      question:`∫₀^${n} x² dx = ?`,
      answer:n*n*n/3
    };
  }


  if(type==="integral_linear"){

    const a=randInt(2,9);
    const b=randInt(1,8);
    const upper=randInt(2,7);

    return {
      type:type,
      question:
        `∫₀^${upper} (${a}x + ${b}) dx = ?`,
      answer:
        a*upper*upper/2+
        b*upper
    };
  }


  if(type==="derivative"){

    const a=randInt(2,9);
    const n=randInt(2,5);
    const x=randInt(1,6);

    return {
      type:type,
      question:
        `f(x)=${a}x^${n}일 때 f'(${x})는?`,
      answer:
        a*n*Math.pow(x,n-1)
    };
  }


  if(type==="matrix_trace"){

    const a=randInt(1,9);
    const b=randInt(1,9);

    return {
      type:type,
      question:
        `행렬 [[${a},0],[0,${b}]]의 trace는?`,
      answer:a+b
    };
  }


  if(type==="determinant"){

    const a=randInt(1,8);
    const b=randInt(1,8);
    const c=randInt(1,8);
    const d=randInt(1,8);

    return {
      type:type,
      question:
        `det [[${a},${b}],[${c},${d}]] = ?`,
      answer:a*d-b*c
    };
  }


  if(type==="probability"){

    const success=randInt(2,7);
    const total=randInt(success+1,12);

    return {
      type:type,
      question:
        `성공 ${success}회 / 전체 ${total}회일 때 경험적 확률은?`,
      answer:success/total
    };
  }


  if(type==="complex"){

    const a=randInt(1,8);
    const b=randInt(1,8);

    return {
      type:type,
      question:
        `z=${a}+${b}i일 때 |z|²는?`,
      answer:a*a+b*b
    };
  }


  if(type==="limit"){

    const a=randInt(2,9);
    const b=randInt(1,9);
    const x=randInt(1,7);

    return {
      type:type,
      question:
        `lim(x→${x}) (${a}x + ${b}) = ?`,
      answer:a*x+b
    };
  }


  if(type==="vector"){

    const a=randInt(1,8);
    const b=randInt(1,8);
    const c=randInt(1,8);
    const d=randInt(1,8);

    return {
      type:type,
      question:
        `벡터 (${a},${b})·(${c},${d}) = ?`,
      answer:a*c+b*d
    };
  }


  if(type==="circle_integral"){

    const r=randInt(2,8);

    return {
      type:type,
      question:
        `반지름 ${r}인 원의 둘레를 π로 나타내면?`,
      answer:`${2*r}π`
    };
  }


  const r=randInt(2,10);
  const angle=randomChoice([30,45,60,90,120]);

  return {
    type:type,
    question:
      `반지름 ${r}인 원에서 중심각 ${angle}°인 부채꼴의 넓이는? (π로 나타내세요)`,
    answer:
      `${r*r*angle/360}π`
  };
}


/* =====================================================
   대학 심화
===================================================== */

function generateUniversityHard(){

  const types=[
    "trig_integral",
    "chain_rule",
    "matrix_determinant",
    "complex_square",
    "expectation",
    "eigenvalue",
    "geometric_series",
    "cross_product",
    "circle_area",
    "circle_sector"
  ];

  const type=chooseType(types);


  if(type==="trig_integral"){

    const a=randInt(1,7);

    return {
      type:type,
      question:
        `∫₀^π ${a}sin(x) dx ÷ ${a} = ?`,
      answer:2
    };
  }


  if(type==="chain_rule"){

    const a=randInt(2,7);
    const x=randInt(1,6);

    return {
      type:type,
      question:
        `f(x)=(${a}x)²일 때 f'(${x})는?`,
      answer:2*a*a*x
    };
  }


  if(type==="matrix_determinant"){

    const a=randInt(1,5);
    const b=randInt(1,5);
    const c=randInt(1,5);

    return {
      type:type,
      question:
        `diag(${a},${b},${c})의 행렬식은?`,
      answer:a*b*c
    };
  }


  if(type==="complex_square"){

    const a=randInt(1,9);

    return {
      type:type,
      question:`z=${a}i일 때 z²는?`,
      answer:-a*a
    };
  }


  if(type==="expectation"){

    const x1=randInt(1,5);
    const x2=randInt(6,10);
    const p=randomChoice([.2,.3,.4,.6,.7,.8]);

    return {
      type:type,
      question:
        `X가 ${x1}을 확률 ${p}, ${x2}를 확률 ${1-p}로 가질 때 E[X]는?`,
      answer:
        p*x1+(1-p)*x2
    };
  }


  if(type==="eigenvalue"){

    const a=randInt(2,9);
    const b=randInt(2,9);

    return {
      type:type,
      question:
        `행렬 [[${a},0],[0,${b}]]의 고유값 중 작은 값은?`,
      answer:Math.min(a,b)
    };
  }


  if(type==="geometric_series"){

    const a=randInt(1,5);
    const r=randInt(2,3);
    const n=randInt(3,7);

    return {
      type:type,
      question:
        `등비수열의 첫째항 ${a}, 공비 ${r}일 때 첫 ${n}개 항의 합은?`,
      answer:
        a*(Math.pow(r,n)-1)/(r-1)
    };
  }


  if(type==="cross_product"){

    const a=randInt(1,5);
    const b=randInt(1,5);

    return {
      type:type,
      question:
        `벡터 (${a},0,0) × (0,${b},0)의 크기는?`,
      answer:a*b
    };
  }


  if(type==="circle_area"){

    const r=randInt(2,10);

    return {
      type:type,
      question:
        `반지름 ${r}인 원의 넓이는? (π로 나타내세요)`,
      answer:`${r*r}π`
    };
  }


  const r=randInt(2,9);
  const angle=randomChoice(
    [30,45,60,90,120,180]
  );

  return {
    type:type,
    question:
      `반지름 ${r}, 중심각 ${angle}°인 부채꼴의 넓이는? (π로 나타내세요)`,
    answer:
      `${r*r*angle/360}π`
  };
}


/* =====================================================
   문제 생성
===================================================== */

function createQuestion(){

  let attempts=0;

  while(attempts<1000){

    attempts++;

    const level=chooseDifficulty();

    let question;

    if(level==="high"){
      question=generateHigh();
    }else if(level==="university"){
      question=generateUniversity();
    }else{
      question=generateUniversityHard();
    }

    if(question.type===lastQuestionType){
      continue;
    }

    const key=
      `${level}|${question.type}|${question.question}|${formatNumber(question.answer)}`;

    if(usedQuestionKeys.has(key)){
      continue;
    }

    usedQuestionKeys.add(key);
    lastQuestionType=question.type;
    question.level=level;

    return question;
  }

  return {
    level:"high",
    type:"fallback_"+Date.now(),
    question:"x² - 7x + 12 = 0의 한 근은?",
    answer:3
  };
}


/* =====================================================
   선지
===================================================== */

function makeChoices(answer,level){

  /* ---- π 포함 문제 ---- */

  if(
    typeof answer==="string" &&
    answer.endsWith("π")
  ){

    const coefficient=parseFloat(
      answer.replace("π","")
    );

    if(Number.isFinite(coefficient)){

      const choices=[answer];

      let step;

      if(Math.abs(coefficient)>=20){
        step=.5;
      }else{
        step=.25;
      }

      const offsets=[
        -step*2,
        -step,
        step,
        step*2
      ];

      offsets.forEach(
        offset=>{

          const value=
            coefficient+offset;

          if(value<=0){
            return;
          }

          const text=
            `${Number(value.toFixed(2))}π`;

          if(!choices.includes(text)){
            choices.push(text);
          }
        }
      );

      while(choices.length<5){

        const direction=
          choices.length%2===0
          ?1
          :-1;

        const value=
          coefficient+
          direction*
          step*
          (choices.length*.5);

        if(value>0){

          const text=
            `${Number(value.toFixed(2))}π`;

          if(!choices.includes(text)){
            choices.push(text);
          }else{
            break;
          }
        }else{
          break;
        }
      }

      while(choices.length<5){
        choices.push(
          `${Number(
            (coefficient+choices.length*step)
            .toFixed(2)
          )}π`
        );
      }

      shuffle(choices);

      return choices;
    }
  }


  /* ---- 원의 방정식 ---- */

  if(
    typeof answer==="string" &&
    /^x²\+y²=\d+$/.test(answer)
  ){

    const n=
      Number(answer.split("=")[1]);

    const offsets=[
      -2,-1,1,2
    ];

    const choices=[
      answer
    ];

    offsets.forEach(
      offset=>{
        const value=n+offset;

        if(value>0){
          choices.push(
            `x²+y²=${value}`
          );
        }
      }
    );

    shuffle(choices);

    return choices;
  }


  /* ---- 숫자 문제 ---- */

  if(
    typeof answer==="number" &&
    Number.isFinite(answer)
  ){

    const choices=[answer];

    const abs=Math.abs(answer);

    let step;

    if(abs<10){
      step=0.5;
    }else if(abs<50){
      step=1;
    }else if(abs<200){
      step=2;
    }else if(abs<1000){
      step=5;
    }else{
      step=Math.max(
        5,
        Math.round(abs*.01)
      );
    }

    let attempts=0;

    while(
      choices.length<5 &&
      attempts<500
    ){

      attempts++;

      let offset;

      if(
        Number.isInteger(answer)
      ){

        offset=
          randomChoice([
            -step,
            step,
            -step*2,
            step*2
          ]);

      }else{

        offset=
          randomChoice([
            -step,
            step,
            -step/2,
            step/2
          ]);

      }

      let wrong=
        answer+offset;

      if(
        !Number.isInteger(answer)
      ){

        wrong=
          Math.round(wrong*100)/100;
      }

      if(
        !choices.some(
          value=>sameAnswer(value,wrong)
        )
      ){

        choices.push(wrong);
      }
    }

    /* 안전망 */

    let extraStep=
      step/2;

    while(
      choices.length<5
    ){

      let wrong=
        answer+
        (
          choices.length%2===0
          ?1
          :-1
        )*
        extraStep;

      if(
        !Number.isInteger(answer)
      ){
        wrong=
          Math.round(wrong*100)/100;
      }

      if(
        !choices.some(
          value=>sameAnswer(value,wrong)
        )
      ){

        choices.push(wrong);

      }else{

        extraStep+=step/2;
      }
    }

    shuffle(choices);

    return choices;
  }


  return [
    answer,
    "보기 2",
    "보기 3",
    "보기 4",
    "보기 5"
  ];
}

function shuffle(array){

  for(
    let i=array.length-1;
    i>0;
    i--
  ){

    const j=
      Math.floor(
        Math.random()*(i+1)
      );

    [
      array[i],
      array[j]
    ]=[
      array[j],
      array[i]
    ];
  }
}


/* =====================================================
   게임 상태 표시
===================================================== */

function renderGameStatus(){

  document.getElementById("gameScore")
    .textContent=gameScore;

  document.getElementById("questionTime")
    .textContent=questionTime;

  document.getElementById("gameSolved")
    .textContent=gameSolved;

  document.getElementById("wrongStreak")
    .textContent=
      `${wrongStreak} / ${MAX_WRONG_STREAK}`;
}


/* =====================================================
   문제 표시
===================================================== */

function showQuestion(){

  if(!gameRunning){
    return;
  }

  currentQuestion=createQuestion();

  const config=
    difficultyConfig[
      currentQuestion.level
    ];

  document.getElementById("difficulty")
    .textContent=
      `${config.label} · 정답 +${config.score}점`;

  document.getElementById("question")
    .textContent=
      currentQuestion.question;

  const choices=
    makeChoices(
      currentQuestion.answer,
      currentQuestion.level
    );

  currentQuestion.choices=choices;

  const choicesBox=
    document.getElementById("choices");

  choicesBox.innerHTML="";

  const labels=[
    "①","②","③","④","⑤"
  ];

  choices.forEach(
    (choice,index)=>{

      const button=
        document.createElement("button");

      button.className="choice-btn";

      button.textContent=
        `${labels[index]} ${formatNumber(choice)}`;

      button.onclick=()=>{
        answerQuestion(
          index,
          button
        );
      };

      choicesBox.appendChild(button);
    }
  );

  document.getElementById("gameMessage")
    .textContent=
      "정답을 선택하세요.";

  startQuestionTimer();
}


/* =====================================================
   문제 타이머 20초
===================================================== */

function startQuestionTimer(){

  if(questionTimer){
    clearInterval(questionTimer);
  }

  questionTime=QUESTION_TIME;

  renderGameStatus();

  document.getElementById(
    "questionTimerBar"
  ).style.width="100%";

  questionTimer=
    setInterval(
      ()=>{

        questionTime--;

        renderGameStatus();

        document.getElementById(
          "questionTimerBar"
        ).style.width=
          `${Math.max(
            0,
            questionTime/
            QUESTION_TIME*
            100
          )}%`;

        if(questionTime<=0){

          clearInterval(
            questionTimer
          );

          questionTimer=null;

          questionTimeout();
        }

      },
      1000
    );
}


/* =====================================================
   시간 초과 = 오답
===================================================== */

function questionTimeout(){

  if(!gameRunning){
    return;
  }

  document.querySelectorAll(
    ".choice-btn"
  ).forEach(
    button=>{
      button.disabled=true;
    }
  );

  wrongStreak++;

  renderGameStatus();

  if(
    wrongStreak>=MAX_WRONG_STREAK
  ){

    document.getElementById(
      "gameMessage"
    ).textContent=
      "⏰ 5번 연속 오답으로 게임 종료!";

    setTimeout(
      ()=>{
        endMathGame();
      },
      450
    );

    return;
  }

  document.getElementById(
    "gameMessage"
  ).textContent=
    `⏰ 시간 초과! 연속 오답 ${wrongStreak}/${MAX_WRONG_STREAK}`;

  setTimeout(
    ()=>{
      if(gameRunning){
        showQuestion();
      }
    },
    500
  );
}


/* =====================================================
   답 처리
===================================================== */

function answerQuestion(
  index,
  clickedButton
){

  if(!gameRunning){
    return;
  }

  if(questionTimer){
    clearInterval(questionTimer);
    questionTimer=null;
  }

  document.querySelectorAll(
    ".choice-btn"
  ).forEach(
    button=>{
      button.disabled=true;
    }
  );

  const selected=
    currentQuestion.choices[index];

  const correct=
    sameAnswer(
      selected,
      currentQuestion.answer
    );

  if(correct){

    clickedButton.classList.add(
      "correct"
    );

    const points=
      difficultyConfig[
        currentQuestion.level
      ].score;

    gameScore+=points;
    gameSolved++;
    wrongStreak=0;

    document.getElementById(
      "gameMessage"
    ).textContent=
      `✅ 정답! +${points}점`;

  }else{

    clickedButton.classList.add(
      "wrong"
    );

    wrongStreak++;

    document.getElementById(
      "gameMessage"
    ).textContent=
      `❌ 오답! 연속 오답 ${wrongStreak}/${MAX_WRONG_STREAK}`;

  }

  renderGameStatus();

  if(
    wrongStreak>=MAX_WRONG_STREAK
  ){

    setTimeout(
      ()=>{
        endMathGame();
      },
      500
    );

    return;
  }

  setTimeout(
    ()=>{
      if(gameRunning){
        showQuestion();
      }
    },
    500
  );
}


/* =====================================================
   게임 시작
===================================================== */

function startMathGame(){

  if(gameRunning){
    return;
  }

  const nickname=
    document.getElementById(
      "gameNickname"
    ).value.trim();

  if(!nickname){

    alert(
      "랭킹에 표시할 닉네임을 입력해주세요."
    );

    document.getElementById(
      "gameNickname"
    ).focus();

    return;
  }

  gameRunning=true;

  gameScore=0;
  questionTime=QUESTION_TIME;
  gameSolved=0;
  wrongStreak=0;
  currentQuestion=null;
  usedQuestionKeys=new Set();
  lastQuestionType=null;

  /* 게임 중 닉네임 잠금 */

  document.getElementById(
    "gameNickname"
  ).disabled=true;

  document.getElementById(
    "result"
  ).classList.remove(
    "show"
  );

  document.getElementById(
    "startGameBtn"
  ).disabled=true;

  document.getElementById(
    "startGameBtn"
  ).textContent=
    "게임 중...";

  renderGameStatus();

  showQuestion();
}


/* =====================================================
   게임 종료
===================================================== */

function endMathGame(){

  if(!gameRunning){
    return;
  }

  gameRunning=false;

  if(questionTimer){

    clearInterval(
      questionTimer
    );

    questionTimer=null;
  }

  document.querySelectorAll(
    ".choice-btn"
  ).forEach(
    button=>{
      button.disabled=true;
    }
  );

  /* 닉네임 다시 입력 */

  document.getElementById(
    "gameNickname"
  ).disabled=false;

  document.getElementById(
    "startGameBtn"
  ).disabled=false;

  document.getElementById(
    "startGameBtn"
  ).textContent=
    "다시 하기";

  document.getElementById(
    "questionTime"
  ).textContent="0";

  document.getElementById(
    "questionTimerBar"
  ).style.width="0%";

  const nickname=
    document.getElementById(
      "gameNickname"
    ).value.trim();

  const reason=
    wrongStreak>=MAX_WRONG_STREAK
    ? "5번 연속 오답"
    : "게임 종료";

  document.getElementById(
    "gameMessage"
  ).textContent=
    `${reason}!`;

  if(gameScore>bestGameScore){

    bestGameScore=gameScore;

    localStorage.setItem(
      BEST_KEY,
      String(bestGameScore)
    );
  }

  document.getElementById(
    "result"
  ).classList.add(
    "show"
  );

  document.getElementById(
    "resultScore"
  ).textContent=
    `${gameScore}점`;

  document.getElementById(
    "resultInfo"
  ).textContent=
    `${nickname}님 · ${gameSolved}문제 정답 · ${reason}`;

  saveRanking(
    nickname,
    gameScore
  );
}


/* =====================================================
   랭킹
===================================================== */

function getRanking(){

  const data=
    loadJSON(
      RANKING_KEY,
      []
    );

  return Array.isArray(data)
    ? data
    : [];
}

function saveRanking(
  nickname,
  score
){

  const ranking=
    getRanking();

  ranking.push({
    name:nickname,
    score:score,
    time:Date.now()
  });

  ranking.sort(
    (a,b)=>
      b.score-a.score ||
      a.time-b.time
  );

  localStorage.setItem(
    RANKING_KEY,
    JSON.stringify(
      ranking.slice(0,20)
    )
  );

  renderRanking();
}

function renderRanking(){

  const body=
    document.getElementById(
      "rankingBody"
    );

  if(!body){
    return;
  }

  const ranking=
    getRanking();

  if(ranking.length===0){

    body.innerHTML=`
      <tr>
        <td colspan="3">
          아직 기록이 없습니다.
        </td>
      </tr>
    `;

    return;
  }

  body.innerHTML=
    ranking.map(
      (item,index)=>`
        <tr>
          <td>${index+1}</td>
          <td>${escapeHTML(item.name)}</td>
          <td>${item.score}</td>
        </tr>
      `
    ).join("");
}


/* =====================================================
   초기화
===================================================== */

document.getElementById(
  "gameBest"
);

renderRanking();
render();
restorePage();


/* 좋아요 취소시간 실시간 갱신 */

setInterval(
  ()=>{
    render();
  },
  1000
);
</script>

</body>
</html>
```
