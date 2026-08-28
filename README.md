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
   움직이는 배경 교표
========================= */

.logo-float{
 position:fixed;
 left:0;
 top:0;
 width:64px;
 height:64px;
 z-index:0;
 pointer-events:none;
 opacity:.11;
 filter:blur(.15px);
 will-change:transform;
}

.logo-float-1{animation:move1 17s linear infinite}
.logo-float-2{width:56px;height:56px;animation:move2 20s linear infinite}
.logo-float-3{width:48px;height:48px;animation:move3 18s linear infinite}
.logo-float-4{width:60px;height:60px;animation:move4 21s linear infinite}
.logo-float-5{width:52px;height:52px;animation:move5 16s linear infinite}
.logo-float-6{width:68px;height:68px;animation:move6 23s linear infinite}
.logo-float-7{width:50px;height:50px;animation:move7 19s linear infinite}
.logo-float-8{width:58px;height:58px;animation:move8 22s linear infinite}
.logo-float-9{width:44px;height:44px;animation:move9 17s linear infinite}
.logo-float-10{width:62px;height:62px;animation:move10 24s linear infinite}
.logo-float-11{width:54px;height:54px;animation:move11 20s linear infinite}
.logo-float-12{width:46px;height:46px;animation:move12 18s linear infinite}

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

/* =========================
   공통
========================= */

main{
 max-width:1050px;
 margin:24px auto;
 padding:0 14px;
 position:relative;
 z-index:2;
}

