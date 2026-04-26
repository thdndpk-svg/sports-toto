<!DOCTYPE html>
<html lang="ko">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width,initial-scale=1.0,maximum-scale=1,user-scalable=0"/>
<title>WIN-4 스포츠 분석 Pro</title>
<style>
*{box-sizing:border-box;margin:0;padding:0;}
:root{
  --bg:#0f1117;--bg2:#1a1d27;--bg3:#22263a;
  --card:#1e2235;--line:#2d3250;
  --text:#e8eaf6;--sub:#7986cb;--muted:#4a5280;
  --gold:#ffd700;--gold2:#ffb300;
  --green:#00e676;--green2:#1de9b6;
  --red:#ff5252;--blue:#448aff;--purple:#e040fb;
}
html,body{min-height:100vh;background:var(--bg);color:var(--text);font-family:-apple-system,BlinkMacSystemFont,"Segoe UI","Apple SD Gothic Neo","Malgun Gothic",sans-serif;-webkit-text-size-adjust:100%;}

/* 네비 */
.nav{position:sticky;top:0;z-index:200;background:rgba(15,17,23,.95);backdrop-filter:blur(16px);border-bottom:1px solid var(--line);padding:0 16px;height:56px;display:flex;align-items:center;justify-content:space-between;}
.nav-logo{display:flex;align-items:center;gap:8px;}
.nav-logo-icon{width:32px;height:32px;background:linear-gradient(135deg,var(--gold),var(--gold2));border-radius:10px;display:flex;align-items:center;justify-content:center;font-size:16px;}
.nav-title{font-size:20px;font-weight:900;letter-spacing:-.5px;background:linear-gradient(90deg,var(--gold),#fff);-webkit-background-clip:text;-webkit-text-fill-color:transparent;}
.nav-right{display:flex;align-items:center;gap:6px;}
.nav-update{font-size:11px;color:var(--muted);font-weight:600;}
.nav-btn{background:none;border:none;color:var(--sub);cursor:pointer;padding:7px 10px;border-radius:10px;font-size:12px;font-weight:700;display:flex;align-items:center;gap:4px;}
.nav-btn:hover{background:var(--line);color:var(--text);}

/* 탭 바 */
.tab-bar{position:sticky;top:56px;z-index:150;background:rgba(15,17,23,.95);backdrop-filter:blur(12px);border-bottom:1px solid var(--line);display:flex;}
.tab-item{flex:1;padding:12px 6px;text-align:center;font-size:12px;font-weight:800;color:var(--muted);cursor:pointer;border-bottom:2px solid transparent;transition:.15s;display:flex;flex-direction:column;align-items:center;gap:3px;}
.tab-item .tab-icon{font-size:18px;}
.tab-item.active{color:var(--gold);border-bottom-color:var(--gold);}

/* 페이지 */
.page{display:none;max-width:480px;margin:0 auto;padding:16px 14px 90px;}
.page.show{display:block;}

/* 상태 배너 */
.status-banner{background:var(--bg2);border:1px solid var(--line);border-radius:14px;padding:10px 14px;margin-bottom:14px;display:flex;align-items:center;gap:10px;font-size:12px;font-weight:700;}
.status-dot{width:7px;height:7px;border-radius:50%;flex-shrink:0;}
.dot-green{background:var(--green);box-shadow:0 0 8px var(--green);}
.dot-red{background:var(--red);}
.dot-yellow{background:var(--gold);box-shadow:0 0 8px var(--gold);}

/* 섹션 헤더 */
.sec-hd{display:flex;align-items:center;justify-content:space-between;margin-bottom:12px;}
.sec-title{font-size:11px;font-weight:900;color:var(--muted);letter-spacing:2px;text-transform:uppercase;}
.sec-badge{background:linear-gradient(135deg,var(--gold),var(--gold2));color:#000;font-size:10px;font-weight:900;padding:3px 8px;border-radius:999px;}

/* TOP4 카드 */
.card{background:var(--card);border:1px solid var(--line);border-radius:20px;padding:16px;margin-bottom:12px;position:relative;overflow:hidden;transition:.15s;cursor:pointer;}
.card:active{transform:scale(.99);}
.card::before{content:"";position:absolute;top:0;left:0;right:0;height:3px;border-radius:20px 20px 0 0;}
.card.rank1::before{background:linear-gradient(90deg,var(--gold),var(--gold2));}
.card.rank2::before{background:linear-gradient(90deg,#c0c0c0,#e0e0e0);}
.card.rank3::before{background:linear-gradient(90deg,#cd7f32,#e8a87c);}
.card.rank4::before{background:linear-gradient(90deg,var(--blue),#82b1ff);}
.card-top{display:flex;justify-content:space-between;align-items:flex-start;margin-bottom:12px;}
.card-left{display:flex;align-items:center;gap:10px;}
.card-rank-badge{width:26px;height:26px;border-radius:8px;display:flex;align-items:center;justify-content:center;font-size:12px;font-weight:900;flex-shrink:0;}
.rank1 .card-rank-badge{background:linear-gradient(135deg,var(--gold),var(--gold2));color:#000;}
.rank2 .card-rank-badge{background:linear-gradient(135deg,#b0b0b0,#e0e0e0);color:#000;}
.rank3 .card-rank-badge{background:linear-gradient(135deg,#cd7f32,#e8a87c);color:#000;}
.rank4 .card-rank-badge{background:linear-gradient(135deg,var(--blue),#82b1ff);color:#000;}
.card-info{display:flex;flex-direction:column;gap:2px;}
.card-league{font-size:9px;font-weight:900;letter-spacing:1px;text-transform:uppercase;}
.lc-해외축구{color:#448aff;}.lc-한국축구{color:#1de9b6;}.lc-미국야구{color:#ff6e40;}.lc-한국야구{color:#e040fb;}
.card-sub{font-size:10px;color:var(--muted);font-weight:700;}
.card-rate-box{text-align:right;}
.card-rate-lbl{font-size:9px;font-weight:800;color:var(--muted);letter-spacing:1px;margin-bottom:2px;}
.card-rate{font-size:24px;font-weight:900;line-height:1;}
.rate-h{color:var(--green);}.rate-m{color:var(--gold);}.rate-l{color:var(--sub);}
.match-box{background:var(--bg3);border-radius:12px;padding:11px;margin-bottom:11px;}
.match-teams{display:flex;align-items:center;justify-content:space-between;gap:6px;margin-bottom:6px;}
.team{flex:1;text-align:center;}
.team-name{font-size:12px;font-weight:900;line-height:1.3;word-break:keep-all;}
.team-prob{font-size:11px;font-weight:700;margin-top:2px;}
.tp-home{color:var(--green);}.tp-away{color:var(--red);}
.vs{font-size:10px;font-weight:900;color:var(--muted);flex-shrink:0;}
.draw-row{text-align:center;font-size:10px;color:var(--muted);font-weight:700;margin-top:4px;}
.prob-bar{height:7px;border-radius:999px;background:var(--line);overflow:hidden;display:flex;margin-bottom:10px;}
.pb-home{height:100%;border-radius:999px 0 0 999px;background:linear-gradient(90deg,var(--green2),var(--green));}
.pb-away{height:100%;border-radius:0 999px 999px 0;background:linear-gradient(90deg,var(--red),#ff8a80);}
.bm-row{display:flex;align-items:center;gap:5px;flex-wrap:wrap;}
.bm-chip{font-size:10px;background:var(--line);border-radius:6px;padding:2px 6px;font-weight:700;color:var(--sub);}
.game-time-row{font-size:10px;color:var(--muted);font-weight:700;margin-bottom:8px;display:flex;align-items:center;gap:4px;}
.tdot{width:5px;height:5px;border-radius:50%;background:var(--green);box-shadow:0 0 5px var(--green);}

/* 오늘 경기 탭 */
.filter-row{display:flex;gap:8px;margin-bottom:14px;overflow-x:auto;padding-bottom:4px;}
.filter-row::-webkit-scrollbar{display:none;}
.filter-btn{flex-shrink:0;padding:7px 14px;border-radius:999px;font-size:12px;font-weight:800;border:1.5px solid var(--line);background:var(--bg2);color:var(--muted);cursor:pointer;transition:.15s;}
.filter-btn.on{background:var(--card);color:var(--text);border-color:var(--sub);}
.filter-btn.on.fl-all{border-color:var(--gold);color:var(--gold);}
.filter-btn.on.fl-해외축구{border-color:#448aff;color:#448aff;}
.filter-btn.on.fl-한국축구{border-color:#1de9b6;color:#1de9b6;}
.filter-btn.on.fl-미국야구{border-color:#ff6e40;color:#ff6e40;}
.filter-btn.on.fl-한국야구{border-color:#e040fb;color:#e040fb;}

/* 경기 리스트 카드 */
.match-item{background:var(--card);border:1px solid var(--line);border-radius:16px;padding:14px;margin-bottom:10px;cursor:pointer;transition:.15s;}
.match-item:hover{border-color:var(--sub);}
.match-item:active{transform:scale(.99);}
.mi-top{display:flex;justify-content:space-between;align-items:center;margin-bottom:10px;}
.mi-league{display:flex;align-items:center;gap:6px;}
.mi-league-dot{width:8px;height:8px;border-radius:50%;}
.mi-league-name{font-size:10px;font-weight:900;letter-spacing:1px;}
.mi-time{font-size:11px;color:var(--muted);font-weight:700;}
.mi-teams{display:flex;align-items:center;justify-content:space-between;gap:8px;margin-bottom:10px;}
.mi-team{flex:1;}
.mi-team-name{font-size:13px;font-weight:900;line-height:1.3;word-break:keep-all;}
.mi-prob{font-size:11px;font-weight:700;margin-top:2px;}
.mi-vs{font-size:10px;color:var(--muted);font-weight:900;text-align:center;}
.mi-bar{height:6px;border-radius:999px;background:var(--line);overflow:hidden;display:flex;margin-bottom:8px;}
.mi-bar-h{height:100%;border-radius:999px 0 0 999px;background:linear-gradient(90deg,var(--green2),var(--green));}
.mi-bar-a{height:100%;border-radius:0 999px 999px 0;background:linear-gradient(90deg,var(--red),#ff8a80);}
.mi-bottom{display:flex;align-items:center;justify-content:space-between;}
.mi-bm{font-size:10px;color:var(--muted);}
.mi-rate{font-size:16px;font-weight:900;}

/* 상세 모달 */
.modal-overlay{position:fixed;inset:0;background:rgba(0,0,0,.7);z-index:500;display:none;align-items:flex-end;justify-content:center;}
.modal-overlay.show{display:flex;}
.modal{background:var(--bg2);border-radius:24px 24px 0 0;padding:20px 18px 40px;width:100%;max-width:480px;max-height:90vh;overflow-y:auto;animation:slideUp .25s ease;}
@keyframes slideUp{from{transform:translateY(100%);}to{transform:translateY(0);}}
.modal-handle{width:40px;height:4px;border-radius:2px;background:var(--line);margin:0 auto 16px;}
.modal-close{position:absolute;top:16px;right:18px;background:var(--line);border:none;border-radius:50%;width:32px;height:32px;color:var(--text);font-size:16px;cursor:pointer;display:flex;align-items:center;justify-content:center;}
.modal-league{font-size:11px;font-weight:900;letter-spacing:2px;margin-bottom:6px;}
.modal-match{font-size:18px;font-weight:900;margin-bottom:4px;line-height:1.3;}
.modal-time{font-size:12px;color:var(--muted);font-weight:700;margin-bottom:16px;}
.modal-rate-grid{display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-bottom:16px;}
.modal-rate-box{background:var(--bg3);border-radius:14px;padding:14px;text-align:center;}
.modal-rate-box.draw{grid-column:span 2;}
.mrb-label{font-size:11px;font-weight:800;color:var(--muted);margin-bottom:4px;}
.mrb-team{font-size:12px;font-weight:800;color:var(--sub);margin-bottom:6px;word-break:keep-all;}
.mrb-val{font-size:28px;font-weight:900;}
.modal-bar-wrap{margin-bottom:16px;}
.modal-bar-labels{display:flex;justify-content:space-between;font-size:11px;font-weight:800;color:var(--muted);margin-bottom:6px;}
.modal-bar{height:10px;border-radius:999px;background:var(--line);overflow:hidden;display:flex;}
.modal-bar-h{height:100%;border-radius:999px 0 0 999px;background:linear-gradient(90deg,var(--green2),var(--green));}
.modal-bar-a{height:100%;border-radius:0 999px 999px 0;background:linear-gradient(90deg,var(--red),#ff8a80);}
.modal-bm-title{font-size:11px;font-weight:900;color:var(--muted);margin-bottom:8px;letter-spacing:1px;}
.modal-bm-list{display:flex;flex-wrap:wrap;gap:6px;}
.modal-bm-chip{background:var(--bg3);border-radius:8px;padding:5px 10px;font-size:12px;font-weight:700;color:var(--sub);}

/* API 설정 */
.api-box{background:var(--bg2);border:1px solid var(--line);border-radius:16px;padding:16px;margin-bottom:14px;}
.api-box h3{font-size:14px;font-weight:900;color:var(--gold);margin-bottom:8px;}
.api-box p{font-size:12px;color:var(--sub);line-height:1.7;margin-bottom:10px;}
.api-row{display:flex;gap:8px;}
.api-input{flex:1;background:var(--bg3);border:1px solid var(--line);border-radius:10px;padding:10px 12px;font-size:13px;color:var(--text);outline:none;}
.api-input:focus{border-color:var(--gold);}
.api-save{background:linear-gradient(135deg,var(--gold),var(--gold2));color:#000;border:none;border-radius:10px;padding:10px 14px;font-size:13px;font-weight:900;cursor:pointer;white-space:nowrap;}

/* 하단 고정 탭 */
.bottom-nav{position:fixed;bottom:0;left:0;right:0;background:rgba(26,29,39,.97);backdrop-filter:blur(16px);border-top:1px solid var(--line);padding:6px 0 calc(6px + env(safe-area-inset-bottom));display:flex;justify-content:space-around;z-index:100;}
.bnav-btn{display:flex;flex-direction:column;align-items:center;gap:3px;padding:5px 16px;border:none;background:none;cursor:pointer;color:var(--muted);font-size:10px;font-weight:700;}
.bnav-btn.active{color:var(--gold);}
.bnav-icon{font-size:20px;}

/* 공통 */
.empty{text-align:center;padding:40px 20px;color:var(--muted);}
.empty-icon{font-size:36px;margin-bottom:10px;}
.empty-txt{font-size:14px;font-weight:700;color:var(--sub);margin-bottom:6px;}
.empty-sub{font-size:12px;line-height:1.6;}
.demo-badge{background:rgba(255,183,0,.1);border:1px solid rgba(255,183,0,.25);color:var(--gold);font-size:11px;font-weight:800;padding:10px 14px;border-radius:10px;text-align:center;margin-bottom:14px;line-height:1.7;}
.spinner{display:inline-block;width:20px;height:20px;border:2px solid var(--line);border-top-color:var(--gold);border-radius:50%;animation:spin .8s linear infinite;}
@keyframes spin{to{transform:rotate(360deg);}}
</style>
</head>
<body>

<!-- 네비 -->
<nav class="nav">
  <div class="nav-logo">
    <div class="nav-logo-icon">🏆</div>
    <span class="nav-title">WIN-4</span>
  </div>
  <div class="nav-right">
    <span class="nav-update" id="navUpdate">-</span>
    <button class="nav-btn" id="refreshBtn" onclick="loadAll()">↻ 새로고침</button>
  </div>
</nav>

<!-- 상단 탭 -->
<div class="tab-bar">
  <div class="tab-item active" data-page="home" onclick="switchPage('home')">
    <span class="tab-icon">🏆</span>TOP 4
  </div>
  <div class="tab-item" data-page="today" onclick="switchPage('today')">
    <span class="tab-icon">📅</span>오늘경기
  </div>
  <div class="tab-item" data-page="settings" onclick="switchPage('settings')">
    <span class="tab-icon">⚙️</span>설정
  </div>
</div>

<!-- ── 페이지1: TOP4 ── -->
<div class="page show" id="page-home">
  <div class="status-banner">
    <div class="status-dot dot-yellow" id="statusDot"></div>
    <span id="statusText">초기화 중...</span>
  </div>
  <div class="demo-badge" id="demoBadge" style="display:none;">
    ⚠️ 데모 데이터 표시 중 — API 키를 설정 탭에서 입력하세요
  </div>
  <div class="sec-hd">
    <div class="sec-title">Today's Best 4</div>
    <div class="sec-badge">승률 TOP 선별</div>
  </div>
  <div id="top4Area">
    <div class="empty"><div class="spinner"></div><br><br>로딩 중...</div>
  </div>
</div>

<!-- ── 페이지2: 오늘경기 ── -->
<div class="page" id="page-today">
  <div class="sec-hd" style="margin-bottom:10px;">
    <div class="sec-title">오늘의 전체 경기</div>
    <div class="sec-badge" id="todayCnt">-</div>
  </div>
  <!-- 필터 -->
  <div class="filter-row" id="filterRow">
    <button class="filter-btn on fl-all" data-filter="전체" onclick="setFilter('전체',this)">전체</button>
    <button class="filter-btn fl-해외축구" data-filter="해외축구" onclick="setFilter('해외축구',this)">⚽ 해외축구</button>
    <button class="filter-btn fl-한국축구" data-filter="한국축구" onclick="setFilter('한국축구',this)">🇰🇷 한국축구</button>
    <button class="filter-btn fl-미국야구" data-filter="미국야구" onclick="setFilter('미국야구',this)">⚾ 미국야구</button>
    <button class="filter-btn fl-한국야구" data-filter="한국야구" onclick="setFilter('한국야구',this)">🏟️ 한국야구</button>
  </div>
  <div id="todayArea">
    <div class="empty"><div class="spinner"></div><br><br>로딩 중...</div>
  </div>
</div>

<!-- ── 페이지3: 설정 ── -->
<div class="page" id="page-settings">
  <div class="api-box">
    <h3>🔑 Odds API 키 설정</h3>
    <p>무료 API 키 발급: <b>the-odds-api.com</b><br>월 500회 무료 · 브라우저에 안전하게 저장됩니다.</p>
    <div class="api-row">
      <input class="api-input" id="apiKeyInput" type="password" placeholder="API 키 입력..."/>
      <button class="api-save" onclick="saveApiKey()">저장</button>
    </div>
    <div id="apiStatus" style="margin-top:10px;font-size:12px;color:var(--muted);font-weight:700;"></div>
  </div>
  <div style="background:var(--bg2);border:1px solid var(--line);border-radius:16px;padding:16px;">
    <h3 style="font-size:14px;font-weight:900;color:var(--sub);margin-bottom:12px;">ℹ️ 앱 안내</h3>
    <div style="font-size:12px;color:var(--muted);line-height:2;">
      📡 데이터: Pinnacle·Bet365·Bwin 등 8개 북메이커<br>
      ⚽ 종목: EPL·라리가·분데스·세리에A·UCL·K리그·MLB·KBO<br>
      🤖 AI승률: 배당률 역산 + Pinnacle 가중치 2배<br>
      🏆 TOP4: 그날 경기 중 승률 가장 높은 4경기 자동 선별<br>
      ⚠️ 본 서비스는 참고용이며 베팅을 권장하지 않습니다.
    </div>
  </div>
</div>

<!-- 경기 상세 모달 -->
<div class="modal-overlay" id="modalOverlay" onclick="closeModal(event)">
  <div class="modal" id="modal" style="position:relative;">
    <div class="modal-handle"></div>
    <button class="modal-close" onclick="closeModal()">✕</button>
    <div id="modalContent"></div>
  </div>
</div>

<script>
// ── 설정 ─────────────────────────────────────────────────────────
const ODDS_API_BASE = "https://api.the-odds-api.com/v4";
const BOOKMAKERS    = "pinnacle,betway,unibet,draftkings,fanduel,bet365,bwin";
const SPORTS = [
  {key:"soccer_epl",               label:"해외축구", sub:"EPL"},
  {key:"soccer_spain_la_liga",     label:"해외축구", sub:"라리가"},
  {key:"soccer_germany_bundesliga",label:"해외축구", sub:"분데스리가"},
  {key:"soccer_italy_serie_a",     label:"해외축구", sub:"세리에A"},
  {key:"soccer_uefa_champs_league",label:"해외축구", sub:"챔피언스리그"},
  {key:"soccer_korea_kleague1",    label:"한국축구", sub:"K리그1"},
  {key:"baseball_mlb",             label:"미국야구", sub:"MLB"},
  {key:"baseball_kbo",             label:"한국야구", sub:"KBO"},
];
const STORAGE_KEY = "win4_api_key_v2";
const RANK_LABELS  = ["🥇","🥈","🥉","4"];
const LEAGUE_COLORS = {"해외축구":"#448aff","한국축구":"#1de9b6","미국야구":"#ff6e40","한국야구":"#e040fb"};

let DATA     = {top4:[], all:[]};
let curFilter= "전체";
let curPage  = "home";

// ── 페이지 전환 ───────────────────────────────────────────────────
function switchPage(page){
  curPage = page;
  document.querySelectorAll(".page").forEach(p=>p.classList.remove("show"));
  document.querySelectorAll(".tab-item").forEach(t=>t.classList.remove("active"));
  document.getElementById("page-"+page).classList.add("show");
  document.querySelector(`.tab-item[data-page="${page}"]`).classList.add("active");
}

// ── 유틸 ─────────────────────────────────────────────────────────
function rateColor(r){ return r>=60?"rate-h":r>=50?"rate-m":"rate-l"; }
function rateColorModal(r){ return r>=60?"var(--green)":r>=50?"var(--gold)":"var(--sub)"; }
function setStatus(type,text){
  document.getElementById("statusDot").className="status-dot "+(type==="ok"?"dot-green":type==="err"?"dot-red":"dot-yellow");
  document.getElementById("statusText").textContent=text;
}
function toKST(iso){
  try{ return new Date(iso).toLocaleString("ko-KR",{timeZone:"Asia/Seoul",month:"2-digit",day:"2-digit",hour:"2-digit",minute:"2-digit",hour12:false}); }
  catch{ return iso.slice(0,10); }
}
function getApiKey(){ return localStorage.getItem(STORAGE_KEY)||""; }
function saveApiKey(){
  const k=document.getElementById("apiKeyInput").value.trim();
  if(!k){ alert("API 키를 입력해주세요."); return; }
  localStorage.setItem(STORAGE_KEY,k);
  document.getElementById("apiStatus").innerHTML=`<span style="color:var(--green)">✅ 저장 완료! 새로고침합니다...</span>`;
  setTimeout(()=>loadAll(),800);
}

// ── 오즈 계산 ─────────────────────────────────────────────────────
function calcRates(game, sport){
  const home=game.home_team, away=game.away_team;
  const bms=game.bookmakers||[];
  if(!bms.length) return null;
  let hp=[],ap=[],dp=[];
  bms.forEach(bm=>{
    const w=bm.key==="pinnacle"?2:1;
    (bm.markets||[]).forEach(mkt=>{
      if(mkt.key!=="h2h") return;
      const oc={};
      (mkt.outcomes||[]).forEach(o=>oc[o.name]=o.price);
      if(oc[home]) for(let i=0;i<w;i++) hp.push(1/oc[home]);
      if(oc[away]) for(let i=0;i<w;i++) ap.push(1/oc[away]);
      if(oc["Draw"]) for(let i=0;i<w;i++) dp.push(1/oc["Draw"]);
    });
  });
  if(!hp.length) return null;
  const avg=a=>a.reduce((s,v)=>s+v,0)/a.length;
  const ah=avg(hp),aa=ap.length?avg(ap):0,ad=dp.length?avg(dp):0,tot=ah+aa+ad;
  const hr=+(ah/tot*100).toFixed(1), ar=+(aa/tot*100).toFixed(1);
  const dr=dp.length?+(ad/tot*100).toFixed(1):null;
  const bmNames=bms.map(b=>b.title);
  return {
    id:game.id, league:sport.label, sub_league:sport.sub,
    home, away, match:`${home} vs ${away}`,
    game_time:toKST(game.commence_time),
    home_rate:hr, away_rate:ar, draw_rate:dr, win_rate:hr,
    bookmakers:bmNames, bm_count:bmNames.length,
    source:bmNames.slice(0,3).join(", ")+(bmNames.length>3?` 외 ${bmNames.length-3}개`:""),
  };
}

// ── TOP4 선정: 그날 승률 가장 높은 4경기 ─────────────────────────
function pickTop4(games){
  // 승률 내림차순 정렬
  const sorted=[...games].sort((a,b)=>b.win_rate-a.win_rate);
  const top4=[], seen={};
  // 1차: 리그별 다양성 (각 리그 1개씩)
  for(const g of sorted){
    const k=g.league+g.sub_league;
    if(!seen[k]&&top4.length<4){top4.push(g);seen[k]=1;}
  }
  // 2차: 그래도 4개 미만이면 순수 승률순으로 채우기
  for(const g of sorted){
    if(!top4.includes(g)&&top4.length<4) top4.push(g);
  }
  // 최종 TOP4도 승률 내림차순
  return top4.sort((a,b)=>b.win_rate-a.win_rate);
}

// ── API 호출 ──────────────────────────────────────────────────────
async function fetchSport(key, sport, apiKey){
  try{
    const url=`${ODDS_API_BASE}/sports/${key}/odds?apiKey=${apiKey}&regions=us,eu,uk&markets=h2h&bookmakers=${BOOKMAKERS}&dateFormat=iso&oddsFormat=decimal`;
    const r=await fetch(url);
    if(r.status===401) throw new Error("API_KEY_ERROR");
    if(r.status===422||r.status===404) return [];
    if(!r.ok) return [];
    return (await r.json()).map(g=>calcRates(g,sport)).filter(Boolean);
  }catch(e){
    if(e.message==="API_KEY_ERROR") throw e;
    return [];
  }
}

// ── 렌더: TOP4 카드 ───────────────────────────────────────────────
function top4CardHTML(g, rank){
  const hw=Math.round(g.home_rate/(g.home_rate+g.away_rate)*100);
  return `<div class="card rank${rank}" onclick='openModal(${JSON.stringify(g)})'>
    <div class="card-top">
      <div class="card-left">
        <div class="card-rank-badge">${RANK_LABELS[rank-1]}</div>
        <div class="card-info">
          <div class="card-league lc-${g.league}">${g.league} · ${g.sub_league}</div>
          <div class="card-sub">${g.game_time}</div>
        </div>
      </div>
      <div class="card-rate-box">
        <div class="card-rate-lbl">홈팀 AI 승률</div>
        <div class="card-rate ${rateColor(g.home_rate)}">${g.home_rate}%</div>
      </div>
    </div>
    <div class="match-box">
      <div class="match-teams">
        <div class="team"><div class="team-name">${g.home}</div><div class="team-prob tp-home">${g.home_rate}%</div></div>
        <div class="vs">VS</div>
        <div class="team"><div class="team-name" style="text-align:right">${g.away}</div><div class="team-prob tp-away" style="text-align:right">${g.away_rate}%</div></div>
      </div>
      ${g.draw_rate!=null?`<div class="draw-row">무승부 ${g.draw_rate}%</div>`:""}
    </div>
    <div class="prob-bar" style="margin-bottom:10px;">
      <div class="pb-home" style="width:${hw}%"></div>
      <div class="pb-away" style="width:${100-hw}%"></div>
    </div>
    <div class="bm-row">
      ${g.bookmakers.slice(0,4).map(b=>`<span class="bm-chip">${b}</span>`).join("")}
      ${g.bm_count>4?`<span style="font-size:10px;color:var(--muted);">외 ${g.bm_count-4}개</span>`:""}
    </div>
  </div>`;
}

function renderTop4(top4){
  const el=document.getElementById("top4Area");
  if(!top4.length){
    el.innerHTML=`<div class="empty"><div class="empty-icon">📭</div><div class="empty-txt">오늘 분석 가능한 경기가 없습니다</div><div class="empty-sub">경기 일정이 없거나 오즈가 아직 공개 전입니다</div></div>`;
    return;
  }
  el.innerHTML=top4.map((g,i)=>top4CardHTML(g,i+1)).join("");
}

// ── 렌더: 오늘경기 리스트 ────────────────────────────────────────
function renderToday(games, filter){
  const filtered = filter==="전체" ? games : games.filter(g=>g.league===filter);
  const el=document.getElementById("todayArea");
  document.getElementById("todayCnt").textContent=`${filtered.length}경기`;

  if(!filtered.length){
    el.innerHTML=`<div class="empty"><div class="empty-icon">📭</div><div class="empty-txt">${filter} 경기가 없습니다</div></div>`;
    return;
  }

  // 리그별 그룹
  const groups={};
  filtered.forEach(g=>{
    const k=g.league+" "+g.sub_league;
    if(!groups[k]) groups[k]={league:g.league,sub:g.sub_league,games:[]};
    groups[k].games.push(g);
  });

  el.innerHTML=Object.values(groups).map(gr=>`
    <div style="margin-bottom:20px;">
      <div style="display:flex;align-items:center;gap:8px;margin-bottom:10px;">
        <div style="width:10px;height:10px;border-radius:50%;background:${LEAGUE_COLORS[gr.league]||'#fff'};box-shadow:0 0 6px ${LEAGUE_COLORS[gr.league]||'#fff'};"></div>
        <span style="font-size:12px;font-weight:900;color:${LEAGUE_COLORS[gr.league]||'#fff'};letter-spacing:1px;">${gr.league} · ${gr.sub}</span>
        <span style="font-size:11px;color:var(--muted);font-weight:700;">${gr.games.length}경기</span>
      </div>
      ${gr.games.map(g=>matchItemHTML(g)).join("")}
    </div>`).join("");
}

function matchItemHTML(g){
  const hw=Math.round(g.home_rate/(g.home_rate+g.away_rate)*100);
  const lc=LEAGUE_COLORS[g.league]||"#fff";
  return `<div class="match-item" onclick='openModal(${JSON.stringify(g)})'>
    <div class="mi-top">
      <div class="mi-league">
        <div class="mi-league-dot" style="background:${lc};box-shadow:0 0 5px ${lc};"></div>
        <span class="mi-league-name" style="color:${lc};">${g.sub_league}</span>
      </div>
      <div class="mi-time">${g.game_time}</div>
    </div>
    <div class="mi-teams">
      <div class="mi-team">
        <div class="mi-team-name">${g.home}</div>
        <div class="mi-prob" style="color:var(--green);">${g.home_rate}%</div>
      </div>
      <div class="mi-vs">VS</div>
      <div class="mi-team" style="text-align:right;">
        <div class="mi-team-name">${g.away}</div>
        <div class="mi-prob" style="color:var(--red);text-align:right;">${g.away_rate}%</div>
      </div>
    </div>
    <div class="mi-bar" style="margin-bottom:8px;">
      <div class="mi-bar-h" style="width:${hw}%"></div>
      <div class="mi-bar-a" style="width:${100-hw}%"></div>
    </div>
    <div class="mi-bottom">
      <span class="mi-bm">${g.source}</span>
      <span class="mi-rate ${rateColor(g.home_rate)}">${g.home_rate}%</span>
    </div>
  </div>`;
}

// ── 필터 ──────────────────────────────────────────────────────────
function setFilter(filter, btn){
  curFilter=filter;
  document.querySelectorAll(".filter-btn").forEach(b=>{
    b.classList.remove("on");
    b.className=b.className.replace(/ on/g,"");
  });
  btn.classList.add("on");
  renderToday(DATA.all, curFilter);
}

// ── 모달 ──────────────────────────────────────────────────────────
function openModal(g){
  const hw=Math.round(g.home_rate/(g.home_rate+g.away_rate)*100);
  const lc=LEAGUE_COLORS[g.league]||"#fff";
  document.getElementById("modalContent").innerHTML=`
    <div class="modal-league" style="color:${lc};">${g.league} · ${g.sub_league}</div>
    <div class="modal-match">${g.home} vs ${g.away}</div>
    <div class="modal-time">🕐 ${g.game_time}</div>
    <div class="modal-rate-grid">
      <div class="modal-rate-box">
        <div class="mrb-label">홈팀 승률</div>
        <div class="mrb-team">${g.home}</div>
        <div class="mrb-val" style="color:${rateColorModal(g.home_rate)};">${g.home_rate}%</div>
      </div>
      <div class="modal-rate-box">
        <div class="mrb-label">원정팀 승률</div>
        <div class="mrb-team">${g.away}</div>
        <div class="mrb-val" style="color:var(--red);">${g.away_rate}%</div>
      </div>
      ${g.draw_rate!=null?`<div class="modal-rate-box draw"><div class="mrb-label">무승부</div><div class="mrb-val" style="color:var(--muted);font-size:22px;">${g.draw_rate}%</div></div>`:""}
    </div>
    <div class="modal-bar-wrap">
      <div class="modal-bar-labels"><span>${g.home}</span><span>${g.away}</span></div>
      <div class="modal-bar">
        <div class="modal-bar-h" style="width:${hw}%"></div>
        <div class="modal-bar-a" style="width:${100-hw}%"></div>
      </div>
    </div>
    <div class="modal-bm-title">📡 분석 북메이커 (${g.bm_count}개)</div>
    <div class="modal-bm-list">
      ${g.bookmakers.map(b=>`<span class="modal-bm-chip">${b}</span>`).join("")}
    </div>`;
  document.getElementById("modalOverlay").classList.add("show");
}
function closeModal(e){
  if(!e||e.target===document.getElementById("modalOverlay"))
    document.getElementById("modalOverlay").classList.remove("show");
}

// ── 데모 데이터 ───────────────────────────────────────────────────
function loadDemo(){
  const now=new Date().toLocaleString("ko-KR",{timeZone:"Asia/Seoul",month:"2-digit",day:"2-digit",hour:"2-digit",minute:"2-digit",hour12:false});
  const demo=[
    {id:"d1",league:"해외축구",sub_league:"라리가",home:"레알 마드리드",away:"바르셀로나",match:"레알 마드리드 vs 바르셀로나",game_time:now,home_rate:62.3,away_rate:24.4,draw_rate:13.3,win_rate:62.3,bookmakers:["Pinnacle","Bet365","Bwin","Unibet","Betway","DraftKings","FanDuel","Draftkings"],bm_count:8,source:"Pinnacle, Bet365, Bwin 외 5개"},
    {id:"d2",league:"미국야구",sub_league:"MLB",home:"New York Yankees",away:"Boston Red Sox",match:"NYY vs BOS",game_time:now,home_rate:58.2,away_rate:41.8,draw_rate:null,win_rate:58.2,bookmakers:["DraftKings","FanDuel","Pinnacle"],bm_count:6,source:"DraftKings, FanDuel, Pinnacle 외 3개"},
    {id:"d3",league:"해외축구",sub_league:"EPL",home:"Manchester City",away:"Arsenal",match:"Man City vs Arsenal",game_time:now,home_rate:55.1,away_rate:26.3,draw_rate:18.6,win_rate:55.1,bookmakers:["Pinnacle","Bet365","Bwin"],bm_count:5,source:"Pinnacle, Bet365, Bwin 외 2개"},
    {id:"d4",league:"한국야구",sub_league:"KBO",home:"KIA 타이거즈",away:"삼성 라이온즈",match:"KIA vs 삼성",game_time:now,home_rate:53.7,away_rate:46.3,draw_rate:null,win_rate:53.7,bookmakers:["Pinnacle","Betway"],bm_count:3,source:"Pinnacle, Betway"},
    {id:"d5",league:"한국축구",sub_league:"K리그1",home:"울산 HD",away:"전북 현대",match:"울산 vs 전북",game_time:now,home_rate:51.2,away_rate:27.2,draw_rate:21.6,win_rate:51.2,bookmakers:["Pinnacle","Unibet"],bm_count:4,source:"Pinnacle, Unibet 외 1개"},
    {id:"d6",league:"해외축구",sub_league:"분데스리가",home:"Bayern Munich",away:"Borussia Dortmund",match:"Bayern vs Dortmund",game_time:now,home_rate:67.4,away_rate:18.2,draw_rate:14.4,win_rate:67.4,bookmakers:["Pinnacle","Bet365","Bwin","Unibet"],bm_count:6,source:"Pinnacle, Bet365, Bwin 외 3개"},
    {id:"d7",league:"미국야구",sub_league:"MLB",home:"Los Angeles Dodgers",away:"San Francisco Giants",match:"LAD vs SF",game_time:now,home_rate:64.8,away_rate:35.2,draw_rate:null,win_rate:64.8,bookmakers:["DraftKings","FanDuel","Pinnacle","Betway"],bm_count:5,source:"DraftKings, FanDuel, Pinnacle 외 2개"},
    {id:"d8",league:"해외축구",sub_league:"세리에A",home:"Inter Milan",away:"Juventus",match:"Inter vs Juventus",game_time:now,home_rate:48.3,away_rate:28.5,draw_rate:23.2,win_rate:48.3,bookmakers:["Pinnacle","Bet365"],bm_count:4,source:"Pinnacle, Bet365 외 2개"},
  ];
  const top4=pickTop4(demo);
  DATA={top4, all:demo};
  document.getElementById("demoBadge").style.display="block";
  renderTop4(top4);
  renderToday(demo, curFilter);
  document.getElementById("todayCnt").textContent=`${demo.length}경기`;
  setStatus("yellow","데모 데이터 — 설정 탭에서 API 키를 입력하세요");
  document.getElementById("navUpdate").textContent="데모";
}

// ── 메인 로드 ─────────────────────────────────────────────────────
async function loadAll(){
  const apiKey=getApiKey();
  if(!apiKey){ loadDemo(); return; }

  document.getElementById("demoBadge").style.display="none";
  document.getElementById("top4Area").innerHTML=`<div class="empty"><div class="spinner"></div><br><br>오즈 데이터 수집 중...</div>`;
  document.getElementById("todayArea").innerHTML=`<div class="empty"><div class="spinner"></div><br><br>로딩 중...</div>`;
  setStatus("yellow","실시간 오즈 데이터 수집 중...");
  document.getElementById("refreshBtn").disabled=true;

  try{
    const allGames=[];
    for(const sport of SPORTS){
      setStatus("yellow",`${sport.label} ${sport.sub} 수집 중...`);
      const games=await fetchSport(sport.key, sport, apiKey);
      allGames.push(...games);
    }

    const top4=pickTop4(allGames);
    DATA={top4, all:allGames.sort((a,b)=>b.win_rate-a.win_rate)};

    renderTop4(top4);
    renderToday(DATA.all, curFilter);
    document.getElementById("todayCnt").textContent=`${DATA.all.length}경기`;

    const t=new Date().toLocaleTimeString("ko-KR",{timeZone:"Asia/Seoul",hour:"2-digit",minute:"2-digit"});
    document.getElementById("navUpdate").textContent=t+" 갱신";
    setStatus("ok",`실시간 데이터 · ${allGames.length}경기 분석 완료`);

  }catch(err){
    if(err.message==="API_KEY_ERROR"){
      localStorage.removeItem(STORAGE_KEY);
      setStatus("err","API 키 오류 — 설정 탭에서 키를 확인하세요");
    } else {
      setStatus("err","데이터 로드 실패 — 잠시 후 다시 시도해주세요");
    }
    loadDemo();
  }finally{
    document.getElementById("refreshBtn").disabled=false;
    // 설정 탭 상태 업데이트
    const k=getApiKey();
    document.getElementById("apiStatus").innerHTML=k?
      `<span style="color:var(--green)">✅ API 키 등록됨 (앞 8자리: ${k.slice(0,8)}...)</span>`:
      `<span style="color:var(--muted)">❌ API 키 미등록 (데모 모드)</span>`;
    if(k) document.getElementById("apiKeyInput").value=k;
  }
}

// 초기 실행
loadAll();
</script>
</body>
</html>
