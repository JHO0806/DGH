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
  opacity:.08;
  will-change:transform;
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

h1{
  margin:0;
  font-size:30px;
}

.sub{
  margin-top:7px;
  opacity:.9;
}

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

.page.active{
  display:block;
}

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

.full{
  grid-column:1/-1;
}

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

.back-btn{
  margin-bottom:16px;
}

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
}

.menu-icon{
  font-size:50px;
  margin-bottom:14px;
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
}

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

.modal.show{
  display:flex;
}

.modal-card{
  background:#fff;
  border-radius:17px;
  padding:22px;
  width:min(430px,100%);
  box-shadow:0 15px 50px #0005;
}

.modal-card h3{
  margin-top:0;
}

.error{
  color:#b73550;
  font-size:13px;
  margin-top:8px;
  min-height:18px;
}

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

.nickname-row input{
  flex:1;
}

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
  min-height:125px;
  display:flex;
  align-items:center;
  justify-content:center;
  text-align:center;
  font-size:23px;
  font-weight:900;
  color:#24151b;
  line-height:1.6;
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

.result.show{
  display:block;
}

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

@media(max-width:650px){
  .grid{grid-template-columns:1fr}
  .full{grid-column:auto}
  h1{font-size:23px}
  .logo{width:65px;height:65px}
  .menu-grid{grid-template-columns:1fr}
  .menu-title h2{font-size:26px}
  .game-status{grid-template-columns:1fr 1fr}
  .choices{grid-template-columns:1fr}
  .question{font-size:20px}
  .nickname-row{flex-direction:column}
  .logo-float{opacity:.06}
}
</style>

</head>

<body>

<div id="floatingLogos"></div>

<header class="hero">
<div class="top">

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

</div>
</header>

<section id="menuPage" class="page active">

<div class="menu-wrap">

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

</div>

</section>

<section id="guestbookPage" class="page">

<main>

<button class="secondary back-btn" onclick="showPage('menuPage')">
← 메뉴로 돌아가기
</button>

<section class="panel">

<h2>✍️ 방문록 남기기</h2>

<div class="grid">

<input
id="name"
maxlength="30"
placeholder="이름 또는 닉네임"

>

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

</main>

</section>

<section id="gamePage" class="page">

<main>

<button class="secondary back-btn" onclick="showPage('menuPage')">
← 메뉴로 돌아가기
</button>

<section class="game-box">

<h2 class="game-title">
🎮 랜덤 수학 미니게임
</h2>

<p class="game-description">
쉬운 문제부터 어려운 문제까지 나옵니다.
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
고등학교 수준 이상의 랜덤 수학문제
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

게임 시작 </button>

</div>

<div id="result" class="result">

<div id="resultScore" class="result-score">
0점
</div>

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

</main>

</section>

<div id="modal" class="modal">

<div class="modal-card">

<h3 id="modalTitle">
비밀번호 확인
</h3>

<input
id="checkPw"
type="password"
placeholder="비밀번호"

>

<div id="pwError" class="error"></div>

<div class="actions">

<button
class="secondary"
onclick="closeModal()"

>

취소 </button>

<button onclick="confirmPassword()">
확인
</button>

</div>

</div>

</div>

<script>

/* =====================================================
   배경 대광 로고
===================================================== */

function createLogoSVG(){

return (
'<svg viewBox="0 0 200 200" width="100%" height="100%" xmlns="http://www.w3.org/2000/svg">' +

'<circle cx="100" cy="100" r="94" fill="#8a2340"/>' +

'<circle cx="100" cy="100" r="76" fill="none" stroke="#fff" stroke-width="8"/>' +

'<path d="M58 63 Q100 42 142 63 L136 118 Q132 146 100 163 Q68 146 64 118 Z" fill="#8a2340" stroke="#fff" stroke-width="3"/>' +

'<path d="M74 72 L88 61 L100 72 L112 61 L126 72 L126 83 L74 83 Z" fill="#fff"/>' +

'<text x="100" y="101" text-anchor="middle" fill="#fff" font-family="Georgia" font-size="13" font-weight="700">LUX ET SAL</text>' +

'<text x="100" y="128" text-anchor="middle" fill="#fff" font-family="serif" font-size="27" font-weight="700">大光</text>' +

'<text x="100" y="28" text-anchor="middle" fill="#fff" font-family="Georgia" font-size="9" font-weight="700">DAE GWANG HIGH SCHOOL</text>' +

'<text x="100" y="185" text-anchor="middle" fill="#fff" font-family="serif" font-size="9" font-weight="700">대 광 고 등 학 교</text>' +

'</svg>'
);

}

var floatingLogos=
document.getElementById("floatingLogos");

for(
var i=0;
i<12;
i++
){

var logo=
document.createElement("div");

logo.className="logo-float";

logo.innerHTML=
createLogoSVG();

logo.style.animationDelay=
(-(i*1.7))+"s";

floatingLogos.appendChild(
logo
);

}


/* =====================================================
   페이지
===================================================== */

var PAGE_KEY=
"daekwang_bigbit_current_page_final";

function showPage(pageId){

document
.querySelectorAll(".page")
.forEach(
function(page){
page.classList.remove("active");
}
);

var page=
document.getElementById(pageId);

if(!page){
return;
}

page.classList.add("active");

sessionStorage.setItem(
PAGE_KEY,
pageId
);

window.scrollTo(
0,
0
);

}

function restorePage(){

var saved=
sessionStorage.getItem(
PAGE_KEY
);

var valid=[
"menuPage",
"guestbookPage",
"gamePage"
];

if(
saved &&
valid.indexOf(saved)!==-1
){

showPage(saved);

}else{

showPage("menuPage");

}

}


/* =====================================================
   방문록
===================================================== */

var STORAGE_KEY=
"daekwang_bigbit_festival_guestbook_v2";

var LIKE_KEY=
"daekwang_bigbit_festival_likes_v3";

var MASTER_PASSWORD=
"20100806";

