<html lang="ko">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>대광고등학교 큰빛축제 방문록</title>

<style>
*{box-sizing:border-box}
html,body{margin:0;padding:0}

body{
 font-family:"Malgun Gothic","Noto Sans KR",sans-serif;
 background:#f7eef1;
 color:#24151b;
 user-select:none;
 overflow-x:hidden;
 position:relative;
}

input,textarea,button{font:inherit}

.hero{
 background:linear-gradient(135deg,#64152f,#8f2948);
 color:#fff;
 padding:28px 18px 34px;
 box-shadow:0 4px 16px #0002;
 position:relative;
 z-index:2;
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
 z-index:2;
}

.panel{
 background:#fff;
 border-radius:18px;
 padding:20px;
 box-shadow:0 4px 18px #6d203714;
 margin-bottom:20px;
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
 user-select:text;
 background:#fff;
}

textarea{
 min-height:105px;
 resize:vertical;
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

.modal{
 position:fixed;
 inset:0;
 background:#2b0d1799;
 display:none;
 align-items:center;
 justify-content:center;
 padding:18px;
 z-index:10;
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

footer{
 text-align:center;
 color:#806d76;
 font-size:12px;
 padding:8px 20px 30px;
}

.master{
 margin-top:10px;
 padding:12px;
 background:#fff5e8;
 border:1px solid #ecd39c;
 border-radius:10px;
 font-size:13px;
 color:#77551b;
}

/* 좋아요 */
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
 cursor:pointer;
 transition:.15s;
}

.like-btn:hover{
 background:#faedf1;
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
 cursor:pointer;
}

.cancel-like:disabled{
 background:#f3f1f2;
 color:#aaa0a5;
 cursor:not-allowed;
}

/* ==========================================
   외부 배경 대광고 로고 애니메이션
   ========================================== */

.bg-logo{
 position:fixed;
 width:130px;
 height:130px;
 border-radius:50%;
 border:5px solid #8a2947;
 color:#8a2947;
 background:rgba(255,255,255,.22);
 display:flex;
 align-items:center;
 justify-content:center;
 text-align:center;
 font-weight:900;
 font-size:34px;
 line-height:1;
 opacity:.075;
 filter:blur(1px);
 pointer-events:none;
 z-index:0;
 box-shadow:0 0 35px rgba(116,27,56,.12);
}

.bg-logo::after{
 content:"DAE KWANG";
 position:absolute;
 left:50%;
 top:67%;
 transform:translate(-50%,-50%);
 font-size:10px;
 letter-spacing:2px;
 white-space:nowrap;
 font-weight:700;
}

.bg-logo-1{
 top:12%;
 left:-35px;
 animation:floatLogo1 18s ease-in-out infinite alternate;
}

.bg-logo-2{
 top:47%;
 right:-40px;
 width:170px;
 height:170px;
 font-size:42px;
 animation:floatLogo2 22s ease-in-out infinite alternate;
}

.bg-logo-3{
 top:78%;
 left:18%;
 width:100px;
 height:100px;
 font-size:27px;
 animation:floatLogo3 20s ease-in-out infinite alternate;
}

.bg-logo-4{
 top:68%;
 right:20%;
 width:115px;
 height:115px;
 font-size:29px;
 animation:floatLogo4 25s ease-in-out infinite alternate;
}

@keyframes floatLogo1{
 0%{transform:translate(0,0) rotate(-8deg)}
 50%{transform:translate(90px,45px) rotate(7deg)}
 100%{transform:translate(25px,110px) rotate(-5deg)}
}

@keyframes floatLogo2{
 0%{transform:translate(0,0) rotate(8deg)}
 50%{transform:translate(-100px,-55px) rotate(-6deg)}
 100%{transform:translate(-45px,70px) rotate(5deg)}
}

@keyframes floatLogo3{
 0%{transform:translate(0,0) rotate(5deg)}
 50%{transform:translate(65px,-40px) rotate(-8deg)}
 100%{transform:translate(-35px,-90px) rotate(4deg)}
}

@keyframes floatLogo4{
 0%{transform:translate(0,0) rotate(-6deg)}
 50%{transform:translate(-75px,35px) rotate(8deg)}
 100%{transform:translate(40px,-55px) rotate(-4deg)}
}

@media(max-width:650px){

 .grid{
  grid-template-columns:1fr;
 }

 .full{
  grid-column:auto;
 }

 h1{
  font-size:23px;
 }

 .logo{
  width:65px;
  height:65px;
 }

 .like-area{
  width:100%;
 }

 .bg-logo{
  opacity:.055;
 }

 .bg-logo-1{
  left:-55px;
 }

 .bg-logo-2{
  right:-70px;
 }

 .bg-logo-3{
  left:-20px;
 }

 .bg-logo-4{
  right:-20px;
 }
}
</style>

</head>

<body>

<!-- ==========================================
     외부 배경 애니메이션
========================================== -->

<div class="bg-logo bg-logo-1">大光</div>
<div class="bg-logo bg-logo-2">大光</div>
<div class="bg-logo bg-logo-3">大光</div>
<div class="bg-logo bg-logo-4">大光</div>

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
<div class="sub">우리들의 축제, 우리들의 기록 · 큰빛축제 방문록</div>
</div>

</div>

</header>

<main>

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

<div id="modal" class="modal">

<div class="modal-card">

<h3 id="modalTitle">비밀번호 확인</h3>

<input id="checkPw" type="password" placeholder="비밀번호">

<div id="pwError" class="error"></div>

<div class="actions">

<button class="secondary" onclick="closeModal()">
취소
</button>

<button onclick="confirmPassword()">
확인
</button>

</div>

</div>

</div>

<script>

/* ================================
   기본 설정
================================ */

const STORAGE_KEY =
"daekwang_bigbit_festival_guestbook_v2";

const LIKE_KEY =
"daekwang_bigbit_festival_likes_v3";

const MASTER_PASSWORD =
"20100806";

const LIKE_CANCEL_DELAY =
7000;

let entries =
JSON.parse(
 localStorage.getItem(STORAGE_KEY) || "[]"
);

let likes =
JSON.parse(
 localStorage.getItem(LIKE_KEY) || "{}"
);

let pending=null;


/* ================================
   저장
================================ */

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


/* ================================
   HTML 특수문자 처리
================================ */

function escapeHTML(s){

 return String(s).replace(
  /[&<>"']/g,
  c=>({
   "&":"&amp;",
   "<":"&lt;",
   ">":"&gt;",
   '"':"&quot;",
   "'":"&#039;"
  }[c])
 );

}


/* ================================
   날짜
================================ */

function formatDate(iso){

 const d=new Date(iso);

 const p=n =>
 String(n).padStart(2,"0");

 return `${d.getFullYear()}년 ${p(d.getMonth()+1)}월 ${p(d.getDate())}일 ${p(d.getHours())}시 ${p(d.getMinutes())}분 ${p(d.getSeconds())}초`;

}


/* ================================
   방문록 등록
================================ */

function addEntry(){

 const name =
 document.getElementById("name")
 .value.trim();

 const pw =
 document.getElementById("password")
 .value;

 const message =
 document.getElementById("message")
 .value.trim();


 if(!name || !pw || !message){

  alert(
   "이름(닉네임), 비밀번호, 내용을 모두 입력해주세요."
  );

  return;

 }


 const id =
 crypto.randomUUID
 ?
 crypto.randomUUID()
 :
 String(Date.now()+Math.random());


 entries.unshift({

  id:id,

  name:name,

  message:message,

  password:pw,

  createdAt:new Date().toISOString()

 });


 save();

 render();


 document.getElementById("name").value="";
 document.getElementById("password").value="";
 document.getElementById("message").value="";

}


/* ================================
   좋아요 데이터 형식
================================ */

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


/* ================================
   좋아요 추가
   누를 때마다 +1
================================ */

function addLike(id){

 const data =
 normalizeLikes(id);

 data.count++;

 data.times.push(
  Date.now()
 );

 saveLikes();

 render();

}


/* ================================
   취소 가능한 좋아요 찾기
================================ */

function getCancelableIndex(id){

 const data =
 likes[id];

 if(
  !data ||
  !Array.isArray(data.times)
 ){

  return -1;

 }

 const now=Date.now();

 return data.times.findIndex(
  time =>
  now-time >= LIKE_CANCEL_DELAY
 );

}


/* ================================
   좋아요 취소
================================ */

function cancelLike(id){

 const data =
 likes[id];

 if(
  !data ||
  !Array.isArray(data.times)
 ){

  return;

 }


 const index =
 getCancelableIndex(id);


 if(index===-1){

  alert(
   "좋아요를 누른 후 7초가 지나야 취소할 수 있습니다."
  );

  return;

 }


 data.times.splice(index,1);

 data.count--;

 if(data.count<0){
  data.count=0;
 }

 saveLikes();

 render();

}


/* ================================
   취소 버튼 글자
================================ */

function getCancelText(id){

 const data =
 likes[id];

 if(
  !data ||
  !data.times ||
  !data.times.length
 ){

  return "좋아요 취소";

 }


 const now=Date.now();


 const canCancel =
 data.times.some(
  time =>
  now-time>=LIKE_CANCEL_DELAY
 );


 if(canCancel){

  return "좋아요 취소";

 }


 const earliest =
 Math.min(...data.times);


 const remain =
 Math.max(
  0,
  Math.ceil(
   (LIKE_CANCEL_DELAY-(now-earliest))/1000
  )
 );


 return `${remain}초 후 취소`;

}


/* ================================
   방문록 출력
================================ */

function render(){

 const box =
 document.getElementById("entries");


 document.getElementById("count")
 .textContent =
 `${entries.length}개`;


 if(!entries.length){

  box.innerHTML=
  `
  <div class="empty">
  아직 등록된 방문록이 없습니다.<br>
  첫 번째 기록을 남겨보세요!
  </div>
  `;

  return;

 }


 box.innerHTML =
 entries.map(e=>{

  const data =
  normalizeLikes(e.id);

  const cancelAvailable =
  getCancelableIndex(e.id)!==-1;

  const cancelText =
  getCancelText(e.id);


  return `

  <article class="entry">

   <div class="entry-head">

    <div class="name">
    ${escapeHTML(e.name)}
    </div>

    <div class="time">
    작성: ${formatDate(e.createdAt)}
    ${
     e.updatedAt
     ?
     `<br>수정: ${formatDate(e.updatedAt)}`
     :
     ""
    }
    </div>

   </div>


   <div class="content">
   ${escapeHTML(e.message)}
   </div>


   <div class="actions">

    <div class="like-area">

     <button
      class="like-btn"
      onclick="addLike('${e.id}')"
     >
      ❤️ 좋아요
     </button>

     <span class="like-count">
      ${data.count}
     </span>

     <button
      class="cancel-like"
      onclick="cancelLike('${e.id}')"
      ${cancelAvailable ? "" : "disabled"}
     >
      ${cancelText}
     </button>

    </div>


    <button
     class="secondary"
     onclick="requestAction('edit','${e.id}')"
    >
    수정
    </button>


    <button
     class="danger"
     onclick="requestAction('delete','${e.id}')"
    >
    삭제
    </button>

   </div>

  </article>

  `;

 }).join("");

}


/* ================================
   수정 / 삭제 요청
================================ */

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
  ()=>{
   document
   .getElementById("checkPw")
   .focus();
  },
  50
 );

}


/* ================================
   모달 닫기
================================ */

function closeModal(){

 pending=null;

 document
 .getElementById("modal")
 .classList
 .remove("show");

}


/* ================================
   비밀번호 확인
================================ */

function confirmPassword(){

 if(!pending)return;


 const e =
 entries.find(
  x=>x.id===pending.id
 );


 const pw =
 document
 .getElementById("checkPw")
 .value;


 if(
  !e ||
  !(pw===e.password ||
    pw===MASTER_PASSWORD)
 ){

  document
  .getElementById("pwError")
  .textContent =
  "비밀번호가 올바르지 않습니다.";

  return;

 }


 const action =
 pending.action;

 const id =
 pending.id;


 closeModal();


 if(action==="delete"){

  if(
   confirm(
    "이 방문록을 삭제할까요?"
   )
  ){

   entries =
   entries.filter(
    x=>x.id!==id
   );

   delete likes[id];

   save();

   saveLikes();

   render();

  }

 }


 else{

  const target =
  entries.find(
   x=>x.id===id
  );


  const newName =
  prompt(
   "이름 또는 닉네임",
   target.name
  );

  if(newName===null)return;


  const newMessage =
  prompt(
   "방문록 내용",
   target.message
  );

  if(newMessage===null)return;


  if(
   !newName.trim() ||
   !newMessage.trim()
  ){

   alert(
    "내용을 비워둘 수 없습니다."
   );

   return;

  }


  target.name =
  newName.trim();

  target.message =
  newMessage.trim();

  target.updatedAt =
  new Date().toISOString();


  save();

  render();

 }

}


/* ================================
   모달 바깥 클릭
================================ */

document
.getElementById("modal")
.addEventListener(
 "click",
 e=>{

  if(e.target.id==="modal"){

   closeModal();

  }

 }
);


/* ================================
   ESC
================================ */

document.addEventListener(
 "keydown",
 e=>{

  if(e.key==="Escape"){

   closeModal();

  }

 }
);


/* ================================
   좋아요 타이머
================================ */

setInterval(
 ()=>{
  render();
 },
 1000
);


/* ================================
   시작
================================ */

render();

</script>

</body>
</html>
```
