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
   게임
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
 margin-bottom:14px;
}

.question{
 min-height:105px;
 display:flex;
 align-items:center;
 justify-content:center;
 text-align:center;
 font-size:25px;
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
  font-size:22px;
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

<!-- =====================================================
     배경 로고
===================================================== -->

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
30초 동안 최대한 많은 문제를 풀어보세요.
문제의 종류와 숫자는 계속 무작위로 바뀝니다.
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
<span class="status-label">남은 시간</span>
<span id="gameTime" class="status-value">30</span>
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
   페이지 전환
===================================================== */

function showPage(pageId){

 document.querySelectorAll(".page").forEach(
  page=>{
   page.classList.remove("active");
  }
 );

 const target=document.getElementById(pageId);

 if(target){
  target.classList.add("active");
 }

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

 const p=n=>String(n).padStart(2,"0");

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

 const data=normalizeLikes(id);

 data.count++;

 data.times.push(Date.now());

 saveLikes();

 render();

}


function getCancelableIndex(id){

 const data=likes[id];

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

 const data=likes[id];

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

 const data=likes[id];

 if(
  !data||
  !data.times||
  !data.times.length
 ){

  return "좋아요 취소";

 }


 const now=Date.now();

 const canCancel=
 data.times.some(
  time=>
   now-time>=LIKE_CANCEL_DELAY
 );


 if(canCancel){

  return "좋아요 취소";

 }


 const earliest=
 Math.min(...data.times);


 const remain=
 Math.max(
  0,
  Math.ceil(
   (LIKE_CANCEL_DELAY-(now-earliest))/1000
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

 document.getElementById("modal")
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
 document.getElementById("checkPw").value;


 if(
  !e||
  !(pw===e.password||
    pw===MASTER_PASSWORD)
 ){

  document.getElementById("pwError")
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

const GAME_TIME=30;

const RANKING_KEY=
"daekwang_bigbit_math_ranking_v2";

const BEST_KEY=
"daekwang_bigbit_math_best_v2";


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
let gameTime=GAME_TIME;
let gameSolved=0;
let gameTimer=null;
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
   랜덤 기본 함수
===================================================== */

function randInt(min,max){

 return Math.floor(
  Math.random()*(max-min+1)
 )+min;

}


function randFloat(min,max){

 return Math.random()*(max-min)+min;

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

 if(d===1)return String(n);

 return `${n}/${d}`;

}


/* =====================================================
   보기용 값
===================================================== */

function formatNumber(value){

 if(
  typeof value==="number" &&
  Number.isFinite(value)
 ){

  if(
   Math.abs(
    value-Math.round(value)
   )<1e-10
  ){

   return String(
    Math.round(value)
   );

  }

  return String(
   Math.round(value*100)/100
  );

 }

 return String(value);

}


/* =====================================================
   난이도 선택
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


/* =====================================================
   랜덤 선택
===================================================== */

function randomChoice(array){

 return array[
  Math.floor(
   Math.random()*array.length
  )
 ];

}


/* =====================================================
   유형 ID가 연속되지 않게 선택
===================================================== */

function chooseType(types){

 if(types.length===1){

  return types[0];

 }

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
  "k_add_small",
  "k_sub_small",
  "k_compare",
  "k_count",
  "k_double",
  "k_half"
 ];

 const type=
  chooseType(types);

 let a,b,answer,question;


 if(type==="k_add_small"){

  a=randInt(1,10);
  b=randInt(1,10);

  answer=a+b;

  question=
   `${a} + ${b} = ?`;

 }


 else if(type==="k_sub_small"){

  a=randInt(2,15);
  b=randInt(1,a);

  answer=a-b;

  question=
   `${a} - ${b} = ?`;

 }


 else if(type==="k_compare"){

  a=randInt(1,20);
  b=randInt(1,20);

  answer=
   a>b
   ?a
   :a<b
   ?b
   :a;

  question=
   `다음 두 수 중 더 큰 수는? ${a} , ${b}`;

 }


 else if(type==="k_count"){

  const groups=randInt(2,5);
  const each=randInt(1,5);

  answer=groups*each;

  question=
   `사탕이 ${groups}묶음 있고, 한 묶음에 ${each}개가 있습니다. 모두 몇 개일까요?`;

 }


 else if(type==="k_double"){

  a=randInt(1,10);

  answer=a*2;

  question=
   `${a}의 2배는 얼마일까요?`;

 }


 else{

  a=randInt(2,20);

  answer=a/2;

  question=
   `${a}의 절반은 얼마일까요?`;

 }


 return {
  level:"kindergarten",
  type:type,
  question:question,
  answer:answer
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
  "el_missing"
 ];

 const type=
  chooseType(types);

 let question,answer;


 if(type==="el_add"){

  const a=randInt(10,99);
  const b=randInt(10,99);

  answer=a+b;

  question=
   `${a} + ${b} = ?`;

 }


 else if(type==="el_sub"){

  const a=randInt(30,180);
  const b=randInt(5,a);

  answer=a-b;

  question=
   `${a} - ${b} = ?`;

 }


 else if(type==="el_mul"){

  const a=randInt(2,12);
  const b=randInt(2,12);

  answer=a*b;

  question=
   `${a} × ${b} = ?`;

 }


 else if(type==="el_money"){

  const price=randInt(5,30)*100;
  const count=randInt(2,5);

  answer=price*count;

  question=
   `한 개에 ${price.toLocaleString()}원인 물건 ${count}개의 가격은?`;

 }


 else if(type==="el_time"){

  const hour=randInt(1,11);
  const add=randInt(1,6);

  answer=hour+add;

  question=
   `오후 ${hour}시에 시작해서 ${add}시간 후의 시간은?`;

 }


 else{

  const x=randInt(2,30);
  const b=randInt(1,20);
  const sum=x+b;

  answer=x;

  question=
   `□ + ${b} = ${sum}일 때 □는?`;

 }


 return {
  level:"elementaryLow",
  type:type,
  question:question,
  answer:answer
 };

}


/* =====================================================
   초등 고학년
===================================================== */

function generateElementaryHigh(){

 const types=[
  "eh_add_decimal",
  "eh_div",
  "eh_fraction",
  "eh_percent",
  "eh_area",
  "eh_average",
  "eh_ratio"
 ];

 const type=
  chooseType(types);

 let question,answer;


 if(type==="eh_add_decimal"){

  const a=randInt(10,99);
  const b=randInt(10,99);

  answer=a+b;

  question=
   `${a} + ${b} = ?`;

 }


 else if(type==="eh_div"){

  const b=randInt(2,12);
  const q=randInt(2,25);
  const a=b*q;

  answer=q;

  question=
   `${a} ÷ ${b} = ?`;

 }


 else if(type==="eh_fraction"){

  const d=randInt(2,10);
  const n=randInt(1,d-1);

  const d2=randInt(2,10);
  const n2=randInt(1,d2-1);

  answer=
   n/d+n2/d2;

  question=
   `${fraction(n,d)} + ${fraction(n2,d2)} = ?`;

 }


 else if(type==="eh_percent"){

  const base=randInt(2,20)*50;
  const p=randomChoice([10,20,25,30,40,50]);

  answer=base*p/100;

  question=
   `${base}의 ${p}%는?`;

 }


 else if(type==="eh_area"){

  const w=randInt(3,20);
  const h=randInt(3,20);

  answer=w*h;

  question=
   `가로 ${w}, 세로 ${h}인 직사각형의 넓이는?`;

 }


 else if(type==="eh_average"){

  const n=randInt(3,6);
  const values=[];

  for(let i=0;i<n;i++){

   values.push(
    randInt(5,30)
   );

  }

  const total=
   values.reduce(
    (a,b)=>a+b,
    0
   );

  answer=total/n;

  question=
   `${values.join(", ")}의 평균은?`;

 }


 else{

  const ratioA=randInt(2,9);
  const ratioB=randInt(2,9);
  const multiplier=randInt(2,8);

  const b=ratioB*multiplier;

  answer=ratioA*multiplier;

  question=
   `A:B=${ratioA}:${ratioB}이고 B=${b}일 때 A는?`;

 }


 return {
  level:"elementaryHigh",
  type:type,
  question:question,
  answer:answer
 };

}


/* =====================================================
   중학교
===================================================== */

function generateMiddle(){

 const types=[
  "m_linear",
  "m_system",
  "m_factor",
  "m_square",
  "m_percent_change",
  "m_probability",
  "m_pythagoras",
  "m_function"
 ];

 const type=
  chooseType(types);

 let question,answer;


 if(type==="m_linear"){

  const a=randInt(2,9);
  const x=randInt(-9,12);
  const b=randInt(-15,15);
  const c=a*x+b;

  answer=x;

  question=
   `${a}x ${b>=0?"+ "+b:"- "+Math.abs(b)} = ${c}일 때 x는?`;

 }


 else if(type==="m_system"){

  const x=randInt(1,9);
  const y=randInt(1,9);

  const a1=randInt(2,6);
  const b1=randInt(1,5);

  const a2=randInt(1,5);
  const b2=randInt(2,6);

  const c1=a1*x+b1*y;
  const c2=a2*x+b2*y;

  answer=x;

  question=
   `연립방정식 ${a1}x + ${b1}y = ${c1}, ${a2}x + ${b2}y = ${c2}일 때 x는?`;

 }


 else if(type==="m_factor"){

  const r1=randInt(-8,8);
  const r2=randInt(-8,8);

  answer=r1;

  question=
   `x² - ${(r1+r2)}x + ${r1*r2} = 0의 한 근은?`;

 }


 else if(type==="m_square"){

  const a=randInt(2,12);
  const b=randInt(2,12);

  answer=(a+b)*(a+b);

  question=
   `(${a}+${b})² = ?`;

 }


 else if(type==="m_percent_change"){

  const original=randInt(10,80)*100;
  const p=randomChoice([10,15,20,25,30]);

  answer=original*(100+p)/100;

  question=
   `가격이 ${original}원에서 ${p}% 상승했다면 새 가격은?`;

 }


 else if(type==="m_probability"){

  const red=randInt(1,8);
  const blue=randInt(1,8);
  const total=red+blue;

  answer=red/total;

  question=
   `빨간 공 ${red}개, 파란 공 ${blue}개가 있을 때 빨간 공을 뽑을 확률은?`;

 }


 else if(type==="m_pythagoras"){

  const a=randInt(3,12);
  const b=randInt(3,12);

  answer=Math.sqrt(a*a+b*b);

  question=
   `직각삼각형의 두 직각변이 ${a}, ${b}일 때 빗변의 길이는?`;

 }


 else{

  const a=randInt(2,8);
  const b=randInt(-10,10);

  const x=randInt(-5,10);

  answer=a*x+b;

  question=
   `f(x)=${a}x${b>=0?"+ "+b:"- "+Math.abs(b)}일 때 f(${x})는?`;

 }


 return {
  level:"middle",
  type:type,
  question:question,
  answer:answer
 };

}


/* =====================================================
   고등학교
===================================================== */

function generateHigh(){

 const types=[
  "h_quadratic_root",
  "h_log",
  "h_exponent",
  "h_trig",
  "h_sequence",
  "h_derivative_basic",
  "h_derivative_power",
  "h_probability_binomial",
  "h_combinatorics",
  "h_function_value"
 ];

 const type=
  chooseType(types);

 let question,answer;


 if(type==="h_quadratic_root"){

  const r1=randInt(-9,9);
  const r2=randInt(-9,9);

  const B=-(r1+r2);
  const C=r1*r2;

  answer=r1;

  question=
   `x² ${B>=0?"+ "+B:"- "+Math.abs(B)}x ${C>=0?"+ "+C:"- "+Math.abs(C)}=0의 한 근은?`;

 }


 else if(type==="h_log"){

  const base=randomChoice([2,3,4,5]);

  const exponent=randInt(2,6);

  const value=Math.pow(base,exponent);

  answer=exponent;

  question=
   `log_${base}(${value}) = ?`;

 }


 else if(type==="h_exponent"){

  const base=randomChoice([2,3,5]);

  const a=randInt(2,6);
  const b=randInt(1,4);

  answer=Math.pow(base,a+b);

  question=
   `${base}^${a} × ${base}^${b} = ?`;

 }


 else if(type==="h_trig"){

  const data=randomChoice([
   {q:"sin 30°",a:0.5},
   {q:"cos 60°",a:0.5},
   {q:"sin 90°",a:1},
   {q:"cos 0°",a:1},
   {q:"tan 45°",a:1}
  ]);

  answer=data.a;

  question=
   `${data.q} = ?`;

 }


 else if(type==="h_sequence"){

  const first=randInt(1,10);
  const d=randInt(2,8);
  const n=randInt(5,15);

  answer=first+(n-1)*d;

  question=
   `등차수열의 첫째항이 ${first}, 공차가 ${d}일 때 ${n}번째 항은?`;

 }


 else if(type==="h_derivative_basic"){

  const a=randInt(2,12);

  answer=a;

  question=
   `f(x)=${a}x일 때 f'(x)는?`;

 }


 else if(type==="h_derivative_power"){

  const n=randInt(2,6);
  const x=randInt(1,8);

  answer=n*Math.pow(x,n-1);

  question=
   `f(x)=x^${n}일 때 f'(${x})는?`;

 }


 else if(type==="h_probability_binomial"){

  const n=randInt(3,6);
  const success=randInt(0,n);

  const p=0.5;

  answer=
   Math.round(
    1000000*
    (
     combination(n,success)*
     Math.pow(p,success)*
     Math.pow(1-p,n-success)
    )
   )/1000000;

  question=
   `동전을 ${n}번 던질 때 앞면이 정확히 ${success}번 나올 확률은?`;

 }


 else if(type==="h_combinatorics"){

  const n=randInt(5,10);
  const r=randInt(2,n-2);

  answer=combination(n,r);

  question=
   `C(${n},${r}) = ?`;

 }


 else{

  const a=randInt(2,8);
  const x=randInt(-5,8);
  const b=randInt(-12,12);

  answer=a*x*x+b;

  question=
   `f(x)=${a}x² ${b>=0?"+ "+b:"- "+Math.abs(b)}일 때 f(${x})는?`;

 }


 return {
  level:"high",
  type:type,
  question:question,
  answer:answer
 };

}


/* =====================================================
   대학
===================================================== */

function generateUniversity(){

 const types=[
  "u_integral_power",
  "u_integral_linear",
  "u_derivative_product",
  "u_matrix_trace",
  "u_determinant",
  "u_probability",
  "u_complex_abs",
  "u_limit_linear",
  "u_vector_dot",
  "u_stat_mean"
 ];

 const type=
  chooseType(types);

 let question,answer;


 if(type==="u_integral_power"){

  const n=randInt(2,8);

  answer=
   n*n*n/3;

  question=
   `∫₀^${n} x² dx = ?`;

 }


 else if(type==="u_integral_linear"){

  const a=randInt(2,9);
  const b=randInt(1,8);
  const upper=randInt(2,7);

  answer=
   a*upper*upper/2+
   b*upper;

  question=
   `∫₀^${upper} (${a}x + ${b}) dx = ?`;

 }


 else if(type==="u_derivative_product"){

  const a=randInt(2,8);
  const x=randInt(1,6);

  answer=
   2*a*x+a;

  question=
   `f(x)=x²·${a}x 일 때 f'(${x})는?`;

 }


 else if(type==="u_matrix_trace"){

  const a=randInt(1,9);
  const b=randInt(1,9);

  answer=a+b;

  question=
   `행렬 [[${a},0],[0,${b}]]의 trace는?`;

 }


 else if(type==="u_determinant"){

  const a=randInt(1,8);
  const b=randInt(1,8);
  const c=randInt(1,8);
  const d=randInt(1,8);

  answer=a*d-b*c;

  question=
   `det [[${a},${b}],[${c},${d}]] = ?`;

 }


 else if(type==="u_probability"){

  const success=randInt(2,7);
  const total=randInt(success+1,12);

  answer=
   success/total;

  question=
   `성공 ${success}회 / 전체 ${total}회일 때 경험적 확률은?`;

 }


 else if(type==="u_complex_abs"){

  const a=randInt(1,8);
  const b=randInt(1,8);

  answer=
   Math.sqrt(a*a+b*b);

  question=
   `z=${a}+${b}i일 때 |z|는?`;

 }


 else if(type==="u_limit_linear"){

  const a=randInt(2,9);
  const b=randInt(1,9);
  const x=randInt(1,7);

  answer=a*x+b;

  question=
   `lim(x→${x}) (${a}x + ${b}) = ?`;

 }


 else if(type==="u_vector_dot"){

  const a=randInt(1,8);
  const b=randInt(1,8);
  const c=randInt(1,8);
  const d=randInt(1,8);

  answer=a*c+b*d;

  question=
   `벡터 (${a},${b})·(${c},${d}) = ?`;

 }


 else{

  const count=randInt(3,6);
  const values=[];

  for(let i=0;i<count;i++){

   values.push(
    randInt(10,40)
   );

  }

  const total=
   values.reduce(
    (sum,v)=>sum+v,
    0
   );

  answer=total/count;

  question=
   `자료 ${values.join(", ")}의 산술평균은?`;

 }


 return {
  level:"university",
  type:type,
  question:question,
  answer:answer
 };

}


/* =====================================================
   대학 심화
===================================================== */

function generateUniversityHard(){

 const types=[
  "uh_integral_trig",
  "uh_derivative_chain",
  "uh_matrix_det3",
  "uh_complex_square",
  "uh_expectation",
  "uh_eigen_simple",
  "uh_series",
  "uh_vector_cross",
  "uh_log_derivative"
 ];

 const type=
  chooseType(types);

 let question,answer;


 if(type==="uh_integral_trig"){

  const n=randInt(1,7);

  answer=
   2;

  question=
   `∫₀^π ${n}sin(x) dx ÷ ${n} = ?`;

 }


 else if(type==="uh_derivative_chain"){

  const a=randInt(2,7);
  const x=randInt(1,6);

  answer=
   2*a*x;

  question=
   `f(x)=(${a}x)²일 때 f'(${x})는?`;

 }


 else if(type==="uh_matrix_det3"){

  const a=randInt(1,5);
  const b=randInt(1,5);
  const c=randInt(1,5);

  answer=a*b*c;

  question=
   `대각행렬 diag(${a},${b},${c})의 행렬식은?`;

 }


 else if(type==="uh_complex_square"){

  const a=randInt(1,7);

  answer=-(a*a);

  question=
   `복소수 z=${a}i일 때 z²는?`;

 }


 else if(type==="uh_expectation"){

  const x1=randInt(1,5);
  const x2=randInt(6,10);

  const p=randomChoice([0.2,0.3,0.4,0.6,0.7,0.8]);

  answer=
   p*x1+(1-p)*x2;

  question=
   `X가 ${x1}을 확률 ${p}, ${x2}를 확률 ${1-p}로 가질 때 E[X]는?`;

 }


 else if(type==="uh_eigen_simple"){

  const a=randInt(2,9);
  const b=randInt(2,9);

  answer=a;

  question=
   `행렬 [[${a},0],[0,${b}]]의 고유값 중 작은 값은?`;

 }


 else if(type==="uh_series"){

  const a=randInt(1,5);
  const r=randInt(1,3);
  const n=randInt(3,7);

  if(r===1){

   answer=a*n;

   question=
    `수열 ${a},${a},${a},...의 첫 ${n}개 항의 합은?`;

  }else{

   answer=
    a*(Math.pow(r,n)-1)/(r-1);

   question=
    `등비수열의 첫째항 ${a}, 공비 ${r}일 때 첫 ${n}개 항의 합은?`;

  }

 }


 else if(type==="uh_vector_cross"){

  const a=randInt(1,5);
  const b=randInt(1,5);

  answer=a*b;

  question=
   `벡터 (${a},0,0) × (0,${b},0)의 크기는?`;

 }


 else{

  const a=randInt(2,9);

  answer=1;

  question=
   `f(x)=ln(${a}x)의 도함수에서 x=1/${a}일 때의 값은?`;

 }


 return {
  level:"universityHard",
  type:type,
  question:question,
  answer:answer
 };

}


/* =====================================================
   조합
===================================================== */

function combination(n,r){

 if(
  r<0||
  r>n
 ){
  return 0;
 }

 r=Math.min(r,n-r);

 let result=1;

 for(let i=1;i<=r;i++){

  result=
   result*(n-r+i)/i;

 }

 return Math.round(result);

}


/* =====================================================
   최종 문제 생성
===================================================== */

function createQuestion(){

 let question=null;

 let attempts=0;


 while(attempts<300){

  attempts++;


  const level=
   chooseDifficulty();


  if(level==="kindergarten"){
   question=
    generateKindergarten();
  }
  else if(level==="elementaryLow"){
   question=
    generateElementaryLow();
  }
  else if(level==="elementaryHigh"){
   question=
    generateElementaryHigh();
  }
  else if(level==="middle"){
   question=
    generateMiddle();
  }
  else if(level==="high"){
   question=
    generateHigh();
  }
  else if(level==="university"){
   question=
    generateUniversity();
  }
  else{
   question=
    generateUniversityHard();
  }


  /* 같은 유형 연속 방지 */

  if(
   question.type===lastQuestionType
  ){

   continue;

  }


  /* 문제 자체 중복 방지 */

  const key=
   `${question.level}|${question.type}|${question.question}|${formatNumber(question.answer)}`;


  if(
   usedQuestionKeys.has(key)
  ){

   continue;

  }


  usedQuestionKeys.add(key);

  lastQuestionType=
   question.type;

  question.key=
   key;

  return question;

 }


 /* 혹시라도 300회 실패하면 강제로 새로운 기본 문제 */

 const a=randInt(1,100);
 const b=randInt(1,100);

 const fallback={
  level:"elementaryLow",
  type:"fallback_"+Date.now(),
  question:`${a} + ${b} = ?`,
  answer:a+b
 };

 lastQuestionType=
  fallback.type;

 return fallback;

}


/* =====================================================
   오답 보기 만들기
===================================================== */

function makeChoices(answer,level){

 const choices=[
  answer
 ];

 let attempts=0;


 function different(value){

  return !choices.some(
   existing=>
    Math.abs(
     Number(existing)-Number(value)
    )<0.000001
  );

 }


 while(
  choices.length<5 &&
  attempts<500
 ){

  attempts++;


  let offset;


  if(
   typeof answer==="number" &&
   Number.isFinite(answer)
  ){

   const magnitude=
    Math.max(
     1,
     Math.abs(answer)
    );


   if(
    level==="kindergarten"
   ){

    offset=randInt(1,5);

   }
   else if(
    level==="elementaryLow"
   ){

    offset=randInt(1,10);

   }
   else if(
    level==="elementaryHigh"
   ){

    offset=randInt(1,15);

   }
   else if(
    level==="middle"
   ){

    offset=randInt(1,20);

   }
   else if(
    level==="high"
   ){

    offset=randInt(1,25);

   }
   else{

    offset=
     Math.max(
      1,
      Math.round(
       magnitude*
       randFloat(.08,.35)
      )
     );

   }


   const direction=
    Math.random()<.5
    ?-1
    :1;


   let wrong=
    answer+
    direction*offset;


   if(
    Math.random()<.35
   ){

    wrong=
     answer+
     randInt(-3,3);

   }


   if(
    !Number.isInteger(answer)
   ){

    wrong=
     Math.round(
      wrong*100
     )/100;

   }


   if(
    different(wrong)
   ){

    choices.push(wrong);

   }

  }

 }


 /* 안전망 */

 while(choices.length<5){

  let extra=
   typeof answer==="number"
   ?
   answer+choices.length*7+3
   :
   "보기 "+(choices.length+1);


  if(
   typeof extra==="number" &&
   !different(extra)
  ){

   extra+=13;

  }


  if(different(extra)){

   choices.push(extra);

  }

 }


 /* 섞기 */

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
   보기 표시
===================================================== */

function showQuestion(){

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
  "①",
  "②",
  "③",
  "④",
  "⑤"
 ];


 choices.forEach(
  (choice,index)=>{

   const button=
    document.createElement("button");

   button.className=
    "choice-btn";

   button.textContent=
    `${labels[index]} ${formatNumber(choice)}`;


   button.addEventListener(
    "click",
    ()=>{
     answerQuestion(
      index,
      button
     );
    }
   );


   box.appendChild(button);

  }
 );


 document.getElementById("gameMessage")
 .textContent=
 "정답이라고 생각하는 답을 선택하세요.";

}


/* =====================================================
   정답 처리
===================================================== */

function answerQuestion(
 index,
 clickedButton
){

 if(!gameRunning)return;


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


  document.getElementById("gameScore")
  .textContent=
   gameScore;


  document.getElementById("gameSolved")
  .textContent=
   gameSolved;


  document.getElementById("gameMessage")
  .textContent=
   `정답! +${points}점`;

 }
 else{

  clickedButton.classList.add(
   "wrong"
  );


  buttons.forEach(
   button=>{

    const text=
     button.textContent
      .replace(
       /^[①②③④⑤]\s*/,
       ""
      )
      .trim();


    if(
     Math.abs(
      Number(text)-
      Number(currentQuestion.answer)
     )<0.000001
    ){

     button.classList.add(
      "correct"
     );

    }

   }
  );


  document.getElementById(
   "gameMessage"
  ).textContent=
   `오답! 정답은 ${formatNumber(currentQuestion.answer)}입니다.`;

 }


 setTimeout(
  ()=>{

   if(gameRunning){

    showQuestion();

   }

  },
  350
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

 gameScore=0;

 gameTime=GAME_TIME;

 gameSolved=0;

 currentQuestion=null;

 usedQuestionKeys=
  new Set();

 lastQuestionType=
  null;


 document.getElementById("gameScore")
 .textContent="0";

 document.getElementById("gameTime")
 .textContent=
  GAME_TIME;

 document.getElementById("gameSolved")
 .textContent="0";

 document.getElementById(
  "gameMessage"
 ).textContent=
  "게임 시작!";


 document.getElementById("result")
 .classList
 .remove("show");


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
  "gameMessage"
 ).textContent=
  "시간 종료!";


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
 ).classList.add("show");


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
   좋아요 1초 갱신
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

</script>

</body>
</html>
```