var LIKE_CANCEL_DELAY=
7000;

function safeRead(key,fallback){

try{

var raw=
localStorage.getItem(key);

if(raw===null){
return fallback;
}

return JSON.parse(raw);

}catch(error){

return fallback;

}

}

var entries=
safeRead(
STORAGE_KEY,
[]
);

var likes=
safeRead(
LIKE_KEY,
{}
);

if(!Array.isArray(entries)){
entries=[];
}

if(
!likes ||
typeof likes!=="object"
){
likes={};
}

var pending=null;


function saveEntries(){

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
function(char){

var map={
"&":"&amp;",
"<":"&lt;",
">":"&gt;",
'"':"&quot;",
"'":"&#039;"
};

return map[char];

}
);

}

function formatDate(iso){

var d=
new Date(iso);

function pad(n){

return String(n).padStart(
2,
"0"
);

}

return (
d.getFullYear()+
"년 "+
pad(d.getMonth()+1)+
"월 "+
pad(d.getDate())+
"일 "+
pad(d.getHours())+
"시 "+
pad(d.getMinutes())+
"분 "+
pad(d.getSeconds())+
"초"
);

}

function addEntry(){

var name=
document.getElementById(
"name"
).value.trim();

var password=
document.getElementById(
"password"
).value;

var message=
document.getElementById(
"message"
).value.trim();

if(
!name ||
!password ||
!message
){

alert(
"이름(닉네임), 비밀번호, 내용을 모두 입력해주세요."
);

return;

}

var id;

if(
window.crypto &&
typeof window.crypto.randomUUID==="function"
){

id=
window.crypto.randomUUID();

}else{

id=
String(Date.now())+
String(Math.random());

}

entries.unshift({

id:id,
name:name,
message:message,
password:password,
createdAt:
new Date().toISOString()

});

saveEntries();
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

if(
typeof likes[id]==="number"
){

likes[id]={
count:likes[id],
times:[]
};

}

if(
!Array.isArray(
likes[id].times
)
){

likes[id].times=[];

}

if(
typeof likes[id].count!=="number"
){

likes[id].count=0;

}

return likes[id];

}

function addLike(id){

var data=
normalizeLikes(id);

data.count++;
data.times.push(
Date.now()
);

saveLikes();
render();

}

function getCancelableIndex(id){

var data=
likes[id];

if(
!data ||
!Array.isArray(data.times)
){

return -1;

}

var now=
Date.now();

return data.times.findIndex(
function(timestamp){

return (
now-timestamp>=
LIKE_CANCEL_DELAY
);

}
);

}

function cancelLike(id){

var data=
likes[id];

if(!data){
return;
}

var index=
getCancelableIndex(id);

if(index===-1){

alert(
"좋아요를 누른 후 7초가 지나야 취소할 수 있습니다."
);

return;
}

data.times.splice(
index,
1
);

data.count=
Math.max(
0,
data.count-1
);

saveLikes();
render();

}

function getCancelText(id){

var data=
likes[id];

if(
!data ||
!data.times ||
!data.times.length
){

return "좋아요 취소";

}

var now=
Date.now();

var available=
data.times.some(
function(timestamp){

return (
now-timestamp>=
LIKE_CANCEL_DELAY
);

}
);

if(available){

return "좋아요 취소";

}

var earliest=
Math.min.apply(
Math,
data.times
);

var remain=
Math.max(
0,
Math.ceil(
(
LIKE_CANCEL_DELAY-
(now-earliest)
)/1000
)
);

return (
String(remain)+
"초 후 취소"
);

}


/* =====================================================
   방문록 렌더링
===================================================== */

function render(){

var box=
document.getElementById(
"entries"
);

var count=
document.getElementById(
"count"
);

if(
!box ||
!count
){
return;
}

count.textContent=
String(entries.length)+
"개";

if(entries.length===0){

box.innerHTML=
'<div class="empty">아직 등록된 방문록이 없습니다.<br>첫 번째 기록을 남겨보세요!</div>';

return;

}

var html="";

entries.forEach(
function(entry){

var data=
normalizeLikes(
entry.id
);

var canCancel=
getCancelableIndex(
entry.id
)!==-1;

html+=
'<article class="entry">'+

'<div class="entry-head">'+

'<div class="name">'+
escapeHTML(entry.name)+
'</div>'+

'<div class="time">'+
'작성: '+
formatDate(entry.createdAt)+
(
entry.updatedAt
?
'<br>수정: '+
formatDate(entry.updatedAt)
:
''
)+
'</div>'+

'</div>'+

'<div class="content">'+
escapeHTML(entry.message)+
'</div>'+

'<div class="actions">'+

'<div class="like-area">'+

'<button class="like-btn" onclick="addLike(\''+
entry.id+
'\')">❤️ 좋아요</button>'+

'<span class="like-count">'+
data.count+
'</span>'+

'<button class="cancel-like" onclick="cancelLike(\''+
entry.id+
'\')" '+
(canCancel ? '' : 'disabled')+
'>'+
getCancelText(entry.id)+
'</button>'+

'</div>'+

'<button class="secondary" onclick="requestAction(\'edit\',\''+
entry.id+
'\')">수정</button>'+

'<button class="danger" onclick="requestAction(\'delete\',\''+
entry.id+
'\')">삭제</button>'+

'</div>'+

'</article>';

}
);

box.innerHTML=
html;

}


/* =====================================================
   수정 삭제
===================================================== */

function requestAction(action,id){

pending={
action:action,
id:id
};

document.getElementById(
"checkPw"
).value="";

document.getElementById(
"pwError"
).textContent="";

document.getElementById(
"modalTitle"
).textContent=
action==="edit"
?
"수정을 위한 비밀번호 확인"
:
"삭제를 위한 비밀번호 확인";

document.getElementById(
"modal"
).classList.add(
"show"
);

setTimeout(
function(){

document.getElementById(
"checkPw"
).focus();

},
50
);

}