.page{
 display:none;
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

/* =========================
   메뉴
========================= */

.menu-wrap{
 min-height:calc(100vh - 150px);
 display:flex;
 align-items:center;
 justify-content:center;
 padding:25px 0 40px;
}

.menu{
 width:min(760px,100%);
}

.menu-title{
 text-align:center;
 margin-bottom:28px;
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
}

.menu-card{
 background:#fff;
 border:1px solid #ead6dc;
 border-radius:22px;
 padding:32px 20px;
 text-align:center;
 box-shadow:0 6px 22px #6d203714;
 cursor:pointer;
 transition:.2s;
}

.menu-card:hover{
 transform:translateY(-5px);
 box-shadow:0 10px 28px #6d203725;
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
 cursor:pointer;
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
 z-index:20;
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

/* =========================
   수학게임
========================= */

.game-box{
 background:#fff;
 border-radius:18px;
 padding:20px;
 box-shadow:0 4px 18px #6d203714;
 margin-bottom:20px;
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
 grid-template-columns:repeat(5,1fr);
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
 min-height:110px;
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

 .menu-grid{
  grid-template-columns:1fr;
 }

 .menu-title h2{
  font-size:26px;
 }

 .game-status{
  grid-template-columns:1fr 1fr;
 }

 .choices{
  grid-template-columns:1fr;
 }

 .question{
  font-size:21px;
 }

 .nickname-row{
  flex-direction:column;
 }

 .logo-float{
  opacity:.08;
 }
}
</style>

</head>

<body>

<!-- =========================
     배경 로고
========================= -->

<div class="logo-float logo-float-1">
<svg viewBox="0 0 200 200" width="100%" height="100%" xmlns="http://www.w3.org/2000/svg">
<circle cx="100" cy="100" r="94" fill="#8a2340"/>
<circle cx="100" cy="100" r="76" fill="none" stroke="#fff" stroke-width="8"/>
<path d="M58 63 Q100 42 142 63 L136 118 Q132 146 100 163 Q68 146 64 118 Z" fill="#8a2340" stroke="#fff" stroke-width="3"/>
<path d="M74 72 L88 61 L100 72 L112 61 L126 72 L126 83 L74 83 Z" fill="#fff"/>
<text x="100" y="101" text-anchor="middle" fill="#fff" font-family="Georgia" font-size="13" font-weight="700">LUX ET SAL</text>
<text x="100" y="128" text-anchor="middle" fill="#fff" font-family="serif" font-size="27" font-weight="700">大光</text>
<text x="100" y="28" text-anchor="middle" fill="#fff" font-family="Georgia" font-size="9" font-weight="700">DAE GWANG HIGH SCHOOL</text>
<text x="100" y="185" text-anchor="middle" fill="#fff" font-family="serif" font-size="9" font-weight="700">대 광 고 등 학 교</text>
</svg>
</div>

<div class="logo-float logo-float-2">
<svg viewBox="0 0 200 200" width="100%" height="100%" xmlns="http://www.w3.org/2000/svg">
<circle cx="100" cy="100" r="94" fill="#8a2340"/>
<circle cx="100" cy="100" r="76" fill="none" stroke="#fff" stroke-width="8"/>
<path d="M58 63 Q100 42 142 63 L136 118 Q132 146 100 163 Q68 146 64 118 Z" fill="#8a2340" stroke="#fff" stroke-width="3"/>
<path d="M74 72 L88 61 L100 72 L112 61 L126 72 L126 83 L74 83 Z" fill="#fff"/>
<text x="100" y="101" text-anchor="middle" fill="#fff" font-family="Georgia" font-size="13" font-weight="700">LUX ET SAL</text>
<text x="100" y="128" text-anchor="middle" fill="#fff" font-family="serif" font-size="27" font-weight="700">大光</text>
<text x="100" y="28" text-anchor="middle" fill="#fff" font-family="Georgia" font-size="9" font-weight="700">DAE GWANG HIGH SCHOOL</text>
<text x="100" y="185" text-anchor="middle" fill="#fff" font-family="serif" font-size="9" font-weight="700">대 광 고 등 학 교</text>
</svg>
</div>

<div class="logo-float logo-float-3">
<svg viewBox="0 0 200 200" width="100%" height="100%" xmlns="http://www.w3.org/2000/svg">
<circle cx="100" cy="100" r="94" fill="#8a2340"/>
<circle cx="100" cy="100" r="76" fill="none" stroke="#fff" stroke-width="8"/>
<path d="M58 63 Q100 42 142 63 L136 118 Q132 146 100 163 Q68 146 64 118 Z" fill="#8a2340" stroke="#fff" stroke-width="3"/>
<path d="M74 72 L88 61 L100 72 L112 61 L126 72 L126 83 L74 83 Z" fill="#fff"/>
<text x="100" y="101" text-anchor="middle" fill="#fff" font-family="Georgia" font-size="13" font-weight="700">LUX ET SAL</text>
<text x="100" y="128" text-anchor="middle" fill="#fff" font-family="serif" font-size="27" font-weight="700">大光</text>
<text x="100" y="28" text-anchor="middle" fill="#fff" font-family="Georgia" font-size="9" font-weight="700">DAE GWANG HIGH SCHOOL</text>
<text x="100" y="185" text-anchor="middle" fill="#fff" font-family="serif" font-size="9" font-weight="700">대 광 고 등 학 교</text>
</svg>
</div>

<div class="logo-float logo-float-4">
<svg viewBox="0 0 200 200" width="100%" height="100%" xmlns="http://www.w3.org/2000/svg">
<circle cx="100" cy="100" r="94" fill="#8a2340"/>
<circle cx="100" cy="100" r="76" fill="none" stroke="#fff" stroke-width="8"/>
<path d="M58 63 Q100 42 142 63 L136 118 Q132 146 100 163 Q68 146 64 118 Z" fill="#8a2340" stroke="#fff" stroke-width="3"/>
<path d="M74 72 L88 61 L100 72 L112 61 L126 72 L126 83 L74 83 Z" fill="#fff"/>
<text x="100" y="101" text-anchor="middle" fill="#fff" font-family="Georgia" font-size="13" font-weight="700">LUX ET SAL</text>
<text x="100" y="128" text-anchor="middle" fill="#fff" font-family="serif" font-size="27" font-weight="700">大光</text>
<text x="100" y="28" text-anchor="middle" fill="#fff" font-family="Georgia" font-size="9" font-weight="700">DAE GWANG HIGH SCHOOL</text>
<text x="100" y="185" text-anchor="middle" fill="#fff" font-family="serif" font-size="9" font-weight="700">대 광 고 등 학 교</text>
</svg>
</div>

<div class="logo-float logo-float-5">
<svg viewBox="0 0 200 200" width="100%" height="100%" xmlns="http://www.w3.org/2000/svg">
<circle cx="100" cy="100" r="94" fill="#8a2340"/>
<circle cx="100" cy="100" r="76" fill="none" stroke="#fff" stroke-width="8"/>
<path d="M58 63 Q100 42 142 63 L136 118 Q132 146 100 163 Q68 146 64 118 Z" fill="#8a2340" stroke="#fff" stroke-width="3"/>
<path d="M74 72 L88 61 L100 72 L112 61 L126 72 L126 83 L74 83 Z" fill="#fff"/>
<text x="100" y="101" text-anchor="middle" fill="#fff" font-family="Georgia" font-size="13" font-weight="700">LUX ET SAL</text>
<text x="100" y="128" text-anchor="middle" fill="#fff" font-family="serif" font-size="27" font-weight="700">大光</text>
<text x="100" y="28" text-anchor="middle" fill="#fff" font-family="Georgia" font-size="9" font-weight="700">DAE GWANG HIGH SCHOOL</text>
<text x="100" y="185" text-anchor="middle" fill="#fff" font-family="serif" font-size="9" font-weight="700">대 광 고 등 학 교</text>
</svg>
</div>

<div class="logo-float logo-float-6">
<svg viewBox="0 0 200 200" width="100%" height="100%" xmlns="http://www.w3.org/2000/svg">
<circle cx="100" cy="100" r="94" fill="#8a2340"/>
<circle cx="100" cy="100" r="76" fill="none" stroke="#fff" stroke-width="8"/>
<path d="M58 63 Q100 42 142 63 L136 118 Q132 146 100 163 Q68 146 64 118 Z" fill="#8a2340" stroke="#fff" stroke-width="3"/>
<path d="M74 72 L88 61 L100 72 L112 61 L126 72 L126 83 L74 83 Z" fill="#fff"/>
<text x="100" y="101" text-anchor="middle" fill="#fff" font-family="Georgia" font-size="13" font-weight="700">LUX ET SAL</text>
<text x="100" y="128" text-anchor="middle" fill="#fff" font-family="serif" font-size="27" font-weight="700">大光</text>
<text x="100" y="28" text-anchor="middle" fill="#fff" font-family="Georgia" font-size="9" font-weight="700">DAE GWANG HIGH SCHOOL</text>
<text x="100" y="185" text-anchor="middle" fill="#fff" font-family="serif" font-size="9" font-weight="700">대 광 고 등 학 교</text>
</svg>
</div>

<div class="logo-float logo-float-7">
<svg viewBox="0 0 200 200" width="100%" height="100%" xmlns="http://www.w3.org/2000/svg">
<circle cx="100" cy="100" r="94" fill="#8a2340"/>
<circle cx="100" cy="100" r="76" fill="none" stroke="#fff" stroke-width="8"/>
<path d="M58 63 Q100 42 142 63 L136 118 Q132 146 100 163 Q68 146 64 118 Z" fill="#8a2340" stroke="#fff" stroke-width="3"/>
<path d="M74 72 L88 61 L100 72 L112 61 L126 72 L126 83 L74 83 Z" fill="#fff"/>
<text x="100" y="101" text-anchor="middle" fill="#fff" font-family="Georgia" font-size="13" font-weight="700">LUX ET SAL</text>
<text x="100" y="128" text-anchor="middle" fill="#fff" font-family="serif" font-size="27" font-weight="700">大光</text>
<text x="100" y="28" text-anchor="middle" fill="#fff" font-family="Georgia" font-size="9" font-weight="700">DAE GWANG HIGH SCHOOL</text>
<text x="100" y="185" text-anchor="middle" fill="#fff" font-family="serif" font-size="9" font-weight="700">대 광 고 등 학 교</text>
</svg>
</div>

<div class="logo-float logo-float-8">
<svg viewBox="0 0 200 200" width="100%" height="100%" xmlns="http://www.w3.org/2000/svg">
<circle cx="100" cy="100" r="94" fill="#8a2340"/>
<circle cx="100" cy="100" r="76" fill="none" stroke="#fff" stroke-width="8"/>
<path d="M58 63 Q100 42 142 63 L136 118 Q132 146 100 163 Q68 146 64 118 Z" fill="#8a2340" stroke="#fff" stroke-width="3"/>
<path d="M74 72 L88 61 L100 72 L112 61 L126 72 L126 83 L74 83 Z" fill="#fff"/>
<text x="100" y="101" text-anchor="middle" fill="#fff" font-family="Georgia" font-size="13" font-weight="700">LUX ET SAL</text>
<text x="100" y="128" text-anchor="middle" fill="#fff" font-family="serif" font-size="27" font-weight="700">大光</text>
<text x="100" y="28" text-anchor="middle" fill="#fff" font-family="Georgia" font-size="9" font-weight="700">DAE GWANG HIGH SCHOOL</text>
<text x="100" y="185" text-anchor="middle" fill="#fff" font-family="serif" font-size="9" font-weight="700">대 광 고 등 학 교</text>
</svg>
</div>

<div class="logo-float logo-float-9">
<svg viewBox="0 0 200 200" width="100%" height="100%" xmlns="http://www.w3.org/2000/svg">
<circle cx="100" cy="100" r="94" fill="#8a2340"/>
<circle cx="100" cy="100" r="76" fill="none" stroke="#fff" stroke-width="8"/>
<path d="M58 63 Q100 42 142 63 L136 118 Q132 146 100 163 Q68 146 64 118 Z" fill="#8a2340" stroke="#fff" stroke-width="3"/>
<path d="M74 72 L88 61 L100 72 L112 61 L126 72 L126 83 L74 83 Z" fill="#fff"/>
<text x="100" y="101" text-anchor="middle" fill="#fff" font-family="Georgia" font-size="13" font-weight="700">LUX ET SAL</text>
<text x="100" y="128" text-anchor="middle" fill="#fff" font-family="serif" font-size="27" font-weight="700">大光</text>
<text x="100" y="28" text-anchor="middle" fill="#fff" font-family="Georgia" font-size="9" font-weight="700">DAE GWANG HIGH SCHOOL</text>
<text x="100" y="185" text-anchor="middle" fill="#fff" font-family="serif" font-size="9" font-weight="700">대 광 고 등 학 교</text>
</svg>
</div>

<div class="logo-float logo-float-10">
<svg viewBox="0 0 200 200" width="100%" height="100%" xmlns="http://www.w3.org/2000/svg">
<circle cx="100" cy="100" r="94" fill="#8a2340"/>
<circle cx="100" cy="100" r="76" fill="none" stroke="#fff" stroke-width="8"/>
<path d="M58 63 Q100 42 142 63 L136 118 Q132 146 100 163 Q68 146 64 118 Z" fill="#8a2340" stroke="#fff" stroke-width="3"/>
<path d="M74 72 L88 61 L100 72 L112 61 L126 72 L126 83 L74 83 Z" fill="#fff"/>
<text x="100" y="101" text-anchor="middle" fill="#fff" font-family="Georgia" font-size="13" font-weight="700">LUX ET SAL</text>
<text x="100" y="128" text-anchor="middle" fill="#fff" font-family="serif" font-size="27" font-weight="700">大光</text>
<text x="100" y="28" text-anchor="middle" fill="#fff" font-family="Georgia" font-size="9" font-weight="700">DAE GWANG HIGH SCHOOL</text>
<text x="100" y="185" text-anchor="middle" fill="#fff" font-family="serif" font-size="9" font-weight="700">대 광 고 등 학 교</text>
</svg>
</div>

<div class="logo-float logo-float-11">
<svg viewBox="0 0 200 200" width="100%" height="100%" xmlns="http://www.w3.org/2000/svg">
<circle cx="100" cy="100" r="94" fill="#8a2340"/>
<circle cx="100" cy="100" r="76" fill="none" stroke="#fff" stroke-width="8"/>
<path d="M58 63 Q100 42 142 63 L136 118 Q132 146 100 163 Q68 146 64 118 Z" fill="#8a2340" stroke="#fff" stroke-width="3"/>
<path d="M74 72 L88 61 L100 72 L112 61 L126 72 L126 83 L74 83 Z" fill="#fff"/>
<text x="100" y="101" text-anchor="middle" fill="#fff" font-family="Georgia" font-size="13" font-weight="700">LUX ET SAL</text>
<text x="100" y="128" text-anchor="middle" fill="#fff" font-family="serif" font-size="27" font-weight="700">大光</text>
<text x="100" y="28" text-anchor="middle" fill="#fff" font-family="Georgia" font-size="9" font-weight="700">DAE GWANG HIGH SCHOOL</text>
<text x="100" y="185" text-anchor="middle" fill="#fff" font-family="serif" font-size="9" font-weight="700">대 광 고 등 학 교</text>
</svg>
</div>

<div class="logo-float logo-float-12">
<svg viewBox="0 0 200 200" width="100%" height="100%" xmlns="http://www.w3.org/2000/svg">
<circle cx="100" cy="100" r="94" fill="#8a2340"/>
<circle cx="100" cy="100" r="76" fill="none" stroke="#fff" stroke-width="8"/>
<path d="M58 63 Q100 42 142 63 L136 118 Q132 146 100 163 Q68 146 64 118 Z" fill="#8a2340" stroke="#fff" stroke-width="3"/>
<path d="M74 72 L88 61 L100 72 L112 61 L126 72 L126 83 L74 83 Z" fill="#fff"/>
<text x="100" y="101" text-anchor="middle" fill="#fff" font-family="Georgia" font-size="13" font-weight="700">LUX ET SAL</text>
<text x="100" y="128" text-anchor="middle" fill="#fff" font-family="serif" font-size="27" font-weight="700">大光</text>
<text x="100" y="28" text-anchor="middle" fill="#fff" font-family="Georgia" font-size="9" font-weight="700">DAE GWANG HIGH SCHOOL</text>
<text x="100" y="185" text-anchor="middle" fill="#fff" font-family="serif" font-size="9" font-weight="700">대 광 고 등 학 교</text>
</svg>
</div>

<!-- =========================
     헤더
========================= -->

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

<!-- =========================
     메뉴
========================= -->

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
<p>랜덤 수학문제를 풀고 랭킹에 도전!</p>
</div>

</div>

</div>

</div>

</section>

<!-- =========================
     방문록
========================= -->

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

<button onclick="addEntry()">
방문록 등록
</button>

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

<!-- =========================
     수학게임
========================= -->

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
30초 동안 최대한 많은 문제를 풀어보세요. 각 문제에는 20초의 제한시간이 있습니다.
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
<span class="status-label">전체 시간</span>
<span id="gameTime" class="status-value">30</span>
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
<span class="status-label">최고 기록</span>
<span id="gameBest" class="status-value">0</span>
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

<!-- =========================
     비밀번호 모달
========================= -->

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
   페이지 상태 저장
===================================================== */

const PAGE_KEY=
"daekwang_bigbit_current_page_v2";


function showPage(pageId){

 document.querySelectorAll(".page").forEach(
  page=>{
   page.classList.remove("active");
  }
 );

 const target=
  document.getElementById(pageId);

 if(!target)return;

 target.classList.add("active");

 sessionStorage.setItem(
  PAGE_KEY,
  pageId
 );

 window.scrollTo(0,0);

}


/* =====================================================
   방문록
===================================================== */

const STORAGE_KEY=
"daekwang_bigbit_festival_guestbook_v2";

const LIKE_KEY=
"daekwang_bigbit_festival_likes_v3";

const MASTER_PASSWORD=
"20100806";

const LIKE_CANCEL_DELAY=
7000;

let entries=
JSON.parse(
 localStorage.getItem(STORAGE_KEY)||"[]"
);

let likes=
JSON.parse(
 localStorage.getItem(LIKE_KEY)||"{}"
);

let pending=null;


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


function formatDate(iso){

 const d=new Date(iso);

 const p=n=>
  String(n).padStart(2,"0");

 return `${d.getFullYear()}년 ${p(d.getMonth()+1)}월 ${p(d.getDate())}일 ${p(d.getHours())}시 ${p(d.getMinutes())}분 ${p(d.getSeconds())}초`;

}


function addEntry(){

 const name=
  document.getElementById("name")
  .value.trim();

 const pw=
  document.getElementById("password")
  .value;

 const message=
  document.getElementById("message")
  .value.trim();


 if(!name||!pw||!message){

  alert(
   "이름(닉네임), 비밀번호, 내용을 모두 입력해주세요."
  );

  return;

 }


 const id=
  window.crypto&&crypto.randomUUID
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

 const data=
  normalizeLikes(id);

 data.count++;

 data.times.push(
  Date.now()
 );

 saveLikes();

 render();

}


function getCancelableIndex(id){

 const data=
  likes[id];

 if(
  !data||
  !Array.isArray(data.times)
 ){

  return -1;

 }


 const now=Date.now();

 return data.times.findIndex(
  time=>
   now-time>=LIKE_CANCEL_DELAY
 );

}


function cancelLike(id){

 const data=
  likes[id];

 if(!data)return;


 const index=
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


function getCancelText(id){

 const data=
  likes[id];

 if(
  !data||
  !data.times||
  !data.times.length
 ){

  return "좋아요 취소";

 }


 const now=Date.now();

 const available=
  data.times.some(
   time=>
    now-time>=LIKE_CANCEL_DELAY
  );

 if(available){

  return "좋아요 취소";

 }


 const earliest=
  Math.min(...data.times);


 const remain=
  Math.max(
   0,
   Math.ceil(
    (
     LIKE_CANCEL_DELAY-
     (now-earliest)
    )/1000
   )
  );


 return `${remain}초 후 취소`;

}


function render(){

 const box=
  document.getElementById("entries");

 const count=
  document.getElementById("count");

 if(!box||!count)return;


 count.textContent=
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


 box.innerHTML=
  entries.map(e=>{

   const data=
    normalizeLikes(e.id);

   const cancelAvailable=
    getCancelableIndex(e.id)!==-1;

   const cancelText=
    getCancelText(e.id);


   return `

   <article class="entry">

    <div class="entry-head">

     <div class="name">
     ${escapeHTML(e.name)}
     </div>

     <div class="time">
     작성:
     ${formatDate(e.createdAt)}
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
       ${cancelAvailable?"":"disabled"}
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


 document.getElementById("modal")
 .classList.add("show");


 setTimeout(
  ()=>{
   document
   .getElementById("checkPw")
   .focus();
  },
  50
 );

}


function closeModal(){

 pending=null;

 document
 .getElementById("modal")
 .classList
 .remove("show");

}


function confirmPassword(){

 if(!pending)return;


 const e=
  entries.find(
   x=>x.id===pending.id
  );


 const pw=
  document
  .getElementById("checkPw")
  .value;


 if(
  !e||
  !(pw===e.password||
    pw===MASTER_PASSWORD)
 ){

  document
  .getElementById("pwError")
  .textContent=
   "비밀번호가 올바르지 않습니다.";

  return;

 }


 const action=
  pending.action;

 const id=
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
     x=>x.id!==id
    );

   delete likes[id];

   save();
   saveLikes();
   render();

  }

 }


 else{

  const target=
   entries.find(
    x=>x.id===id
   );

  if(!target)return;


  const newName=
   prompt(
    "이름 또는 닉네임",
    target.name
   );

  if(newName===null)return;


  const newMessage=
   prompt(
    "방문록 내용",
    target.message
   );

  if(newMessage===null)return;


  if(
   !newName.trim()||
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


  save();
  render();

 }

}


/* =====================================================
   모달
===================================================== */

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


document.addEventListener(
 "keydown",
 e=>{

  if(e.key==="Escape"){

   closeModal();

  }

 }
);


/* =====================================================
   수학게임
===================================================== */

const GAME_TOTAL_TIME=
 30;

const QUESTION_TIME=
 20;

const RANKING_KEY=
 "daekwang_bigbit_math_ranking_v4";

const BEST_KEY=
 "daekwang_bigbit_math_best_v4";


const difficultyConfig={

 kindergarten:{
  label:"🟢 유치원",
  score:1,
  weight:29
 },

 elementaryLow:{
  label:"🟢 초등 저학년",
  score:2,
  weight:23
 },

 elementaryHigh:{
  label:"🟡 초등 고학년",
  score:3,
  weight:18
 },

 middle:{
  label:"🟡 중학교",
  score:5,
  weight:14
 },

 high:{
  label:"🟠 고등학교",
  score:8,
  weight:9
 },

 university:{
  label:"🔴 대학",
  score:12,
  weight:5
 },

 universityHard:{
  label:"🔴 대학 심화",
  score:16,
  weight:2
 }

};


let gameRunning=false;

let gameScore=0;

let gameTime=GAME_TOTAL_TIME;

let questionTime=QUESTION_TIME;

let gameSolved=0;

let gameTimer=null;

let questionTimer=null;

let currentQuestion=null;

let usedQuestionKeys=new Set();

let lastQuestionType=null;

let bestGameScore=
 Number(
  localStorage.getItem(BEST_KEY)||0
 );


document.getElementById("gameBest")
.textContent=
 bestGameScore;


/* =====================================================
   공통 수학 함수
===================================================== */

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


function gcd(a,b){

 a=Math.abs(a);
 b=Math.abs(b);

 while(b){

  const t=a%b;

  a=b;
  b=t;

 }

 return a||1;

}


function fraction(n,d){

 if(d===0)d=1;

 if(d<0){

  n=-n;
  d=-d;

 }

 const g=gcd(n,d);

 n/=g;
 d/=g;

 if(d===1){

  return String(n);

 }

 return `${n}/${d}`;

}


function combination(n,r){

 if(r<0||r>n){

  return 0;

 }

 r=Math.min(r,n-r);

 let result=1;

 for(
  let i=1;
  i<=r;
  i++
 ){

  result=
   result*(n-r+i)/i;

 }

 return Math.round(result);

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
  )<0.0000001
 ){

  return String(
   Math.round(value)
  );

 }

 return String(
  Math.round(value*100)/100
 );

}


/* =====================================================
   난이도
===================================================== */

function chooseDifficulty(){

 const keys=
  Object.keys(
   difficultyConfig
  );

 let total=0;

 keys.forEach(
  key=>{
   total+=
    difficultyConfig[key].weight;
  }
 );

 let r=
  Math.random()*total;


 for(const key of keys){

  r-=
   difficultyConfig[key].weight;

  if(r<=0){

   return key;

  }

 }

 return keys[0];

}


function chooseType(types){

 let pool=
  types.filter(
   type=>type!==lastQuestionType
  );

 if(!pool.length){

  pool=types;

 }

 return randomChoice(pool);

}


/* =====================================================
   유치원
===================================================== */

function generateKindergarten(){

 const types=[
  "k_add",
  "k_sub",
  "k_compare",
  "k_count",
  "k_double",
  "k_half",
  "k_shape_count"
 ];

 const type=
  chooseType(types);


 if(type==="k_add"){

  const a=randInt(1,10);
  const b=randInt(1,10);

  return {
   type,
   question:`${a} + ${b} = ?`,
   answer:a+b
  };

 }


 if(type==="k_sub"){

  const a=randInt(2,15);
  const b=randInt(1,a);

  return {
   type,
   question:`${a} - ${b} = ?`,
   answer:a-b
  };

 }


 if(type==="k_compare"){

  const a=randInt(1,20);
  const b=randInt(1,20);

  return {
   type,
   question:`다음 두 수 중 더 큰 수는?  ${a} , ${b}`,
   answer:Math.max(a,b)
  };

 }


 if(type==="k_count"){

  const groups=randInt(2,5);
  const each=randInt(1,5);

  return {
   type,
   question:`사탕 ${groups}묶음이 있고 한 묶음에 ${each}개입니다. 모두 몇 개일까요?`,
   answer:groups*each
  };

 }


 if(type==="k_double"){

  const a=randInt(1,10);

  return {
   type,
   question:`${a}의 2배는?`,
   answer:a*2
  };

 }


 if(type==="k_half"){

  const a=randInt(2,20)*2;

  return {
   type,
   question:`${a}의 절반은?`,
   answer:a/2
  };

 }


 const shapes=[
  {name:"삼각형",count:3},
  {name:"사각형",count:4},
  {name:"오각형",count:5},
  {name:"육각형",count:6}
 ];

 const shape=
  randomChoice(shapes);

 return {
  type,
  question:`${shape.name}의 변은 몇 개일까요?`,
  answer:shape.count
 };

}


/* =====================================================
   초등 저학년
===================================================== */

function generateElementaryLow(){

 const types=[
  "el_add",
  "el_sub",
  "el_mul",
  "el_money",
  "el_time",
  "el_missing",
  "el_shape_side"
 ];

 const type=
  chooseType(types);


 if(type==="el_add"){

  const a=randInt(10,99);
  const b=randInt(10,99);

  return {
   type,
   question:`${a} + ${b} = ?`,
   answer:a+b
  };

 }


 if(type==="el_sub"){

  const a=randInt(30,180);
  const b=randInt(5,a);

  return {
   type,
   question:`${a} - ${b} = ?`,
   answer:a-b
  };

 }


 if(type==="el_mul"){

  const a=randInt(2,12);
  const b=randInt(2,12);

  return {
   type,
   question:`${a} × ${b} = ?`,
   answer:a*b
  };

 }


 if(type==="el_money"){

  const price=randInt(5,30)*100;
  const count=randInt(2,5);

  return {
   type,
   question:`한 개에 ${price.toLocaleString()}원인 물건 ${count}개의 가격은?`,
   answer:price*count
  };

 }


 if(type==="el_time"){

  const hour=randInt(1,11);
  const add=randInt(1,6);

  return {
   type,
   question:`오후 ${hour}시에 시작해서 ${add}시간 후는 몇 시일까요?`,
   answer:hour+add
  };

 }


 if(type==="el_missing"){

  const x=randInt(2,30);
  const b=randInt(1,20);

  return {
   type,
   question:`□ + ${b} = ${x+b}일 때 □는?`,
   answer:x
  };

 }


 const sides=[
  {name:"삼각형",value:3},
  {name:"사각형",value:4},
  {name:"오각형",value:5},
  {name:"육각형",value:6},
  {name:"팔각형",value:8}
 ];

 const shape=
  randomChoice(sides);

 return {
  type,
  question:`${shape.name}의 변의 개수는?`,
  answer:shape.value
 };

}


/* =====================================================
   초등 고학년
===================================================== */

function generateElementaryHigh(){

 const types=[
  "eh_div",
  "eh_fraction",
  "eh_percent",
  "eh_area_rect",
  "eh_average",
  "eh_ratio",
  "eh_circle_basic",
  "eh_triangle_area",
  "eh_perimeter"
 ];

 const type=
  chooseType(types);


 if(type==="eh_div"){

  const b=randInt(2,12);
  const q=randInt(2,25);

  return {
   type,
   question:`${b*q} ÷ ${b} = ?`,
   answer:q
  };

 }


 if(type==="eh_fraction"){

  const d=randInt(2,10);
  const n=randInt(1,d-1);

  const d2=randInt(2,10);
  const n2=randInt(1,d2-1);

  return {
   type,
   question:`${fraction(n,d)} + ${fraction(n2,d2)} = ?`,
   answer:n/d+n2/d2
  };

 }


 if(type==="eh_percent"){

  const base=randInt(2,20)*50;
  const p=randomChoice([10,20,25,30,40,50]);

  return {
   type,
   question:`${base}의 ${p}%는?`,
   answer:base*p/100
  };

 }


 if(type==="eh_area_rect"){

  const w=randInt(3,20);
  const h=randInt(3,20);

  return {
   type,
   question:`가로 ${w}, 세로 ${h}인 직사각형의 넓이는?`,
   answer:w*h
  };

 }


 if(type==="eh_average"){

  const n=randInt(3,6);
  const values=[];

  for(let i=0;i<n;i++){

   values.push(randInt(5,30));

  }

  const total=
   values.reduce(
    (a,b)=>a+b,
    0
   );

  return {
   type,
   question:`${values.join(", ")}의 평균은?`,
   answer:total/n
  };

 }


 if(type==="eh_ratio"){

  const a=randInt(2,9);
  const b=randInt(2,9);
  const multiplier=randInt(2,8);

  return {
   type,
   question:`A:B=${a}:${b}이고 B=${b*multiplier}일 때 A는?`,
   answer:a*multiplier
  };

 }


 if(type==="eh_circle_basic"){

  const r=randInt(2,10);

  return {
   type,
   question:`반지름이 ${r}인 원의 지름은?`,
   answer:r*2
  };

 }


 if(type==="eh_triangle_area"){

  const base=randInt(3,15);
  const height=randInt(3,15);

  return {
   type,
   question:`밑변 ${base}, 높이 ${height}인 삼각형의 넓이는?`,
   answer:base*height/2
  };

 }


 const w=randInt(3,20);
 const h=randInt(3,20);

 return {
  type,
  question:`가로 ${w}, 세로 ${h}인 직사각형의 둘레는?`,
  answer:2*(w+h)
 };

}


/* =====================================================
   중학교
===================================================== */

function generateMiddle(){

 const types=[
  "m_linear",
  "m_factor",
  "m_square",
  "m_percent",
  "m_probability",
  "m_pythagoras",
  "m_function",
  "m_triangle_angle",
  "m_rectangle_perimeter",
  "m_circle_area"
 ];

 const type=
  chooseType(types);


 if(type==="m_linear"){

  const a=randInt(2,9);
  const x=randInt(-9,12);
  const b=randInt(-15,15);
  const c=a*x+b;

  return {
   type,
   question:`${a}x ${b>=0?"+ "+b:"- "+Math.abs(b)} = ${c}일 때 x는?`,
   answer:x
  };

 }


 if(type==="m_factor"){

  const r1=randInt(-8,8);
  const r2=randInt(-8,8);

  const B=-(r1+r2);
  const C=r1*r2;

  return {
   type,
   question:`x² ${B>=0?"+ "+B:"- "+Math.abs(B)}x ${C>=0?"+ "+C:"- "+Math.abs(C)} = 0의 한 근은?`,
   answer:r1
  };

 }


 if(type==="m_square"){

  const a=randInt(2,12);
  const b=randInt(2,12);

  return {
   type,
   question:`(${a}+${b})² = ?`,
   answer:(a+b)*(a+b)
  };

 }


 if(type==="m_percent"){

  const original=randInt(10,80)*100;
  const p=randomChoice([10,15,20,25,30]);

  return {
   type,
   question:`${original}원이 ${p}% 올랐을 때 가격은?`,
   answer:original*(100+p)/100
  };

 }


 if(type==="m_probability"){

  const red=randInt(1,8);
  const blue=randInt(1,8);

  return {
   type,
   question:`빨간 공 ${red}개, 파란 공 ${blue}개가 있을 때 빨간 공을 뽑을 확률은?`,
   answer:red/(red+blue)
  };

 }


 if(type==="m_pythagoras"){

  const a=randInt(3,12);
  const b=randInt(3,12);

  return {
   type,
   question:`직각삼각형의 두 직각변이 ${a}, ${b}일 때 빗변의 길이는?`,
   answer:Math.sqrt(a*a+b*b)
  };

 }


 if(type==="m_function"){

  const a=randInt(2,8);
  const b=randInt(-10,10);
  const x=randInt(-5,10);

  return {
   type,
   question:`f(x)=${a}x ${b>=0?"+ "+b:"- "+Math.abs(b)}일 때 f(${x})는?`,
   answer:a*x+b
  };

 }


 if(type==="m_triangle_angle"){

  const a=randInt(30,80);
  const b=randInt(20,70);
  const c=180-a-b;

  if(c<=10){
   return generateMiddle();
  }

  return {
   type,
   question:`삼각형의 두 내각이 ${a}°, ${b}°일 때 나머지 한 각은?`,
   answer:c
  };

 }


 if(type==="m_rectangle_perimeter"){

  const w=randInt(3,20);
  const h=randInt(3,20);

  return {
   type,
   question:`가로 ${w}, 세로 ${h}인 직사각형의 둘레는?`,
   answer:2*(w+h)
  };

 }


 const r=randInt(2,9);

 return {
  type,
  question:`반지름이 ${r}인 원의 넓이를 πr²로 나타낼 때 π의 계수는?`,
  answer:r*r
 };

}


/* =====================================================
   고등학교
===================================================== */

function generateHigh(){

 const types=[
  "h_quadratic",
  "h_log",
  "h_exponent",
  "h_trig",
  "h_sequence",
  "h_derivative",
  "h_probability",
  "h_combinatorics",
  "h_triangle_area",
  "h_circle_angle",
  "h_coordinate_distance",
  "h_parabola_value"
 ];

 const type=
  chooseType(types);


 if(type==="h_quadratic"){

  const r1=randInt(-9,9);
  const r2=randInt(-9,9);

  const B=-(r1+r2);
  const C=r1*r2;

  return {
   type,
   question:`x² ${B>=0?"+ "+B:"- "+Math.abs(B)}x ${C>=0?"+ "+C:"- "+Math.abs(C)}=0의 한 근은?`,
   answer:r1
  };

 }


 if(type==="h_log"){

  const base=randomChoice([2,3,4,5]);
  const exponent=randInt(2,6);

  return {
   type,
   question:`log_${base}(${Math.pow(base,exponent)}) = ?`,
   answer:exponent
  };

 }


 if(type==="h_exponent"){

  const base=randomChoice([2,3,5]);
  const a=randInt(2,6);
  const b=randInt(1,4);

  return {
   type,
   question:`${base}^${a} × ${base}^${b} = ?`,
   answer:Math.pow(base,a+b)
  };

 }


 if(type==="h_trig"){

  const data=randomChoice([
   {q:"sin 30°",a:.5},
   {q:"cos 60°",a:.5},
   {q:"sin 90°",a:1},
   {q:"cos 0°",a:1},
   {q:"tan 45°",a:1}
  ]);

  return {
   type,
   question:`${data.q} = ?`,
   answer:data.a
  };

 }


 if(type==="h_sequence"){

  const first=randInt(1,10);
  const d=randInt(2,8);
  const n=randInt(5,15);

  return {
   type,
   question:`등차수열의 첫째항이 ${first}, 공차가 ${d}일 때 ${n}번째 항은?`,
   answer:first+(n-1)*d
  };

 }


 if(type==="h_derivative"){

  const n=randInt(2,6);
  const x=randInt(1,8);

  return {
   type,
   question:`f(x)=x^${n}일 때 f'(${x})는?`,
   answer:n*Math.pow(x,n-1)
  };

 }


 if(type==="h_probability"){

  const n=randInt(3,6);
  const success=randInt(0,n);

  return {
   type,
   question:`동전을 ${n}번 던질 때 앞면이 정확히 ${success}번 나올 확률은?`,
   answer:combination(n,success)*Math.pow(.5,n)
  };

 }


 if(type==="h_combinatorics"){

  const n=randInt(5,10);
  const r=randInt(2,n-2);

  return {
   type,
   question:`C(${n}, ${r}) = ?`,
   answer:combination(n,r)
  };

 }


 if(type==="h_triangle_area"){

  const base=randInt(4,16);
  const height=randInt(4,16);

  return {
   type,
   question:`밑변 ${base}, 높이 ${height}인 삼각형의 넓이는?`,
   answer:base*height/2
  };

 }


 if(type==="h_circle_angle"){

  const radius=randInt(2,9);
  const angle=randomChoice([30,45,60,90]);

  return {
   type,
   question:`반지름 ${radius}인 원에서 중심각이 ${angle}°인 부채꼴의 중심각 비율은?`,
   answer:angle/360
  };

 }


 if(type==="h_coordinate_distance"){

  const x1=randInt(-6,6);
  const y1=randInt(-6,6);
  const x2=randInt(-6,6);
  const y2=randInt(-6,6);

  return {
   type,
   question:`두 점 (${x1},${y1}), (${x2},${y2}) 사이의 거리는?`,
   answer:Math.sqrt(
    Math.pow(x2-x1,2)+
    Math.pow(y2-y1,2)
   )
  };

 }


 const a=randInt(2,8);
 const x=randInt(-5,8);

 return {
  type,
  question:`f(x)=${a}x²일 때 f(${x})는?`,
  answer:a*x*x
 };

}


/* =====================================================
   대학
===================================================== */

function generateUniversity(){

 const types=[
  "u_integral",
  "u_integral_linear",
  "u_derivative",
  "u_trace",
  "u_determinant",
  "u_probability",
  "u_complex",
  "u_limit",
  "u_vector",
  "u_geometry"
 ];

 const type=
  chooseType(types);


 if(type==="u_integral"){

  const n=randInt(2,8);

  return {
   type,
   question:`∫₀^${n} x² dx = ?`,
   answer:n*n*n/3
  };

 }


 if(type==="u_integral_linear"){

  const a=randInt(2,9);
  const b=randInt(1,8);
  const upper=randInt(2,7);

  return {
   type,
   question:`∫₀^${upper} (${a}x + ${b}) dx = ?`,
   answer:a*upper*upper/2+b*upper
  };

 }


 if(type==="u_derivative"){

  const a=randInt(2,8);
  const x=randInt(1,6);

  return {
   type,
   question:`f(x)=${a}x²일 때 f'(${x})는?`,
   answer:2*a*x
  };

 }


 if(type==="u_trace"){

  const a=randInt(1,9);
  const b=randInt(1,9);

  return {
   type,
   question:`행렬 [[${a},0],[0,${b}]]의 trace는?`,
   answer:a+b
  };

 }


 if(type==="u_determinant"){

  const a=randInt(1,8);
  const b=randInt(1,8);
  const c=randInt(1,8);
  const d=randInt(1,8);

  return {
   type,
   question:`det [[${a},${b}],[${c},${d}]] = ?`,
   answer:a*d-b*c
  };

 }


 if(type==="u_probability"){

  const success=randInt(2,7);
  const total=randInt(success+1,12);

  return {
   type,
   question:`성공 ${success}회 / 전체 ${total}회일 때 경험적 확률은?`,
   answer:success/total
  };

 }


 if(type==="u_complex"){

  const a=randInt(1,8);
  const b=randInt(1,8);

  return {
   type,
   question:`z=${a}+${b}i일 때 |z|²는?`,
   answer:a*a+b*b
  };

 }


 if(type==="u_limit"){

  const a=randInt(2,9);
  const b=randInt(1,9);
  const x=randInt(1,7);

  return {
   type,
   question:`lim(x→${x}) (${a}x + ${b}) = ?`,
   answer:a*x+b
  };

 }


 if(type==="u_vector"){

  const a=randInt(1,8);
  const b=randInt(1,8);
  const c=randInt(1,8);
  const d=randInt(1,8);

  return {
   type,
   question:`벡터 (${a},${b})·(${c},${d}) = ?`,
   answer:a*c+b*d
  };

 }


 const r=randInt(2,8);
 const angle=randomChoice([90,180,270]);

 return {
  type,
  question:`반지름 ${r}인 원에서 중심각 ${angle}°가 나타내는 부채꼴의 넓이를 πr² 기준으로 나타낸 비율은?`,
  answer:angle/360
 };

}


/* =====================================================
   대학 심화
===================================================== */

function generateUniversityHard(){

 const types=[
  "uh_integral_trig",
  "uh_chain",
  "uh_matrix",
  "uh_complex",
  "uh_expectation",
  "uh_eigen",
  "uh_series",
  "uh_vector_cross",
  "uh_geometry_coordinate"
 ];

 const type=
  chooseType(types);


 if(type==="uh_integral_trig"){

  const n=randInt(1,7);

  return {
   type,
   question:`∫₀^π ${n}sin(x) dx ÷ ${n} = ?`,
   answer:2
  };

 }


 if(type==="uh_chain"){

  const a=randInt(2,7);
  const x=randInt(1,6);

  return {
   type,
   question:`f(x)=(${a}x)²일 때 f'(${x})는?`,
   answer:2*a*a*x
  };

 }


 if(type==="uh_matrix"){

  const a=randInt(1,5);
  const b=randInt(1,5);
  const c=randInt(1,5);

  return {
   type,
   question:`diag(${a},${b},${c})의 행렬식은?`,
   answer:a*b*c
  };

 }


 if(type==="uh_complex"){

  const a=randInt(1,7);

  return {
   type,
   question:`z=${a}i일 때 z²는?`,
   answer:-a*a
  };

 }


 if(type==="uh_expectation"){

  const x1=randInt(1,5);
  const x2=randInt(6,10);
  const p=randomChoice([.2,.3,.4,.6,.7,.8]);

  return {
   type,
   question:`X가 ${x1}을 확률 ${p}, ${x2}를 확률 ${1-p}로 가질 때 E[X]는?`,
   answer:p*x1+(1-p)*x2
  };

 }


 if(type==="uh_eigen"){

  const a=randInt(2,9);
  const b=randInt(2,9);

  return {
   type,
   question:`행렬 [[${a},0],[0,${b}]]의 고유값 중 작은 값은?`,
   answer:Math.min(a,b)
  };

 }


 if(type==="uh_series"){

  const a=randInt(1,5);
  const r=randInt(2,3);
  const n=randInt(3,7);

  return {
   type,
   question:`등비수열의 첫째항 ${a}, 공비 ${r}일 때 첫 ${n}개 항의 합은?`,
   answer:a*(Math.pow(r,n)-1)/(r-1)
  };

 }


 if(type==="uh_vector_cross"){

  const a=randInt(1,5);
  const b=randInt(1,5);

  return {
   type,
   question:`벡터 (${a},0,0) × (0,${b},0)의 크기는?`,
   answer:a*b
  };

 }


 const x1=randInt(-5,5);
 const y1=randInt(-5,5);
 const x2=randInt(-5,5);
 const y2=randInt(-5,5);

 return {
  type,
  question:`좌표평면에서 (${x1},${y1})과 (${x2},${y2})를 잇는 선분의 길이의 제곱은?`,
  answer:
   Math.pow(x2-x1,2)+
   Math.pow(y2-y1,2)
 };

}


/* =====================================================
   문제 생성
===================================================== */

function createQuestion(){

 let attempts=0;


 while(attempts<500){

  attempts++;


  const level=
   chooseDifficulty();


  let q;


  if(level==="kindergarten"){
   q=generateKindergarten();
  }
  else if(level==="elementaryLow"){
   q=generateElementaryLow();
  }
  else if(level==="elementaryHigh"){
   q=generateElementaryHigh();
  }
  else if(level==="middle"){
   q=generateMiddle();
  }
  else if(level==="high"){
   q=generateHigh();
  }
  else if(level==="university"){
   q=generateUniversity();
  }
  else{
   q=generateUniversityHard();
  }


  if(q.type===lastQuestionType){

   continue;

  }


  const key=
   `${level}|${q.type}|${q.question}|${formatNumber(q.answer)}`;


  if(
   usedQuestionKeys.has(key)
  ){

   continue;

  }


  usedQuestionKeys.add(key);

  lastQuestionType=
   q.type;


  return {
   level:level,
   type:q.type,
   question:q.question,
   answer:q.answer,
   key:key
  };

 }


 const a=randInt(1,100);
 const b=randInt(1,100);

 return {
  level:"elementaryLow",
  type:"fallback_"+Date.now(),
  question:`${a} + ${b} = ?`,
  answer:a+b,
  key:"fallback_"+Date.now()
 };

}


/* =====================================================
   보기 만들기
===================================================== */

function makeChoices(answer,level){

 const choices=[answer];

 let attempts=0;


 while(
  choices.length<5&&
  attempts<500
 ){

  attempts++;


  if(
   typeof answer==="number"&&
   Number.isFinite(answer)
  ){

   let range;


   if(level==="kindergarten"){

    range=5;

   }
   else if(level==="elementaryLow"){

    range=10;

   }
   else if(level==="elementaryHigh"){

    range=15;

   }
   else if(level==="middle"){

    range=20;

   }
   else if(level==="high"){

    range=25;

   }
   else{

    range=
     Math.max(
      2,
      Math.round(
       Math.abs(answer)*.25
      )
     );

   }


   let wrong=
    answer+
    randomChoice([
     -1,1,-2,2,
     -range,
     range
    ]);


   if(!Number.isInteger(answer)){

    wrong=
     Math.round(
      wrong*100
     )/100;

   }


   const duplicate=
    choices.some(
     value=>
      Math.abs(
       Number(value)-Number(wrong)
      )<0.000001
    );


   if(!duplicate){

    choices.push(wrong);

   }

  }

 }


 while(choices.length<5){

  let extra=
   answer+
   choices.length*7+
   3;


  while(
   choices.some(
    value=>
     Math.abs(
      Number(value)-Number(extra)
     )<0.000001
   )
  ){

   extra+=7;

  }


  choices.push(extra);

 }


 for(
  let i=choices.length-1;
  i>0;
  i--
 ){

  const j=
   Math.floor(
    Math.random()*(i+1)
   );


  [
   choices[i],
   choices[j]
  ]=[
   choices[j],
   choices[i]
  ];

 }


 return choices;

}


/* =====================================================
   문제 표시
===================================================== */

function showQuestion(){

 if(!gameRunning)return;


 currentQuestion=
  createQuestion();


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


 currentQuestion.choices=
  choices;


 const box=
  document.getElementById("choices");


 box.innerHTML="";


 const labels=[
  "①","②","③","④","⑤"
 ];


 choices.forEach(
  (choice,index)=>{

   const button=
    document.createElement("button");


   button.className=
    "choice-btn";


   button.textContent=
    `${labels[index]} ${formatNumber(choice)}`;


   button.onclick=
    ()=>{
     answerQuestion(
      index,
      button
     );
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
   문제별 20초
===================================================== */

function startQuestionTimer(){

 if(questionTimer){

  clearInterval(questionTimer);

 }


 questionTime=
  QUESTION_TIME;


 updateQuestionTimer();


 questionTimer=
  setInterval(
   ()=>{

    questionTime--;

    updateQuestionTimer();


    if(questionTime<=0){

     clearInterval(questionTimer);

     questionTimer=null;

     questionTimeout();

    }

   },
   1000
  );

}


function updateQuestionTimer(){

 document.getElementById(
  "questionTime"
 ).textContent=
  questionTime;


 document.getElementById(
  "questionTimerBar"
 ).style.width=
  `${Math.max(
   0,
   questionTime/QUESTION_TIME*100
  )}%`;

}


function questionTimeout(){

 if(!gameRunning)return;


 document.querySelectorAll(
  ".choice-btn"
 ).forEach(
  button=>{
   button.disabled=true;
  }
 );


 document.getElementById(
  "gameMessage"
 ).textContent=
  "⏰ 시간 초과! 다음 문제로 넘어갑니다.";


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

 if(!gameRunning)return;


 if(questionTimer){

  clearInterval(questionTimer);

  questionTimer=null;

 }


 const buttons=
  document.querySelectorAll(
   ".choice-btn"
  );


 buttons.forEach(
  button=>{
   button.disabled=true;
  }
 );


 const selected=
  currentQuestion.choices[index];


 const correct=
  Math.abs(
   Number(selected)-
   Number(currentQuestion.answer)
  )<0.000001;


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


  document.getElementById(
   "gameScore"
  ).textContent=
   gameScore;


  document.getElementById(
   "gameSolved"
  ).textContent=
   gameSolved;


  document.getElementById(
   "gameMessage"
  ).textContent=
   `✅ 정답! +${points}점`;

 }
 else{

  clickedButton.classList.add(
   "wrong"
  );


  document.getElementById(
   "gameMessage"
  ).textContent=
   `❌ 오답! 정답은 ${formatNumber(currentQuestion.answer)}입니다.`;

 }


 setTimeout(
  ()=>{

   if(gameRunning){

    showQuestion();

   }

  },
  450
 );

}


/* =====================================================
   게임 시작
===================================================== */

function startMathGame(){

 if(gameRunning)return;


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

 /* 게임 중 닉네임 입력 잠금 */

 document.getElementById(
  "gameNickname"
 ).disabled=true;


 gameScore=0;

 gameTime=
  GAME_TOTAL_TIME;

 questionTime=
  QUESTION_TIME;

 gameSolved=0;

 currentQuestion=null;

 usedQuestionKeys=
  new Set();

 lastQuestionType=null;


 document.getElementById(
  "gameScore"
 ).textContent="0";

 document.getElementById(
  "gameTime"
 ).textContent=
  GAME_TOTAL_TIME;

 document.getElementById(
  "questionTime"
 ).textContent=
  QUESTION_TIME;

 document.getElementById(
  "gameSolved"
 ).textContent="0";


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


 showQuestion();


 gameTimer=
  setInterval(
   ()=>{

    gameTime--;

    document.getElementById(
     "gameTime"
    ).textContent=
     gameTime;


    if(gameTime<=0){

     endMathGame();

    }

   },
   1000
  );

}


/* =====================================================
   게임 종료
===================================================== */

function endMathGame(){

 if(!gameRunning)return;


 gameRunning=false;


 if(gameTimer){

  clearInterval(gameTimer);

  gameTimer=null;

 }


 if(questionTimer){

  clearInterval(questionTimer);

  questionTimer=null;

 }


 /* 게임이 끝나면 닉네임 다시 입력 가능 */

 document.getElementById(
  "gameNickname"
 ).disabled=false;


 document.querySelectorAll(
  ".choice-btn"
 ).forEach(
  button=>{
   button.disabled=true;
  }
 );


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


 document.getElementById(
  "gameMessage"
 ).textContent=
  "⏰ 전체 게임 시간이 끝났습니다!";


 const nickname=
  document.getElementById(
   "gameNickname"
  ).value.trim();


 if(gameScore>bestGameScore){

  bestGameScore=
   gameScore;


  localStorage.setItem(
   BEST_KEY,
   String(bestGameScore)
  );


  document.getElementById(
   "gameBest"
  ).textContent=
   bestGameScore;

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
  `${nickname}님 · ${gameSolved}문제 정답`;


 saveRanking(
  nickname,
  gameScore
 );

}


/* =====================================================
   랭킹
===================================================== */

function getRanking(){

 try{

  const data=
   JSON.parse(
    localStorage.getItem(
     RANKING_KEY
    )||"[]"
   );


  return Array.isArray(data)
   ?data
   :[];

 }
 catch(error){

  return[];

 }

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
   b.score-a.score||
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


 if(!body)return;


 const ranking=
  getRanking();


 if(!ranking.length){

  body.innerHTML=
  `
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
   새로고침해도 현재 페이지 유지
===================================================== */

function restorePage(){

 const savedPage=
  sessionStorage.getItem(
   PAGE_KEY
  );


 const validPages=[
  "menuPage",
  "guestbookPage",
  "gamePage"
 ];


 if(
  savedPage&&
  validPages.includes(savedPage)
 ){

  showPage(savedPage);

 }else{

  showPage("menuPage");

 }

}


/* =====================================================
   좋아요 시간 갱신
===================================================== */

setInterval(
 ()=>{
  render();
 },
 1000
);


/* =====================================================
   시작
===================================================== */

renderRanking();

render();

restorePage();

</script>

</body>
</html>
```
