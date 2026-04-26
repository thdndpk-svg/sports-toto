cat > /home/claude/sports/index.html << 'HTMLEOF'
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
  --shadow:0 8px 32px rgba(0,0,0,.4);
}
html,body{min-height:100vh;background:var(--bg);color:var(--text);font-family:-apple-system,BlinkMacSystemFont,"Segoe UI","Apple SD Gothic Neo","Malgun Gothic",sans-serif;-webkit-text-size-adjust:100%;}
.nav{position:sticky;top:0;z-index:100;background:rgba(15,17,23,.92);backdrop-filter:blur(16px);border-bottom:1px solid var(--line);padding:0 16px;height:56px;display:flex;align-items:center;justify-content:space-between;}
.nav-logo{display:flex;align-items:center;gap:8px;}
.nav-logo-icon{width:32px;height:32px;background:linear-gradient(135deg,var(--gold),var(--gold2));border-radius:10px;display:flex;align-items:center;justify-content:center;font-size:16px;}
.nav-title{font-size:20px;font-weight:900;letter-spacing:-.5px;background:linear-gradient(90deg,var(--gold),#fff);-webkit-background-clip:text;-webkit-text-fill-color:transparent;}
.nav-right{display:flex;align-items:center;gap:8px;}
.nav-btn{background:none;border:none;color:var(--sub);cursor:pointer;padding:8px;border-radius:10px;transition:.15s;font-size:13px;font-weight:700;display:flex;align-items:center;gap:4px;}
.nav-btn:hover{background:var(--line);color:var(--text);}
.nav-update{font-size:11px;color:var(--muted);font-weight:600;}
.wrap{max-width:480px;margin:0 auto;padding:16px 14px 100px;}
.status-banner{background:var(--bg2);border:1px solid var(--line);border-radius:16px;padding:12px 16px;margin-bottom:16px;display:flex;align-items:center;gap:10px;font-size:13px;font-weight:700;}
.status-dot{width:8px;height:8px;border-radius:50%;flex-shrink:0;}
.dot-green{background:var(--green);box-shadow:0 0 8px var(--green);}
.dot-red{background:var(--red);}
.dot-yellow{background:var(--gold);box-shadow:0 0 8px var(--gold);}
.section-header{display:flex;align-items:center;justify-content:space-between;margin-bottom:14px;}
.section-title{font-size:11px;font-weight:900;color:var(--muted);letter-spacing:2px;text-transform:uppercase;}
.section-badge{background:linear-gradient(135deg,var(--gold),var(--gold2));color:#000;font-size:10px;font-weight:900;padding:3px 8px;border-radius:999px;}
.card{background:var(--card);border:1px solid var(--line);border-radius:20px;padding:18px;margin-bottom:12px;position:relative;overflow:hidden;transition:.15s;}
.card:active{transform:scale(.99);}
.card::before{content:"";position:absolute;top:0;left:0;right:0;height:3px;border-radius:20px 20px 0 0;}
.card.rank1::before{background:linear-gradient(90deg,var(--gold),var(--gold2));}
.card.rank2::before{background:linear-gradient(90deg,#c0c0c0,#e0e0e0);}
.card.rank3::before{background:linear-gradient(90deg,#cd7f32,#e8a87c);}
.card.rank4::before{background:linear-gradient(90deg,var(--blue),#82b1ff);}
.card-top{display:flex;justify-content:space-between;align-items:flex-start;margin-bottom:14px;}
.card-left{display:flex;align-items:center;gap:10px;}
.card-rank{width:28px;height:28px;border-radius:8px;display:flex;align-items:center;justify-content:center;font-size:13px;font-weight:900;flex-shrink:0;}
.rank1 .card-rank{background:linear-gradient(135deg,var(--gold),var(--gold2));color:#000;}
.rank2 .card-rank{background:linear-gradient(135deg,#b0b0b0,#e0e0e0);color:#000;}
.rank3 .card-rank{background:linear-gradient(135deg,#cd7f32,#e8a87c);color:#000;}
.rank4 .card-rank{background:linear-gradient(135deg,var(--blue),#82b1ff);color:#000;}
.card-league-wrap{display:flex;flex-direction:column;gap:2px;}
.card-league{font-size:10px;font-weight:900;letter-spacing:1px;text-transform:uppercase;}
.league-해외축구{color:#448aff;}.league-한국축구{color:#1de9b6;}.league-미국야구{color:#ff6e40;}.league-한국야구{color:#e040fb;}
.card-sub{font-size:11px;color:var(--muted);font-weight:700;}
.card-rate-wrap{text-align:right;}
.card-rate-label{font-size:9px;font-weight:800;color:var(--muted);letter-spacing:1px;margin-bottom:2px;}
.card-rate{font-size:26px;font-weight:900;line-height:1;}
.rate-high{color:var(--green);}.rate-mid{color:var(--gold);}.rate-low{color:var(--sub);}
.match-box{background:var(--bg3);border-radius:12px;padding:12px;margin-bottom:12px;}
.match-teams{display:flex;align-items:center;justify-content:space-between;gap:8px;margin-bottom:8px;}
.team{flex:1;text-align:center;}
.team-name{font-size:13px;font-weight:900;line-height:1.3;word-break:keep-all;}
.team-prob{font-size:11px;font-weight:700;margin-top:3px;}
.home-prob{color:var(--green);}.away-prob{color:var(--red);}
.vs-box{font-size:11px;font-weight:900;color:var(--muted);padding:0 4px;flex-shrink:0;}
.draw-row{text-align:center;font-size:11px;color:var(--muted);font-weight:700;margin-top:4px;}
.prob-bar-wrap{margin-bottom:12px;}
.prob-bar-labels{display:flex;justify-content:space-between;font-size:10px;font-weight:800;color:var(--muted);margin-bottom:4px;}
.prob-bar{height:8px;border-radius:999px;background:var(--line);overflow:hidden;display:flex;}
.prob-bar-home{height:100%;border-radius:999px 0 0 999px;background:linear-gradient(90deg,var(--green2),var(--green));}
.prob-bar-away{height:100%;border-radius:0 999px 999px 0;background:linear-gradient(90deg,var(--red),#ff8a80);}
.bm-row{display:flex;align-items:center;gap:6px;flex-wrap:wrap;}
.bm-icon{font-size:10px;background:var(--line);border-radius:6px;padding:3px 7px;font-weight:700;color:var(--sub);}
.bm-count{font-size:10px;color:var(--muted);font-weight:700;}
.game-time{font-size:11px;color:var(--muted);font-weight:700;margin-bottom:8px;display:flex;align-items:center;gap:4px;}
.time-dot{width:6px;height:6px;border-radius:50%;background:var(--green);box-shadow:0 0 6px var(--green);}
.all-section{margin-top:24px;}
.league-group{margin-bottom:20px;}
.league-title{font-size:12px;font-weight:900;letter-spacing:1px;padding:6px 12px;border-radius:8px;margin-bottom:8px;display:inline-block;}
.lt-해외축구{background:rgba(68,138,255,.15);color:#448aff;}
.lt-한국축구{background:rgba(29,233,182,.15);color:#1de9b6;}
.lt-미국야구{background:rgba(255,110,64,.15);color:#ff6e40;}
.lt-한국야구{background:rgba(224,64,251,.15);color:#e040fb;}
.mini-card{background:var(--card);border:1px solid var(--line);border-radius:14px;padding:12px 14px;margin-bottom:8px;display:flex;align-items:center;justify-content:space-between;gap:10px;}
.mini-left{display:flex;flex-direction:column;gap:3px;}
.mini-match{font-size:13px;font-weight:800;color:var(--text);}
.mini-time{font-size:11px;color:var(--muted);font-weight:600;}
.mini-rate{font-size:18px;font-weight:900;}
.mini-bm{font-size:10px;color:var(--muted);font-weight:600;margin-top:2px;}
.bottom-tab{position:fixed;bottom:0;left:0;right:0;background:rgba(26,29,39,.97);backdrop-filter:blur(16px);border-top:1px solid var(--line);padding:8px 0 calc(8px + env(safe-area-inset-bottom));display:flex;justify-content:space-around;z-index:100;}
.tab-btn{display:flex;flex-direction:column;align-items:center;gap:4px;padding:6px 20px;border:none;background:none;cursor:pointer;color:var(--muted);font-size:10px;font-weight:700;transition:.15s;}
.tab-btn.active{color:var(--gold);}
.tab-icon{font-size:20px;}
.empty-state{text-align:center;padding:40px 20px;color:var(--muted);}
.empty-icon{font-size:40px;margin-bottom:12px;}
.empty-text{font-size:14px;font-weight:700;margin-bottom:6px;color:var(--sub);}
.empty-sub{font-size:12px;line-height:1.6;}
.demo-badge{background:rgba(255,183,0,.12);border:1px solid rgba(255,183,0,.3);color:var(--gold);font-size:11px;font-weight:800;padding:10px 14px;border-radius:10px;text-align:center;margin-bottom:14px;line-height:1.6;}
.spinner{display:inline-block;width:20px;height:20px;border:2px solid var(--line);border-top-color:var(--gold);border-radius:50%;animation:spin .8s linear infinite;vertical-align:middle;}
@keyframes spin{to{transform:rotate(360deg);}}
.all-toggle{background:var(--bg2);border:1px solid var(--line);border-radius:12px;padding:10px 16px;width:100%;font-size:13px;font-weight:800;color:var(--sub);cursor:pointer;margin-top:8px;display:flex;align-items:center;justify-content:center;gap:6px;}
.all-toggle:hover{background:var(--line);color:var(--text);}
.api-setup{background:var(--bg2);border:1px solid var(--line);border-radius:16px;padding:16px;margin-bottom:16px;}
.api-setup h3{font-size:14px;font-weight:900;color:var(--gold);margin-bottom:10px;}
.api-setup p{font-size:12px;color:var(--sub);line-height:1.7;margin-bottom:8px;}
.api-input-row{display:flex;gap:8px;margin-top:10px;}
.api-input{flex:1;background:var(--bg3);border:1px solid var(--line);border-radius:10px;padding:10px 12px;font-size:13px;color:var(--text);outline:none;}
.api-input:focus{border-color:var(--gold);}
.api-save-btn{background:linear-gradient(135deg,var(--gold),var(--gold2));color:#000;border:none;border-radius:10px;padding:10px 16px;font-size:13px;font-weight:900;cursor:pointer;white-space:nowrap;}
</style>
</head>
<body>

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

<div class="wrap">

  <!-- 상태 배너 -->
  <div class="status-banner">
    <div class="status-dot dot-yellow" id="statusDot"></div>
    <span id="statusText">초기화 중...</span>
  </div>

  <!-- API 키 입력 (저장 전에만 표시) -->
  <div class="api-setup" id="apiSetup" style="display:none;">
    <h3>🔑 Odds API 키 설정</h3>
    <p>무료 API 키 발급: <b>the-odds-api.com</b> (월 500회 무료)<br>키를 입력하면 브라우저에 안전하게 저장됩니다.</p>
    <div class="api-input-row">
      <input class="api-input" id="apiKeyInput" type="password" placeholder="API 키 입력..."/>
      <button class="api-save-btn" onclick="saveApiKey()">저장</button>
    </div>
  </div>

  <!-- 데모 배지 -->
  <div class="demo-badge" id="demoBadge" style="display:none;">
    ⚠️ 데모 데이터 표시 중<br>
    실제 데이터는 아래 API 키를 입력하거나<br>
    GitHub Actions에 ODDS_API_KEY Secret을 등록하세요.
  </div>

  <!-- TOP 4 -->
  <div class="section-header">
    <div class="section-title">Today's Best 4</div>
    <div class="section-badge">AI 선별</div>
  </div>
  <div id="top4Area">
    <div class="empty-state"><div class="spinner"></div><br><br>로딩 중...</div>
  </div>

  <!-- 전체 경기 토글 버튼 -->
  <button class="all-toggle" id="allToggle" onclick="toggleAll()" style="display:none;">
    📋 전체 경기 보기
  </button>

  <!-- 전체 경기 목록 -->
  <div class="all-section" id="allArea" style="display:none;"></div>

</div>

<!-- 하단 탭 -->
<div class="bottom-tab">
  <button class="tab-btn active" onclick="scrollToTop()"><span class="tab-icon">🏆</span>TOP4</button>
  <button class="tab-btn" onclick="toggleAll()"><span class="tab-icon">📋</span>전체경기</button>
  <button class="tab-btn" onclick="showInfo()"><span class="tab-icon">ℹ️</span>안내</button>
</div>

<script>
// ── 설정 ─────────────────────────────────────────────────────────
const ODDS_API_BASE = "https://api.the-odds-api.com/v4";
const BOOKMAKERS    = "pinnacle,betway,unibet,draftkings,fanduel,bet365,bwin";
const SPORTS = [
  {key:"soccer_epl",            label:"해외축구", sub:"EPL"},
  {key:"soccer_spain_la_liga",  label:"해외축구", sub:"라리가"},
  {key:"soccer_germany_bundesliga",label:"해외축구",sub:"분데스리가"},
  {key:"soccer_italy_serie_a",  label:"해외축구", sub:"세리에A"},
  {key:"soccer_uefa_champs_league",label:"해외축구",sub:"챔피언스리그"},
  {key:"soccer_korea_kleague1", label:"한국축구", sub:"K리그1"},
  {key:"baseball_mlb",          label:"미국야구", sub:"MLB"},
  {key:"baseball_kbo",          label:"한국야구", sub:"KBO"},
];
const STORAGE_KEY = "win4_api_key";
const RANK_LABELS = ["🥇","🥈","🥉","4"];

let allShown = false;
let DATA = null;

// ── API 키 관리 ───────────────────────────────────────────────────
function getApiKey(){ return localStorage.getItem(STORAGE_KEY)||""; }
function saveApiKey(){
  const key = document.getElementById("apiKeyInput").value.trim();
  if(!key){ alert("API 키를 입력해주세요."); return; }
  localStorage.setItem(STORAGE_KEY, key);
  document.getElementById("apiSetup").style.display="none";
  alert("✅ API 키가 저장되었습니다!");
  loadAll();
}

// ── 유틸 ─────────────────────────────────────────────────────────
function rateColor(r){ return r>=60?"rate-high":r>=50?"rate-mid":"rate-low"; }
function setStatus(type, text){
  const dot=document.getElementById("statusDot");
  dot.className="status-dot "+(type==="ok"?"dot-green":type==="err"?"dot-red":"dot-yellow");
  document.getElementById("statusText").textContent=text;
}
function toKST(isoStr){
  try{
    const dt=new Date(isoStr);
    return dt.toLocaleString("ko-KR",{timeZone:"Asia/Seoul",month:"2-digit",day:"2-digit",hour:"2-digit",minute:"2-digit",hour12:false});
  }catch{return isoStr.slice(0,10);}
}
function todayKST(){
  return new Date().toLocaleDateString("ko-KR",{timeZone:"Asia/Seoul",year:"numeric",month:"2-digit",day:"2-digit"}).replace(/\. /g,"-").replace(".","");
}

// ── 오즈 계산 ─────────────────────────────────────────────────────
function calcRates(game, sportInfo){
  const home=game.home_team, away=game.away_team;
  const bookmakers=game.bookmakers||[];
  if(!bookmakers.length) return null;

  let hp=[],ap=[],dp=[];
  bookmakers.forEach(bm=>{
    const w = bm.key==="pinnacle"?2:1;
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

  const avg=arr=>arr.reduce((s,v)=>s+v,0)/arr.length;
  const ah=avg(hp), aa=ap.length?avg(ap):0, ad=dp.length?avg(dp):0;
  const tot=ah+aa+ad;
  const hr=+(ah/tot*100).toFixed(1), ar=+(aa/tot*100).toFixed(1);
  const dr=dp.length?+(ad/tot*100).toFixed(1):null;
  const bmNames=bookmakers.map(b=>b.title);

  return {
    id:game.id, league:sportInfo.label, sub_league:sportInfo.sub,
    home, away, match:`${home} vs ${away}`,
    game_time:toKST(game.commence_time),
    home_rate:hr, away_rate:ar, draw_rate:dr, win_rate:hr,
    bookmakers:bmNames, bm_count:bmNames.length,
    source:bmNames.slice(0,3).join(", ")+(bmNames.length>3?` 외 ${bmNames.length-3}개`:""),
  };
}

// ── API 호출 ──────────────────────────────────────────────────────
async function fetchSport(key, sportInfo, apiKey){
  try{
    const url=`${ODDS_API_BASE}/sports/${key}/odds?apiKey=${apiKey}&regions=us,eu,uk&markets=h2h&bookmakers=${BOOKMAKERS}&dateFormat=iso&oddsFormat=decimal`;
    const r=await fetch(url);
    if(r.status===401) throw new Error("API 키가 잘못되었습니다.");
    if(r.status===429) throw new Error("API 요청 한도 초과");
    if(r.status===422) return [];   // 시즌 없음
    if(!r.ok) return [];
    const games=await r.json();
    return games.map(g=>calcRates(g,sportInfo)).filter(Boolean);
  }catch(e){
    console.warn(key,e.message);
    if(e.message.includes("API 키")) throw e;
    return [];
  }
}

// ── TOP4 선정 ─────────────────────────────────────────────────────
function pickTop4(games){
  const sorted=[...games].sort((a,b)=>b.win_rate-a.win_rate);
  const top4=[], seen={};
  // 1차: 리그별 1개씩
  for(const g of sorted){
    const k=g.league+g.sub_league;
    if(!seen[k]&&top4.length<4){top4.push(g);seen[k]=1;}
  }
  // 2차: 부족하면 승률순 채우기
  for(const g of sorted){
    if(!top4.includes(g)&&top4.length<4) top4.push(g);
  }
  return top4;
}

// ── 렌더링 ───────────────────────────────────────────────────────
function cardHTML(g, rank){
  const rc=`rank${rank}`;
  const hw=Math.round(g.home_rate/(g.home_rate+g.away_rate)*100);
  return `<div class="card ${rc}">
    <div class="card-top">
      <div class="card-left">
        <div class="card-rank">${RANK_LABELS[rank-1]}</div>
        <div class="card-league-wrap">
          <div class="card-league league-${g.league}">${g.league}</div>
          <div class="card-sub">${g.sub_league}</div>
        </div>
      </div>
      <div class="card-rate-wrap">
        <div class="card-rate-label">홈팀 AI 승률</div>
        <div class="card-rate ${rateColor(g.home_rate)}">${g.home_rate}%</div>
      </div>
    </div>
    <div class="game-time"><div class="time-dot"></div>${g.game_time}</div>
    <div class="match-box">
      <div class="match-teams">
        <div class="team"><div class="team-name">${g.home}</div><div class="team-prob home-prob">${g.home_rate}%</div></div>
        <div class="vs-box">VS</div>
        <div class="team"><div class="team-name">${g.away}</div><div class="team-prob away-prob">${g.away_rate}%</div></div>
      </div>
      ${g.draw_rate!=null?`<div class="draw-row">무승부 ${g.draw_rate}%</div>`:""}
    </div>
    <div class="prob-bar-wrap">
      <div class="prob-bar-labels"><span>${g.home}</span><span>${g.away}</span></div>
      <div class="prob-bar">
        <div class="prob-bar-home" style="width:${hw}%"></div>
        <div class="prob-bar-away" style="width:${100-hw}%"></div>
      </div>
    </div>
    <div class="bm-row">
      ${g.bookmakers.slice(0,4).map(b=>`<span class="bm-icon">${b}</span>`).join("")}
      ${g.bm_count>4?`<span class="bm-count">외 ${g.bm_count-4}개</span>`:""}
    </div>
  </div>`;
}

function renderTop4(top4){
  const el=document.getElementById("top4Area");
  if(!top4.length){
    el.innerHTML=`<div class="empty-state"><div class="empty-icon">📭</div><div class="empty-text">오늘 분석 가능한 경기가 없습니다</div><div class="empty-sub">경기 일정이 없거나 오즈가 아직 공개되지 않았습니다</div></div>`;
    return;
  }
  el.innerHTML=top4.map((g,i)=>cardHTML(g,i+1)).join("");
}

function renderAll(games){
  const el=document.getElementById("allArea");
  if(!games.length){el.innerHTML=`<div class="empty-state"><div class="empty-sub">전체 경기 데이터가 없습니다</div></div>`;return;}
  const groups={};
  games.forEach(g=>{
    const k=g.league+" "+g.sub_league;
    if(!groups[k])groups[k]={league:g.league,sub:g.sub_league,games:[]};
    groups[k].games.push(g);
  });
  el.innerHTML=Object.values(groups).map(gr=>`
    <div class="league-group">
      <div class="league-title lt-${gr.league}">${gr.league} ${gr.sub}</div>
      ${gr.games.map(g=>`
        <div class="mini-card">
          <div class="mini-left">
            <div class="mini-match">${g.match}</div>
            <div class="mini-time">🕐 ${g.game_time}</div>
            <div class="mini-bm">${g.source}</div>
          </div>
          <div class="mini-rate ${rateColor(g.home_rate)}">${g.home_rate}%</div>
        </div>`).join("")}
    </div>`).join("");
}

// ── 데모 데이터 ───────────────────────────────────────────────────
function loadDemo(){
  const today=todayKST();
  const demo={
    top4:[
      {id:"d1",league:"해외축구",sub_league:"라리가",home:"레알 마드리드",away:"바르셀로나",match:"레알 마드리드 vs 바르셀로나",game_time:`${today} 22:00`,home_rate:58.3,away_rate:28.4,draw_rate:13.3,win_rate:58.3,bookmakers:["Pinnacle","Bet365","Bwin","Unibet"],bm_count:8,source:"Pinnacle, Bet365, Bwin 외 5개"},
      {id:"d2",league:"미국야구",sub_league:"MLB",home:"New York Yankees",away:"Boston Red Sox",match:"NYY vs BOS",game_time:`${today} 08:05`,home_rate:61.2,away_rate:38.8,draw_rate:null,win_rate:61.2,bookmakers:["DraftKings","FanDuel","Pinnacle"],bm_count:6,source:"DraftKings, FanDuel, Pinnacle 외 3개"},
      {id:"d3",league:"한국야구",sub_league:"KBO",home:"KIA 타이거즈",away:"삼성 라이온즈",match:"KIA vs 삼성",game_time:`${today} 17:00`,home_rate:55.7,away_rate:44.3,draw_rate:null,win_rate:55.7,bookmakers:["Pinnacle","Betway"],bm_count:3,source:"Pinnacle, Betway"},
      {id:"d4",league:"한국축구",sub_league:"K리그1",home:"울산 HD",away:"전북 현대",match:"울산 vs 전북",game_time:`${today} 19:30`,home_rate:52.1,away_rate:27.3,draw_rate:20.6,win_rate:52.1,bookmakers:["Pinnacle","Unibet"],bm_count:4,source:"Pinnacle, Unibet 외 1개"},
    ],
    all_today:[]
  };
  document.getElementById("demoBadge").style.display="block";
  document.getElementById("apiSetup").style.display="block";
  renderTop4(demo.top4);
  renderAll([]);
  document.getElementById("allToggle").style.display="none";
  setStatus("yellow","데모 데이터 표시 중 — API 키를 입력하면 실제 데이터로 전환됩니다");
  document.getElementById("navUpdate").textContent="데모";
}

// ── 메인 로드 ─────────────────────────────────────────────────────
async function loadAll(){
  const apiKey=getApiKey();
  if(!apiKey){ loadDemo(); return; }

  document.getElementById("apiSetup").style.display="none";
  document.getElementById("demoBadge").style.display="none";
  document.getElementById("top4Area").innerHTML=`<div class="empty-state"><div class="spinner"></div><br><br>오즈 데이터 수집 중...</div>`;
  setStatus("yellow","실시간 오즈 데이터 수집 중...");
  document.getElementById("refreshBtn").disabled=true;

  try{
    const allGames=[];
    for(const sport of SPORTS){
      setStatus("yellow",`${sport.label} ${sport.sub} 수집 중...`);
      const games=await fetchSport(sport.key, sport, apiKey);
      allGames.push(...games);
    }

    if(!allGames.length){
      setStatus("yellow","경기 데이터 없음 — 경기 일정이 없거나 오즈가 아직 공개 전입니다");
      renderTop4([]);
      renderAll([]);
      return;
    }

    const top4=pickTop4(allGames);
    DATA={top4, all:allGames};

    renderTop4(top4);
    renderAll(allGames.sort((a,b)=>b.win_rate-a.win_rate));

    const now=new Date().toLocaleTimeString("ko-KR",{timeZone:"Asia/Seoul",hour:"2-digit",minute:"2-digit"});
    document.getElementById("navUpdate").textContent=now+" 갱신";
    setStatus("ok",`실시간 데이터 · 총 ${allGames.length}경기 분석 완료`);

    const toggle=document.getElementById("allToggle");
    toggle.style.display="flex";
    toggle.innerHTML=`📋 전체 경기 보기 (${allGames.length}경기)`;

  }catch(err){
    console.error(err);
    if(err.message.includes("API 키")){
      setStatus("err","API 키 오류 — 키를 확인해주세요");
      localStorage.removeItem(STORAGE_KEY);
      document.getElementById("apiSetup").style.display="block";
      document.getElementById("apiKeyInput").value="";
    } else {
      setStatus("err","데이터 로드 실패 — 잠시 후 다시 시도해주세요");
    }
    loadDemo();
  }finally{
    document.getElementById("refreshBtn").disabled=false;
  }
}

function toggleAll(){
  allShown=!allShown;
  document.getElementById("allArea").style.display=allShown?"block":"none";
  const cnt=DATA?.all?.length||0;
  document.getElementById("allToggle").innerHTML=allShown?
    `📋 전체 경기 접기`:
    `📋 전체 경기 보기 (${cnt}경기)`;
  if(allShown) document.getElementById("allArea").scrollIntoView({behavior:"smooth"});
}

function scrollToTop(){ window.scrollTo({top:0,behavior:"smooth"}); }

function showInfo(){
  const key=getApiKey();
  alert(`WIN-4 스포츠 분석 Pro\n\n📡 데이터 출처\nThe Odds API (Pinnacle·Bet365·Bwin 등)\n해외축구 / 한국축구 / MLB / KBO\n\n🔑 API 키 상태\n${key?"✅ 등록됨 (앞 8자리: "+key.slice(0,8)+"...)":"❌ 미등록 (데모 모드)"}\n\n🤖 AI 승률 계산\n여러 북메이커 배당률 집계\nPinnacle 가중치 2배 적용\n\n⚠️ 주의\n본 서비스는 참고용이며\n스포츠 베팅을 권장하지 않습니다.`);
}

// ── 초기 실행 ─────────────────────────────────────────────────────
loadAll();
</script>
</body>
</html>
HTMLEOF
echo "완료"