function closeModal(){

pending=null;

document.getElementById(
"modal"
).classList.remove(
"show"
);

}

function confirmPassword(){

if(!pending){
return;
}

var entry=
entries.find(
function(item){
return item.id===pending.id;
}
);

var password=
document.getElementById(
"checkPw"
).value;

if(
!entry ||
!(
password===entry.password ||
password===MASTER_PASSWORD
)
){

document.getElementById(
"pwError"
).textContent=
"비밀번호가 올바르지 않습니다.";

return;

}

var action=
pending.action;

var id=
pending.id;

closeModal();


if(action==="delete"){

if(
confirm(
"이 방문록을 삭제할까요?"
)
){

entries=
entries.filter(
function(item){
return item.id!==id;
}
);

delete likes[id];

saveEntries();
saveLikes();
render();

}

return;

}


var target=
entries.find(
function(item){
return item.id===id;
}
);

if(!target){
return;
}

var newName=
prompt(
"이름 또는 닉네임",
target.name
);

if(newName===null){
return;
}

var newMessage=
prompt(
"방문록 내용",
target.message
);

if(newMessage===null){
return;
}

if(
!newName.trim() ||
!newMessage.trim()
){

alert(
"내용을 비워둘 수 없습니다."
);

return;
}

target.name=
newName.trim();

target.message=
newMessage.trim();

target.updatedAt=
new Date().toISOString();

saveEntries();
render();

}

document
.getElementById("modal")
.addEventListener(
"click",
function(event){

if(
event.target.id==="modal"
){

closeModal();

}

}
);

document.addEventListener(
"keydown",
function(event){

if(
event.key==="Escape"
){

closeModal();

}

}
);


/* =====================================================
   수학 게임
===================================================== */

var QUESTION_TIME=
20;

var MAX_WRONG_STREAK=
5;

var RANKING_KEY=
"daekwang_bigbit_math_ranking_final4";

var BEST_KEY=
"daekwang_bigbit_math_best_final4";

var difficultyConfig={

high:{
label:"🟠 고등학교",
score:8,
weight:78
},

university:{
label:"🔴 대학",
score:12,
weight:17
},

universityHard:{
label:"🔴 대학 심화",
score:16,
weight:5
}

};

var gameRunning=false;
var gameScore=0;
var questionTime=QUESTION_TIME;
var gameSolved=0;
var wrongStreak=0;
var questionTimer=null;
var currentQuestion=null;
var usedQuestionKeys={};
var lastQuestionType=null;

var bestGameScore=
Number(
localStorage.getItem(
BEST_KEY
)||0
);


/* =====================================================
   랜덤 / 수학
===================================================== */

function randInt(min,max){

return Math.floor(
Math.random()*
(max-min+1)
)+min;

}

function randomChoice(array){

return array[
Math.floor(
Math.random()*
array.length
)
];

}

function gcd(a,b){

a=Math.abs(a);
b=Math.abs(b);

while(b){

var t=
a%b;

a=b;
b=t;

}

return a||1;

}

function combination(n,r){

if(
r<0 ||
r>n
){

return 0;

}

r=
Math.min(
r,
n-r
);

var result=1;

for(
var i=1;
i<=r;
i++
){

result=
result*
(n-r+i)/
i;

}

return Math.round(result);

}

function sameAnswer(a,b){

if(
typeof a==="number" &&
typeof b==="number"
){

return Math.abs(a-b)<0.000001;

}

return String(a)===
String(b);

}

function formatNumber(value){

if(
typeof value!=="number"
){

return String(value);

}

if(
!Number.isFinite(value)
){

return "∞";

}

if(
Math.abs(
value-Math.round(value)
)<0.000001
){

return String(
Math.round(value)
);

}

return String(
Math.round(value*100)/100
);

}

function shuffle(array){

for(
var i=array.length-1;
i>0;
i--
){

var j=
Math.floor(
Math.random()*
(i+1)
);

var temp=
array[i];

array[i]=
array[j];

array[j]=
temp;

}

}


/* =====================================================
   난이도
===================================================== */

function chooseDifficulty(){

var keys=
Object.keys(
difficultyConfig
);

var total=0;

keys.forEach(
function(key){

total+=
difficultyConfig[key].weight;

}
);

var r=
Math.random()*
total;

for(
var i=0;
i<keys.length;
i++
){

r-=
difficultyConfig[
keys[i]
].weight;

if(r<=0){

return keys[i];

}

}

return "high";

}

function chooseType(types){

var pool=
types.filter(
function(type){
return type!==lastQuestionType;
}
);

if(
!pool.length
){

pool=types;

}

return randomChoice(
pool
);

}


/* =====================================================
   고등학교 수준 문제
===================================================== */

