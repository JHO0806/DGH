<html lang="ko">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<title>대광고등학교 큰빛축제</title>
<style>
*{box-sizing:border-box}
html,body{margin:0;padding:0}
body{font-family:"Malgun Gothic","Noto Sans KR",sans-serif;background:#f7eef1;color:#24151b;user-select:none;overflow-x:hidden}
input,textarea,button{font:inherit}
input,textarea{user-select:text}
#floatingLogos{position:fixed;inset:0;z-index:0;pointer-events:none;overflow:hidden}
.logo-float{position:absolute;left:0;top:0;width:58px;height:58px;opacity:.08;pointer-events:none}
.logo-float:nth-child(1){animation:m1 17s linear infinite}
.logo-float:nth-child(2){animation:m2 20s linear infinite}
.logo-float:nth-child(3){animation:m3 18s linear infinite}
.logo-float:nth-child(4){animation:m4 21s linear infinite}
.logo-float:nth-child(5){animation:m5 16s linear infinite}
.logo-float:nth-child(6){animation:m6 23s linear infinite}
.logo-float:nth-child(7){animation:m7 19s linear infinite}
.logo-float:nth-child(8){animation:m8 22s linear infinite}
.logo-float:nth-child(9){animation:m9 17s linear infinite}
.logo-float:nth-child(10){animation:m10 24s linear infinite}
.logo-float:nth-child(11){animation:m11 20s linear infinite}
.logo-float:nth-child(12){animation:m12 18s linear infinite}
@keyframes m1{0%{transform:translate(0,118vh)}100%{transform:translate(82vw,-18vh)}}
@keyframes m2{0%{transform:translate(18vw,120vh)}100%{transform:translate(103vw,-18vh)}}
@keyframes m3{0%{transform:translate(35vw,120vh)}100%{transform:translate(118vw,-16vh)}}
@keyframes m4{0%{transform:translate(-7vw,117vh)}100%{transform:translate(74vw,-18vh)}}
@keyframes m5{0%{transform:translate(49vw,121vh)}100%{transform:translate(126vw,-15vh)}}
@keyframes m6{0%{transform:translate(7vw,120vh)}100%{transform:translate(96vw,-20vh)}}
@keyframes m7{0%{transform:translate(66vw,121vh)}100%{transform:translate(129vw,-14vh)}}
@keyframes m8{0%{transform:translate(26vw,122vh)}100%{transform:translate(110vw,-19vh)}}
@keyframes m9{0%{transform:translate(-4vw,119vh)}100%{transform:translate(87vw,-18vh)}}
@keyframes m10{0%{transform:translate(43vw,121vh)}100%{transform:translate(120vw,-17vh)}}
@keyframes m11{0%{transform:translate(72vw,120vh)}100%{transform:translate(132vw,-15vh)}}
@keyframes m12{0%{transform:translate(11vw,123vh)}100%{transform:translate(105vw,-21vh)}}
.hero{background:linear-gradient(135deg,#64152f,#8f2948);color:#fff;padding:28px 18px 34px;box-shadow:0 4px 16px #0002;position:relative;z-index:10}
.top{max-width:1050px;margin:auto;display:flex;align-items:center;gap:18px}
.logo{width:78px;height:78px;border:3px solid #fff;border-radius:50%;background:#fff;display:grid;place-items:center;flex:none;box-shadow:0 3px 10px #0004}
.mark{color:#741b38;font-weight:900;font-size:25px;line-height:1;text-align:center}
.mark small{display:block;font-size:8px;letter-spacing:1px;margin-top:3px}
h1{margin:0;font-size:30px}.sub{margin-top:7px;opacity:.9}
.page{display:none;position:relative;z-index:5}.page.active{display:block}
main{max-width:1050px;margin:24px auto;padding:0 14px;position:relative;z-index:5}
.menu-wrap{min-height:calc(100vh - 150px);display:flex;align-items:center;justify-content:center;padding:25px 0 40px;position:relative;z-index:6}
.menu{width:min(760px,100%);position:relative;z-index:7}
.menu-title{text-align:center;margin-bottom:28px}.menu-title h2{margin:0;color:#741b38;font-size:31px}.menu-title p{margin:10px 0 0;color:#806d76}
.menu-grid{display:grid;grid-template-columns:1fr 1fr;gap:18px;position:relative;z-index:8}
.menu-card{background:#fff;border:1px solid #ead6dc;border-radius:22px;padding:32px 20px;text-align:center;box-shadow:0 8px 28px #6d203725;cursor:pointer;transition:.2s;position:relative;z-index:9}
.menu-card:hover{transform:translateY(-5px)}
.menu-icon{font-size:50px;margin-bottom:14px}.menu-card h3{margin:0;color:#741b38;font-size:22px}.menu-card p{color:#806d76;margin:9px 0 0;font-size:14px}
.panel,.game-box{background:#fff;border-radius:18px;padding:20px;box-shadow:0 4px 18px #6d203714;margin-bottom:20px;position:relative;z-index:5}
.panel h2{margin:0 0 15px;font-size:20px}
.grid{display:grid;grid-template-columns:1fr 1fr;gap:12px}
input,textarea{width:100%;border:1px solid #dccbd1;border-radius:10px;padding:12px;outline:none;background:#fff}
input:disabled{background:#f1edef;color:#8f858a}
textarea{min-height:105px;resize:none}
input:focus,textarea:focus{border-color:#8a2947;box-shadow:0 0 0 3px #8a29471a}
.full{grid-column:1/-1}
button{border:0;border-radius:10px;padding:11px 18px;cursor:pointer;background:#741b38;color:#fff;font-weight:700}
button.secondary{background:#f1e5e9;color:#5d1930}.danger{background:#b73550!important}
.actions{display:flex;gap:8px;justify-content:flex-end;margin-top:12px;flex-wrap:wrap}
.hint{font-size:13px;color:#76636b;margin-top:8px}
.back-btn{margin-bottom:16px}
.entry{border:1px solid #ead6dc;border-radius:15px;padding:17px;margin-top:12px;background:#fffafb}
.entry-head{display:flex;justify-content:space-between;gap:10px;align-items:center}.name{font-weight:800;font-size:17px}.time{font-size:12px;color:#7d6c74;text-align:right}
.content{white-space:pre-wrap;line-height:1.65;margin:12px 0}.tag{display:inline-block;background:#f3e3e8;color:#741b38;border-radius:999px;padding:4px 9px;font-size:12px}.empty{text-align:center;color:#8b7b82;padding:35px 10px}
.like-area{display:flex;align-items:center;gap:7px;flex-wrap:wrap}.like-btn{background:#fff;color:#8a2947;border:1px solid #ead6dc}.like-count{min-width:28px;text-align:center;color:#8a2947;font-weight:800}.cancel-like{background:#f1e5e9;color:#5d1930}.cancel-like:disabled{background:#f3f1f2;color:#aaa0a5;cursor:not-allowed}
.modal{position:fixed;inset:0;background:#2b0d1799;display:none;align-items:center;justify-content:center;padding:18px;z-index:100}.modal.show{display:flex}.modal-card{background:#fff;border-radius:17px;padding:22px;width:min(430px,100%);box-shadow:0 15px 50px #0005}.modal-card h3{margin-top:0}.error{color:#b73550;font-size:13px;margin-top:8px;min-height:18px}
.game-title{text-align:center;color:#741b38;margin:0 0 8px;font-size:25px}.game-description{text-align:center;color:#806d76;margin:0 0 18px;font-size:14px}
.game-status{display:grid;grid-template-columns:repeat(4,1fr);gap:10px;margin-bottom:18px}.status-box{background:#f8eff2;border:1px solid #ead6dc;border-radius:12px;padding:12px;text-align:center}.status-label{display:block;color:#806d76;font-size:12px;margin-bottom:4px}.status-value{color:#741b38;font-weight:900;font-size:18px}
.game-screen{border:1px solid #ead6dc;border-radius:16px;padding:22px;background:linear-gradient(180deg,#fffafb,#f6e9ed)}.difficulty{display:inline-block;padding:6px 11px;border-radius:999px;background:#f1dce3;color:#741b38;font-size:12px;font-weight:800;margin-bottom:10px}
.question-timer-wrap{width:100%;height:8px;background:#eadde1;border-radius:999px;overflow:hidden;margin-bottom:12px}#questionTimerBar{height:100%;width:100%;background:#8a2947;transition:width 1s linear}
.question{min-height:125px;display:flex;align-items:center;justify-content:center;text-align:center;font-size:23px;font-weight:900;line-height:1.6;padding:8px;word-break:break-word}
.choices{display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-top:16px}.choice-btn{background:#fff;color:#5d1930;border:1px solid #dccbd1;padding:14px 12px;min-height:54px}.choice-btn.correct{background:#dff3e5;color:#176b32}.choice-btn.wrong{background:#fde2e2;color:#a12831}
.game-message{text-align:center;color:#806d76;min-height:23px;margin-top:14px;font-size:14px}.game-start-wrap{text-align:center;margin-top:16px}.big-btn{padding:14px 25px;font-size:16px}
.result{display:none;text-align:center;padding:12px 0 2px}.result.show{display:block}.result-score{color:#741b38;font-size:31px;font-weight:900}.result-info{color:#806d76;font-size:14px}
.ranking-box{margin-top:20px;border-top:1px solid #ead6dc;padding-top:20px}.ranking-title{color:#741b38;font-size:20px;font-weight:900;margin-bottom:12px}.ranking-table{width:100%;border-collapse:collapse}.ranking-table th,.ranking-table td{padding:10px 8px;text-align:center;border-bottom:1px solid #eee1e5;font-size:14px}.ranking-table th{background:#f4e6ea;color:#741b38}
@media(max-width:650px){.grid{grid-template-columns:1fr}.full{grid-column:auto}h1{font-size:23px}.logo{width:65px;height:65px}.menu-grid{grid-template-columns:1fr}.menu-title h2{font-size:26px}.game-status{grid-template-columns:1fr 1fr}.choices{grid-template-columns:1fr}.question{font-size:20px}.logo-float{opacity:.06}}
</style>
</head>

<body>

<div id="floatingLogos"></div>

<header class="hero">
<div class="top">
<div class="logo"><div class="mark">大光<small>DAE KWANG</small></div></div>
<div><h1>대광고등학교 큰빛축제</h1><div class="sub">우리들의 축제, 우리들의 기록</div></div>
</div>
</header>

<section id="menuPage" class="page">

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
<p>쉬운 문제부터 어려운 문제까지 도전!</p>
</div>

</div>
</div>
</div>

</section>

<section id="guestbookPage" class="page">

<main>

<button class="secondary back-btn" onclick="showPage('menuPage')">← 메뉴로 돌아가기</button>

<section class="panel">
<h2>✍️ 방문록 남기기</h2>

<div class="grid">

<input id="name" maxlength="30" placeholder="이름 또는 닉네임">

<input id="password" type="password" maxlength="30" placeholder="수정·삭제용 비밀번호">

<textarea id="message" class="full" maxlength="1000" placeholder="큰빛축제에서 느낀 점을 남겨보세요."></textarea>

</div>

<div class="actions">
<button onclick="addEntry()">방문록 등록</button>
</div>

<div class="hint">
※ 작성할 때 입력한 비밀번호로 본인 글을 수정·삭제할 수 있습니다.
</div>

</section>

<section class="panel">

<h2>📖 큰빛축제 방문록 <span id="count" class="tag">0개</span></h2>

<div id="entries"></div>

</section>

</main>

</section>

<section id="gamePage" class="page">

<main>

<button class="secondary back-btn" onclick="showPage('menuPage')">← 메뉴로 돌아가기</button>

<section class="game-box">

<h2 class="game-title">🎮 랜덤 수학 미니게임</h2>

<p class="game-description">
쉬운 문제부터 어려운 문제까지 나옵니다.
문제마다 20초의 제한시간이 있으며 5번 연속 오답이면 종료됩니다.
</p>

<div class="nickname-row">

<input id="gameNickname" maxlength="20" placeholder="랭킹에 표시할 닉네임">

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

<div id="difficulty" class="difficulty">게임을 시작해주세요</div>

<div class="question-timer-wrap">
<div id="questionTimerBar"></div>
</div>

<div id="question" class="question">고등학교 수준 이상의 랜덤 수학문제</div>

<div id="choices" class="choices"></div>

<div id="gameMessage" class="game-message">
닉네임을 입력한 뒤 게임 시작을 눌러주세요.
</div>

</div>

<div class="game-start-wrap">

<button id="startGameBtn" class="big-btn" onclick="startMathGame()">게임 시작</button>

</div>

<div id="result" class="result">

<div id="resultScore" class="result-score">0점</div>
<div id="resultInfo" class="result-info"></div>

</div>

<div class="ranking-box">

<div class="ranking-title">🏆 큰빛축제 수학게임 랭킹</div>

<table class="ranking-table">

<thead>
<tr><th>순위</th><th>닉네임</th><th>점수</th></tr>
</thead>

<tbody id="rankingBody"></tbody>

</table>

</div>

</section>

</main>

</section>

<div id="modal" class="modal">

<div class="modal-card">

<h3 id="modalTitle">비밀번호 확인</h3>

<input id="checkPw" type="password" placeholder="비밀번호">

<div id="pwError" class="error"></div>

<div class="actions">

<button class="secondary" onclick="closeModal()">취소</button> <button onclick="confirmPassword()">확인</button>

</div>

</div>

</div>

<script>

/* =====================================================
   배경 로고
===================================================== */

function createLogo(){
return '<svg viewBox="0 0 200 200" width="100%" height="100%" xmlns="http://www.w3.org/2000/svg">'+
'<circle cx="100" cy="100" r="94" fill="#8a2340"/>'+
'<circle cx="100" cy="100" r="76" fill="none" stroke="#fff" stroke-width="8"/>'+
'<path d="M58 63 Q100 42 142 63 L136 118 Q132 146 100 163 Q68 146 64 118 Z" fill="#8a2340" stroke="#fff" stroke-width="3"/>'+
'<text x="100" y="101" text-anchor="middle" fill="#fff" font-family="Georgia" font-size="13" font-weight="700">LUX ET SAL</text>'+
'<text x="100" y="132" text-anchor="middle" fill="#fff" font-family="serif" font-size="28" font-weight="700">大光</text>'+
'<text x="100" y="28" text-anchor="middle" fill="#fff" font-family="Georgia" font-size="9" font-weight="700">DAE GWANG HIGH SCHOOL</text>'+
'<text x="100" y="185" text-anchor="middle" fill="#fff" font-family="serif" font-size="9" font-weight="700">대 광 고 등 학 교</text>'+
'</svg>';
}

var floating=document.getElementById("floatingLogos");

for(var i=0;i<12;i++){
var lg=document.createElement("div");
lg.className="logo-float";
lg.innerHTML=createLogo();
lg.style.animationDelay=(-(i*1.7))+"s";
floating.appendChild(lg);
}


/* =====================================================
   현재 페이지 저장
   핵심: localStorage + URL hash
===================================================== */

var PAGE_KEY="daekwang_current_page_v_final";

function validPage(id){
return id==="menuPage"||id==="guestbookPage"||id==="gamePage";
}

function showPage(id){

if(!validPage(id)){
id="menuPage";
}

document.querySelectorAll(".page").forEach(function(page){
page.classList.remove("active");
});

var target=document.getElementById(id);

if(!target){
return;
}

target.classList.add("active");

localStorage.setItem(PAGE_KEY,id);

if(location.hash!=="#"+id){
history.replaceState(null,"","#"+id);
}

window.scrollTo(0,0);
}

function restorePage(){

var id="";

if(location.hash){
id=location.hash.substring(1);
}

if(!validPage(id)){
id=localStorage.getItem(PAGE_KEY)||"menuPage";
}

if(!validPage(id)){
id="menuPage";
}

showPage(id);
}

window.addEventListener("hashchange",function(){

var id=location.hash.substring(1);

if(validPage(id)){

document.querySelectorAll(".page").forEach(function(page){
page.classList.remove("active");
});

document.getElementById(id).classList.add("active");

localStorage.setItem(PAGE_KEY,id);

window.scrollTo(0,0);

}

});


/* =====================================================
   방문록
===================================================== */

var STORAGE_KEY="daekwang_guestbook_final";
var LIKE_KEY="daekwang_likes_final";
var MASTER_PASSWORD="20100806";
var LIKE_DELAY=7000;

function readData(key,fallback){

try{

var value=localStorage.getItem(key);

if(value===null){
return fallback;
}

return JSON.parse(value);

}catch(e){

return fallback;

}

}

var entries=readData(STORAGE_KEY,[]);
var likes=readData(LIKE_KEY,{});
var pending=null;

if(!Array.isArray(entries)){
entries=[];
}

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

return {
"&":"&amp;",
"<":"&lt;",
">":"&gt;",
'"':"&quot;",
"'":"&#039;"
}[char];

}
);

}

function formatDate(value){

var d=new Date(value);

function p(n){
return String(n).padStart(2,"0");
}

return d.getFullYear()+
"년 "+
p(d.getMonth()+1)+
"월 "+
p(d.getDate())+
"일 "+
p(d.getHours())+
"시 "+
p(d.getMinutes())+
"분 "+
p(d.getSeconds())+
"초";

}

function addEntry(){

var name=document.getElementById("name").value.trim();
var password=document.getElementById("password").value;
var message=document.getElementById("message").value.trim();

if(!name||!password||!message){

alert("이름(닉네임), 비밀번호, 내용을 모두 입력해주세요.");
return;

}

var id=
window.crypto&&typeof crypto.randomUUID==="function"
?
crypto.randomUUID()
:
String(Date.now())+String(Math.random());

entries.unshift({

id:id,
name:name,
message:message,
password:password,
createdAt:new Date().toISOString()

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

function normalizeLike(id){

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

return likes[id];

}

function addLike(id){

var data=normalizeLike(id);

data.count++;
data.times.push(Date.now());

saveLikes();
render();

}

function cancelIndex(id){

var data=likes[id];

if(
!data||
!Array.isArray(data.times)
){
return -1;
}

var now=Date.now();

return data.times.findIndex(
function(time){
return now-time>=LIKE_DELAY;
}
);

}

function cancelLike(id){

var data=likes[id];

if(!data){
return;
}

var index=cancelIndex(id);

if(index===-1){

alert("좋아요를 누른 후 7초가 지나야 취소할 수 있습니다.");
return;

}

data.times.splice(index,1);
data.count=Math.max(0,data.count-1);

saveLikes();
render();

}

function cancelText(id){

var data=likes[id];

if(!data||!data.times.length){
return "좋아요 취소";
}

var now=Date.now();

if(
data.times.some(
function(time){
return now-time>=LIKE_DELAY;
}
)
){

return "좋아요 취소";

}

var earliest=Math.min.apply(Math,data.times);

var remain=Math.max(
0,
Math.ceil(
(LIKE_DELAY-(now-earliest))/1000
)
);

return String(remain)+"초 후 취소";

}


/* =====================================================
   방문록 출력
===================================================== */

function render(){

var box=document.getElementById("entries");
var count=document.getElementById("count");

if(!box||!count){
return;
}

count.textContent=String(entries.length)+"개";

if(entries.length===0){

box.innerHTML=
'<div class="empty">아직 등록된 방문록이 없습니다.<br>첫 번째 기록을 남겨보세요!</div>';

return;

}

var html="";

entries.forEach(
function(entry){

var like=normalizeLike(entry.id);

var canCancel=
cancelIndex(entry.id)!==-1;

html+=
'<article class="entry">'+
'<div class="entry-head">'+
'<div class="name">'+
escapeHTML(entry.name)+
'</div>'+
'<div class="time">'+
"작성: "+
formatDate(entry.createdAt)+
(entry.updatedAt?
"<br>수정: "+
formatDate(entry.updatedAt)
:
"")+
"</div>"+
"</div>"+
'<div class="content">'+
escapeHTML(entry.message)+
"</div>"+
'<div class="actions">'+
'<div class="like-area">'+
'<button class="like-btn" onclick="addLike(\''+
entry.id+
'\')">❤️ 좋아요</button>'+
'<span class="like-count">'+
like.count+
"</span>"+
'<button class="cancel-like" onclick="cancelLike(\''+
entry.id+
'\')" '+
(canCancel?"":"disabled")+
">"+
cancelText(entry.id)+
"</button>"+
"</div>"+
'<button class="secondary" onclick="requestAction(\'edit\',\''+
entry.id+
"\')\">수정</button>"+
'<button class="danger" onclick="requestAction(\'delete\',\''+
entry.id+
"\')\">삭제</button>"+
"</div>"+
"</article>";

}
);

box.innerHTML=html;

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
?
"수정을 위한 비밀번호 확인"
:
"삭제를 위한 비밀번호 확인";

document.getElementById("modal").classList.add("show");

setTimeout(
function(){
document.getElementById("checkPw").focus();
},
50
);

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

var entry=
entries.find(
function(item){
return item.id===pending.id;
}
);

var password=
document.getElementById("checkPw").value;

if(
!entry||
!(
password===entry.password||
password===MASTER_PASSWORD
)
){

document.getElementById("pwError")
.textContent=
"비밀번호가 올바르지 않습니다.";

return;

}

var action=pending.action;
var id=pending.id;

closeModal();

if(action==="delete"){

if(confirm("이 방문록을 삭제할까요?")){

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
!newName.trim()||
!newMessage.trim()
){

alert("내용을 비워둘 수 없습니다.");
return;

}

target.name=newName.trim();
target.message=newMessage.trim();
target.updatedAt=new Date().toISOString();

saveEntries();
render();

}

document.getElementById("modal").addEventListener(
"click",
function(event){

if(event.target.id==="modal"){
closeModal();
}

}
);

document.addEventListener(
"keydown",
function(event){

if(event.key==="Escape"){
closeModal();
}

}
);


/* =====================================================
   수학 게임
===================================================== */

var QUESTION_TIME=20;
var MAX_WRONG=5;

var RANKING_KEY=
"daekwang_math_ranking_final";

var BEST_KEY=
"daekwang_math_best_final";

var difficulty={

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

hard:{
label:"🔴 대학 심화",
score:16,
weight:5
}

};

var gameRunning=false;
var gameScore=0;
var gameSolved=0;
var wrongStreak=0;
var questionTime=QUESTION_TIME;
var questionTimer=null;
var currentQuestion=null;
var usedQuestions={};
var lastType="";

var bestScore=
Number(
localStorage.getItem(BEST_KEY)||0
);


/* =====================================================
   수학 유틸
===================================================== */

function rand(min,max){

return Math.floor(
Math.random()*(max-min+1)
)+min;

}

function pick(arr){

return arr[
Math.floor(
Math.random()*arr.length
)
];

}

function shuffle(arr){

for(
var i=arr.length-1;
i>0;
i--
){

var j=
Math.floor(
Math.random()*(i+1)
);

var temp=
arr[i];

arr[i]=arr[j];
arr[j]=temp;

}

return arr;

}

function gcd(a,b){

a=Math.abs(a);
b=Math.abs(b);

while(b){
var t=a%b;
a=b;
b=t;
}

return a||1;

}

function comb(n,r){

if(r<0||r>n){
return 0;
}

r=Math.min(r,n-r);

var result=1;

for(var i=1;i<=r;i++){

result=
result*(n-r+i)/i;

}

return Math.round(result);

}

function equal(a,b){

if(
typeof a==="number"&&
typeof b==="number"
){

return Math.abs(a-b)<0.000001;

}

return String(a)===String(b);

}

function niceNumber(value){

if(typeof value!=="number"){
return String(value);
}

if(Math.abs(value-Math.round(value))<0.000001){
return String(Math.round(value));
}

return String(
Math.round(value*100)/100
);

}


/* =====================================================
   난이도
===================================================== */

function chooseDifficulty(){

var total=0;
var keys=Object.keys(difficulty);

keys.forEach(
function(key){
total+=difficulty[key].weight;
}
);

var r=Math.random()*total;

for(
var i=0;
i<keys.length;
i++
){

r-=difficulty[keys[i]].weight;

if(r<=0){
return keys[i];
}

}

return "high";

}

function chooseType(types){

var candidates=
types.filter(
function(type){
return type!==lastType;
}
);

if(!candidates.length){
candidates=types;
}

return pick(candidates);

}


/* =====================================================
   고등학교
===================================================== */

function highQuestion(){

var types=[
"quadratic",
"vertex",
"function",
"exponential",
"log",
"trig",
"sequence",
"probability",
"combination",
"permutation",
"triangle",
"pythagoras",
"distance",
"midpoint",
"circleArea",
"circleCircumference",
"sector",
"arc",
"circleEquation",
"chord",
"vector",
"derivative",
"tangent",
"integral"
];

var type=chooseType(types);


/* 이차방정식 */

if(type==="quadratic"){

var r1=rand(-9,9);
var r2=rand(-9,9);
var B=-(r1+r2);
var C=r1*r2;

return {
type:type,
question:
"x² "+
(B>=0?"+ "+B:"- "+Math.abs(B))+
"x "+
(C>=0?"+ "+C:"- "+Math.abs(C))+
"=0의 한 근은?",
answer:r1
};

}


/* 꼭짓점 */

if(type==="vertex"){

var a=pick([1,2,3,-1,-2]);
var h=rand(-6,6);
var k=rand(-8,8);
var b=-2*a*h;
var c=a*h*h+k;

return {
type:type,
question:
"f(x)="+
a+
"x² "+
(b>=0?"+ "+b:"- "+Math.abs(b))+
"x "+
(c>=0?"+ "+c:"- "+Math.abs(c))+
"의 꼭짓점의 x좌표는?",
answer:h
};

}


/* 함수 */

if(type==="function"){

var fa=rand(2,7);
var fb=rand(-7,7);
var fx=rand(-5,7);

return {
type:type,
question:
"f(x)="+
fa+
"x "+
(fb>=0?"+ "+fb:"- "+Math.abs(fb))+
"일 때 f("+
fx+
")는?",
answer:
fa*fx+fb
};

}


/* 지수 */

if(type==="exponential"){

var base=pick([2,3,5]);
var ea=rand(2,5);
var eb=rand(1,4);

return {
type:type,
question:
base+
"^"+
ea+
" × "+
base+
"^"+
eb+
" = ?",
answer:
Math.pow(base,ea+eb)
};

}


/* 로그 */

if(type==="log"){

var lb=pick([2,3,5]);
var le=rand(2,6);

return {
type:type,
question:
"log_"+
lb+
"("+
Math.pow(lb,le)+
") = ?",
answer:le
};

}


/* 삼각함수 */

if(type==="trig"){

var trig=pick([
{q:"sin 30°",a:.5},
{q:"cos 60°",a:.5},
{q:"sin 90°",a:1},
{q:"cos 0°",a:1},
{q:"tan 45°",a:1},
{q:"cos 120°",a:-.5}
]);

return {
type:type,
question:trig.q+" = ?",
answer:trig.a
};

}


/* 등차수열 */

if(type==="sequence"){

var first=rand(1,15);
var d=rand(2,8);
var n=rand(5,15);

return {
type:type,
question:
"등차수열의 첫째항이 "+
first+
", 공차가 "+
d+
"일 때 "+
n+
"번째 항은?",
answer:
first+(n-1)*d
};

}


/* 확률 */

if(type==="probability"){

var pn=rand(4,7);
var ps=rand(1,pn-1);

return {
type:type,
question:
"공정한 동전을 "+
pn+
"번 던질 때 앞면이 정확히 "+
ps+
"번 나올 확률은?",
answer:
comb(pn,ps)*Math.pow(.5,pn)
};

}


/* 조합 */

if(type==="combination"){

var cn=rand(7,12);
var cr=rand(2,cn-2);

return {
type:type,
question:
cn+
"C"+
cr+
"의 값은?",
answer:comb(cn,cr)
};

}


/* 순열 */

if(type==="permutation"){

var pn2=rand(5,9);
var pr=rand(2,4);
var pv=1;

for(var pi=0;pi<pr;pi++){
pv*=pn2-pi;
}

return {
type:type,
question:
pn2+
"P"+
pr+
"의 값은?",
answer:pv
};

}


/* 삼각형 넓이 */

if(type==="triangle"){

var base2=rand(5,20);
var height=rand(5,20);

return {
type:type,
question:
"밑변 "+
base2+
", 높이 "+
height+
"인 삼각형의 넓이는?",
answer:
base2*height/2
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

var tri=pick(triples);
var multi=rand(1,3);

return {
type:type,
question:
"직각삼각형의 두 직각변이 "+
tri[0]*multi+
", "+
tri[1]*multi+
"일 때 빗변의 길이는?",
answer:
tri[2]*multi
};

}


/* 거리 */

if(type==="distance"){

var x1=rand(-8,8);
var y1=rand(-8,8);
var x2=rand(-8,8);
var y2=rand(-8,8);

return {
type:type,
question:
"두 점 ("+
x1+
","+
y1+
"), ("+
x2+
","+
y2+
") 사이의 거리는?",
answer:
Math.sqrt(
Math.pow(x2-x1,2)+
Math.pow(y2-y1,2)
)
};

}


/* 중점 */

if(type==="midpoint"){

var mx1=rand(-10,10);
var mx2=rand(-10,10);

return {
type:type,
question:
"두 점 ("+
mx1+
",0), ("+
mx2+
",0)의 중점의 x좌표는?",
answer:
(mx1+mx2)/2
};

}


/* 원 넓이 */

if(type==="circleArea"){

var r1=rand(2,12);

return {
type:type,
question:
"반지름 "+
r1+
"인 원의 넓이는? (π로 나타내세요)",
answer:
(r1*r1)+"π"
};

}


/* 원 둘레 */

if(type==="circleCircumference"){

var r2=rand(2,12);

return {
type:type,
question:
"반지름 "+
r2+
"인 원의 둘레는? (π로 나타내세요)",
answer:
(2*r2)+"π"
};

}


/* 부채꼴 */

if(type==="sector"){

var rs=rand(3,10);
var angle=pick([30,45,60,90,120,180]);
var sc=rs*rs*angle/360;

return {
type:type,
question:
"반지름 "+
rs+
", 중심각 "+
angle+
"°인 부채꼴의 넓이는? (π로 나타내세요)",
answer:
niceNumber(sc)+"π"
};

}


/* 호 */

if(type==="arc"){

var rr=rand(3,10);
var arcAngle=pick([30,45,60,90,120,180]);
var ac=2*rr*arcAngle/360;

return {
type:type,
question:
"반지름 "+
rr+
", 중심각 "+
arcAngle+
"°인 호의 길이는? (π로 나타내세요)",
answer:
niceNumber(ac)+"π"
};

}


/* 원의 방정식 */

if(type==="circleEquation"){

var re=rand(2,10);

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


/* 현 */

if(type==="chord"){

var chordR=rand(5,12);
var chordD=rand(1,chordR-2);

return {
type:type,
question:
"반지름이 "+
chordR+
"인 원에서 중심에서 현까지의 거리가 "+
chordD+
"일 때 현의 길이는?",
answer:
2*Math.sqrt(
chordR*chordR-
chordD*chordD
)
};

}


/* 벡터 내적 */

if(type==="vector"){

var va=rand(1,9);
var vb=rand(1,9);
var vc=rand(1,9);
var vd=rand(1,9);

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


/* 미분 */

if(type==="derivative"){

var da=rand(2,7);
var dn=rand(2,6);
var dx=rand(1,6);

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
Math.pow(dx,dn-1)
};

}


/* 접선 */

if(type==="tangent"){

var ta=rand(2,7);
var tx=rand(1,6);

return {
type:type,
question:
"f(x)="+
ta+
"x²일 때 x="+
tx+
"에서 접선의 기울기는?",
answer:
2*ta*tx
};

}


/* 적분 */

var ia=rand(2,8);
var ix=rand(2,6);

return {
type:"integral",
question:
"∫₀^"+
ix+
" "+
ia+
"x dx = ?",
answer:
ia*ix*ix/2
};

}


/* =====================================================
   대학
===================================================== */

function universityQuestion(){

var types=[
"integral",
"derivative",
"limit",
"det",
"trace",
"vector",
"complex",
"expectation",
"circle"
];

var type=chooseType(types);

if(type==="integral"){

var n=rand(2,8);

return {
type:type,
question:
"∫₀^"+
n+
"x² dx = ?",
answer:n*n*n/3
};

}

if(type==="derivative"){

var a=rand(2,8);
var p=rand(2,5);
var x=rand(1,6);

return {
type:type,
question:
"f(x)="+
a+
"x^"+
p+
"일 때 f'("+
x+
")는?",
answer:
a*p*Math.pow(x,p-1)
};

}

if(type==="limit"){

var la=rand(2,9);
var lb=rand(1,9);
var lx=rand(1,7);

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
la*lx+lb
};

}

if(type==="det"){

var a1=rand(1,8);
var b1=rand(1,8);
var c1=rand(1,8);
var d1=rand(1,8);

return {
type:type,
question:
"det [["+
a1+
","+
b1+
"],["+
c1+
","+
d1+
"]] = ?",
answer:
a1*d1-b1*c1
};

}

if(type==="trace"){

var tr1=rand(1,9);
var tr2=rand(1,9);

return {
type:type,
question:
"행렬 [["+
tr1+
",0],[0,"+
tr2+
"]]의 trace는?",
answer:tr1+tr2
};

}

if(type==="vector"){

var x1=rand(1,8);
var y1=rand(1,8);
var x2=rand(1,8);
var y2=rand(1,8);

return {
type:type,
question:
"("+
x1+
","+
y1+
")·("+
x2+
","+
y2+
") = ?",
answer:
x1*x2+y1*y2
};

}

if(type==="complex"){

var ca=rand(1,8);
var cb=rand(1,8);

return {
type:type,
question:
"z="+
ca+
"+"+
cb+
"i일 때 |z|²는?",
answer:
ca*ca+cb*cb
};

}

if(type==="expectation"){

var ex1=rand(1,5);
var ex2=rand(6,10);
var pr=pick([.2,.3,.4,.6,.7,.8]);

return {
type:type,
question:
"X가 "+
ex1+
"을 확률 "+
pr+
", "+
ex2+
"를 확률 "+
(1-pr)+
"로 가질 때 E[X]는?",
answer:
pr*ex1+(1-pr)*ex2
};

}

var cr=rand(3,10);

return {
type:"circle",
question:
"반지름 "+
cr+
"인 원의 넓이는? (π로 나타내세요)",
answer:
(cr*cr)+"π"
};

}


/* =====================================================
   대학 심화
===================================================== */

function hardQuestion(){

var types=[
"hIntegral",
"hChain",
"hMatrix",
"hComplex",
"hSeries",
"hCross",
"hCircle"
];

var type=chooseType(types);

if(type==="hIntegral"){

var a=rand(1,7);

return {
type:type,
question:
"∫₀^π "+
a+
"sin(x) dx = ?",
answer:
2*a
};

}

if(type==="hChain"){

var a2=rand(2,7);
var x2=rand(1,5);
var inner=a2*x2*x2+1;

return {
type:type,
question:
"f(x)=("+
a2+
"x²+1)³일 때 x="+
x2+
"에서 f'(x)는?",
answer:
6*a2*x2*inner*inner
};

}

if(type==="hMatrix"){

var m1=rand(1,5);
var m2=rand(1,5);
var m3=rand(1,5);

return {
type:type,
question:
"diag("+
m1+
","+
m2+
","+
m3+
")의 행렬식은?",
answer:
m1*m2*m3
};

}

if(type==="hComplex"){

var hz=rand(1,9);

return {
type:type,
question:
"z="+
hz+
"i일 때 z²는?",
answer:
-hz*hz
};

}

if(type==="hSeries"){

var sf=rand(1,5);
var sr=pick([2,3]);
var sn=rand(3,7);

return {
type:type,
question:
"첫째항 "+
sf+
", 공비 "+
sr+
"인 등비수열의 첫 "+
sn+
"개 항의 합은?",
answer:
sf*
(Math.pow(sr,sn)-1)/
(sr-1)
};

}

if(type==="hCross"){

var xa=rand(2,7);
var xb=rand(2,7);

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

var hc=rand(3,9);
var ha=pick([30,45,60,90,120]);

return {
type:"hCircle",
question:
"반지름 "+
hc+
", 중심각 "+
ha+
"°인 부채꼴의 넓이는? (π로 나타내세요)",
answer:
niceNumber(
hc*hc*ha/360
)+"π"
};

}


/* =====================================================
   문제 생성
===================================================== */

function createQuestion(){

var count=0;

while(count<1000){

count++;

var level=chooseDifficulty();
var q;

if(level==="high"){
q=highQuestion();
}else if(level==="university"){
q=universityQuestion();
}else{
q=hardQuestion();
}

if(q.type===lastType){
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

if(usedQuestions[key]){
continue;
}

usedQuestions[key]=true;
lastType=q.type;
q.level=level;

return q;

}

return {
level:"high",
type:"fallback",
question:"x² - 7x + 12 = 0의 한 근은?",
answer:3
};

}


/* =====================================================
   비슷한 5지선다
===================================================== */

function makeChoices(answer){

if(
typeof answer==="string" &&
answer.indexOf("π")!==-1
){

var coeff=
parseFloat(
answer.replace("π","")
);

var step=
Math.abs(coeff)>=20
?
.5
:
.25;

var result=[
answer
];

[
-step*2,
-step,
step,
step*2
].forEach(
function(offset){

var value=
coeff+offset;

if(value>0){

var text=
niceNumber(value)+"π";

if(result.indexOf(text)===-1){
result.push(text);
}

}

}
);

while(result.length<5){

var v=
coeff+
(result.length%2===0?1:-1)*
step*3;

var t=
niceNumber(v)+"π";

if(
v>0&&
result.indexOf(t)===-1
){

result.push(t);

}else{

break;

}

}

while(result.length<5){

result.push(
niceNumber(
coeff+
(result.length*.25)
)+"π"
);

}

return shuffle(result);

}


if(
typeof answer==="string" &&
answer.indexOf("x²+y²=")===0
){

var n=
Number(
answer.split("=")[1]
);

return shuffle([
answer,
"x²+y²="+Math.max(1,n-2),
"x²+y²="+Math.max(1,n-1),
"x²+y²="+(n+1),
"x²+y²="+(n+2)
]);

}


if(
typeof answer==="number" &&
Number.isFinite(answer)
){

var result2=[
answer
];

var abs=
Math.abs(answer);

var step2;

if(abs<5){
step2=.25;
}else if(abs<20){
step2=.5;
}else if(abs<100){
step2=1;
}else if(abs<500){
step2=2;
}else if(abs<2000){
step2=5;
}else{
step2=Math.max(
10,
Math.round(abs*.01)
);
}

[
-step2*2,
-step2,
step2,
step2*2
].forEach(
function(offset){

var value=
answer+offset;

if(
!Number.isInteger(answer)
){

value=
Math.round(value*100)/100;

}

if(
result2.every(
function(item){
return !equal(item,value);
}
)
){

result2.push(value);

}

}
);

var tiny=
step2/2;

while(result2.length<5){

var value2=
answer+
(result2.length%2===0?1:-1)*
tiny;

if(!Number.isInteger(answer)){
value2=
Math.round(value2*100)/100;
}

if(
result2.every(
function(item){
return !equal(item,value2);
}
)
){

result2.push(value2);

}else{

tiny+=step2/2;

}

}

return shuffle(result2);

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
   게임 상태
===================================================== */

function renderGameStatus(){

document.getElementById("gameScore").textContent=
gameScore;

document.getElementById("questionTime").textContent=
questionTime;

document.getElementById("gameSolved").textContent=
gameSolved;

document.getElementById("wrongStreak").textContent=
wrongStreak+
" / "+
MAX_WRONG;

}


/* =====================================================
   문제 출력
===================================================== */

function showQuestion(){

if(!gameRunning){
return;
}

currentQuestion=
createQuestion();

var config=
difficulty[
currentQuestion.level
];

document.getElementById("difficulty")
.textContent=
config.label+
" · 정답 +"+
config.score+
"점";

document.getElementById("question")
.textContent=
currentQuestion.question;

var choices=
makeChoices(
currentQuestion.answer
);

currentQuestion.choices=
choices;

var box=
document.getElementById("choices");

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
document.createElement("button");

button.className=
"choice-btn";

button.textContent=
labels[index]+
" "+
niceNumber(choice);

button.onclick=
function(){
answerQuestion(index,button);
};

box.appendChild(button);

}
);

document.getElementById("gameMessage")
.textContent=
"정답을 선택하세요.";

startQuestionTimer();

}


/* =====================================================
   문제 타이머
===================================================== */

function startQuestionTimer(){

if(questionTimer){
clearInterval(questionTimer);
}

questionTime=
QUESTION_TIME;

renderGameStatus();

document.getElementById(
"questionTimerBar"
).style.width="100%";

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

if(questionTime<=0){

clearInterval(questionTimer);
questionTimer=null;

questionTimeout();

}

},
1000
);

}


/* =====================================================
   시간 초과
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
wrongStreak>=MAX_WRONG
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
MAX_WRONG;

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
   답 처리
===================================================== */

function answerQuestion(index,button){

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
function(item){
item.disabled=true;
}
);

var selected=
currentQuestion.choices[index];

var correct=
equal(
selected,
currentQuestion.answer
);

if(correct){

button.classList.add("correct");

gameScore+=
difficulty[
currentQuestion.level
].score;

gameSolved++;

wrongStreak=0;

document.getElementById(
"gameMessage"
).textContent=
"✅ 정답!";

}else{

button.classList.add("wrong");

wrongStreak++;

document.getElementById(
"gameMessage"
).textContent=
"❌ 오답! 연속 오답 "+
wrongStreak+
"/"+
MAX_WRONG;

}

renderGameStatus();

if(
wrongStreak>=MAX_WRONG
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
gameSolved=0;
wrongStreak=0;
questionTime=QUESTION_TIME;
currentQuestion=null;
usedQuestions={};
lastType="";

document.getElementById(
"gameNickname"
).disabled=true;

document.getElementById(
"startGameBtn"
).disabled=true;

document.getElementById(
"startGameBtn"
).textContent=
"게임 중...";

document.getElementById(
"result"
).classList.remove("show");

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

clearInterval(questionTimer);
questionTimer=null;

}

document.querySelectorAll(
".choice-btn"
).forEach(
function(button){
button.disabled=true;
}
);

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
wrongStreak>=MAX_WRONG
?
"5번 연속 오답"
:
"게임 종료";

document.getElementById(
"gameMessage"
).textContent=
"게임 종료 · "+
reason;

if(
gameScore>
bestScore
){

bestScore=
gameScore;

localStorage.setItem(
BEST_KEY,
String(bestScore)
);

}

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

document.getElementById(
"result"
).classList.add("show");

saveRanking(
nickname,
gameScore
);

}


/* =====================================================
   랭킹
===================================================== */

function getRanking(){

var data=
readData(
RANKING_KEY,
[]
);

if(!Array.isArray(data)){
return [];
}

return data;

}

function saveRanking(name,score){

var ranking=
getRanking();

ranking.push({
name:name,
score:score,
time:Date.now()
});

ranking.sort(
function(a,b){

if(b.score!==a.score){
return b.score-a.score;
}

return a.time-b.time;

}
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

var body=
document.getElementById(
"rankingBody"
);

if(!body){
return;
}

var ranking=
getRanking();

if(!ranking.length){

body.innerHTML=
"<tr><td colspan=\"3\">아직 기록이 없습니다.</td></tr>";

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

render();
renderRanking();
restorePage();

</script>

</body>
</html>
