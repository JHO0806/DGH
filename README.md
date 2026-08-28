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
}

input,textarea,button{font:inherit}

/* =========================
   배경
========================= */

body::before{
 content:"";
 position:fixed;
 inset:0;
 background:
 radial-gradient(circle at 15% 20%,rgba(137,39,70,.045),transparent 25%),
 radial-gradient(circle at 85% 75%,rgba(137,39,70,.035),transparent 28%);
 pointer-events:none;
 z-index:-2;
}


/* =========================
   대광고 로고 애니메이션
========================= */

.logo-float{
 position:fixed;
 left:0;
 top:0;
 width:68px;
 height:68px;
 z-index:0;
 pointer-events:none;
 opacity:.14;
 filter:blur(.2px);
 will-change:transform;
}

/* 회전 없음 */

.logo-float-1{
 animation:moveLogo1 17s linear infinite;
 animation-delay:-1s;
}

.logo-float-2{
 width:58px;
 height:58px;
 animation:moveLogo2 20s linear infinite;
 animation-delay:-7s;
}

.logo-float-3{
 width:52px;
 height:52px;
 animation:moveLogo3 18s linear infinite;
 animation-delay:-12s;
}

.logo-float-4{
 width:62px;
 height:62px;
 animation:moveLogo4 21s linear infinite;
 animation-delay:-4s;
}

.logo-float-5{
 width:48px;
 height:48px;
 animation:moveLogo5 16s linear infinite;
 animation-delay:-9s;
}

.logo-float-6{
 width:56px;
 height:56px;
 animation:moveLogo6 23s linear infinite;
 animation-delay:-17s;
}

.logo-float-7{
 width:64px;
 height:64px;
 animation:moveLogo7 19s linear infinite;
 animation-delay:-14s;
}

.logo-float-8{
 width:50px;
 height:50px;
 animation:moveLogo8 22s linear infinite;
 animation-delay:-3s;
}

.logo-float-9{
 width:60px;
 height:60px;
 animation:moveLogo9 18s linear infinite;
 animation-delay:-6s;
}

.logo-float-10{
 width:45px;
 height:45px;
 animation:moveLogo10 21s linear infinite;
 animation-delay:-15s;
}

.logo-float-11{
 width:54px;
 height:54px;
 animation:moveLogo11 17s linear infinite;
 animation-delay:-11s;
}

.logo-float-12{
 width:66px;
 height:66px;
 animation:moveLogo12 24s linear infinite;
 animation-delay:-20s;
}


/* =========================
   아래에서 오른쪽 위로 이동
   모든 로고 정방향 고정
========================= */

@keyframes moveLogo1{
 0%{transform:translate3d(3vw,118vh,0)}
 100%{transform:translate3d(78vw,-18vh,0)}
}

@keyframes moveLogo2{
 0%{transform:translate3d(18vw,120vh,0)}
 100%{transform:translate3d(102vw,-17vh,0)}
}

@keyframes moveLogo3{
 0%{transform:translate3d(36vw,119vh,0)}
 100%{transform:translate3d(118vw,-15vh,0)}
}

@keyframes moveLogo4{
 0%{transform:translate3d(-8vw,116vh,0)}
 100%{transform:translate3d(72vw,-18vh,0)}
}

@keyframes moveLogo5{
 0%{transform:translate3d(52vw,121vh,0)}
 100%{transform:translate3d(125vw,-16vh,0)}
}

@keyframes moveLogo6{
 0%{transform:translate3d(8vw,120vh,0)}
 100%{transform:translate3d(93vw,-20vh,0)}
}

@keyframes moveLogo7{
 0%{transform:translate3d(67vw,120vh,0)}
 100%{transform:translate3d(128vw,-13vh,0)}
}

@keyframes moveLogo8{
 0%{transform:translate3d(27vw,122vh,0)}
 100%{transform:translate3d(111vw,-19vh,0)}
}

@keyframes moveLogo9{
 0%{transform:translate3d(-4vw,121vh,0)}
 100%{transform:translate3d(86vw,-16vh,0)}
}

@keyframes moveLogo10{
 0%{transform:translate3d(44vw,123vh,0)}
 100%{transform:translate3d(118vw,-18vh,0)}
}

@keyframes moveLogo11{
 0%{transform:translate3d(74vw,121vh,0)}
 100%{transform:translate3d(132vw,-14vh,0)}
}