function generateHigh(){

var types=[

"quadratic_root",
"quadratic_vertex",
"polynomial_value",
"function_composition",
"function_inverse",
"exponential",
"logarithm",
"log_equation",
"trigonometric_value",
"trigonometric_equation",
"arithmetic_sequence",
"geometric_sequence",
"sequence_sum",
"binomial_probability",
"combination",
"permutation",
"triangle_area",
"triangle_angle",
"pythagoras",
"coordinate_distance",
"coordinate_midpoint",
"circle_area",
"circle_circumference",
"circle_sector_area",
"circle_arc",
"circle_equation",
"circle_chord",
"vector_dot",
"vector_magnitude",
"derivative",
"tangent_slope",
"quadratic_derivative",
"integral_basic",
"area_between_curve"

];

var type=
chooseType(types);


/* 이차방정식 */

if(type==="quadratic_root"){

var r1=
randInt(-10,10);

var r2=
randInt(-10,10);

var B=
-(r1+r2);

var C=
r1*r2;

return {
type:type,
question:
"x² "+
(B>=0 ? "+ "+B : "- "+Math.abs(B))+
"x "+
(C>=0 ? "+ "+C : "- "+Math.abs(C))+
" = 0의 한 근은?",
answer:r1
};

}


/* 꼭짓점 */

if(type==="quadratic_vertex"){

var a=
randomChoice(
[1,2,3,-1,-2]
);

var h=
randInt(-6,6);

var k=
randInt(-10,10);

var b=
-2*a*h;

var c=
a*h*h+k;

return {
type:type,
question:
"f(x)="+a+"x² "+
(b>=0 ? "+ "+b : "- "+Math.abs(b))+
"x "+
(c>=0 ? "+ "+c : "- "+Math.abs(c))+
"의 꼭짓점의 x좌표는?",
answer:h
};

}


/* 다항식 */

if(type==="polynomial_value"){

var pa=
randInt(2,6);

var pb=
randInt(-8,8);

var pc=
randInt(-10,10);

var px=
randInt(-4,6);

var pvalue=
pa*px*px+
pb*px+
pc;

return {
type:type,
question:
"P(x)="+
pa+
"x² "+
(pb>=0 ? "+ "+pb : "- "+Math.abs(pb))+
"x "+
(pc>=0 ? "+ "+pc : "- "+Math.abs(pc))+
"일 때 P("+
px+
")의 값은?",
answer:pvalue
};

}


/* 합성함수 */

if(type==="function_composition"){

var fa=
randInt(2,7);

var fb=
randInt(-6,6);

var gx=
randInt(-5,7);

return {
type:type,
question:
"f(x)="+fa+"x "+
(fb>=0 ? "+ "+fb : "- "+Math.abs(fb))+
", g(x)=x²일 때 f(g("+
gx+
"))는?",
answer:
fa*gx*gx+
fb
};

}


/* 역함수 */

if(type==="function_inverse"){

var ia=
randInt(2,8);

var ib=
randInt(-8,8);

var ix=
randInt(-5,8);

return {
type:type,
question:
"f(x)="+ia+"x "+
(ib>=0 ? "+ "+ib : "- "+Math.abs(ib))+
"일 때 f⁻¹("+
(ia*ix+ib)+
")는?",
answer:ix
};

}


/* 지수 */

if(type==="exponential"){

var base=
randomChoice(
[2,3,5]
);

var ea=
randInt(2,5);

var eb=
randInt(1,4);

return {
type:type,
question:
base+"^"+ea+
" × "+
base+"^"+eb+
" = ?",
answer:
Math.pow(
base,
ea+eb
)
};

}


/* 로그 */

if(type==="logarithm"){

var lb=
randomChoice(
[2,3,4,5]
);

var le=
randInt(2,6);

return {
type:type,
question:
"log_"+lb+
"("+
Math.pow(lb,le)+
") = ?",
answer:le
};

}


/* 로그 방정식 */

if(type==="log_equation"){

var logBase=
randomChoice(
[2,3,5]
);

var logAnswer=
randInt(2,6);

return {
type:type,
question:
"log_"+
logBase+
"(x) = "+
logAnswer+
"일 때 x는?",
answer:
Math.pow(
logBase,
logAnswer
)
};

}


/* 삼각함수 */

if(type==="trigonometric_value"){

var trig=
randomChoice([

{q:"sin 30°",a:.5},
{q:"cos 60°",a:.5},
{q:"sin 90°",a:1},
{q:"cos 0°",a:1},
{q:"tan 45°",a:1},
{q:"sin 150°",a:.5},
{q:"cos 120°",a:-.5}

]);

return {
type:type,
question:
trig.q+
" = ?",
answer:trig.a
};

}


/* 삼각함수 방정식 */

if(type==="trigonometric_equation"){

var angle=
randomChoice(
[30,45,60,90]
);

var trigValue;

if(angle===30){
trigValue=.5;
}

if(angle===45){
trigValue=Math.sqrt(2)/2;
}

if(angle===60){
trigValue=Math.sqrt(3)/2;
}

if(angle===90){
trigValue=1;
}

return {
type:type,
question:
"0°≤θ≤90°에서 sin θ = "+
formatNumber(trigValue)+
"일 때 θ는?",
answer:angle
};

}


/* 등차수열 */

if(type==="arithmetic_sequence"){

var af=
randInt(-10,20);

var ad=
randInt(2,10);

var an=
randInt(6,20);

return {
type:type,
question:
"등차수열의 첫째항이 "+
af+
", 공차가 "+
ad+
"일 때 "+
an+
"번째 항은?",
answer:
af+
(an-1)*ad
};

}


/* 등비수열 */

if(type==="geometric_sequence"){

var gf=
randInt(1,5);

var gr=
randomChoice(
[2,3,-2]
);

var gn=
randInt(4,8);

return {
type:type,
question:
"등비수열의 첫째항이 "+
gf+
", 공비가 "+
gr+
"일 때 "+
gn+
"번째 항은?",
answer:
gf*
Math.pow(
gr,
gn-1
)
};

}


/* 수열 합 */

if(type==="sequence_sum"){

var sf=
randInt(1,10);

var sd=
randInt(2,7);

var sn=
randInt(5,12);

return {
type:type,
question:
"첫째항 "+
sf+
", 공차 "+
sd+
"인 등차수열의 첫 "+
sn+
"개 항의 합은?",
answer:
sn*
(2*sf+(sn-1)*sd)/
2
};

}


/* 이항확률 */

if(type==="binomial_probability"){

var bn=
randInt(4,7);

var bs=
randInt(1,bn-1);

return {
type:type,
question:
"공정한 동전을 "+
bn+
"번 던질 때 앞면이 정확히 "+
bs+
"번 나올 확률은?",
answer:
combination(bn,bs)*
Math.pow(.5,bn)
};

}


/* 조합 */

if(type==="combination"){

var cn=
randInt(7,12);

var cr=
randInt(2,cn-2);

return {
type:type,
question:
cn+
"C"+
cr+
"의 값은?",
answer:
combination(cn,cr)
};

}


/* 순열 */

if(type==="permutation"){

var pn=
randInt(5,9);

var pr=
randInt(2,4);

var pvalue=1;

for(
var pi=0;
pi<pr;
pi++
){

pvalue*=
pn-pi;

}

return {
type:type,
question:
pn+
"P"+
pr+
"의 값은?",
answer:pvalue
};

}


/* 삼각형 */

if(type==="triangle_area"){

var tb=
randInt(5,20);

var th=
randInt(5,20);

return {
type:type,
question:
"밑변 "+
tb+
", 높이 "+
th+
"인 삼각형의 넓이는?",
answer:
tb*th/2
};

}


if(type==="triangle_angle"){

var ta=
randInt(25,80);

var tb2=
randInt(25,75);

var tc=
180-ta-tb2;

if(tc<=15){

return generateHigh();

}

return {
type:type,
question:
"삼각형의 두 내각이 "+
ta+
"°, "+
tb2+
"°일 때 나머지 한 각은?",
answer:tc
};

}


/* 피타고라스 */

if(type==="pythagoras"){

var triples=[
[3,4,5],
[5,12,13],
[8,15,17],
[7,24,25]
];

var triple=
randomChoice(triples);

var multiple=
randInt(1,3);

return {
type:type,
question:
"직각삼각형의 두 직각변이 "+
triple[0]*multiple+
", "+
triple[1]*multiple+
"일 때 빗변의 길이는?",
answer:
triple[2]*multiple
};

}


/* 좌표 거리 */

if(type==="coordinate_distance"){

var x1=
randInt(-8,8);

var y1=
randInt(-8,8);

var x2=
randInt(-8,8);

var y2=
randInt(-8,8);

return {
type:type,
question:
"두 점 ("+
x1+
","+y1+
"), ("+
x2+
","+y2+
") 사이의 거리는?",
answer:
Math.sqrt(
Math.pow(x2-x1,2)+
Math.pow(y2-y1,2)
)
};

}


/* 중점 */

if(type==="coordinate_midpoint"){

var mx1=
randInt(-10,10);

var my1=
randInt(-10,10);

var mx2=
randInt(-10,10);

var my2=
randInt(-10,10);

return {
type:type,
question:
"두 점 ("+
mx1+
","+my1+
"), ("+
mx2+
","+my2+
")의 중점의 x좌표는?",
answer:
(mx1+mx2)/2
};

}


/* 원 넓이 */

if(type==="circle_area"){

var ra=
randInt(2,12);

return {
type:type,
question:
"반지름 "+
ra+
"인 원의 넓이를 π를 사용하여 나타내면?",
answer:
(ra*ra)+"π"
};

}


/* 원 둘레 */

if(type==="circle_circumference"){

var rc=
randInt(2,12);

return {
type:type,
question:
"반지름 "+
rc+
"인 원의 둘레를 π를 사용하여 나타내면?",
answer:
(2*rc)+"π"
};

}


/* 부채꼴 */

if(type==="circle_sector_area"){

var rs=
randInt(3,10);

var sa=
randomChoice(
[30,45,60,90,120,180]
);

var sc=
rs*rs*sa/360;

return {
type:type,
question:
"반지름 "+
rs+
", 중심각 "+
sa+
"°인 부채꼴의 넓이는?",
answer:
Number(sc.toFixed(2))+"π"
};

}


/* 호 */

if(type==="circle_arc"){

var rar=
randInt(3,10);

var aa=
randomChoice(
[30,45,60,90,120,180]
);

var ac=
2*rar*aa/360;

return {
type:type,
question:
"반지름 "+
rar+
", 중심각 "+
aa+
"°인 호의 길이는?",
answer:
Number(ac.toFixed(2))+"π"
};

}


/* 원의 방정식 */

if(type==="circle_equation"){

var re=
randInt(2,10);

return {
type:type,
question:
"중심이 원점이고 반지름이 "+
re+
"인 원의 방정식은?",
answer:
"x²+y²="+
(re*re)
};

}


/* 원의 현 */

if(type==="circle_chord"){

var rr=
randInt(5,12);

var dd=
randInt(1,rr-2);

var chord=
2*Math.sqrt(
rr*rr-dd*dd
);

return {
type:type,
question:
"반지름이 "+
rr+
"인 원에서 중심에서 현까지의 거리가 "+
dd+
"일 때 현의 길이는?",
answer:chord
};

}


/* 벡터 내적 */

if(type==="vector_dot"){

var va=
randInt(1,9);

var vb=
randInt(1,9);

var vc=
randInt(1,9);

var vd=
randInt(1,9);

return {
type:type,
question:
"벡터 ("+
va+
","+
vb+
")와 ("+
vc+
","+
vd+
")의 내적은?",
answer:
va*vc+
vb*vd
};

}


/* 벡터 크기 */

if(type==="vector_magnitude"){

var vma=
randInt(3,10);

var vmb=
randInt(3,10);

return {
type:type,
question:
"벡터 ("+
vma+
","+
vmb+
")의 크기는?",
answer:
Math.sqrt(
vma*vma+
vmb*vmb
)
};

}


/* 미분 */

if(type==="derivative"){

var dn=
randInt(2,6);

var da=
randInt(2,7);

var dx=
randInt(1,6);

return {
type:type,
question:
"f(x)="+
da+
"x^"+
dn+
"일 때 f'("+
dx+
")는?",
answer:
da*
dn*
Math.pow(
dx,
dn-1
)
};

}


/* 접선 기울기 */

if(type==="tangent_slope"){

var tA=
randInt(2,7);

var tX=
randInt(1,6);

return {
type:type,
question:
"f(x)="+
tA+
"x²일 때 x="+
tX+
"에서의 접선의 기울기는?",
answer:
2*tA*tX
};

}


/* 이차함수 미분 */

if(type==="quadratic_derivative"){

var qa=
randInt(2,7);

var qb=
randInt(-8,8);

var qx=
randInt(-4,7);

return {
type:type,
question:
"f(x)="+
qa+
"x² "+
(qb>=0 ? "+ "+qb : "- "+Math.abs(qb))+
"x일 때 f'("+
qx+
")는?",
answer:
2*qa*qx+
qb
};

}


/* 적분 */

if(type==="integral_basic"){

var ia=
randInt(2,8);

var inum=
randInt(2,6);

return {
type:type,
question:
"∫₀^"+
inum+
" "+
ia+
"x dx = ?",
answer:
ia*inum*inum/2
};

}


/* 곡선과 x축 넓이 */

var areaA=
randInt(1,5);

var areaN=
randInt(1,5);

return {
type:"area_between_curve",
question:
"y="+
areaA+
"x와 x=0, x="+
areaN+
", x축으로 둘러싸인 도형의 넓이는?",
answer:
areaA*
areaN*
areaN/
2
};

}


/* =====================================================
   대학
===================================================== */

function generateUniversity(){

var types=[
"u_integral",
"u_derivative",
"u_definite_integral",
"u_limit",
"u_matrix_trace",
"u_matrix_det",
"u_probability",
"u_complex",
"u_vector",
"u_circle"
];

var type=
chooseType(types);


if(type==="u_integral"){

var n=
randInt(2,8);

return {
type:type,
question:
"∫₀^"+
n+
" x² dx = ?",
answer:
n*n*n/3
};

}


if(type==="u_derivative"){

var ua=
randInt(2,8);

var un=
randInt(2,5);

var ux=
randInt(1,6);

return {
type:type,
question:
"f(x)="+
ua+
"x^"+
un+
"일 때 f'("+
ux+
")는?",
answer:
ua*
un*
Math.pow(
ux,
un-1
)
};

}


if(type==="u_definite_integral"){

var ul=
randInt(2,8);

var ub=
randInt(1,6);

var un2=
randInt(2,6);

return {
type:type,
question:
"∫₀^"+
un2+
" ("+
ul+
"x+"+
ub+
") dx = ?",
answer:
ul*
un2*
un2/
2+
ub*
un2
};

}


if(type==="u_limit"){

var la=
randInt(2,9);

var lb=
randInt(1,9);

var lx=
randInt(1,7);

return {
type:type,
question:
"lim(x→"+
lx+
")("+
la+
"x+"+
lb+
") = ?",
answer:
la*lx+
lb
};

}


if(type==="u_matrix_trace"){

var ma=
randInt(1,9);

var mb=
randInt(1,9);

return {
type:type,
question:
"행렬 [["+
ma+
",0],[0,"+
mb+
"]]의 trace는?",
answer:
ma+mb
};

}


if(type==="u_matrix_det"){

var m1=
randInt(1,7);

var m2=
randInt(1,7);

var m3=
randInt(1,7);

var m4=
randInt(1,7);

return {
type:type,
question:
"det [["+
m1+
","+
m2+
"],["+
m3+
","+
m4+
"]]의 값은?",
answer:
m1*m4-
m2*m3
};

}


if(type==="u_probability"){

var us=
randInt(2,7);

var ut=
randInt(us+1,12);

return {
type:type,
question:
"성공 "+
us+
"회 / 전체 "+
ut+
"회일 때 경험적 확률은?",
answer:
us/ut
};

}


if(type==="u_complex"){

var ca=
randInt(1,8);

var cb=
randInt(1,8);

return {
type:type,
question:
"z="+
ca+
" + "+
cb+
"i일 때 |z|²는?",
answer:
ca*ca+
cb*cb
};

}


if(type==="u_vector"){

var va=
randInt(1,8);

var vb=
randInt(1,8);

var vc=
randInt(1,8);

var vd=
randInt(1,8);

return {
type:type,
question:
"벡터 ("+
va+
","+
vb+
")·("+
vc+
","+
vd+
") = ?",
answer:
va*vc+
vb*vd
};

}


var cr=
randInt(3,10);

return {
type:"u_circle",
question:
"반지름 "+
cr+
"인 원의 넓이를 π로 나타내면?",
answer:
(cr*cr)+"π"
};

}