@keyframes moveLogo12{
 0%{transform:translate3d(12vw,123vh,0)}
 100%{transform:translate3d(104vw,-21vh,0)}
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
   본문
========================= */

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


/* =========================
   푸터
========================= */

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

 .like-area{
  width:100%;
 }

 .logo-float{
  opacity:.11;
 }

 .logo-float-1{width:54px;height:54px}
 .logo-float-2{width:47px;height:47px}
 .logo-float-3{width:42px;height:42px}
 .logo-float-4{width:50px;height:50px}
 .logo-float-5{width:39px;height:39px}
 .logo-float-6{width:45px;height:45px}
 .logo-float-7{width:51px;height:51px}
 .logo-float-8{width:41px;height:41px}
 .logo-float-9{width:48px;height:48px}
 .logo-float-10{width:37px;height:37px}
 .logo-float-11{width:44px;height:44px}
 .logo-float-12{width:52px;height:52px}
}
</style>

</head>

<body>

<!-- =====================================================
     움직이는 대광고 로고 12개
     SVG 방식이라 확대/축소해도 깨지지 않음
====================================================== -->

<div class="logo-float logo-float-1">
<svg viewBox="0 0 200 200" width="100%" height="100%" xmlns="http://www.w3.org/2000/svg">
<circle cx="100" cy="100" r="94" fill="#8a2340"/>
<circle cx="100" cy="100" r="76" fill="none" stroke="#fff" stroke-width="8"/>
<path d="M58 63 Q100 42 142 63 L136 118 Q132 146 100 163 Q68 146 64 118 Z" fill="#8a2340" stroke="#fff" stroke-width="3"/>
<path d="M74 72 L88 61 L100 72 L112 61 L126 72 L126 83 L74 83 Z" fill="#fff"/>
<text x="100" y="101" text-anchor="middle" fill="#fff" font-family="Georgia,serif" font-size="13" font-weight="700">LUX ET SAL</text>
<text x="100" y="128" text-anchor="middle" fill="#fff" font-family="serif" font-size="27" font-weight="700">大光</text>
<text x="100" y="28" text-anchor="middle" fill="#fff" font-family="Georgia,serif" font-size="9" font-weight="700">DAE GWANG HIGH SCHOOL</text>
<text x="100" y="185" text-anchor="middle" fill="#fff" font-family="serif" font-size="9" font-weight="700">대 광 고 등 학 교</text>
</svg>
</div>

<div class="logo-float logo-float-2">
<svg viewBox="0 0 200 200" width="100%" height="100%" xmlns="http://www.w3.org/2000/svg">
<circle cx="100" cy="100" r="94" fill="#8a2340"/>
<circle cx="100" cy="100" r="76" fill="none" stroke="#fff" stroke-width="8"/>
<path d="M58 63 Q100 42 142 63 L136 118 Q132 146 100 163 Q68 146 64 118 Z" fill="#8a2340" stroke="#fff" stroke-width="3"/>
<path d="M74 72 L88 61 L100 72 L112 61 L126 72 L126 83 L74 83 Z" fill="#fff"/>
<text x="100" y="101" text-anchor="middle" fill="#fff" font-family="Georgia,serif" font-size="13" font-weight="700">LUX ET SAL</text>
<text x="100" y="128" text-anchor="middle" fill="#fff" font-family="serif" font-size="27" font-weight="700">大光</text>
<text x="100" y="28" text-anchor="middle" fill="#fff" font-family="Georgia,serif" font-size="9" font-weight="700">DAE GWANG HIGH SCHOOL</text>
<text x="100" y="185" text-anchor="middle" fill="#fff" font-family="serif" font-size="9" font-weight="700">대 광 고 등 학 교</text>
</svg>
</div>

<div class="logo-float logo-float-3">
<svg viewBox="0 0 200 200" width="100%" height="100%" xmlns="http://www.w3.org/2000/svg">
<circle cx="100" cy="100" r="94" fill="#8a2340"/>
<circle cx="100" cy="100" r="76" fill="none" stroke="#fff" stroke-width="8"/>
<path d="M58 63 Q100 42 142 63 L136 118 Q132 146 100 163 Q68 146 64 118 Z" fill="#8a2340" stroke="#fff" stroke-width="3"/>
<path d="M74 72 L88 61 L100 72 L112 61 L126 72 L126 83 L74 83 Z" fill="#fff"/>
<text x="100" y="101" text-anchor="middle" fill="#fff" font-family="Georgia,serif" font-size="13" font-weight="700">LUX ET SAL</text>
<text x="100" y="128" text-anchor="middle" fill="#fff" font-family="serif" font-size="27" font-weight="700">大光</text>
<text x="100" y="28" text-anchor="middle" fill="#fff" font-family="Georgia,serif" font-size="9" font-weight="700">DAE GWANG HIGH SCHOOL</text>
<text x="100" y="185" text-anchor="middle" fill="#fff" font-family="serif" font-size="9" font-weight="700">대 광 고 등 학 교</text>
</svg>
</div>

<div class="logo-float logo-float-4">
<svg viewBox="0 0 200 200" width="100%" height="100%" xmlns="http://www.w3.org/2000/svg">
<circle cx="100" cy="100" r="94" fill="#8a2340"/>
<circle cx="100" cy="100" r="76" fill="none" stroke="#fff" stroke-width="8"/>
<path d="M58 63 Q100 42 142 63 L136 118 Q132 146 100 163 Q68 146 64 118 Z" fill="#8a2340" stroke="#fff" stroke-width="3"/>
<path d="M74 72 L88 61 L100 72 L112 61 L126 72 L126 83 L74 83 Z" fill="#fff"/>
<text x="100" y="101" text-anchor="middle" fill="#fff" font-family="Georgia,serif" font-size="13" font-weight="700">LUX ET SAL</text>
<text x="100" y="128" text-anchor="middle" fill="#fff" font-family="serif" font-size="27" font-weight="700">大光</text>
<text x="100" y="28" text-anchor="middle" fill="#fff" font-family="Georgia,serif" font-size="9" font-weight="700">DAE GWANG HIGH SCHOOL</text>
<text x="100" y="185" text-anchor="middle" fill="#fff" font-family="serif" font-size="9" font-weight="700">대 광 고 등 학 교</text>
</svg>
</div>

<div class="logo-float logo-float-5">
<svg viewBox="0 0 200 200" width="100%" height="100%" xmlns="http://www.w3.org/2000/svg">
<circle cx="100" cy="100" r="94" fill="#8a2340"/>
<circle cx="100" cy="100" r="76" fill="none" stroke="#fff" stroke-width="8"/>
<path d="M58 63 Q100 42 142 63 L136 118 Q132 146 100 163 Q68 146 64 118 Z" fill="#8a2340" stroke="#fff" stroke-width="3"/>
<path d="M74 72 L88 61 L100 72 L112 61 L126 72 L126 83 L74 83 Z" fill="#fff"/>
<text x="100" y="101" text-anchor="middle" fill="#fff" font-family="Georgia,serif" font-size="13" font-weight="700">LUX ET SAL</text>
<text x="100" y="128" text-anchor="middle" fill="#fff" font-family="serif" font-size="27" font-weight="700">大光</text>
<text x="100" y="28" text-anchor="middle" fill="#fff" font-family="Georgia,serif" font-size="9" font-weight="700">DAE GWANG HIGH SCHOOL</text>
<text x="100" y="185" text-anchor="middle" fill="#fff" font-family="serif" font-size="9" font-weight="700">대 광 고 등 학 교</text>
</svg>
</div>

<div class="logo-float logo-float-6">
<svg viewBox="0 0 200 200" width="100%" height="100%" xmlns="http://www.w3.org/2000/svg">
<circle cx="100" cy="100" r="94" fill="#8a2340"/>
<circle cx="100" cy="100" r="76" fill="none" stroke="#fff" stroke-width="8"/>
<path d="M58 63 Q100 42 142 63 L136 118 Q132 146 100 163 Q68 146 64 118 Z" fill="#8a2340" stroke="#fff" stroke-width="3"/>
<path d="M74 72 L88 61 L100 72 L112 61 L126 72 L126 83 L74 83 Z" fill="#fff"/>
<text x="100" y="101" text-anchor="middle" fill="#fff" font-family="Georgia,serif" font-size="13" font-weight="700">LUX ET SAL</text>
<text x="100" y="128" text-anchor="middle" fill="#fff" font-family="serif" font-size="27" font-weight="700">大光</text>
<text x="100" y="28" text-anchor="middle" fill="#fff" font-family="Georgia,serif" font-size="9" font-weight="700">DAE GWANG HIGH SCHOOL</text>
<text x="100" y="185" text-anchor="middle" fill="#fff" font-family="serif" font-size="9" font-weight="700">대 광 고 등 학 교</text>
</svg>
</div>