/* =====================================================
   대학 심화
===================================================== */

function generateUniversityHard(){

var types=[
"uh_integral_trig",
"uh_chain_rule",
"uh_determinant",
"uh_complex",
"uh_expectation",
"uh_geometric_series",
"uh_cross_product",
"uh_circle_sector",
"uh_coordinate_geometry"
];

var type=
chooseType(types);


if(type==="uh_integral_trig"){

var ua=
randInt(1,7);

return {
type:type,
question:
"∫₀^π "+
ua+
"sin(x) dx = ?",
answer:
2*ua
};

}


if(type==="uh_chain_rule"){

var ca=
randInt(2,7);

var cx=
randInt(1,6);

var inner=
ca*cx*cx+1;

return {
type:type,
question:
"f(x)=("+
ca+
"x²+1)³일 때 x="+
cx+
"에서 f'(x)는?",
answer:
6*
ca*
cx*
inner*
inner
};

}


if(type==="uh_determinant"){

var da=
randInt(1,5);

var db=
randInt(1,5);

var dc=
randInt(1,5);

return {
type:type,
question:
"diag("+
da+
","+
db+
","+
dc+
")의 행렬식은?",
answer:
da*db*dc
};

}


if(type==="uh_complex"){

var za=
randInt(1,9);

return {
type:type,
question:
"z="+
za+
"i일 때 z²는?",
answer:
-za*za
};

}


if(type==="uh_expectation"){

var ex1=
randInt(1,5);

var ex2=
randInt(6,10);

var prob=
randomChoice(
[.2,.3,.4,.6,.7,.8]
);

return {
type:type,
question:
"X가 "+
ex1+
"을 확률 "+
prob+
", "+
ex2+
"를 확률 "+
(1-prob)+
"로 가질 때 E[X]는?",
answer:
prob*ex1+
(1-prob)*ex2
};

}


if(type==="uh_geometric_series"){

var gsA=
randInt(1,5);

var gsR=
randomChoice(
[2,3]
);

var gsN=
randInt(3,7);

return {
type:type,
question:
"첫째항 "+
gsA+
", 공비 "+
gsR+
"인 등비수열의 첫 "+
gsN+
"개 항의 합은?",
answer:
gsA*
(Math.pow(gsR,gsN)-1)/
(gsR-1)
};

}


if(type==="uh_cross_product"){

var xa=
randInt(2,7);

var xb=
randInt(2,7);

return {
type:type,
question:
"벡터 ("+
xa+
",0,0)과 (0,"+
xb+
",0)의 외적의 크기는?",
answer:
xa*xb
};

}


if(type==="uh_circle_sector"){

var rr=
randInt(3,9);

var angle=
randomChoice(
[30,45,60,90,120]
);

return {
type:type,
question:
"반지름 "+
rr+
", 중심각 "+
angle+
"°인 부채꼴의 넓이는?",
answer:
Number(
(rr*rr*angle/360)
.toFixed(2)
)+"π"
};

}


var x1=
randInt(-5,5);

var y1=
randInt(-5,5);

var x2=
randInt(-5,5);

var y2=
randInt(-5,5);

return {
type:"uh_coordinate_geometry",
question:
"두 점 ("+
x1+
","+
y1+
"), ("+
x2+
","+
y2+
") 사이 거리의 제곱은?",
answer:
Math.pow(x2-x1,2)+
Math.pow(y2-y1,2)
};

}