<div class="logo-float logo-float-7">
<svg viewBox="0 0 200 200" width="100%" height="100%" xmlns="http://www.w3.org/2000/svg">
<circle cx="100" cy="100" r="94" fill="#8a2340"/>
<circle cx="100" cy="100" r="76" fill="none" stroke="#fff" stroke-width="8"/>
<path d="M58 63 Q100 42 142 63 L136 118 Q132 146 100 163 Q68 146 64 118 Z" fill="#8a2340" stroke="#fff" stroke-width="3"/>
<path d="M74 72 L88 61 L100 72 L112 61 L126 72 L126 83 L74 83 Z" fill="#fff"/>
<text x="100" y="101" text-anchor="middle" fill="#fff" font-family="Georgia,serif" font-size="13" font-weight="700">LUX ET SAL</text>
<text x="100" y="128" text-anchor="middle" fill="#fff" font-family="serif" font-size="27" font-weight="700">大光</text>
<text x="100" y="28" text-anchor="middle" fill="#fff" font-family="Georgia,serif" font-size="9" font-weight="700">DAE GWANG HIGH SCHOOL</text>
<text x="100" y="185" text-anchor="middle" fill="#fff" font-family="serif" font-size="9" font-weight="700">대 광 고 등 학 교</text>
</svg>
</div>

<div class="logo-float logo-float-8">
<svg viewBox="0 0 200 200" width="100%" height="100%" xmlns="http://www.w3.org/2000/svg">
<circle cx="100" cy="100" r="94" fill="#8a2340"/>
<circle cx="100" cy="100" r="76" fill="none" stroke="#fff" stroke-width="8"/>
<path d="M58 63 Q100 42 142 63 L136 118 Q132 146 100 163 Q68 146 64 118 Z" fill="#8a2340" stroke="#fff" stroke-width="3"/>
<path d="M74 72 L88 61 L100 72 L112 61 L126 72 L126 83 L74 83 Z" fill="#fff"/>
<text x="100" y="101" text-anchor="middle" fill="#fff" font-family="Georgia,serif" font-size="13" font-weight="700">LUX ET SAL</text>
<text x="100" y="128" text-anchor="middle" fill="#fff" font-family="serif" font-size="27" font-weight="700">大光</text>
<text x="100" y="28" text-anchor="middle" fill="#fff" font-family="Georgia,serif" font-size="9" font-weight="700">DAE GWANG HIGH SCHOOL</text>
<text x="100" y="185" text-anchor="middle" fill="#fff" font-family="serif" font-size="9" font-weight="700">대 광 고 등 학 교</text>
</svg>
</div>

<div class="logo-float logo-float-9">
<svg viewBox="0 0 200 200" width="100%" height="100%" xmlns="http://www.w3.org/2000/svg">
<circle cx="100" cy="100" r="94" fill="#8a2340"/>
<circle cx="100" cy="100" r="76" fill="none" stroke="#fff" stroke-width="8"/>
<path d="M58 63 Q100 42 142 63 L136 118 Q132 146 100 163 Q68 146 64 118 Z" fill="#8a2340" stroke="#fff" stroke-width="3"/>
<path d="M74 72 L88 61 L100 72 L112 61 L126 72 L126 83 L74 83 Z" fill="#fff"/>
<text x="100" y="101" text-anchor="middle" fill="#fff" font-family="Georgia,serif" font-size="13" font-weight="700">LUX ET SAL</text>
<text x="100" y="128" text-anchor="middle" fill="#fff" font-family="serif" font-size="27" font-weight="700">大光</text>
<text x="100" y="28" text-anchor="middle" fill="#fff" font-family="Georgia,serif" font-size="9" font-weight="700">DAE GWANG HIGH SCHOOL</text>
<text x="100" y="185" text-anchor="middle" fill="#fff" font-family="serif" font-size="9" font-weight="700">대 광 고 등 학 교</text>
</svg>
</div>