/* =====================================================
   문제 선택
===================================================== */

function createQuestion(){

var attempts=0;

while(
attempts<1000
){

attempts++;

var level=
chooseDifficulty();

var q;

if(level==="high"){

q=
generateHigh();

}else if(
level==="university"
){

q=
generateUniversity();

}else{

q=
generateUniversityHard();

}

if(
q.type===
lastQuestionType
){

continue;

}

var key=
level+
"|"+
q.type+
"|"+
q.question+
"|"+
String(q.answer);

if(
usedQuestionKeys[key]
){

continue;

}

usedQuestionKeys[key]=true;

lastQuestionType=
q.type;

q.level=
level;

return q;

}

return {
level:"high",
type:"fallback_"+Date.now(),
question:"x² - 7x + 12 = 0의 한 근은?",
answer:3
};

}


/* =====================================================
   비슷한 선지
===================================================== */

function makeChoices(answer,level){

/* π */

if(
typeof answer==="string" &&
answer.indexOf("π")!==-1
){

var coefficient=
parseFloat(
answer.replace("π","")
);

if(
Number.isFinite(coefficient)
){

var choices=[
answer
];

var step=
Math.abs(coefficient)>=20
?0.5
:0.25;

var offsets=[
-step*2,
-step,
step,
step*2
];

offsets.forEach(
function(offset){

var value=
coefficient+
offset;

if(value<=0){
return;
}

var text=
String(
Number(
value.toFixed(2)
)
)+
"π";

if(
choices.indexOf(text)===-1
){

choices.push(text);

}

}
);

while(
choices.length<5
){

var direction=
choices.length%2===0
?1
:-1;

var extra=
coefficient+
direction*
step*
3;

if(extra>0){

var extraText=
String(
Number(
extra.toFixed(2)
)
)+
"π";

if(
choices.indexOf(extraText)===-1
){

choices.push(extraText);

}else{

break;

}

}else{

break;

}

}

shuffle(choices);

return choices;

}

}


/* 원 방정식 */

if(
typeof answer==="string" &&
answer.indexOf("x²+y²=")===0
){

var radiusValue=
Number(
answer.split("=")[1]
);

var equationChoices=[
answer,
"x²+y²="+
Math.max(1,radiusValue-2),
"x²+y²="+
Math.max(1,radiusValue-1),
"x²+y²="+
(radiusValue+1),
"x²+y²="+
(radiusValue+2)
];

shuffle(
equationChoices
);

return equationChoices;

}


/* 일반 숫자 */

if(
typeof answer==="number" &&
Number.isFinite(answer)
){

var numericChoices=[
answer
];

var abs=
Math.abs(answer);

var stepNumber;

if(abs<5){
stepNumber=.25;
}else if(abs<20){
stepNumber=.5;
}else if(abs<100){
stepNumber=1;
}else if(abs<500){
stepNumber=2;
}else if(abs<2000){
stepNumber=5;
}else{
stepNumber=
Math.max(
10,
Math.round(abs*.01)
);
}

var numericOffsets=[
-stepNumber*2,
-stepNumber,
stepNumber,
stepNumber*2
];

numericOffsets.forEach(
function(offset){

var value=
answer+
offset;

if(
!Number.isInteger(answer)
){

value=
Math.round(
value*100
)/100;

}

if(
!numericChoices.some(
function(existing){
return sameAnswer(existing,value);
}
)
){

numericChoices.push(value);

}

}
);

var micro=
stepNumber/2;

while(
numericChoices.length<5
){

var sign=
numericChoices.length%2===0
?1
:-1;

var extraValue=
answer+
sign*
micro;

if(
!Number.isInteger(answer)
){

extraValue=
Math.round(
extraValue*100
)/100;

}

if(
!numericChoices.some(
function(existing){
return sameAnswer(existing,extraValue);
}
)
){

numericChoices.push(
extraValue
);

}else{

micro+=
stepNumber/2;

}

}

shuffle(
numericChoices
);

return numericChoices;

}

return [
answer,
"보기 2",
"보기 3",
"보기 4",
"보기 5"
];

}


/* =====================================================
   상태
===================================================== */

function renderGameStatus(){

document.getElementById(
"gameScore"
).textContent=
gameScore;

document.getElementById(
"questionTime"
).textContent=
questionTime;

document.getElementById(
"gameSolved"
).textContent=
gameSolved;

document.getElementById(
"wrongStreak"
).textContent=
wrongStreak+
" / "+
MAX_WRONG_STREAK;

}


/* =====================================================
   문제 표시
===================================================== */