<div class="logo-float logo-float-10">
<svg viewBox="0 0 200 200" width="100%" height="100%" xmlns="http://www.w3.org/2000/svg">
<circle cx="100" cy="100" r="94" fill="#8a2340"/>
<circle cx="100" cy="100" r="76" fill="none" stroke="#fff" stroke-width="8"/>
<path d="M58 63 Q100 42 142 63 L136 118 Q132 146 100 163 Q68 146 64 118 Z" fill="#8a2340" stroke="#fff" stroke-width="3"/>
<path d="M74 72 L88 61 L100 72 L112 61 L126 72 L126 83 L74 83 Z" fill="#fff"/>
<text x="100" y="101" text-anchor="middle" fill="#fff" font-family="Georgia,serif" font-size="13" font-weight="700">LUX ET SAL</text>
<text x="100" y="128" text-anchor="middle" fill="#fff" font-family="serif" font-size="27" font-weight="700">大光</text>
<text x="100" y="28" text-anchor="middle" fill="#fff" font-family="Georgia,serif" font-size="9" font-weight="700">DAE GWANG HIGH SCHOOL</text>
<text x="100" y="185" text-anchor="middle" fill="#fff" font-family="serif" font-size="9" font-weight="700">대 광 고 등 학 교</text>
</svg>
</div>

<div class="logo-float logo-float-11">
<svg viewBox="0 0 200 200" width="100%" height="100%" xmlns="http://www.w3.org/2000/svg">
<circle cx="100" cy="100" r="94" fill="#8a2340"/>
<circle cx="100" cy="100" r="76" fill="none" stroke="#fff" stroke-width="8"/>
<path d="M58 63 Q100 42 142 63 L136 118 Q132 146 100 163 Q68 146 64 118 Z" fill="#8a2340" stroke="#fff" stroke-width="3"/>
<path d="M74 72 L88 61 L100 72 L112 61 L126 72 L126 83 L74 83 Z" fill="#fff"/>
<text x="100" y="101" text-anchor="middle" fill="#fff" font-family="Georgia,serif" font-size="13" font-weight="700">LUX ET SAL</text>
<text x="100" y="128" text-anchor="middle" fill="#fff" font-family="serif" font-size="27" font-weight="700">大光</text>
<text x="100" y="28" text-anchor="middle" fill="#fff" font-family="Georgia,serif" font-size="9" font-weight="700">DAE GWANG HIGH SCHOOL</text>
<text x="100" y="185" text-anchor="middle" fill="#fff" font-family="serif" font-size="9" font-weight="700">대 광 고 등 학 교</text>
</svg>
</div>

<div class="logo-float logo-float-12">
<svg viewBox="0 0 200 200" width="100%" height="100%" xmlns="http://www.w3.org/2000/svg">
<circle cx="100" cy="100" r="94" fill="#8a2340"/>
<circle cx="100" cy="100" r="76" fill="none" stroke="#fff" stroke-width="8"/>
<path d="M58 63 Q100 42 142 63 L136 118 Q132 146 100 163 Q68 146 64 118 Z" fill="#8a2340" stroke="#fff" stroke-width="3"/>
<path d="M74 72 L88 61 L100 72 L112 61 L126 72 L126 83 L74 83 Z" fill="#fff"/>
<text x="100" y="101" text-anchor="middle" fill="#fff" font-family="Georgia,serif" font-size="13" font-weight="700">LUX ET SAL</text>
<text x="100" y="128" text-anchor="middle" fill="#fff" font-family="serif" font-size="27" font-weight="700">大光</text>
<text x="100" y="28" text-anchor="middle" fill="#fff" font-family="Georgia,serif" font-size="9" font-weight="700">DAE GWANG HIGH SCHOOL</text>
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

<div class="sub">
우리들의 축제, 우리들의 기록 · 큰빛축제 방문록
</div>

</div>

</div>

</header>

<!-- =========================
     방문록 입력
========================= -->

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

<button onclick="addEntry()">
방문록 등록
</button>

</div>

<div class="hint">
※ 작성할 때 입력한 비밀번호로 본인 글을 수정·삭제할 수 있습니다.
</div>

</section>

<!-- =========================
     방문록 목록
========================= -->

<section class="panel">

<h2>
📖 큰빛축제 방문록
<span id="count" class="tag">0개</span>
</h2>

<div id="entries"></div>

</section>

</main>

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
   수정 / 삭제
================================ */

function requestAction(action,id){

 pending={
  action:action,
  id:id
 };

 document.getElementById("checkPw").value="";

 document.getElementById("pwError").textContent="";

 document.getElementById("modalTitle")
 .textContent =
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
   좋아요 취소 타이머
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