function showQuestion(){

if(!gameRunning){
return;
}

currentQuestion=
createQuestion();

var config=
difficultyConfig[
currentQuestion.level
];

document.getElementById(
"difficulty"
).textContent=
config.label+
" · 정답 +"+
config.score+
"점";

document.getElementById(
"question"
).textContent=
currentQuestion.question;

var choices=
makeChoices(
currentQuestion.answer,
currentQuestion.level
);

currentQuestion.choices=
choices;

var box=
document.getElementById(
"choices"
);

box.innerHTML="";

var labels=[
"①",
"②",
"③",
"④",
"⑤"
];

choices.forEach(
function(choice,index){

var button=
document.createElement(
"button"
);

button.className=
"choice-btn";

button.textContent=
labels[index]+
" "+
formatNumber(choice);

button.onclick=
function(){

answerQuestion(
index,
button
);

};

box.appendChild(
button
);

}
);

document.getElementById(
"gameMessage"
).textContent=
"정답을 선택하세요.";

startQuestionTimer();

}


/* =====================================================
   20초 타이머
===================================================== */

function startQuestionTimer(){

if(questionTimer){

clearInterval(
questionTimer
);

}

questionTime=
QUESTION_TIME;

renderGameStatus();

document.getElementById(
"questionTimerBar"
).style.width=
"100%";

questionTimer=
setInterval(
function(){

questionTime--;

renderGameStatus();

document.getElementById(
"questionTimerBar"
).style.width=
Math.max(
0,
questionTime/
QUESTION_TIME*
100
)+
"%";

if(
questionTime<=0
){

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
   시간초과
===================================================== */

function questionTimeout(){

if(!gameRunning){
return;
}

document.querySelectorAll(
".choice-btn"
).forEach(
function(button){
button.disabled=true;
}
);

wrongStreak++;

renderGameStatus();

if(
wrongStreak>=
MAX_WRONG_STREAK
){

document.getElementById(
"gameMessage"
).textContent=
"⏰ 5번 연속 오답으로 게임 종료!";

setTimeout(
function(){
endMathGame();
},
450
);

return;
}

document.getElementById(
"gameMessage"
).textContent=
"⏰ 시간 초과! 연속 오답 "+
wrongStreak+
"/"+
MAX_WRONG_STREAK;

setTimeout(
function(){

if(gameRunning){

showQuestion();

}

},
500
);

}


/* =====================================================
   답
===================================================== */

function answerQuestion(
index,
clickedButton
){

if(!gameRunning){
return;
}

if(questionTimer){

clearInterval(
questionTimer
);

questionTimer=null;

}

document.querySelectorAll(
".choice-btn"
).forEach(
function(button){
button.disabled=true;
}
);

var selected=
currentQuestion.choices[
index
];

var correct=
sameAnswer(
selected,
currentQuestion.answer
);

if(correct){

clickedButton.classList.add(
"correct"
);

var points=
difficultyConfig[
currentQuestion.level
].score;

gameScore+=
points;

gameSolved++;

wrongStreak=0;

document.getElementById(
"gameMessage"
).textContent=
"✅ 정답! +"+
points+
"점";

}else{

clickedButton.classList.add(
"wrong"
);

wrongStreak++;

document.getElementById(
"gameMessage"
).textContent=
"❌ 오답! 연속 오답 "+
wrongStreak+
"/"+
MAX_WRONG_STREAK;

}

renderGameStatus();

if(
wrongStreak>=
MAX_WRONG_STREAK
){

setTimeout(
function(){
endMathGame();
},
500
);

return;
}

setTimeout(
function(){

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

var nickname=
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

questionTime=
QUESTION_TIME;

gameSolved=0;

wrongStreak=0;

currentQuestion=null;

usedQuestionKeys={};

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
   종료
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
function(button){
button.disabled=true;
}
);

/* 종료 후 닉네임 다시 입력 */

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
).textContent=
"0";

document.getElementById(
"questionTimerBar"
).style.width=
"0%";

var nickname=
document.getElementById(
"gameNickname"
).value.trim();

var reason=
wrongStreak>=
MAX_WRONG_STREAK
?
"5번 연속 오답"
:
"게임 종료";

document.getElementById(
"gameMessage"
).textContent=
reason+
"!";

if(
gameScore>
bestGameScore
){

bestGameScore=
gameScore;

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
gameScore+
"점";

document.getElementById(
"resultInfo"
).textContent=
nickname+
"님 · "+
gameSolved+
"문제 정답 · "+
reason;

saveRanking(
nickname,
gameScore
);

}


/* =====================================================
   랭킹
===================================================== */

function getRanking(){

var ranking=
safeRead(
RANKING_KEY,
[]
);

if(
!Array.isArray(ranking)
){

ranking=[];

}

return ranking;

}

function saveRanking(
nickname,
score
){

var ranking=
getRanking();

ranking.push({

name:nickname,
score:score,
time:Date.now()

});

ranking.sort(
function(a,b){

if(
b.score!==
a.score
){

return b.score-a.score;

}

return a.time-b.time;

}
);

localStorage.setItem(
RANKING_KEY,
JSON.stringify(
ranking.slice(
0,
20
)
)
);

renderRanking();

}

function renderRanking(){

var body=
document.getElementById(
"rankingBody"
);

if(!body){
return;
}

var ranking=
getRanking();

if(
ranking.length===0
){

body.innerHTML=
'<tr><td colspan="3">아직 기록이 없습니다.</td></tr>';

return;

}

var html="";

ranking.forEach(
function(item,index){

html+=
"<tr>"+
"<td>"+
(index+1)+
"</td>"+
"<td>"+
escapeHTML(item.name)+
"</td>"+
"<td>"+
item.score+
"</td>"+
"</tr>";

}
);

body.innerHTML=
html;

}


/* =====================================================
   좋아요 시간 갱신
===================================================== */

setInterval(
function(){

render();

},
1000
);


/* =====================================================
   시작
===================================================== */

document.getElementById(
"gameBest"
).textContent=
bestGameScore;

renderRanking();
render();
restorePage();

</script>

</body>
</html>
