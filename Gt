<!DOCTYPE html>

<html lang="fr">
<head>
  <meta name="apple-mobile-web-app-capable" content="yes">
  <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
  <meta name="apple-mobile-web-app-title" content="GT PILOT">
  <meta name="mobile-web-app-capable" content="yes">
  <meta name="theme-color" content="#09090B">
  <link rel="apple-touch-icon" href="icon-512.png">
  <link rel="manifest" href="manifest.json">
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>GT PILOT — Performance System</title>
  <link href="https://fonts.googleapis.com/css2?family=Barlow+Condensed:wght@300;400;600;700;900&family=Barlow:wght@300;400;500&family=Share+Tech+Mono&display=swap" rel="stylesheet">
  <style>
:root {
  --red: #E8001D;
  --orange: #FF5722;
  --gold: #FFC107;
  --dark: #09090B;
  --dark2: #111114;
  --dark3: #1A1A20;
  --border: rgba(255,255,255,0.07);
  --text: #DEDEE8;
  --muted: #55556A;
  --green: #00E676;
  --blue: #00B0FF;
  --purple: #CE93D8;
}
*{margin:0;padding:0;box-sizing:border-box;}
body{font-family:'Barlow',sans-serif;background:var(--dark);color:var(--text);min-height:100vh;overflow-x:hidden;}
body::after{content:'';position:fixed;inset:0;background:radial-gradient(ellipse at 80% 0%,rgba(232,0,29,0.04) 0%,transparent 60%),radial-gradient(ellipse at 0% 100%,rgba(0,176,255,0.03) 0%,transparent 50%);pointer-events:none;z-index:0;}

nav{position:sticky;top:0;z-index:200;background:rgba(9,9,11,0.96);backdrop-filter:blur(24px);border-bottom:1px solid var(–border);display:flex;align-items:center;justify-content:space-between;padding:0 1.5rem;height:56px;}
.logo{font-family:‘Barlow Condensed’,sans-serif;font-weight:900;font-size:1.3rem;letter-spacing:4px;color:#fff;display:flex;align-items:center;gap:8px;text-transform:uppercase;}
.logo-line{width:28px;height:3px;background:linear-gradient(90deg,var(–red),var(–orange));}
.nav-tabs{display:flex;gap:2px;overflow-x:auto;-webkit-overflow-scrolling:touch;}
.nav-tab{font-family:‘Barlow Condensed’,sans-serif;font-weight:700;font-size:0.7rem;letter-spacing:2px;text-transform:uppercase;padding:5px 12px;border:1px solid transparent;border-radius:2px;background:transparent;color:var(–muted);cursor:pointer;transition:all .2s;white-space:nowrap;}
.nav-tab:hover{color:var(–text);}
.nav-tab.active{background:var(–red);color:#fff;border-color:var(–red);}

main{padding:1.5rem;max-width:1360px;margin:0 auto;position:relative;z-index:1;}
.page{display:none;animation:fadeUp .3s ease;}
.page.active{display:block;}
@keyframes fadeUp{from{opacity:0;transform:translateY(10px);}to{opacity:1;transform:translateY(0);}}

.hero{background:linear-gradient(135deg,#111114 0%,#0d0d12 100%);border:1px solid var(–border);border-radius:4px;padding:2.5rem;margin-bottom:1.5rem;position:relative;overflow:hidden;}
.hero::before{content:’’;position:absolute;top:-80px;right:-60px;width:400px;height:400px;background:radial-gradient(circle,rgba(232,0,29,0.1) 0%,transparent 70%);pointer-events:none;}
.hero-eyebrow{font-family:‘Share Tech Mono’,monospace;font-size:.6rem;letter-spacing:4px;color:var(–red);text-transform:uppercase;margin-bottom:.7rem;}
.hero-title{font-family:‘Barlow Condensed’,sans-serif;font-weight:900;font-size:clamp(2.2rem,4vw,3.6rem);line-height:.92;text-transform:uppercase;color:#fff;margin-bottom:.5rem;}
.hero-title em{color:var(–red);font-style:normal;}
.hero-sub{font-size:.85rem;color:var(–muted);margin-bottom:2rem;letter-spacing:.5px;}
.gf-badge{display:inline-flex;align-items:center;gap:6px;background:rgba(0,230,118,.12);border:1px solid rgba(0,230,118,.25);color:var(–green);font-family:‘Barlow Condensed’;font-size:.7rem;font-weight:700;letter-spacing:2px;text-transform:uppercase;padding:4px 12px;border-radius:20px;}

/* PHASE BANNER */
.phase-banner{border-radius:4px;padding:1.2rem 1.5rem;margin-bottom:1.5rem;border:1px solid;position:relative;overflow:hidden;}
.phase-banner::before{content:’’;position:absolute;top:0;left:0;right:0;height:3px;}
.phase-banner.training{background:rgba(0,176,255,.07);border-color:rgba(0,176,255,.25);}
.phase-banner.training::before{background:var(–blue);}
.phase-banner.taper{background:rgba(255,193,7,.07);border-color:rgba(255,193,7,.25);}
.phase-banner.taper::before{background:var(–gold);}
.phase-banner.prerace{background:rgba(232,0,29,.07);border-color:rgba(232,0,29,.25);}
.phase-banner.prerace::before{background:linear-gradient(90deg,var(–red),var(–orange));}
.phase-banner.race{background:rgba(232,0,29,.12);border-color:rgba(232,0,29,.4);}
.phase-banner.race::before{background:linear-gradient(90deg,var(–red),var(–orange));}
.phase-banner.recovery{background:rgba(0,230,118,.07);border-color:rgba(0,230,118,.25);}
.phase-banner.recovery::before{background:var(–green);}
.phase-banner.jetlag{background:rgba(206,147,216,.07);border-color:rgba(206,147,216,.25);}
.phase-banner.jetlag::before{background:var(–purple);}
.phase-label{font-family:‘Share Tech Mono’,monospace;font-size:.55rem;letter-spacing:3px;text-transform:uppercase;margin-bottom:.4rem;}
.phase-banner.training .phase-label{color:var(–blue);}
.phase-banner.taper .phase-label{color:var(–gold);}
.phase-banner.prerace .phase-label,.phase-banner.race .phase-label{color:var(–red);}
.phase-banner.recovery .phase-label{color:var(–green);}
.phase-banner.jetlag .phase-label{color:var(–purple);}
.phase-title{font-family:‘Barlow Condensed’,sans-serif;font-weight:900;font-size:1.4rem;text-transform:uppercase;color:#fff;margin-bottom:.3rem;}
.phase-desc{font-size:.82rem;color:var(–muted);line-height:1.5;}
.phase-meta{display:flex;gap:1rem;margin-top:.8rem;flex-wrap:wrap;}
.phase-chip{font-family:‘Share Tech Mono’;font-size:.6rem;padding:3px 10px;border-radius:10px;border:1px solid;}

.stats-row{display:grid;grid-template-columns:repeat(4,1fr);gap:1px;background:var(–border);border-radius:3px;overflow:hidden;border:1px solid var(–border);}
.stat-box{background:var(–dark2);padding:1.1rem 1.3rem;}
.stat-label{font-family:‘Share Tech Mono’,monospace;font-size:.55rem;letter-spacing:2px;color:var(–muted);text-transform:uppercase;margin-bottom:.35rem;}
.stat-value{font-family:‘Barlow Condensed’,sans-serif;font-weight:800;font-size:1.6rem;color:#fff;line-height:1;}
.stat-value.red{color:var(–red);}
.stat-value.gold{color:var(–gold);}
.stat-value.green{color:var(–green);}
.stat-value.blue{color:var(–blue);}
.stat-value.purple{color:var(–purple);}

.grid-2{display:grid;grid-template-columns:1fr 1fr;gap:1.2rem;}
.grid-3{display:grid;grid-template-columns:repeat(3,1fr);gap:1.2rem;}
.grid-auto{display:grid;grid-template-columns:repeat(auto-fill,minmax(280px,1fr));gap:1.2rem;}

.card{background:var(–dark2);border:1px solid var(–border);border-radius:4px;padding:1.4rem;position:relative;overflow:hidden;transition:border-color .25s;}
.card:hover{border-color:rgba(255,255,255,.12);}
.card-accent{position:absolute;top:0;left:0;right:0;height:2px;}
.card-accent.red{background:linear-gradient(90deg,var(–red),var(–orange));}
.card-accent.gold{background:var(–gold);}
.card-accent.green{background:var(–green);}
.card-accent.blue{background:var(–blue);}
.card-accent.purple{background:var(–purple);}

.card-title{font-family:‘Barlow Condensed’,sans-serif;font-weight:700;font-size:.85rem;letter-spacing:2.5px;text-transform:uppercase;color:var(–text);margin-bottom:1rem;display:flex;align-items:center;gap:8px;}
.section-title{font-family:‘Barlow Condensed’,sans-serif;font-weight:900;font-size:1.3rem;letter-spacing:3px;text-transform:uppercase;color:#fff;margin:2rem 0 1rem;display:flex;align-items:center;gap:10px;}
.section-title::after{content:’’;flex:1;height:1px;background:var(–border);}

.tag{font-family:‘Barlow Condensed’;font-size:.6rem;font-weight:700;letter-spacing:2px;text-transform:uppercase;padding:2px 8px;border-radius:2px;}
.tag-red{background:rgba(232,0,29,.15);border:1px solid rgba(232,0,29,.3);color:var(–red);}
.tag-green{background:rgba(0,230,118,.12);border:1px solid rgba(0,230,118,.25);color:var(–green);}
.tag-gold{background:rgba(255,193,7,.12);border:1px solid rgba(255,193,7,.25);color:var(–gold);}
.tag-blue{background:rgba(0,176,255,.12);border:1px solid rgba(0,176,255,.25);color:var(–blue);}
.tag-purple{background:rgba(206,147,216,.12);border:1px solid rgba(206,147,216,.25);color:var(–purple);}

.alert{border-radius:3px;padding:.85rem 1rem;margin-bottom:.8rem;font-size:.82rem;color:var(–text);line-height:1.5;}
.alert.red{background:rgba(232,0,29,.07);border:1px solid rgba(232,0,29,.2);border-left:3px solid var(–red);}
.alert.gold{background:rgba(255,193,7,.06);border:1px solid rgba(255,193,7,.18);border-left:3px solid var(–gold);}
.alert.green{background:rgba(0,230,118,.06);border:1px solid rgba(0,230,118,.18);border-left:3px solid var(–green);}
.alert.blue{background:rgba(0,176,255,.06);border:1px solid rgba(0,176,255,.18);border-left:3px solid var(–blue);}
.alert.purple{background:rgba(206,147,216,.06);border:1px solid rgba(206,147,216,.18);border-left:3px solid var(–purple);}
.alert-title{font-family:‘Barlow Condensed’;font-weight:700;font-size:.68rem;letter-spacing:2px;text-transform:uppercase;margin-bottom:.3rem;}
.alert.red .alert-title{color:var(–red);}
.alert.gold .alert-title{color:var(–gold);}
.alert.green .alert-title{color:var(–green);}
.alert.blue .alert-title{color:var(–blue);}
.alert.purple .alert-title{color:var(–purple);}

.meal-card{background:var(–dark3);border:1px solid var(–border);border-radius:3px;padding:.9rem 1.1rem;margin-bottom:.5rem;display:flex;align-items:flex-start;gap:12px;transition:border-color .2s,transform .2s;}
.meal-card:hover{border-color:rgba(232,0,29,.3);transform:translateX(3px);}
.meal-time{font-family:‘Share Tech Mono’,monospace;font-size:.6rem;color:var(–red);min-width:52px;padding-top:3px;line-height:1.3;}
.meal-content{flex:1;}
.meal-name{font-family:‘Barlow Condensed’;font-size:.95rem;font-weight:700;color:#fff;margin-bottom:2px;}
.meal-desc{font-size:.78rem;color:var(–muted);line-height:1.45;}
.meal-macros{text-align:right;font-family:‘Share Tech Mono’,monospace;font-size:.6rem;white-space:nowrap;}
.macro-kcal{color:var(–gold);font-size:.9rem;font-weight:700;}

.supp-card{background:var(–dark3);border:1px solid var(–border);border-radius:3px;padding:1rem 1.1rem;margin-bottom:.5rem;display:flex;gap:12px;align-items:flex-start;}
.supp-dot{width:8px;height:8px;border-radius:50%;flex-shrink:0;margin-top:5px;}
.supp-info{flex:1;}
.supp-name{font-family:‘Barlow Condensed’;font-weight:700;font-size:.95rem;color:#fff;margin-bottom:2px;}
.supp-dose{font-family:‘Share Tech Mono’;font-size:.62rem;color:var(–gold);margin-bottom:3px;}
.supp-why{font-size:.78rem;color:var(–muted);line-height:1.4;}
.supp-warning{font-size:.72rem;color:var(–red);margin-top:3px;}

.exercise-item{background:var(–dark3);border:1px solid var(–border);border-radius:3px;padding:.9rem 1.1rem;margin-bottom:.5rem;display:flex;align-items:center;gap:12px;transition:all .2s;}
.exercise-item:hover{border-color:rgba(0,176,255,.35);transform:translateX(4px);}
.ex-num{font-family:‘Barlow Condensed’;font-weight:900;font-size:1.8rem;color:rgba(255,255,255,.07);min-width:38px;}
.ex-info{flex:1;}
.ex-name{font-family:‘Barlow Condensed’;font-weight:700;font-size:.95rem;color:#fff;margin-bottom:2px;}
.ex-detail{font-size:.78rem;color:var(–muted);}
.ex-badge{font-family:‘Share Tech Mono’;font-size:.6rem;padding:3px 9px;border-radius:2px;}

.progress-bar{height:3px;background:rgba(255,255,255,.07);border-radius:2px;overflow:hidden;margin-top:.4rem;}
.progress-fill{height:100%;border-radius:2px;}
.fill-red{background:linear-gradient(90deg,var(–red),var(–orange));}
.fill-gold{background:var(–gold);}
.fill-green{background:var(–green);}
.fill-blue{background:var(–blue);}

.timeline{position:relative;padding-left:22px;}
.timeline::before{content:’’;position:absolute;left:7px;top:8px;bottom:8px;width:1px;background:linear-gradient(180deg,var(–red),rgba(255,255,255,.1));}
.tl-item{position:relative;margin-bottom:1.1rem;}
.tl-item::before{content:’’;position:absolute;left:-18px;top:7px;width:7px;height:7px;border-radius:50%;background:var(–red);border:2px solid var(–dark);}
.tl-time{font-family:‘Share Tech Mono’;font-size:.58rem;color:var(–red);margin-bottom:2px;}
.tl-action{font-family:‘Barlow Condensed’;font-weight:700;color:#fff;font-size:.95rem;margin-bottom:2px;}
.tl-detail{font-size:.78rem;color:var(–muted);line-height:1.4;}

.week-days{display:grid;grid-template-columns:repeat(7,1fr);gap:4px;margin-bottom:1.2rem;}
.day-btn{background:var(–dark3);border:1px solid var(–border);border-radius:3px;padding:.5rem .2rem;text-align:center;cursor:pointer;transition:all .2s;}
.day-btn:hover{border-color:rgba(232,0,29,.4);}
.day-btn.active{background:var(–red);border-color:var(–red);}
.day-name{font-family:‘Barlow Condensed’;font-size:.6rem;letter-spacing:1px;color:var(–muted);text-transform:uppercase;display:block;}
.day-btn.active .day-name{color:rgba(255,255,255,.65);}
.day-num{font-family:‘Barlow Condensed’;font-weight:700;font-size:1rem;color:#fff;display:block;}
.day-dot{width:4px;height:4px;border-radius:50%;margin:3px auto 0;}

.selector{display:flex;gap:3px;background:var(–dark3);border:1px solid var(–border);border-radius:3px;padding:3px;margin-bottom:1.2rem;flex-wrap:wrap;}
.sel-btn{flex:1;padding:.45rem .5rem;background:transparent;border:none;color:var(–muted);font-family:‘Barlow Condensed’;font-size:.68rem;font-weight:700;letter-spacing:1.5px;text-transform:uppercase;border-radius:2px;cursor:pointer;transition:all .2s;white-space:nowrap;}
.sel-btn.active{background:var(–red);color:#fff;}
.sel-btn:hover:not(.active){color:var(–text);}

.hydration-bar{display:flex;gap:3px;margin:.7rem 0;}
.h-unit{flex:1;height:28px;border-radius:2px;background:rgba(0,176,255,.07);border:1px solid rgba(0,176,255,.12);cursor:pointer;transition:all .18s;}
.h-unit.filled{background:rgba(0,176,255,.32);border-color:var(–blue);}
.h-unit:hover{border-color:var(–blue);}

.checklist-item{display:flex;align-items:center;gap:10px;padding:.55rem 0;border-bottom:1px solid rgba(255,255,255,.04);cursor:pointer;transition:opacity .2s;}
.check-box{width:17px;height:17px;border:1.5px solid var(–muted);border-radius:2px;display:flex;align-items:center;justify-content:center;font-size:.65rem;flex-shrink:0;transition:all .2s;}
.checklist-item.done{opacity:.6;}
.checklist-item.done .check-box{background:var(–green);border-color:var(–green);color:#000;}
.checklist-item.done .check-label{text-decoration:line-through;color:var(–muted);}
.check-label{font-size:.85rem;}

.tz-grid{display:grid;grid-template-columns:repeat(4,1fr);gap:1px;background:var(–border);border-radius:3px;overflow:hidden;margin-bottom:1rem;}
.tz-card{background:var(–dark3);padding:.9rem .8rem;text-align:center;}
.tz-city{font-family:‘Barlow Condensed’;font-size:.65rem;font-weight:700;letter-spacing:1.5px;text-transform:uppercase;color:var(–muted);margin-bottom:.3rem;}
.tz-time{font-family:‘Share Tech Mono’;font-size:1.4rem;color:#fff;}
.tz-time.active{color:var(–gold);}

.toggle-section{border:1px solid var(–border);border-radius:3px;overflow:hidden;margin-bottom:.5rem;}
.toggle-header{padding:.85rem 1.1rem;background:var(–dark3);cursor:pointer;display:flex;justify-content:space-between;align-items:center;font-family:‘Barlow Condensed’;font-weight:700;text-transform:uppercase;letter-spacing:1.5px;font-size:.85rem;color:#fff;transition:background .2s;user-select:none;}
.toggle-header:hover{background:#1e1e26;}
.toggle-arrow{transition:transform .25s;color:var(–muted);font-size:.75rem;}
.toggle-body{display:none;padding:1.1rem;background:var(–dark2);border-top:1px solid var(–border);}
.toggle-section.open .toggle-arrow{transform:rotate(180deg);}
.toggle-section.open .toggle-body{display:block;}

.gf-chip{display:inline-flex;align-items:center;gap:4px;font-family:‘Share Tech Mono’;font-size:.58rem;padding:2px 7px;border-radius:10px;background:rgba(0,230,118,.1);border:1px solid rgba(0,230,118,.2);color:var(–green);}

/* CALENDAR STYLES */
.cal-grid{display:grid;grid-template-columns:repeat(7,1fr);gap:2px;margin-bottom:1rem;}
.cal-header-cell{font-family:‘Barlow Condensed’;font-size:.65rem;font-weight:700;letter-spacing:2px;text-transform:uppercase;color:var(–muted);text-align:center;padding:.4rem 0;}
.cal-day{background:var(–dark3);border:1px solid var(–border);border-radius:2px;padding:.4rem;min-height:52px;cursor:pointer;transition:all .2s;position:relative;}
.cal-day:hover{border-color:rgba(255,255,255,.15);}
.cal-day.other-month{opacity:.3;}
.cal-day.today{border-color:var(–red);background:rgba(232,0,29,.08);}
.cal-day-num{font-family:‘Barlow Condensed’;font-weight:700;font-size:.85rem;color:#fff;margin-bottom:2px;}
.cal-day.today .cal-day-num{color:var(–red);}
.cal-event{font-family:‘Barlow Condensed’;font-size:.55rem;font-weight:700;letter-spacing:.5px;padding:1px 4px;border-radius:1px;margin-top:2px;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;}
.cal-event.imsa{background:rgba(0,176,255,.3);color:var(–blue);}
.cal-event.wec{background:rgba(255,193,7,.3);color:var(–gold);}
.cal-event.igtc{background:rgba(232,0,29,.3);color:#ff6b6b;}
.cal-event.gtwc{background:rgba(0,230,118,.25);color:var(–green);}
.cal-event.elms{background:rgba(206,147,216,.25);color:var(–purple);}
.cal-event.nls{background:rgba(255,87,34,.25);color:var(–orange);}
.cal-event.24hseries{background:rgba(255,255,255,.15);color:#fff;}
.cal-event.test{background:rgba(255,255,255,.1);color:var(–muted);}

.event-detail-card{background:var(–dark2);border:1px solid var(–border);border-radius:4px;padding:1.2rem;margin-bottom:1rem;}
.event-champ-badge{font-family:‘Barlow Condensed’;font-size:.65rem;font-weight:700;letter-spacing:2px;text-transform:uppercase;padding:3px 10px;border-radius:2px;margin-bottom:.6rem;display:inline-block;}

::-webkit-scrollbar{width:5px;}
::-webkit-scrollbar-track{background:var(–dark);}
::-webkit-scrollbar-thumb{background:rgba(255,255,255,.08);border-radius:3px;}

.row{display:flex;align-items:center;gap:.8rem;}
.flex1{flex:1;}
.mb1{margin-bottom:.6rem;}
.mb2{margin-bottom:1.2rem;}
.mt1{margin-top:.6rem;}
.muted{color:var(–muted);}
small{font-size:.78rem;color:var(–muted);}
hr.divider{border:none;border-top:1px solid var(–border);margin:.8rem 0;}

@media(max-width:850px){
.grid-2,.grid-3,.stats-row,.tz-grid{grid-template-columns:1fr;}
main{padding:1rem;}
.hero{padding:1.5rem;}
nav{padding:0 .8rem;}
.nav-tabs{gap:1px;}
.nav-tab{padding:4px 7px;font-size:.62rem;}
.logo{font-size:1rem;}
.cal-grid{grid-template-columns:repeat(7,1fr);}
.cal-day{min-height:38px;padding:.25rem;}
.cal-event{display:none;}
.cal-day-num{font-size:.75rem;}
}
</style>

</head>
<body>

<nav>
  <div class="logo">
    <div class="logo-line"></div>
    GT PILOT
  </div>
  <div class="nav-tabs">
    <button class="nav-tab active" onclick="showPage('dashboard',this)">Dashboard</button>
    <button class="nav-tab" onclick="showPage('calendrier',this)">Calendrier</button>
    <button class="nav-tab" onclick="showPage('nutrition',this)">Nutrition</button>
    <button class="nav-tab" onclick="showPage('supplements',this)">Suppléments</button>
    <button class="nav-tab" onclick="showPage('training',this)">Entraînement</button>
    <button class="nav-tab" onclick="showPage('race',this)">Course</button>
    <button class="nav-tab" onclick="showPage('travel',this)">Voyage</button>
  </div>
</nav>

<main>

<!-- ===== DASHBOARD ===== -->

<div class="page active" id="page-dashboard">
  <div class="hero">
    <div class="hero-eyebrow">// Système de performance — Pilote GT Endurance</div>
    <div class="hero-title">GT ENDURANCE<br><em>PERFORMANCE</em></div>
    <div class="hero-sub">Nutrition Gluten-Free · Suppléments · Training · Jet Lag Protocol</div>
    <div class="gf-badge">✓ 100% GLUTEN FREE</div>
  </div>

  <!-- PHASE BANNER DYNAMIQUE -->

  <div id="phase-banner" class="phase-banner training">
    <div class="phase-label" id="phase-label">PHASE ACTUELLE</div>
    <div class="phase-title" id="phase-title">Chargement...</div>
    <div class="phase-desc" id="phase-desc"></div>
    <div class="phase-meta" id="phase-meta"></div>
  </div>

  <div class="stats-row" style="margin-bottom:1.5rem;">
    <div class="stat-box">
      <div class="stat-label">Phase</div>
      <div class="stat-value red" id="stat-phase" style="font-size:1rem;">—</div>
    </div>
    <div class="stat-box">
      <div class="stat-label">Prochaine course</div>
      <div class="stat-value gold" id="stat-nextrace" style="font-size:.85rem;">—</div>
    </div>
    <div class="stat-box">
      <div class="stat-label">Dans</div>
      <div class="stat-value green" id="stat-daysto">—</div>
    </div>
    <div class="stat-box">
      <div class="stat-label">Jet lag</div>
      <div class="stat-value blue" id="stat-jetlag">—</div>
    </div>
  </div>

  <!-- RECOMMANDATIONS DYNAMIQUES -->

  <div class="grid-2" style="margin-bottom:1.5rem;">

```
<!-- NUTRITION DU JOUR -->
<div class="card" id="dash-nutrition-card">
  <div class="card-accent red"></div>
  <div class="card-title">🥗 Nutrition du jour</div>
  <div id="dash-nutrition-content"></div>
</div>

<!-- TRAINING DU JOUR -->
<div class="card" id="dash-training-card">
  <div class="card-accent blue"></div>
  <div class="card-title">💪 Entraînement du jour</div>
  <div id="dash-training-content"></div>
</div>
```

  </div>

  <div class="grid-2" style="margin-bottom:1.5rem;">

```
<!-- SUPPLÉMENTS DU JOUR -->
<div class="card" id="dash-supps-card">
  <div class="card-accent gold"></div>
  <div class="card-title">💊 Suppléments du jour</div>
  <div id="dash-supps-content"></div>
</div>

<!-- HYDRATATION -->
<div class="card">
  <div class="card-accent blue"></div>
  <div class="card-title"><span class="icon">💧</span> Hydratation du jour</div>
  <div style="font-size:.78rem;color:var(--muted);margin-bottom:.6rem;" id="dash-hydra-target">Objectif : 3,5 L/j training</div>
  <div class="hydration-bar" id="hydrationBar"></div>
  <div class="row mt1">
    <small id="hydrationText">0 / 14 verres · 0 ml</small>
    <button onclick="resetHydration()" style="margin-left:auto;background:transparent;border:1px solid var(--border);color:var(--muted);padding:2px 10px;border-radius:2px;font-size:.65rem;cursor:pointer;font-family:'Barlow Condensed';letter-spacing:1px;">RESET</button>
  </div>
</div>
```

  </div>

  <!-- CHECKLIST DYNAMIQUE -->

  <div class="section-title">Checklist du jour</div>
  <div class="grid-2">
    <div class="card" id="dash-checklist-physical">
      <div class="card-title">🏋️ Physique</div>
      <div id="dash-checklist-physical-items"></div>
    </div>
    <div class="card" id="dash-checklist-nutrition">
      <div class="card-title">🥗 Nutrition GF</div>
      <div id="dash-checklist-nutrition-items"></div>
    </div>
  </div>

  <!-- ALERTE JET LAG si applicable -->

  <div id="dash-jetlag-alert" style="display:none;margin-top:1.5rem;"></div>
</div>

<!-- ===== CALENDRIER ===== -->

<div class="page" id="page-calendrier">
  <div class="section-title">Calendrier 2026 <span class="tag tag-red">PUSHPAPY ON TOUR</span></div>

  <div class="stats-row" style="margin-bottom:1.5rem;">
    <div class="stat-box">
      <div class="stat-label">Total événements</div>
      <div class="stat-value gold">29</div>
    </div>
    <div class="stat-box">
      <div class="stat-label">Championnats</div>
      <div class="stat-value blue" style="font-size:1rem;">7</div>
    </div>
    <div class="stat-box">
      <div class="stat-label">24h races</div>
      <div class="stat-value red">5</div>
    </div>
    <div class="stat-box">
      <div class="stat-label">Long haul</div>
      <div class="stat-value purple" style="font-size:1rem;">8</div>
    </div>
  </div>

  <!-- LÉGENDE -->

  <div style="display:flex;gap:.5rem;flex-wrap:wrap;margin-bottom:1rem;">
    <span class="cal-event imsa" style="font-size:.65rem;padding:3px 10px;">IMSA</span>
    <span class="cal-event wec" style="font-size:.65rem;padding:3px 10px;">WEC</span>
    <span class="cal-event igtc" style="font-size:.65rem;padding:3px 10px;">IGTC</span>
    <span class="cal-event gtwc" style="font-size:.65rem;padding:3px 10px;">GTWC</span>
    <span class="cal-event elms" style="font-size:.65rem;padding:3px 10px;">ELMS</span>
    <span class="cal-event nls" style="font-size:.65rem;padding:3px 10px;">NLS</span>
    <span class="cal-event 24hseries" style="font-size:.65rem;padding:3px 10px;">24H Series</span>
    <span class="cal-event test" style="font-size:.65rem;padding:3px 10px;">TEST/PROLOGUE</span>
  </div>

  <!-- NAVIGATION MOIS -->

  <div style="display:flex;align-items:center;gap:1rem;margin-bottom:1rem;">
    <button onclick="changeMonth(-1)" style="background:var(--dark3);border:1px solid var(--border);color:var(--text);padding:6px 14px;border-radius:2px;cursor:pointer;font-family:'Barlow Condensed';font-weight:700;letter-spacing:1px;">◀</button>
    <div style="flex:1;text-align:center;font-family:'Barlow Condensed';font-weight:900;font-size:1.3rem;letter-spacing:3px;text-transform:uppercase;" id="cal-month-title">—</div>
    <button onclick="changeMonth(1)" style="background:var(--dark3);border:1px solid var(--border);color:var(--text);padding:6px 14px;border-radius:2px;cursor:pointer;font-family:'Barlow Condensed';font-weight:700;letter-spacing:1px;">▶</button>
  </div>

  <!-- GRILLE CALENDRIER -->

  <div class="cal-grid" id="cal-header"></div>
  <div class="cal-grid" id="cal-body"></div>

  <!-- ÉVÉNEMENT SÉLECTIONNÉ -->

  <div id="cal-selected-event" style="display:none;"></div>

  <!-- LISTE ÉVÉNEMENTS DU MOIS -->

  <div class="section-title" style="margin-top:1.5rem;">Événements du mois</div>
  <div id="cal-event-list"></div>

  <!-- PROCHAIN LONG HAUL -->

  <div class="section-title">Voyages long-courrier</div>
  <div id="cal-longhaul-list"></div>
</div>

<!-- ===== NUTRITION ===== -->

<div class="page" id="page-nutrition">
  <div class="section-title">Nutrition <span class="gf-badge">GLUTEN FREE</span></div>
  <div class="alert blue" id="nutri-phase-alert" style="margin-bottom:1rem;"></div>
  <div class="selector">
    <button class="sel-btn active" onclick="switchSection('nutri','training',this)">Training</button>
    <button class="sel-btn" onclick="switchSection('nutri','prerace',this)">J-3 Course</button>
    <button class="sel-btn" onclick="switchSection('nutri','race3h',this)">Course 3–6h</button>
    <button class="sel-btn" onclick="switchSection('nutri','race24h',this)">Course 24h</button>
    <button class="sel-btn" onclick="switchSection('nutri','recovery',this)">Récupération</button>
    <button class="sel-btn" onclick="switchSection('nutri','travel',this)">Voyage</button>
  </div>
  <div id="nutri-training">
    <div class="alert gold"><div class="alert-title">⚡ Semaine d'entraînement — Objectifs</div>2 800–3 200 kcal/j selon intensité · Ratio : 55% glucides / 20% protéines / 25% lipides · 100% sans gluten</div>
    <div class="grid-2">
      <div>
        <div class="card-title" style="font-family:'Barlow Condensed';font-weight:700;font-size:.82rem;letter-spacing:2px;text-transform:uppercase;margin-bottom:.8rem;">🌅 Journée type — 100% GF</div>
        <div class="meal-card"><div class="meal-time">07:00</div><div class="meal-content"><div class="meal-name">Petit-déjeuner performance</div><div class="meal-desc">Porridge de flocons de riz ou quinoa + fruits rouges · 2–3 œufs brouillés · Avocat · Pain GF grillé</div><div class="gf-chip mt1">✓ GF</div></div><div class="meal-macros"><div class="macro-kcal">650</div><div>kcal</div></div></div>
        <div class="meal-card"><div class="meal-time">10:00</div><div class="meal-content"><div class="meal-name">Snack pré-séance</div><div class="meal-desc">Banane + shake protéiné GF (whey sans gluten ou protéine de riz) · 30g noix ou amandes</div></div><div class="meal-macros"><div class="macro-kcal">320</div><div>kcal</div></div></div>
        <div class="meal-card"><div class="meal-time">13:00</div><div class="meal-content"><div class="meal-name">Déjeuner carb-focus</div><div class="meal-desc">Riz basmati 200g + saumon ou poulet 150g + légumes vapeur + huile d'olive · Sauce tamari (≠ soja classique)</div></div><div class="meal-macros"><div class="macro-kcal">720</div><div>kcal</div></div></div>
        <div class="meal-card"><div class="meal-time">16:00</div><div class="meal-content"><div class="meal-name">Récupération post-effort</div><div class="meal-desc">Yaourt sans lactose + granola GF + miel · 1 comprimé électrolytes dans 500ml eau</div></div><div class="meal-macros"><div class="macro-kcal">350</div><div>kcal</div></div></div>
        <div class="meal-card"><div class="meal-time">19:30</div><div class="meal-content"><div class="meal-name">Dîner protéines & légumes</div><div class="meal-desc">Bœuf ou thon + patate douce + brocolis + quinoa · Tisane récup (camomille, gingembre)</div></div><div class="meal-macros"><div class="macro-kcal">610</div><div>kcal</div></div></div>
      </div>
      <div>
        <div class="card"><div class="card-accent green"></div><div class="card-title">✅ Bases GF — Sources glucides</div><div style="font-size:.82rem;line-height:2;color:var(--text);">✓ Riz blanc / basmati / complet<br>✓ Quinoa, amarante, sarrasin<br>✓ Pomme de terre, patate douce<br>✓ Maïs, polenta<br>✓ Pain, pâtes & céréales certifiés GF<br>✓ Flocons de riz ou millet<br>✓ Légumineuses (lentilles, pois chiches)</div><hr class="divider"><div class="card-title" style="color:var(--red);">❌ À bannir (gluten caché)</div><div style="font-size:.78rem;line-height:1.9;color:var(--muted);">✗ Sauce soja classique → remplacer par tamari GF<br>✗ Sauces, vinaigrettes industrielles<br>✗ Charcuterie avec additifs<br>✗ Barres énergétiques non certifiées GF<br>✗ Médicaments / suppléments avec amidon de blé<br>✗ Bière (→ cidre ou vin)</div></div>
        <div class="card mt1"><div class="card-accent red"></div><div class="card-title">⚠️ Vigilance en déplacement</div><div style="font-size:.8rem;color:var(--muted);line-height:1.7;">Au Japon : soja = partout → toujours demander tamari/GF<br>USA : "gluten-free" bien indiqué en restaurant<br>Europe : mention allergène obligatoire<br>Asie : contamination croisée fréquente dans les cuisines<br><strong style="color:var(--gold);">Avoir toujours des barres GF certifiées en bagage</strong></div></div>
      </div>
    </div>
  </div>
  <div id="nutri-prerace" style="display:none;">
    <div class="alert red"><div class="alert-title">🏁 J-3 : Carb Loading SANS gluten</div>Augmenter les glucides à 70% de l'apport. Privilégier riz blanc, pomme de terre, quinoa. Dès J-2 : réduire fibres pour éviter inconforts GI en cockpit.</div>
    <div class="grid-2">
      <div>
        <div class="meal-card"><div class="meal-time">J-3</div><div class="meal-content"><div class="meal-name">Carb Loading — Démarrage GF</div><div class="meal-desc">Pâtes GF, riz blanc, pommes de terre · Maintenir protéines · Réduire légumes crucifères doucement</div></div></div>
        <div class="meal-card"><div class="meal-time">J-2</div><div class="meal-content"><div class="meal-name">Carb Loading intensifié</div><div class="meal-desc">Riz blanc exclusif, pommes de terre vapeur, pain GF blanc · Zéro légumineuses · Pas de lactose en excès</div></div></div>
        <div class="meal-card"><div class="meal-time">J-1 soir</div><div class="meal-content"><div class="meal-name">Dîner de confirmation (≤19h)</div><div class="meal-desc">Riz blanc + poulet vapeur + huile d'olive · Pas d'aliment nouveau · Coucher tôt ++</div></div></div>
        <div class="meal-card"><div class="meal-time">J — H-3</div><div class="meal-content"><div class="meal-name">Repas pré-course</div><div class="meal-desc">Riz blanc 200g + 2 œufs + banane + pain GF grillé · 750ml eau + électrolytes · Aucun gras ni fibres</div></div></div>
        <div class="meal-card"><div class="meal-time">J — H-1</div><div class="meal-content"><div class="meal-name">Dernier ravitaillement</div><div class="meal-desc">1 gel GF certifié ou barre de riz maison · 300ml eau · Dernier café si habitude</div></div></div>
      </div>
      <div>
        <div class="card"><div class="card-accent gold"></div><div class="card-title">🧂 Protocole hydratation J-1</div><div class="meal-desc mb2">Sodium-loading : augmenter sel de +1–2g pour retenir les fluides. Peser avant course pour calibrer les pertes sudorales.</div><div class="alert green"><div class="alert-title">✓ Boisson électrolytique maison GF</div>500ml eau · 1g sel rose · 1 pincée bicarbonate · 200ml jus d'orange pur · 1 càs miel. Boire le matin de course.</div><div class="alert gold mt1"><div class="alert-title">⚡ Gel GF recommandés</div>Maurten Gel 100 (GF certifié) · SiS Beta Fuel · Spring Energy (vérifier l'étiquette) · Barres de riz maison avec sirop d'érable</div></div>
      </div>
    </div>
  </div>
  <div id="nutri-race3h" style="display:none;">
    <div class="alert blue"><div class="alert-title">⏱ Course 3–6h — Protocole cockpit</div>60–90g glucides/heure · 500–800ml liquide/heure selon chaleur (40–65°C en cockpit GT fermé). Tous les produits doivent être GF certifiés.</div>
    <div class="grid-2">
      <div>
        <div class="timeline">
          <div class="tl-item"><div class="tl-time">H-30 MIN</div><div class="tl-action">Gel GF + eau</div><div class="tl-detail">1 gel Maurten 100 ou SiS + 250ml eau · Dernière miction</div></div>
          <div class="tl-item"><div class="tl-time">T+45 MIN</div><div class="tl-action">Gel en cockpit</div><div class="tl-detail">Gel isotonique GF + 150ml via système d'hydratation intégré · +sel si chaleur extrême</div></div>
          <div class="tl-item"><div class="tl-time">PIT STOP 1</div><div class="tl-action">Ravitaillement complet</div><div class="tl-detail">Bouteille eau 500ml + électrolytes · Banane ou barre riz GF · 2 gélules de sel</div></div>
          <div class="tl-item"><div class="tl-time">T+2H</div><div class="tl-action">Gel caféiné si besoin</div><div class="tl-detail">Gel caféiné GF (75mg caféine) si fatigue ou relais nocturne approchant</div></div>
          <div class="tl-item"><div class="tl-time">PIT STOP 2+</div><div class="tl-action">Maintien & adaptation</div><div class="tl-detail">Si nausées : réduire concentration gels · Eau plate privilégiée · Pas de boisson gazeuse</div></div>
          <div class="tl-item"><div class="tl-time">H-30 ARRIVÉE</div><div class="tl-action">Dernier gel</div><div class="tl-detail">Gel caféiné si relais final serré · 200ml eau</div></div>
        </div>
      </div>
      <div>
        <div class="card"><div class="card-accent red"></div><div class="card-title">🌡️ Thermorégulation cockpit</div><div class="meal-desc mb1" style="line-height:1.7;">Cockpit GT fermé : <strong style="color:var(--red)">40–65°C</strong>. Transpiration jusqu'à 2L/heure. Une déshydratation de 2% dégrade les réflexes de <strong style="color:var(--gold)">20%</strong>.</div><div style="display:flex;flex-direction:column;gap:.5rem;"><div style="display:flex;justify-content:space-between;font-size:.8rem;border-bottom:1px solid var(--border);padding:.35rem 0;"><span>20–25°C cockpit</span><span style="color:var(--green)">500ml/h</span></div><div style="display:flex;justify-content:space-between;font-size:.8rem;border-bottom:1px solid var(--border);padding:.35rem 0;"><span>35–45°C cockpit</span><span style="color:var(--gold)">800ml/h</span></div><div style="display:flex;justify-content:space-between;font-size:.8rem;padding:.35rem 0;"><span>+50°C cockpit (été)</span><span style="color:var(--red)">1–1,2L/h</span></div></div></div>
        <div class="card mt1"><div class="card-accent green"></div><div class="card-title">✅ Produits GF validés course</div><div style="font-size:.8rem;line-height:1.9;color:var(--text);">✓ Maurten Gel 100 / 160 (GF officiel)<br>✓ SiS Beta Fuel Gel (certifié GF)<br>✓ Precision Hydration gels<br>✓ Barres riz + sirop d'érable (maison)<br>✓ Électrolytes en poudre (Precision, LMNT)<br>✓ Banane (nature — toujours GF)<br>✓ Dattes Medjool (énergie rapide GF)</div></div>
      </div>
    </div>
  </div>
  <div id="nutri-race24h" style="display:none;">
    <div class="alert red"><div class="alert-title">🌙 Course 24h — Gestion énergie multi-relais</div>Planning à synchroniser avec tes relais. Le creux circadien entre 3h et 5h du matin est critique.</div>
    <div class="grid-2">
      <div>
        <div class="timeline">
          <div class="tl-item"><div class="tl-time">H-3 DÉPART</div><div class="tl-action">Repas pré-course GF</div><div class="tl-detail">Riz blanc 200g + poulet vapeur 150g + 2 œufs durs · Banane · 750ml eau + électrolytes</div></div>
          <div class="tl-item"><div class="tl-time">H0–H6 (JOUR)</div><div class="tl-action">Phase glucidique haute</div><div class="tl-detail">60–90g glucides/h · Gels Maurten GF toutes les 45 min · Banane à chaque pit stop</div></div>
          <div class="tl-item"><div class="tl-time">H6 (Pit stop)</div><div class="tl-action">🍚 Repas solide #1</div><div class="tl-detail">Riz blanc + poulet effiloché · Bouillon de poulet chaud · 500ml électrolytes · Dattes × 4</div></div>
          <div class="tl-item"><div class="tl-time">H12 (Minuit)</div><div class="tl-action">🍜 Repas nocturne</div><div class="tl-detail">Soupe miso GF + riz · Pommes de terre vapeur + beurre · Café 100mg · Bouillon sodium +++</div></div>
          <div class="tl-item"><div class="tl-time">H15 (3h du mat)</div><div class="tl-action">🍌 Snack creux circadien</div><div class="tl-detail">Banane + gel caféiné GF 75mg · 2 dattes Medjool · Eau 400ml · Micro-sieste 20 min si possible</div></div>
          <div class="tl-item"><div class="tl-time">H18–H21 (CRITIQUE)</div><div class="tl-action">🔴 Creux circadien</div><div class="tl-detail">Boost caféine 100mg + gel sucre rapide · Chocolat noir GF 2 carrés · Électrolytes +++ · Lumière vive</div></div>
          <div class="tl-item"><div class="tl-time">H21–H24 (AUBE)</div><div class="tl-action">Phase finish</div><div class="tl-detail">Gel caféiné 30 min avant dernier relais · Eau 300ml + sodium · Focus total</div></div>
        </div>
      </div>
      <div>
        <div class="card mb1"><div class="card-accent gold"></div><div class="card-title">☕ Stratégie caféine 24h</div><div class="meal-card"><div class="meal-time">H-1</div><div class="meal-content"><div class="meal-name">Dose départ</div><div class="meal-desc">100mg (1 espresso). Si habitude seulement.</div></div></div><div class="meal-card"><div class="meal-time">H8 (~20h)</div><div class="meal-content"><div class="meal-name">Maintien soirée</div><div class="meal-desc">100mg gel caféiné GF.</div></div></div><div class="meal-card"><div class="meal-time">H16 (~00h)</div><div class="meal-content"><div class="meal-name">Boost nocturne</div><div class="meal-desc">150mg — gel caféiné GF + L-Théanine 100mg.</div></div></div><div class="meal-card"><div class="meal-time">H20 (~4h)</div><div class="meal-content"><div class="meal-name">Creux circadien</div><div class="meal-desc">100mg max. Post micro-sieste 20 min idéalement.</div></div></div><div class="alert red mt1"><div class="alert-title">⚠️ Limite 24h</div>400mg caféine max.</div></div>
        <div class="card"><div class="card-accent blue"></div><div class="card-title">🥡 Box repas avant course</div><div style="font-size:.82rem;line-height:2;color:var(--text);"><strong style="color:var(--gold);">Box 1 (H6) :</strong> Riz + poulet + dattes + électrolytes<br><strong style="color:var(--gold);">Box 2 (H12) :</strong> Soupe miso GF + pomme de terre + café<br><strong style="color:var(--gold);">Box 3 (H15) :</strong> Banane + 2 gels caféinés + bouillon<br><strong style="color:var(--gold);">Box 4 (H21) :</strong> Œufs + pain GF + espresso<br><strong style="color:var(--muted);">+ Gels GF × 12 en permanence dans le cockpit</strong></div></div>
      </div>
    </div>
  </div>
  <div id="nutri-recovery" style="display:none;">
    <div class="alert green"><div class="alert-title">✓ Récupération post-course</div>Fenêtre anabolique : 30–45 min après l'arrivée = critique. Récupération totale : 48–72h selon la durée.</div>
    <div class="grid-2">
      <div>
        <div class="meal-card"><div class="meal-time">0–30 min</div><div class="meal-content"><div class="meal-name">🥤 Shake récupération immédiate GF</div><div class="meal-desc">30g whey GF ou protéine de riz · 1 banane · 200ml lait de coco · 1 càs miel · 300ml eau · 1 sachet électrolytes · 1g sel rose</div></div><div class="meal-macros"><div class="macro-kcal">420</div><div>kcal</div></div></div>
        <div class="meal-card"><div class="meal-time">1–2h</div><div class="meal-content"><div class="meal-name">🍣 Repas récupération anti-inflammatoire</div><div class="meal-desc">Saumon sauvage 180g + riz basmati 150g + brocolis vapeur + huile d'olive · 250ml jus de cerise Montmorency</div></div><div class="meal-macros"><div class="macro-kcal">680</div><div>kcal</div></div></div>
        <div class="meal-card"><div class="meal-time">Soir J+0</div><div class="meal-content"><div class="meal-name">🥘 Dîner anti-inflammatoire</div><div class="meal-desc">Soupe GF (bouillon poulet maison + légumes) · Patate douce rôtie + beurre de noix · 150g poulet · Curcuma + poivre noir + gingembre frais</div></div><div class="meal-macros"><div class="macro-kcal">590</div><div>kcal</div></div></div>
        <div class="meal-card"><div class="meal-time">J+1 matin</div><div class="meal-content"><div class="meal-name">🍳 Petit-déjeuner réparation musculaire</div><div class="meal-desc">3 œufs brouillés + 1 jaune extra · Porridge quinoa + fruits rouges · 250ml jus grenade · Oméga-3 3g · Curcumine 1g</div></div><div class="meal-macros"><div class="macro-kcal">520</div><div>kcal</div></div></div>
      </div>
      <div>
        <div class="card mb1"><div class="card-accent green"></div><div class="card-title">🩺 Biomarqueurs à surveiller</div><div style="display:flex;flex-direction:column;gap:.3rem;font-size:.82rem;"><div style="display:flex;justify-content:space-between;border-bottom:1px solid var(--border);padding:.4rem 0;"><span>HRV matin</span><span style="color:var(--green)">Doit remonter J+2</span></div><div style="display:flex;justify-content:space-between;border-bottom:1px solid var(--border);padding:.4rem 0;"><span>FC repos</span><span style="color:var(--green)">Retour baseline 48h</span></div><div style="display:flex;justify-content:space-between;border-bottom:1px solid var(--border);padding:.4rem 0;"><span>Poids matin</span><span style="color:var(--gold)">Delta ≤ 2kg vs avant</span></div><div style="display:flex;justify-content:space-between;padding:.4rem 0;"><span>Couleur urines</span><span style="color:var(--blue)">Jaune pâle = OK</span></div></div></div>
        <div class="card"><div class="card-accent red"></div><div class="card-title">⚡ Aliments star récupération GF</div><div style="font-size:.82rem;line-height:2;color:var(--text);">🍒 <strong style="color:var(--red);">Cerise Montmorency</strong> — anti-inflammatoire #1<br>🫐 <strong style="color:var(--blue);">Myrtilles</strong> — antioxydants, réduction DOMS<br>🐟 <strong style="color:var(--gold);">Saumon sauvage</strong> — oméga-3, protéine complète<br>🥑 <strong style="color:var(--green);">Avocat</strong> — potassium, graisses saines<br>🍉 <strong style="color:var(--red);">Pastèque</strong> — L-citrulline naturelle</div></div>
      </div>
    </div>
  </div>
  <div id="nutri-travel" style="display:none;">
    <div class="alert gold"><div class="alert-title">✈️ Nutrition en déplacement international</div>GF en avion = risque de contamination élevé. Prépare toujours des collations GF certifiées dans ton bagage cabine.</div>
    <div class="grid-2">
      <div>
        <div class="meal-card"><div class="meal-time">AVANT VOL</div><div class="meal-content"><div class="meal-name">🍚 Repas préparé maison</div><div class="meal-desc">Riz basmati + poulet grillé froid + salade verte · Tupperware hermétique · Solide = OK en sécurité</div></div></div>
        <div class="meal-card"><div class="meal-time">EN VOL</div><div class="meal-content"><div class="meal-name">🥜 Pack snacks GF avion</div><div class="meal-desc">Noix 60g · Beurre d'amande (Justin's GF) · Galettes de riz × 6 · Barres Nakd ou Larabar · Jerky bœuf GF · Dattes × 8 · Chocolat noir 85% GF</div></div></div>
        <div class="meal-card"><div class="meal-time">ARRIVÉE</div><div class="meal-content"><div class="meal-name">🍳 Premier repas — heure locale</div><div class="meal-desc">Riz blanc + protéine simple selon heure locale · Éviter alcool 24h · Électrolytes obligatoires</div></div></div>
        <div class="alert blue mt1"><div class="alert-title">💧 Hydratation en vol</div>Objectif : 300ml eau / heure de vol. Électrolytes toutes les 2h. Alcool = interdit.</div>
      </div>
      <div>
        <div class="card mb1"><div class="card-accent gold"></div><div class="card-title">🌍 Options GF par destination</div>
          <div class="meal-card" style="margin-bottom:.5rem;"><div class="meal-content"><div class="meal-name">🇯🇵 Japon</div><div class="meal-desc">Onigiri nature · Sashimi sans soja · Tamago · "Komugi nashi" = sans blé</div></div></div>
          <div class="meal-card" style="margin-bottom:.5rem;"><div class="meal-content"><div class="meal-name">🇺🇸 USA</div><div class="meal-desc">Chipotle (bol) · Sweetgreen · Whole Foods · Steak + patate au four</div></div></div>
          <div class="meal-card" style="margin-bottom:.5rem;"><div class="meal-content"><div class="meal-name">🇩🇪 Nürburgring</div><div class="meal-desc">Kartoffeln · Fleisch ohne Soße · Demander fiche allergènes (obligatoire UE)</div></div></div>
          <div class="meal-card" style="margin-bottom:.5rem;"><div class="meal-content"><div class="meal-name">🇦🇪 Bahrain / Dubai</div><div class="meal-desc">Riz basmati + grillades · Hummus maison · Hydratation × 2 (chaleur)</div></div></div>
          <div class="meal-card"><div class="meal-content"><div class="meal-name">🇦🇺 Australie</div><div class="meal-desc">Conscience GF très élevée · Cafés avec menu GF · Açaï bowls GF courants</div></div></div>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- ===== SUPPLÉMENTS ===== -->

<div class="page" id="page-supplements">
  <div class="section-title">Suppléments <span class="tag tag-red">GF CERTIFIÉS</span></div>
  <div class="alert red"><div class="alert-title">⚠️ Vigilance gluten dans les suppléments</div>Beaucoup de suppléments contiennent de l'amidon de blé comme excipient. Toujours vérifier le label "gluten-free" ou "certified GF".</div>
  <div class="alert purple" id="supp-phase-alert" style="margin-bottom:1rem;"></div>
  <div class="selector">
    <button class="sel-btn active" onclick="switchSection('supp','base',this)">Stack de base</button>
    <button class="sel-btn" onclick="switchSection('supp','training_supp',this)">À l'entraînement</button>
    <button class="sel-btn" onclick="switchSection('supp','race_supp',this)">En course</button>
    <button class="sel-btn" onclick="switchSection('supp','recovery_supp',this)">Récupération</button>
    <button class="sel-btn" onclick="switchSection('supp','jetlag_supp',this)">Jet Lag</button>
  </div>
  <div id="supp-base">
    <div class="grid-2">
      <div>
        <div class="card-title" style="font-family:'Barlow Condensed';font-weight:700;font-size:.82rem;letter-spacing:2px;text-transform:uppercase;margin-bottom:.8rem;">🌅 Matin (avec petit-déjeuner)</div>
        <div class="supp-card"><div class="supp-dot" style="background:var(--gold)"></div><div class="supp-info"><div class="supp-name">Oméga-3 (EPA + DHA)</div><div class="supp-dose">2–3g/jour · Certifié GF (ex: Thorne, Nordic Naturals)</div><div class="supp-why">Anti-inflammatoire, récupération musculaire, fonction cognitive — essentiel pour la concentration en course.</div></div></div>
        <div class="supp-card"><div class="supp-dot" style="background:var(--gold)"></div><div class="supp-info"><div class="supp-name">Vitamine D3 + K2</div><div class="supp-dose">2 000–4 000 UI/j D3 · 100mcg K2 · GF vérifier</div><div class="supp-why">Immunité, récupération musculaire, santé osseuse. Les pilotes voyagent beaucoup — carence très courante.</div></div></div>
        <div class="supp-card"><div class="supp-dot" style="background:var(--green)"></div><div class="supp-info"><div class="supp-name">Magnésium Bisglycinate</div><div class="supp-dose">300–400mg/j · Forme bisglycinate (meilleure absorption) · GF</div><div class="supp-why">Réduction crampes musculaires, gestion du stress, qualité du sommeil.</div></div></div>
        <div class="supp-card"><div class="supp-dot" style="background:var(--blue)"></div><div class="supp-info"><div class="supp-name">Vitamine C</div><div class="supp-dose">500–1 000mg/j · Buffered C ou liposomale · GF</div><div class="supp-why">Immunité lors des voyages (avion = vecteur d'infection). Antioxydant.</div></div></div>
        <div class="supp-card"><div class="supp-dot" style="background:var(--purple)"></div><div class="supp-info"><div class="supp-name">Zinc + Sélénium</div><div class="supp-dose">15–25mg Zinc · 100mcg Sélénium · GF certifié</div><div class="supp-why">Immunité, testostérone, fonction thyroïdienne. Éviter à jeun.</div></div></div>
      </div>
      <div>
        <div class="card-title" style="font-family:'Barlow Condensed';font-weight:700;font-size:.82rem;letter-spacing:2px;text-transform:uppercase;margin-bottom:.8rem;">🌙 Soir (après dîner)</div>
        <div class="supp-card"><div class="supp-dot" style="background:var(--green)"></div><div class="supp-info"><div class="supp-name">Magnésium Glycinate (soir)</div><div class="supp-dose">200–300mg · 1h avant le sommeil</div><div class="supp-why">Relaxation musculaire, amélioration profondeur du sommeil. Le sommeil est LE facteur #1 de performance pilote.</div></div></div>
        <div class="supp-card"><div class="supp-dot" style="background:var(--purple)"></div><div class="supp-info"><div class="supp-name">L-Théanine</div><div class="supp-dose">200mg soir · Ou 100mg avec caféine le matin</div><div class="supp-why">Relaxation sans somnolence. Combinée à la caféine : focus net sans anxiété.</div></div></div>
        <div class="supp-card"><div class="supp-dot" style="background:var(--blue)"></div><div class="supp-info"><div class="supp-name">Probiotiques</div><div class="supp-dose">10–30 milliards UFC · Souches Lactobacillus + Bifidobacterium · GF</div><div class="supp-why">Essentiel pour les voyageurs internationaux. Protège contre les infections GI.</div></div></div>
        <div class="supp-card"><div class="supp-dot" style="background:var(--gold)"></div><div class="supp-info"><div class="supp-name">Curcumine + Pipérine</div><div class="supp-dose">500–1 000mg curcumine · 5mg pipérine (absorption ×20) · GF</div><div class="supp-why">Puissant anti-inflammatoire naturel. Réduit les douleurs musculaires post-course.</div></div></div>
        <div class="alert green mt1"><div class="alert-title">✓ Marques GF recommandées</div>Thorne Research · Pure Encapsulations · Garden of Life · NOW Sports (certifié GF) · Klean Athlete.</div>
      </div>
    </div>
  </div>
  <div id="supp-training_supp" style="display:none;">
    <div class="alert blue"><div class="alert-title">💪 Suppléments spécifiques entraînement</div>Ces suppléments maximisent la performance à l'entraînement et la récupération. Vérifier certification GF sur chaque produit.</div>
    <div class="grid-2">
      <div>
        <div class="card-title" style="font-family:'Barlow Condensed';font-weight:700;font-size:.82rem;letter-spacing:2px;text-transform:uppercase;margin-bottom:.8rem;">⚡ Pré-entraînement (30–60 min avant)</div>
        <div class="supp-card"><div class="supp-dot" style="background:var(--red)"></div><div class="supp-info"><div class="supp-name">Créatine Monohydrate</div><div class="supp-dose">5g/j en continu · Pas de cycle nécessaire · GF</div><div class="supp-why">Force, puissance explosive, récupération musculaire.</div></div></div>
        <div class="supp-card"><div class="supp-dot" style="background:var(--gold)"></div><div class="supp-info"><div class="supp-name">Caféine + L-Théanine</div><div class="supp-dose">100–150mg caféine + 100–200mg L-Théanine · GF</div><div class="supp-why">Focus net, énergie sans pics ni crash. Idéal avant simulateur ou séance technique.</div></div></div>
        <div class="supp-card"><div class="supp-dot" style="background:var(--green)"></div><div class="supp-info"><div class="supp-name">Électrolytes pré-séance</div><div class="supp-dose">1 comprimé/sachet GF dans 500ml eau</div><div class="supp-why">Prévenir crampes. Indispensable si séance +60 min ou forte chaleur.</div></div></div>
      </div>
      <div>
        <div class="card-title" style="font-family:'Barlow Condensed';font-weight:700;font-size:.82rem;letter-spacing:2px;text-transform:uppercase;margin-bottom:.8rem;">🔄 Post-entraînement (dans les 45 min)</div>
        <div class="supp-card"><div class="supp-dot" style="background:var(--blue)"></div><div class="supp-info"><div class="supp-name">Whey protéine GF ou Protéine de riz</div><div class="supp-dose">25–35g protéines · Whey native GF ou protéine végétale GF</div><div class="supp-why">Synthèse protéique musculaire. Fenêtre anabolique 30–45 min post-effort.</div></div></div>
        <div class="supp-card"><div class="supp-dot" style="background:var(--green)"></div><div class="supp-info"><div class="supp-name">Glutamine</div><div class="supp-dose">5–10g post-effort · GF certifié</div><div class="supp-why">Récupération intestinale. Particulièrement utile après les courses longues.</div></div></div>
        <div class="supp-card"><div class="supp-dot" style="background:var(--red)"></div><div class="supp-info"><div class="supp-name">Jus de cerise Montmorency</div><div class="supp-dose">30ml concentré dans 250ml eau · Post-effort et soir · Naturellement GF</div><div class="supp-why">Réduit les courbatures de 30–40%. Anti-inflammatoire naturel. Validé scientifiquement.</div></div></div>
      </div>
    </div>
  </div>
  <div id="supp-race_supp" style="display:none;">
    <div class="alert red"><div class="alert-title">🏁 Suppléments pendant la course — GF uniquement</div>JAMAIS de nouveau produit le jour J. Cockpit : format gel ou comprimé uniquement.</div>
    <div class="grid-2">
      <div>
        <div class="supp-card"><div class="supp-dot" style="background:var(--gold)"></div><div class="supp-info"><div class="supp-name">Gels glucidiques GF</div><div class="supp-dose">1 gel toutes les 45–60 min · 25–40g glucides/gel · Maurten, SiS, Precision</div><div class="supp-why">Source d'énergie principale en cockpit. Maurten 100 utilise un hydrogel qui réduit les problèmes GI.</div></div></div>
        <div class="supp-card"><div class="supp-dot" style="background:var(--blue)"></div><div class="supp-info"><div class="supp-name">Électrolytes (comprimés ou poudre)</div><div class="supp-dose">1 comprimé/heure par 35°C+ · LMNT, Precision Hydration · GF certifié</div><div class="supp-why">Cockpit GT : pertes sudorales 1–2L/h. Prévenir crampes et hyponatrémie.</div></div></div>
        <div class="supp-card"><div class="supp-dot" style="background:var(--red)"></div><div class="supp-info"><div class="supp-name">Gélules de sel (SaltStick)</div><div class="supp-dose">1–2 gélules/heure si transpiration intense · GF certifié</div><div class="supp-why">Essentiel en été (Le Mans, Fuji, Spa). Prévient les crampes en milieu de course.</div></div></div>
        <div class="supp-card"><div class="supp-dot" style="background:var(--orange)"></div><div class="supp-info"><div class="supp-name">Caféine — gel ou comprimé GF</div><div class="supp-dose">75–100mg / prise · Max 3–4 prises/24h · Planifier stratégiquement</div><div class="supp-why">En 24h : planifier aux creux de vigilance prévisibles (nuit, 4h du matin).</div></div></div>
      </div>
      <div>
        <div class="card"><div class="card-accent gold"></div><div class="card-title">📋 Kit suppléments course (pré-emballé)</div><div style="font-size:.82rem;line-height:2;color:var(--text);">✓ 8–10 gels Maurten 100 (ou SiS Beta Fuel GF)<br>✓ 2 gels caféinés GF (75mg caféine)<br>✓ 1 tube SaltStick Fastchews GF<br>✓ Precision Hydration 1000 × 4–6 sachets<br>✓ 4–6 bananes (pit stops)<br>✓ Barres de riz maison GF × 3<br>✓ Bouillon de poulet thermos (courses nocturnes)<br>✓ Eau plate × format cockpit</div><div class="alert red mt1"><div class="alert-title">⚠️ Règle absolue</div>Aucun produit nouveau le jour de la course.</div></div>
      </div>
    </div>
  </div>
  <div id="supp-recovery_supp" style="display:none;">
    <div class="alert green"><div class="alert-title">✓ Suppléments récupération post-course</div>Après une course 3–24h, le corps est en état de stress oxydatif majeur.</div>
    <div class="grid-auto">
      <div class="card"><div class="card-accent green"></div><div class="card-title">0–30 min post-course</div><div class="supp-card"><div class="supp-dot" style="background:var(--green)"></div><div class="supp-info"><div class="supp-name">Whey GF ou Protéine de riz</div><div class="supp-dose">30g immédiatement</div><div class="supp-why">Relancer la synthèse protéique avec glucides rapides.</div></div></div><div class="supp-card"><div class="supp-dot" style="background:var(--blue)"></div><div class="supp-info"><div class="supp-name">Électrolytes complets</div><div class="supp-dose">1–2 sachets dans 1L eau</div><div class="supp-why">Rééquilibrer sodium, potassium, magnésium.</div></div></div><div class="supp-card"><div class="supp-dot" style="background:var(--red)"></div><div class="supp-info"><div class="supp-name">Jus cerise Montmorency</div><div class="supp-dose">60ml concentré dans eau</div><div class="supp-why">Anti-inflammatoire puissant + mélatonine naturelle.</div></div></div></div>
      <div class="card"><div class="card-accent blue"></div><div class="card-title">Soir J+0</div><div class="supp-card"><div class="supp-dot" style="background:var(--gold)"></div><div class="supp-info"><div class="supp-name">Oméga-3 dose haute</div><div class="supp-dose">3g EPA+DHA</div><div class="supp-why">Dose anti-inflammatoire maximale. Réduit CRP, IL-6.</div></div></div><div class="supp-card"><div class="supp-dot" style="background:var(--green)"></div><div class="supp-info"><div class="supp-name">Magnésium + L-Théanine</div><div class="supp-dose">400mg Mg + 200mg L-Théanine</div><div class="supp-why">Favoriser le sommeil récupérateur post-course de nuit.</div></div></div></div>
      <div class="card"><div class="card-accent red"></div><div class="card-title">J+1 et J+2</div><div class="supp-card"><div class="supp-dot" style="background:var(--green)"></div><div class="supp-info"><div class="supp-name">Glutamine</div><div class="supp-dose">10g matin + 10g soir</div><div class="supp-why">Récupération intestinale et musculaire accélérée.</div></div></div><div class="supp-card"><div class="supp-dot" style="background:var(--purple)"></div><div class="supp-info"><div class="supp-name">Probiotiques renforcés</div><div class="supp-dose">Double dose 2–3 jours</div><div class="supp-why">Rétablir le microbiote perturbé par l'effort et les voyages.</div></div></div></div>
    </div>
  </div>
  <div id="supp-jetlag_supp" style="display:none;">
    <div class="alert gold"><div class="alert-title">✈️ Suppléments — Protocole Jet Lag</div>Un protocole structuré réduit l'adaptation de 50%.</div>
    <div class="grid-2">
      <div>
        <div class="supp-card"><div class="supp-dot" style="background:var(--purple)"></div><div class="supp-info"><div class="supp-name">Mélatonine (faible dose)</div><div class="supp-dose">0,5mg à 1mg · 30 min avant coucher HEURE LOCALE · GF</div><div class="supp-why">Synchronise l'horloge biologique. Utiliser 2–4 jours après arrivée, pas en continu.</div><div class="supp-warning">⚠️ Ne pas prendre le matin. Éviter si décalage &lt; 3h.</div></div></div>
        <div class="supp-card"><div class="supp-dot" style="background:var(--gold)"></div><div class="supp-info"><div class="supp-name">Magnésium + L-Théanine (soir)</div><div class="supp-dose">400mg Magnésium + 200mg L-Théanine · 1h avant coucher local</div><div class="supp-why">Améliore la qualité du sommeil dans un nouveau fuseau.</div></div></div>
        <div class="supp-card"><div class="supp-dot" style="background:var(--red)"></div><div class="supp-info"><div class="supp-name">Ashwagandha KSM-66</div><div class="supp-dose">300–600mg/j · Matin ou soir · GF certifié</div><div class="supp-why">Adaptogène — régule le cortisol perturbé par les voyages. À utiliser en cure lors des grands déplacements.</div></div></div>
        <div class="supp-card"><div class="supp-dot" style="background:var(--blue)"></div><div class="supp-info"><div class="supp-name">Caféine + L-Théanine (matin)</div><div class="supp-dose">100mg + 100mg · Matin heure locale uniquement</div><div class="supp-why">Rester éveillé et alerte selon l'heure locale J+1 et J+2.</div></div></div>
      </div>
      <div>
        <div class="card"><div class="card-accent gold"></div><div class="card-title">📋 Protocole par décalage</div>
          <div class="toggle-section open"><div class="toggle-header" onclick="toggleSection(this)">Voyage EST (+4h à +9h) — Ex: Japon, Asie<span class="toggle-arrow">▼</span></div><div class="toggle-body"><div style="font-size:.82rem;line-height:1.9;color:var(--text);"><strong style="color:var(--gold);">Avant le vol :</strong> exposer au soleil le matin. Éviter caféine après 15h.<br><strong style="color:var(--gold);">Arrivée :</strong> Mélatonine 0,5mg à 22h locale dès J+1.<br><strong style="color:var(--gold);">J+1 à J+3 :</strong> Mg + L-Théanine soir · Soleil matin obligatoire · Ashwagandha</div></div></div>
          <div class="toggle-section"><div class="toggle-header" onclick="toggleSection(this)">Voyage OUEST (-4h à -8h) — Ex: USA<span class="toggle-arrow">▼</span></div><div class="toggle-body"><div style="font-size:.82rem;line-height:1.9;color:var(--text);"><strong style="color:var(--gold);">Avant le vol :</strong> rester éveillé le plus tard possible.<br><strong style="color:var(--gold);">Arrivée :</strong> ne pas dormir avant 22h locale. Caféine matinale.<br><strong style="color:var(--gold);">J+1–3 :</strong> Mg soir · Rythme alimentaire heure locale strict</div></div></div>
          <div class="toggle-section"><div class="toggle-header" onclick="toggleSection(this)">Voyage >12h — Ex: Australie<span class="toggle-arrow">▼</span></div><div class="toggle-body"><div style="font-size:.82rem;line-height:1.9;color:var(--text);"><strong style="color:var(--red);">Arriver 7 jours avant si budget.</strong><br>Mélatonine + Ashwagandha + Mg combinés.<br>"Grounding" + exposition solaire matinale = accélérateur prouvé.</div></div></div>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- ===== TRAINING ===== -->

<div class="page" id="page-training">
  <div class="section-title">Programme Entraînement</div>
  <div class="week-days" id="weekDays"></div>
  <div class="alert gold" id="training-phase-alert" style="margin-bottom:1rem;"></div>
  <div class="selector">
    <button class="sel-btn active" onclick="switchSection('train','semaine',this)">Semaine type</button>
    <button class="sel-btn" onclick="switchSection('train','nuque',this)">Nuque & G-Force</button>
    <button class="sel-btn" onclick="switchSection('train','core',this)">Core & Stabilité</button>
    <button class="sel-btn" onclick="switchSection('train','cardio',this)">Cardio & Endurance</button>
    <button class="sel-btn" onclick="switchSection('train','prerace_fit',this)">Pré-Course</button>
    <button class="sel-btn" onclick="switchSection('train','hotel',this)">Sans salle (voyage)</button>
  </div>
  <div id="train-semaine">
    <div class="alert blue"><div class="alert-title">📅 Structure semaine type (hors déplacement)</div>4–5 séances/sem. Volume réduit J-4 avant course. Objectif : endurance cardiovasculaire, force nuque/épaules, core, résistance mentale.</div>
    <div class="grid-3">
      <div class="card"><div class="card-accent blue"></div><div class="card-title">Lundi — Cardio Endurance</div><div class="exercise-item"><div class="ex-num">01</div><div class="ex-info"><div class="ex-name">Course à pied Zone 2</div><div class="ex-detail">45–60 min · FC 130–145 bpm · Conversation possible</div></div><div class="ex-badge tag tag-green">ZONE 2</div></div><div class="exercise-item"><div class="ex-num">02</div><div class="ex-info"><div class="ex-name">Vélo stationnaire</div><div class="ex-detail">30 min si météo mauvaise · Même FC cible</div></div></div><div class="exercise-item"><div class="ex-num">03</div><div class="ex-info"><div class="ex-name">Étirements dynamiques</div><div class="ex-detail">10 min fin de séance · Ischio, mollets, hanches</div></div></div></div>
      <div class="card"><div class="card-accent red"></div><div class="card-title">Mardi — Force Nuque + Upper</div><div class="exercise-item"><div class="ex-num">01</div><div class="ex-info"><div class="ex-name">Extension nuque harnais</div><div class="ex-detail">4×15 · Avant/arrière/latéral · Progression charge</div></div><div class="ex-badge tag tag-red">G-FORCE</div></div><div class="exercise-item"><div class="ex-num">02</div><div class="ex-info"><div class="ex-name">Tirage nuque caoutchouc</div><div class="ex-detail">3×20 · Bande élastique · Rotation cervicale</div></div></div><div class="exercise-item"><div class="ex-num">03</div><div class="ex-info"><div class="ex-name">Shoulder Press</div><div class="ex-detail">4×10 · Haltères ou barbell · Stabilité scapulaire</div></div></div><div class="exercise-item"><div class="ex-num">04</div><div class="ex-info"><div class="ex-name">Shrugs + Face Pull</div><div class="ex-detail">3×15 chaque · Trapèzes + deltoïdes postérieurs</div></div></div><div class="exercise-item"><div class="ex-num">05</div><div class="ex-info"><div class="ex-name">Grip Training</div><div class="ex-detail">3 séries max · Gripper + pronation/supination avant-bras</div></div></div></div>
      <div class="card"><div class="card-accent green"></div><div class="card-title">Mercredi — Core & Mobilité</div><div class="exercise-item"><div class="ex-num">01</div><div class="ex-info"><div class="ex-name">Planche & variantes</div><div class="ex-detail">4×45 sec · Planche frontale, latérale, dynamique</div></div><div class="ex-badge tag tag-green">CORE</div></div><div class="exercise-item"><div class="ex-num">02</div><div class="ex-info"><div class="ex-name">Anti-rotation (Pallof Press)</div><div class="ex-detail">3×12 chaque côté · Câble ou bande</div></div></div><div class="exercise-item"><div class="ex-num">03</div><div class="ex-info"><div class="ex-name">Dead Bug</div><div class="ex-detail">3×10 · Contrôle respiratoire</div></div></div><div class="exercise-item"><div class="ex-num">04</div><div class="ex-info"><div class="ex-name">Hip Flexor & Piriforme</div><div class="ex-detail">Position assise prolongée en cockpit → priorité</div></div></div></div>
      <div class="card"><div class="card-accent gold"></div><div class="card-title">Jeudi — HIIT + Réactivité</div><div class="exercise-item"><div class="ex-num">01</div><div class="ex-info"><div class="ex-name">HIIT Vélo / Rameur</div><div class="ex-detail">8×20 sec sprint / 40 sec récup · 3 séries · FC max</div></div><div class="ex-badge tag tag-red">HIIT</div></div><div class="exercise-item"><div class="ex-num">02</div><div class="ex-info"><div class="ex-name">Exercices réactivité</div><div class="ex-detail">Tap rapide, ladder drill, réaction visuelle · 20 min</div></div></div><div class="exercise-item"><div class="ex-num">03</div><div class="ex-info"><div class="ex-name">Squats + Fentes bulgares</div><div class="ex-detail">4×12 · Force jambes pour freinage / accélérations</div></div></div></div>
      <div class="card"><div class="card-accent blue"></div><div class="card-title">Vendredi — Endurance + Nuque</div><div class="exercise-item"><div class="ex-num">01</div><div class="ex-info"><div class="ex-name">Natation / Vélo long</div><div class="ex-detail">60–90 min Zone 2 · Natation = récupération active idéale</div></div></div><div class="exercise-item"><div class="ex-num">02</div><div class="ex-info"><div class="ex-name">Nuque harnais léger</div><div class="ex-detail">Volume réduit · 3×12 · Maintien seulement</div></div></div><div class="exercise-item"><div class="ex-num">03</div><div class="ex-info"><div class="ex-name">Core léger</div><div class="ex-detail">Planche 3×30 sec + dead bug · Sans intensité max</div></div></div></div>
      <div class="card"><div class="card-accent green"></div><div class="card-title">Weekend — Récup Active</div><div class="exercise-item"><div class="ex-num">Sat</div><div class="ex-info"><div class="ex-name">Marche 45 min ou vélo léger</div><div class="ex-detail">FC &lt; 120 bpm · Récupération active · Air frais</div></div></div><div class="exercise-item"><div class="ex-num">Dim</div><div class="ex-info"><div class="ex-name">Repos complet ou yoga</div><div class="ex-detail">Mobilité douce · Méditation / sophrologie 15 min</div></div></div><div class="alert green mt1"><div class="alert-title">✓ Récupération weekend</div>Massage, bain chaud, cryothérapie si disponible. 8–9h de sommeil prioritaire.</div></div>
    </div>
  </div>
  <div id="train-nuque" style="display:none;">
    <div class="alert red"><div class="alert-title">⚠️ Nuque & Forces Latérales — Spécifique GT</div>En GT endurance, les forces latérales en virage atteignent 3–4G. C'est LE muscle le plus spécifique au pilotage.</div>
    <div class="grid-2">
      <div>
        <div class="exercise-item"><div class="ex-num">01</div><div class="ex-info"><div class="ex-name">Extension nuque avant — Harnais</div><div class="ex-detail">4×15 reps · Progression charge hebdomadaire · Menton vers poitrine</div></div><div class="ex-badge tag tag-red">PRIORITÉ</div></div>
        <div class="exercise-item"><div class="ex-num">02</div><div class="ex-info"><div class="ex-name">Extension nuque arrière — Harnais</div><div class="ex-detail">4×15 reps · Tête vers arrière · Contrôle total</div></div></div>
        <div class="exercise-item"><div class="ex-num">03</div><div class="ex-info"><div class="ex-name">Flexion latérale nuque</div><div class="ex-detail">4×12 chaque côté · Harnais ou main résistance · Simulation G latéraux</div></div></div>
        <div class="exercise-item"><div class="ex-num">04</div><div class="ex-info"><div class="ex-name">Isométrie nuque (head push)</div><div class="ex-detail">4 directions × 30 sec · Contre résistance main ou mur</div></div></div>
        <div class="exercise-item"><div class="ex-num">05</div><div class="ex-info"><div class="ex-name">Rotation cervicale lestée</div><div class="ex-detail">3×20 chaque sens · Harnais léger · Simulation virage</div></div></div>
        <div class="exercise-item"><div class="ex-num">06</div><div class="ex-info"><div class="ex-name">Shrugs haltères</div><div class="ex-detail">4×15 · Trapèzes supérieurs — soutien nuque</div></div></div>
        <div class="exercise-item"><div class="ex-num">07</div><div class="ex-info"><div class="ex-name">Farmer's Walk</div><div class="ex-detail">4×20m · Charge max tolérée · Stabilité sous charge globale</div></div></div>
      </div>
      <div>
        <div class="card"><div class="card-accent red"></div><div class="card-title">📐 Progression sur 8 semaines</div><div style="font-size:.82rem;line-height:2;color:var(--text);">Sem 1–2 : Apprentissage · Charge légère (2–3kg)<br>Sem 3–4 : +1kg · Volume ++<br>Sem 5–6 : Intensité haute · 5–6kg<br>Sem 7–8 : Simulation GT · Endurance nuque</div><hr class="divider"><div class="card-title">🎯 Objectif physique GT pilote</div><div style="font-size:.82rem;line-height:2;color:var(--muted);">Nuque : résister 4G latéraux × 2h+ sans fatigue<br>Bras : 200+ virages à force constante<br>Core : stabilisation colonne sous vibrations<br>Grip : maintien volant sur 6–24h<br>Cardio : FC stable 130–140 sous pression</div></div>
      </div>
    </div>
  </div>
  <div id="train-core" style="display:none;">
    <div class="alert blue"><div class="alert-title">💪 Core — Stabilité sous vibrations</div>En cockpit GT, la colonne est soumise à des vibrations constantes. Un core fort = protection dos, stabilité volant, endurance sur 24h.</div>
    <div class="grid-2">
      <div>
        <div class="exercise-item"><div class="ex-num">01</div><div class="ex-info"><div class="ex-name">Planche frontale progressive</div><div class="ex-detail">4×60 sec → 4×90 sec en progression</div></div><div class="ex-badge tag tag-blue">BASE</div></div>
        <div class="exercise-item"><div class="ex-num">02</div><div class="ex-info"><div class="ex-name">Planche latérale avec rotation</div><div class="ex-detail">3×12 chaque côté · Rotation thoracique complète</div></div></div>
        <div class="exercise-item"><div class="ex-num">03</div><div class="ex-info"><div class="ex-name">Pallof Press (anti-rotation)</div><div class="ex-detail">4×12 chaque côté · Câble ou bande élastique</div></div><div class="ex-badge tag tag-red">COCKPIT</div></div>
        <div class="exercise-item"><div class="ex-num">04</div><div class="ex-info"><div class="ex-name">Dead Bug</div><div class="ex-detail">3×10 reps lentes · Bas de dos collé au sol</div></div></div>
        <div class="exercise-item"><div class="ex-num">05</div><div class="ex-info"><div class="ex-name">Russian Twist lesté</div><div class="ex-detail">4×20 reps · Médecine-ball 4–6kg · Simulation torsion volant</div></div></div>
        <div class="exercise-item"><div class="ex-num">06</div><div class="ex-info"><div class="ex-name">Gainage instable sur Bosu</div><div class="ex-detail">3×45 sec · Simulation vibrations cockpit GT</div></div></div>
        <div class="exercise-item"><div class="ex-num">07</div><div class="ex-info"><div class="ex-name">Ab Wheel Rollout</div><div class="ex-detail">4×8–12 reps · Éviter l'hyperextension lombaire</div></div><div class="ex-badge tag tag-gold">AVANCÉ</div></div>
      </div>
      <div>
        <div class="card mb1"><div class="card-accent green"></div><div class="card-title">📋 Circuit Core — 30 min chrono</div><div style="font-size:.82rem;line-height:2;color:var(--text);"><strong style="color:var(--gold);">Échauffement 5 min :</strong> Cat-Cow × 10 · Bird-Dog × 10<br><strong style="color:var(--red);">Bloc A (×3) :</strong> Planche 60s → Dead Bug 10 → Hollow Body 30s · Repos 45s<br><strong style="color:var(--red);">Bloc B (×3) :</strong> Pallof Press 12 → Russian Twist 20 → Copenhagen 25s · Repos 45s<br><strong style="color:var(--blue);">Finisher :</strong> Ab Wheel 3×8 · Gainage Bosu 3×45s<br><strong style="color:var(--green);">Retour au calme 5 min :</strong> Hip Flexor · Pigeon · 90/90</div></div>
        <div class="card"><div class="card-accent blue"></div><div class="card-title">🧘 Mobilité colonne & hanches</div><div class="exercise-item" style="margin-bottom:.5rem;"><div class="ex-info"><div class="ex-name">Hip Flexor stretch 90/90</div><div class="ex-detail">2×60 sec chaque · Position demi-agenouillé · Priorité absolue pilote</div></div></div><div class="exercise-item" style="margin-bottom:.5rem;"><div class="ex-info"><div class="ex-name">Pigeon Pose</div><div class="ex-detail">2×60 sec chaque · Piriforme et sciatique</div></div></div><div class="exercise-item"><div class="ex-info"><div class="ex-name">Cat-Cow + rotation thoracique</div><div class="ex-detail">2×15 · Ouvre les vertèbres thoraciques comprimées par le baquet</div></div></div></div>
      </div>
    </div>
  </div>
  <div id="train-cardio" style="display:none;">
    <div class="alert green"><div class="alert-title">❤️ Cardio & Endurance — Spécifique Pilote GT</div>Un pilote GT endurance peut avoir une FC de 140–170 bpm pendant 2–3h de relais.</div>
    <div class="grid-2">
      <div>
        <div class="card mb1"><div class="card-title" style="color:var(--green);">Zone 2 — Endurance aérobie (60–70% FC max)</div><div class="exercise-item" style="margin-bottom:.4rem;"><div class="ex-info"><div class="ex-name">Vélo 60 min Zone 2</div><div class="ex-detail">FC 130–145 bpm · Cadence 85–95 rpm</div></div><div class="ex-badge tag tag-green">LUN</div></div><div class="exercise-item" style="margin-bottom:.4rem;"><div class="ex-info"><div class="ex-name">Course à pied 45 min</div><div class="ex-detail">FC 130–140 bpm · Allure conversationnelle</div></div><div class="ex-badge tag tag-green">VEN</div></div><div class="exercise-item"><div class="ex-info"><div class="ex-name">Natation 45 min</div><div class="ex-detail">Crawl endurance · 100m intervalles × 20</div></div></div></div>
        <div class="card mb1"><div class="card-title" style="color:var(--gold);">Zone 3–4 — Seuil lactique (75–85% FC max)</div><div class="exercise-item" style="margin-bottom:.4rem;"><div class="ex-info"><div class="ex-name">Intervalles 10 min seuil</div><div class="ex-detail">4×10 min à FC 160–170 bpm · Récup 3 min</div></div><div class="ex-badge tag tag-gold">MAR</div></div><div class="exercise-item"><div class="ex-info"><div class="ex-name">Tempo Run 30 min</div><div class="ex-detail">Effort continu soutenu · "Comfortably hard"</div></div></div></div>
        <div class="card"><div class="card-title" style="color:var(--red);">Zone 5 — HIIT (90–100% FC max)</div><div class="exercise-item" style="margin-bottom:.4rem;"><div class="ex-info"><div class="ex-name">Tabata Vélo</div><div class="ex-detail">8×20 sec sprint max / 10 sec repos · 4 séries</div></div><div class="ex-badge tag tag-red">JEU</div></div><div class="exercise-item"><div class="ex-info"><div class="ex-name">Rameur 500m sprints</div><div class="ex-detail">6×500m effort max · Récup = temps × 1,5</div></div></div></div>
      </div>
      <div>
        <div class="card"><div class="card-accent gold"></div><div class="card-title">📊 Planification semaine cardio</div><div style="display:flex;flex-direction:column;gap:.3rem;font-size:.82rem;"><div style="display:flex;justify-content:space-between;border-bottom:1px solid var(--border);padding:.4rem 0;"><span>Lundi</span><span style="color:var(--green)">Zone 2 Vélo 60 min</span></div><div style="display:flex;justify-content:space-between;border-bottom:1px solid var(--border);padding:.4rem 0;"><span>Mardi</span><span style="color:var(--gold)">Intervalles seuil 45 min</span></div><div style="display:flex;justify-content:space-between;border-bottom:1px solid var(--border);padding:.4rem 0;"><span>Mercredi</span><span style="color:var(--muted)">Repos cardio (core)</span></div><div style="display:flex;justify-content:space-between;border-bottom:1px solid var(--border);padding:.4rem 0;"><span>Jeudi</span><span style="color:var(--red)">HIIT 20–25 min</span></div><div style="display:flex;justify-content:space-between;border-bottom:1px solid var(--border);padding:.4rem 0;"><span>Vendredi</span><span style="color:var(--green)">Zone 2 Natation 45 min</span></div><div style="display:flex;justify-content:space-between;border-bottom:1px solid var(--border);padding:.4rem 0;"><span>Samedi</span><span style="color:var(--green)">Zone 2 long 75–90 min</span></div><div style="display:flex;justify-content:space-between;padding:.4rem 0;"><span>Dimanche</span><span style="color:var(--muted)">Repos complet</span></div></div></div>
      </div>
    </div>
  </div>
  <div id="train-prerace_fit" style="display:none;">
    <div class="alert gold"><div class="alert-title">🏁 Semaine de course — Réduction de charge</div>J-7 à J-1 : réduire volume de 40–50%. Le corps doit être frais, pas fatigué.</div>
    <div class="grid-2">
      <div>
        <div class="meal-card"><div class="meal-time">J-7</div><div class="meal-content"><div class="meal-name">Dernière séance intense</div><div class="meal-desc">Nuque + core pleine intensité · Dernière chance de surcharger avant taper</div></div></div>
        <div class="meal-card"><div class="meal-time">J-5</div><div class="meal-content"><div class="meal-name">Cardio léger</div><div class="meal-desc">30 min Zone 2 · Aucune fatigue · Maintien du rythme cardiaque</div></div></div>
        <div class="meal-card"><div class="meal-time">J-4</div><div class="meal-content"><div class="meal-name">Nuque volume réduit</div><div class="meal-desc">2×10 reps · Charge légère · Activation seulement</div></div></div>
        <div class="meal-card"><div class="meal-time">J-3</div><div class="meal-content"><div class="meal-name">Mobilité & étirements</div><div class="meal-desc">30 min yoga/mobilité · Aucun effort · Corps frais</div></div></div>
        <div class="meal-card"><div class="meal-time">J-2</div><div class="meal-content"><div class="meal-name">Marche active</div><div class="meal-desc">30 min marche · Reconnaissance circuit si possible</div></div></div>
        <div class="meal-card"><div class="meal-time">J-1</div><div class="meal-content"><div class="meal-name">Repos complet</div><div class="meal-desc">Étirements 10 min · Visualisation · Sommeil +9h</div></div></div>
      </div>
      <div>
        <div class="card"><div class="card-accent gold"></div><div class="card-title">🧠 Préparation mentale</div><div style="font-size:.82rem;line-height:1.9;color:var(--text);"><strong style="color:var(--gold);">Visualisation :</strong> 15 min/j les 3 jours avant. Ferme les yeux, conduis le circuit mentalement.<br><br><strong style="color:var(--gold);">Sophrologie :</strong> Respiration 4-7-8 pour gérer l'adrénaline du départ.<br><br><strong style="color:var(--gold);">Routine pré-relais :</strong> Échauffement nuque 5 min + respiration profonde + check mental.<br><br><strong style="color:var(--gold);">Réduction stimulation :</strong> J-2 : limiter écrans, réseaux sociaux, stress extérieur.</div></div>
      </div>
    </div>
  </div>
  <div id="train-hotel" style="display:none;">
    <div class="alert blue"><div class="alert-title">🏨 Entraînement sans salle — Chambre d'hôtel, motorhome</div>25–30 min suffisent pour maintenir ton niveau. Zéro équipement requis.</div>
    <div class="grid-2">
      <div>
        <div class="exercise-item"><div class="ex-num">01</div><div class="ex-info"><div class="ex-name">Planche frontale + tapotements épaules</div><div class="ex-detail">4×30 sec · Core + coordination</div></div></div>
        <div class="exercise-item"><div class="ex-num">02</div><div class="ex-info"><div class="ex-name">Push-up décliné sur lit</div><div class="ex-detail">4×12–15 · Pieds sur le lit · Pectoraux hauts + deltoïdes</div></div></div>
        <div class="exercise-item"><div class="ex-num">03</div><div class="ex-info"><div class="ex-name">Nuque isométrique 4 directions</div><div class="ex-detail">Avant, arrière, gauche, droite × 30 sec · Main comme résistance</div></div></div>
        <div class="exercise-item"><div class="ex-num">04</div><div class="ex-info"><div class="ex-name">Slow Squat (5 sec descente)</div><div class="ex-detail">4×10 · Silencieux · Jambes + gainage</div></div></div>
        <div class="exercise-item"><div class="ex-num">05</div><div class="ex-info"><div class="ex-name">Dead Bug au sol</div><div class="ex-detail">3×10 chaque côté · Core profond activé</div></div></div>
        <div class="exercise-item"><div class="ex-num">06</div><div class="ex-info"><div class="ex-name">Mountain Climbers lents</div><div class="ex-detail">3×30 sec · Contrôlé et silencieux · Core + cardio</div></div></div>
        <div class="exercise-item"><div class="ex-num">07</div><div class="ex-info"><div class="ex-name">Burpee sans saut (step)</div><div class="ex-detail">3×10 · Cardio efficace + silencieux + total body</div></div></div>
      </div>
      <div>
        <div class="card mb1"><div class="card-accent blue"></div><div class="card-title">🧳 Kit voyage léger à emporter</div><div style="font-size:.82rem;line-height:2;color:var(--text);">✓ Bande élastique résistance × 2 (nuque + full body)<br>✓ Harnais de nuque pliable (type Neck Flex)<br>✓ Gripper de main (Captains of Crush)<br>✓ Roller de massage compact<br>✓ Balle de lacrosse (trigger points dos, fessiers)<br>✓ Masque de sommeil + bouchons oreilles</div></div>
        <div class="card"><div class="card-accent green"></div><div class="card-title">⏱ Routine express 10 min</div><div style="font-size:.82rem;line-height:2;color:var(--text);">Planche 60 sec → Nuque isométrique 4 dir → Push-up × 15 → Dead Bug × 10 → Hip Flexor 45 sec → Cat-Cow × 10<br><span style="color:var(--muted);">→ Suffit pour activer le corps et soulager les tensions post-vol</span></div></div>
      </div>
    </div>
  </div>
</div>

<!-- ===== RACE ===== -->

<div class="page" id="page-race">
  <div class="section-title">Protocole Course</div>
  <div class="selector">
    <button class="sel-btn active" onclick="switchSection('race','race3',this)">3–6 heures</button>
    <button class="sel-btn" onclick="switchSection('race','race24',this)">24 heures</button>
    <button class="sel-btn" onclick="switchSection('race','relais',this)">Inter-relais</button>
  </div>
  <div id="race-race3">
    <div class="grid-2">
      <div>
        <div class="card-title" style="font-family:'Barlow Condensed';font-weight:700;font-size:.82rem;letter-spacing:2px;text-transform:uppercase;margin-bottom:.8rem;">📋 Timeline complète — Course 3–6h</div>
        <div class="timeline">
          <div class="tl-item"><div class="tl-time">VEILLE — 20H</div><div class="tl-action">Dernier check nutrition</div><div class="tl-detail">Dîner GF léger · Suppléments soir · Sommeil 22h max</div></div>
          <div class="tl-item"><div class="tl-time">JOUR J — 7H</div><div class="tl-action">Réveil & protocole matin</div><div class="tl-detail">750ml eau + électrolytes dès le réveil · Suppléments matin</div></div>
          <div class="tl-item"><div class="tl-time">H-3 COURSE</div><div class="tl-action">Repas pré-course GF</div><div class="tl-detail">Riz blanc + œufs + banane · 750ml eau · Dernier caféine si habitude</div></div>
          <div class="tl-item"><div class="tl-time">H-1 COURSE</div><div class="tl-action">Préparation finale</div><div class="tl-detail">1 gel GF + 300ml eau · Échauffement nuque · Vérifier kit cockpit hydratation</div></div>
          <div class="tl-item"><div class="tl-time">EN COURSE</div><div class="tl-action">Ravitaillement continu</div><div class="tl-detail">1 gel GF toutes les 45 min · Eau en continu · Électrolytes selon chaleur</div></div>
          <div class="tl-item"><div class="tl-time">ARRIVÉE</div><div class="tl-action">Récupération immédiate</div><div class="tl-detail">Whey GF + banane dans les 30 min · 1L eau + électrolytes · Jus cerises</div></div>
        </div>
      </div>
      <div>
        <div class="card"><div class="card-accent red"></div><div class="card-title">🔥 Signaux d'alarme cockpit</div><div style="display:flex;flex-direction:column;gap:.5rem;"><div class="alert red"><div class="alert-title">🚨 Déshydratation</div>Maux de tête, vertiges, vision trouble → augmenter immédiatement hydratation</div><div class="alert gold"><div class="alert-title">⚠️ Crampes musculaires</div>Gélule de sel immédiate + électrolytes → signal de carence sodium</div><div class="alert blue"><div class="alert-title">💡 Hypoglycémie</div>Tremblements, confusion → gel sucre rapide immédiat. Communiquer au team</div></div></div>
      </div>
    </div>
  </div>
  <div id="race-race24" style="display:none;">
    <div class="alert red"><div class="alert-title">🌙 24h — Stratégie complète multi-pilotes</div>Planning nutritionnel et suppléments à coordonner avec les relais de l'équipe.</div>
    <div class="grid-2">
      <div>
        <div class="timeline">
          <div class="tl-item"><div class="tl-time">H-3 DÉPART</div><div class="tl-action">Repas pré-course GF</div><div class="tl-detail">Riz blanc + poulet + électrolytes · 750ml eau · Aucune fibre</div></div>
          <div class="tl-item"><div class="tl-time">H0–H6</div><div class="tl-action">Phase diurne — Glucides++</div><div class="tl-detail">60–90g glucides/h · Gels GF + banane · 700ml eau/h · Sel si chaud</div></div>
          <div class="tl-item"><div class="tl-time">H6–H12</div><div class="tl-action">Repas solides entre relais</div><div class="tl-detail">Riz blanc + poulet ou saumon · Soupe miso · Pas de fibres · 1L eau/h</div></div>
          <div class="tl-item"><div class="tl-time">H12–H18 (minuit)</div><div class="tl-action">Protocole nocturne</div><div class="tl-detail">Gel caféiné 75mg avant chaque relais de nuit · Bouillon chaud · Lumière bleue OFF</div></div>
          <div class="tl-item"><div class="tl-time">H18–H21 (3h–6h)</div><div class="tl-action">🔴 Creux circadien CRITIQUE</div><div class="tl-detail">Boost caféine + gel sucre rapide · Micro-sieste 20 min · Lumière vive au réveil</div></div>
          <div class="tl-item"><div class="tl-time">H21–H24 (aube)</div><div class="tl-action">Phase finish — Focus total</div><div class="tl-detail">Gel caféiné 30 min avant dernier relais · Eau + sodium · Visualisation finish</div></div>
        </div>
      </div>
      <div>
        <div class="card"><div class="card-accent gold"></div><div class="card-title">🛌 Gestion sommeil 24h</div><div style="font-size:.82rem;line-height:1.9;color:var(--text);"><strong style="color:var(--gold);">Micro-sieste :</strong> 15–20 min max. Alarme obligatoire.<br><br><strong style="color:var(--gold);">Environnement :</strong> Masque yeux + bouchons + position semi-allongée. Couverture thermique.<br><br><strong style="color:var(--gold);">Réveil actif :</strong> Lumière vive + eau froide visage + 5 min marche rapide.<br><br><strong style="color:var(--red);">Ne jamais dormir &lt;30 min avant relais.</strong></div></div>
      </div>
    </div>
  </div>
  <div id="race-relais" style="display:none;">
    <div class="alert green"><div class="alert-title">🔄 Protocole inter-relais</div>Les minutes après le relais sont aussi importantes que pendant la conduite.</div>
    <div class="grid-2">
      <div>
        <div class="timeline">
          <div class="tl-item"><div class="tl-time">0–2 MIN</div><div class="tl-action">Sortie voiture</div><div class="tl-detail">500ml eau + électrolytes immédiatement · Sortir du bruit et de la chaleur</div></div>
          <div class="tl-item"><div class="tl-time">2–5 MIN</div><div class="tl-action">Débriefing rapide</div><div class="tl-detail">Retour équipe sur les points tech · Ne pas stresser · Rester focus</div></div>
          <div class="tl-item"><div class="tl-time">5–15 MIN</div><div class="tl-action">Nutrition & récupération active</div><div class="tl-detail">Banane / gel GF / barre de riz · Étirements nuque 3 min</div></div>
          <div class="tl-item"><div class="tl-time">15–30 MIN</div><div class="tl-action">Repos & préparation</div><div class="tl-detail">Position allongée si possible · Respiration calme · Visualiser prochain relais</div></div>
          <div class="tl-item"><div class="tl-time">H-15 MIN</div><div class="tl-action">Activation pré-relais</div><div class="tl-detail">Échauffement nuque 5 min · 1 gel GF + eau · Caféine si relais nocturne</div></div>
          <div class="tl-item"><div class="tl-time">H-5 MIN</div><div class="tl-action">Rituel mental</div><div class="tl-detail">Respiration 4-7-8 × 3 cycles · Focus. Concentration. Circuit.</div></div>
        </div>
      </div>
      <div>
        <div class="card"><div class="card-accent green"></div><div class="card-title">🧘 Respiration 4-7-8</div><div style="font-size:.85rem;line-height:2;color:var(--text);">1. Expire complètement par la bouche<br>2. Inspire par le nez pendant <strong style="color:var(--gold);">4 sec</strong><br>3. Retiens le souffle <strong style="color:var(--gold);">7 sec</strong><br>4. Expire lentement par la bouche <strong style="color:var(--gold);">8 sec</strong><br>5. Répéter 3–4 cycles<br><br><span style="color:var(--muted);">Réduit le cortisol, calme le système nerveux sympathique.</span></div></div>
      </div>
    </div>
  </div>
</div>

<!-- ===== TRAVEL ===== -->

<div class="page" id="page-travel">
  <div class="section-title">Voyage & Jet Lag</div>
  <div id="travel-next-alert" style="margin-bottom:1rem;"></div>
  <div class="card mb2"><div class="card-accent gold"></div><div class="card-title">🌍 Horloges en temps réel</div>
    <div class="tz-grid">
      <div class="tz-card"><div class="tz-city">Bruxelles (Base)</div><div class="tz-time active" id="tz-paris">--:--</div></div>
      <div class="tz-card"><div class="tz-city">Tokyo (+8h)</div><div class="tz-time" id="tz-tokyo">--:--</div></div>
      <div class="tz-card"><div class="tz-city">New York (-6h)</div><div class="tz-time" id="tz-ny">--:--</div></div>
      <div class="tz-card"><div class="tz-city">Dubai (+3h)</div><div class="tz-time" id="tz-dubai">--:--</div></div>
    </div>
  </div>
  <div class="grid-2">
    <div>
      <div class="section-title" style="font-size:1rem;">Destinations GT — Protocoles</div>
      <div class="toggle-section open"><div class="toggle-header" onclick="toggleSection(this)">🇯🇵 Japon — 6H Fuji, 1000km Suzuka <span class="toggle-arrow">▼</span></div><div class="toggle-body"><div style="font-size:.82rem;line-height:1.9;color:var(--text);"><strong style="color:var(--gold);">Décalage :</strong> +8h (Europe). Arriver 5–6 jours avant idéalement.<br><strong style="color:var(--gold);">Nutrition GF :</strong> Riz partout · Sashimi sans soja classique → tamari · Onigiri = GF · Ramen = gluten (éviter)<br><strong style="color:var(--gold);">Protocole :</strong> Mélatonine 0,5mg pendant 3 nuits · Exposer au soleil matin obligatoire · Ashwagandha<br><strong style="color:var(--gold);">Hydratation :</strong> Eau du robinet potable. Conbini = ressources 24h/24.</div></div></div>
      <div class="toggle-section"><div class="toggle-header" onclick="toggleSection(this)">🇩🇪 Nürburgring — 24h N24 <span class="toggle-arrow">▼</span></div><div class="toggle-body"><div style="font-size:.82rem;line-height:1.9;color:var(--text);"><strong style="color:var(--gold);">Décalage :</strong> +1h (depuis Belgique). Impact minimal.<br><strong style="color:var(--gold);">Nutrition GF :</strong> Mention allergène obligatoire en UE. Kartoffeln, Fleisch = base GF.<br><strong style="color:var(--gold);">Spécificités 24h :</strong> Brouillard fréquent à l'aube = visibilité réduite → récupération mentale critique.</div></div></div>
      <div class="toggle-section"><div class="toggle-header" onclick="toggleSection(this)">🇺🇸 USA — IMSA, Daytona, Austin <span class="toggle-arrow">▼</span></div><div class="toggle-body"><div style="font-size:.82rem;line-height:1.9;color:var(--text);"><strong style="color:var(--gold);">Décalage :</strong> -6h (Est) à -9h (Pacifique).<br><strong style="color:var(--gold);">Nutrition GF :</strong> GF très bien indiqué. Chipotle, Sweetgreen, Whole Foods = ressources sûres.<br><strong style="color:var(--gold);">Protocole jet lag :</strong> Rester éveillé jusqu'à 23h locale J1 · Caféine matinale J+1–2.</div></div></div>
      <div class="toggle-section"><div class="toggle-header" onclick="toggleSection(this)">🇦🇺 Australie — Bathurst <span class="toggle-arrow">▼</span></div><div class="toggle-body"><div style="font-size:.82rem;line-height:1.9;color:var(--text);"><strong style="color:var(--gold);">Décalage :</strong> +9h à +11h. L'un des plus difficiles.<br><strong style="color:var(--gold);">Arriver 7 jours avant</strong> si budget et calendrier le permettent.<br><strong style="color:var(--gold);">Protocole :</strong> Mélatonine + Ashwagandha combinés · Grounding · Soleil matin strict</div></div></div>
      <div class="toggle-section"><div class="toggle-header" onclick="toggleSection(this)">🇧🇷 Brésil — 6H São Paulo <span class="toggle-arrow">▼</span></div><div class="toggle-body"><div style="font-size:.82rem;line-height:1.9;color:var(--text);"><strong style="color:var(--gold);">Décalage :</strong> -4h (Belgique). Impact modéré.<br><strong style="color:var(--gold);">Nutrition GF :</strong> Riz, viandes grillées, feijão (haricots) = base GF. Attention aux sauces locales.<br><strong style="color:var(--gold);">Sécurité :</strong> Rester dans zones sécurisées autour du circuit.</div></div></div>
      <div class="toggle-section"><div class="toggle-header" onclick="toggleSection(this)">🇧🇭 Bahrain — 8H Bahrain WEC <span class="toggle-arrow">▼</span></div><div class="toggle-body"><div style="font-size:.82rem;line-height:1.9;color:var(--text);"><strong style="color:var(--gold);">Décalage :</strong> +2h à +3h. Impact modéré.<br><strong style="color:var(--gold);">Chaleur :</strong> 35–45°C extérieur. Cockpit peut dépasser 60°C. Hydratation × 2.<br><strong style="color:var(--gold);">Nutrition GF :</strong> Riz basmati + grillades + hummus maison GF. Éviter pains locaux.</div></div></div>
      <div class="toggle-section"><div class="toggle-header" onclick="toggleSection(this)">🇶🇦 Qatar — WEC 1812km <span class="toggle-arrow">▼</span></div><div class="toggle-body"><div style="font-size:.82rem;line-height:1.9;color:var(--text);"><strong style="color:var(--gold);">Décalage :</strong> +2h (Belgique). Impact minimal.<br><strong style="color:var(--gold);">Chaleur nocturne :</strong> Manche souvent disputée de nuit — températures plus clémentes mais humidité élevée.<br><strong style="color:var(--gold);">Nutrition GF :</strong> Cuisine arabe = riz + viandes grillées. Hôtels internationaux bien équipés.</div></div></div>
    </div>
    <div>
      <div class="section-title" style="font-size:1rem;">Protocole vol long-courrier</div>
      <div class="card"><div class="card-accent gold"></div><div class="card-title">✈️ Check-list avion</div>
        <div class="checklist-item" onclick="toggleCheck(this)"><div class="check-box"></div><span class="check-label">Barres GF certifiées dans bagage cabine</span></div>
        <div class="checklist-item" onclick="toggleCheck(this)"><div class="check-box"></div><span class="check-label">Électrolytes (sachets LMNT ou Precision)</span></div>
        <div class="checklist-item" onclick="toggleCheck(this)"><div class="check-box"></div><span class="check-label">Mélatonine 0,5mg (si vol de nuit)</span></div>
        <div class="checklist-item" onclick="toggleCheck(this)"><div class="check-box"></div><span class="check-label">Magnésium + L-Théanine pour dormir</span></div>
        <div class="checklist-item" onclick="toggleCheck(this)"><div class="check-box"></div><span class="check-label">Masque yeux + bouchons oreilles</span></div>
        <div class="checklist-item" onclick="toggleCheck(this)"><div class="check-box"></div><span class="check-label">Boire 300ml eau/heure de vol</span></div>
        <div class="checklist-item" onclick="toggleCheck(this)"><div class="check-box"></div><span class="check-label">Zero alcool pendant le vol</span></div>
        <div class="checklist-item" onclick="toggleCheck(this)"><div class="check-box"></div><span class="check-label">Se lever et marcher toutes les 90 min</span></div>
        <div class="checklist-item" onclick="toggleCheck(this)"><div class="check-box"></div><span class="check-label">Régler montre sur heure destination dès décollage</span></div>
        <div class="checklist-item" onclick="toggleCheck(this)"><div class="check-box"></div><span class="check-label">Éviter repas avion (gluten caché)</span></div>
      </div>
      <div class="card mt1"><div class="card-accent blue"></div><div class="card-title">⏱ Règle des 3 jours</div><div style="font-size:.82rem;line-height:1.9;color:var(--muted);">Pour chaque 3h de décalage horaire, le corps a besoin d'environ 1 jour d'adaptation complète.<br><strong style="color:var(--text);">Ex : Japon +8h → 2–3 jours d'adaptation naturelle.</strong><br><br>Le protocole suppléments + lumière réduit ce temps de moitié.<br>Pour les grosses courses (24h, WEC) : arriver au moins <strong style="color:var(--gold)">5 jours avant</strong> pour les décalages >6h.</div></div>
    </div>
  </div>
</div>

</main>

<script>
// ============================================================
// CALENDRIER 2026 — PUSHPAPY ON TOUR
// ============================================================
const CALENDAR_2026 = [
  {id:1,  dateStart:"2026-01-16",dateEnd:"2026-01-18",event:"Roar Before the Rolex 24",    championship:"IMSA",      location:"Daytona",          country:"US",duration:null,type:"test"},
  {id:2,  dateStart:"2026-01-21",dateEnd:"2026-01-25",event:"24H Daytona (Rolex 24)",       championship:"IMSA",      location:"Daytona",          country:"US",duration:24,  type:"race"},
  {id:3,  dateStart:"2026-02-13",dateEnd:"2026-02-15",event:"12H Bathurst",                 championship:"IGTC",      location:"Bathurst",         country:"AU",duration:12,  type:"race"},
  {id:4,  dateStart:"2026-03-13",dateEnd:"2026-03-14",event:"NLS 1 – Nürburgring",          championship:"NLS",       location:"Nürburgring",      country:"DE",duration:null,type:"race"},
  {id:5,  dateStart:"2026-03-20",dateEnd:"2026-03-21",event:"NLS 2 – Nürburgring",          championship:"NLS",       location:"Nürburgring",      country:"DE",duration:null,type:"race"},
  {id:6,  dateStart:"2026-03-22",dateEnd:"2026-03-23",event:"Prologue Qatar",               championship:"WEC",       location:"Lusail",           country:"QA",duration:null,type:"test"},
  {id:7,  dateStart:"2026-03-27",dateEnd:"2026-03-28",event:"Qatar 1812km",                 championship:"WEC",       location:"Lusail",           country:"QA",duration:null,type:"race"},
  {id:8,  dateStart:"2026-04-07",dateEnd:"2026-04-08",event:"Essais officiels – Paul Ricard",championship:"GTWC",    location:"Paul Ricard",      country:"FR",duration:null,type:"test"},
  {id:9,  dateStart:"2026-04-10",dateEnd:"2026-04-12",event:"Paul Ricard (Endurance)",      championship:"GTWC",      location:"Paul Ricard",      country:"FR",duration:null,type:"race"},
  {id:10, dateStart:"2026-04-18",dateEnd:"2026-04-19",event:"6H Imola",                     championship:"WEC",       location:"Imola",            country:"IT",duration:6,   type:"race"},
  {id:11, dateStart:"2026-05-01",dateEnd:"2026-05-03",event:"ELMS – Paul Ricard (4H)",      championship:"ELMS",      location:"Paul Ricard",      country:"FR",duration:4,   type:"race"},
  {id:12, dateStart:"2026-05-08",dateEnd:"2026-05-09",event:"6H Spa-Francorchamps",         championship:"WEC",       location:"Spa-Francorchamps",country:"BE",duration:6,   type:"race"},
  {id:13, dateStart:"2026-05-14",dateEnd:"2026-05-17",event:"24H Nürburgring",              championship:"IGTC",      location:"Nürburgring",      country:"DE",duration:24,  type:"race"},
  {id:14, dateStart:"2026-05-19",dateEnd:"2026-05-20",event:"Prologue 24H Spa",             championship:"GTWC",      location:"Spa-Francorchamps",country:"BE",duration:null,type:"test"},
  {id:15, dateStart:"2026-05-29",dateEnd:"2026-05-31",event:"Monza (Endurance)",            championship:"GTWC",      location:"Monza",            country:"IT",duration:null,type:"race"},
  {id:16, dateStart:"2026-06-08",dateEnd:"2026-06-14",event:"24H du Mans",                  championship:"WEC",       location:"Le Mans",          country:"FR",duration:24,  type:"race"},
  {id:17, dateStart:"2026-06-24",dateEnd:"2026-06-28",event:"24H Spa",                      championship:"GTWC",      location:"Spa-Francorchamps",country:"BE",duration:24,  type:"race"},
  {id:18, dateStart:"2026-07-04",dateEnd:"2026-07-05",event:"ELMS – Imola (4H)",            championship:"ELMS",      location:"Imola",            country:"IT",duration:4,   type:"race"},
  {id:19, dateStart:"2026-07-04",dateEnd:"2026-07-05",event:"12H Nürburgring",              championship:"24H Series",location:"Nürburgring",      country:"DE",duration:12,  type:"race"},
  {id:20, dateStart:"2026-07-11",dateEnd:"2026-07-12",event:"6H São Paulo",                 championship:"WEC",       location:"São Paulo",        country:"BR",duration:6,   type:"race"},
  {id:21, dateStart:"2026-08-22",dateEnd:"2026-08-23",event:"ELMS – Spa-Francorchamps (4H)",championship:"ELMS",    location:"Spa-Francorchamps",country:"BE",duration:4,   type:"race"},
  {id:22, dateStart:"2026-08-28",dateEnd:"2026-08-30",event:"Nürburgring (Endurance)",      championship:"GTWC",      location:"Nürburgring",      country:"DE",duration:null,type:"race"},
  {id:23, dateStart:"2026-09-05",dateEnd:"2026-09-06",event:"Lone Star Le Mans – Austin",   championship:"WEC",       location:"Austin",           country:"US",duration:6,   type:"race"},
  {id:24, dateStart:"2026-09-11",dateEnd:"2026-09-13",event:"1000km Suzuka",                championship:"IGTC",      location:"Suzuka",           country:"JP",duration:null,type:"race"},
  {id:25, dateStart:"2026-09-18",dateEnd:"2026-09-20",event:"24H Barcelone",                championship:"24H Series",location:"Barcelona",         country:"ES",duration:24,  type:"race"},
  {id:26, dateStart:"2026-09-26",dateEnd:"2026-09-27",event:"6H Fuji",                      championship:"WEC",       location:"Fuji",             country:"JP",duration:6,   type:"race"},
  {id:27, dateStart:"2026-10-08",dateEnd:"2026-10-10",event:"8H Indianapolis",              championship:"IGTC",      location:"Indianapolis",     country:"US",duration:8,   type:"race"},
  {id:28, dateStart:"2026-10-16",dateEnd:"2026-10-18",event:"Portimão (Endurance)",         championship:"GTWC",      location:"Portimão",         country:"PT",duration:null,type:"race"},
  {id:29, dateStart:"2026-11-06",dateEnd:"2026-11-07",event:"8H Bahrain",                   championship:"WEC",       location:"Bahrain",          country:"BH",duration:8,   type:"race"}
];

const LONG_HAUL = ["US","AU","JP","BR","BH","QA"];
const JETLAG_INFO = {
  "US": {offset:"-6h/-9h", severity:"ÉLEVÉ", flag:"🇺🇸"},
  "AU": {offset:"+9h/+11h", severity:"CRITIQUE", flag:"🇦🇺"},
  "JP": {offset:"+8h", severity:"ÉLEVÉ", flag:"🇯🇵"},
  "BR": {offset:"-4h", severity:"MODÉRÉ", flag:"🇧🇷"},
  "BH": {offset:"+2h", severity:"FAIBLE", flag:"🇧🇭"},
  "QA": {offset:"+2h", severity:"FAIBLE", flag:"🇶🇦"}
};

// ============================================================
// PHASE ENGINE — Détection automatique de la phase
// ============================================================
function getToday() {
  return new Date();
}

function dateStr(d) {
  return d.toISOString().split('T')[0];
}

function diffDays(d1, d2) {
  return Math.round((d2 - d1) / (1000 * 60 * 60 * 24));
}

function getNextEvent(today) {
  const todayStr = dateStr(today);
  return CALENDAR_2026.find(e => e.dateEnd >= todayStr) || null;
}

function getCurrentPhase() {
  const today = getToday();
  const todayStr = dateStr(today);

  // Trouver l'event actif (on est dedans)
  const activeEvent = CALENDAR_2026.find(e => todayStr >= e.dateStart && todayStr <= e.dateEnd);

  // Trouver le prochain event
  const nextEvent = CALENDAR_2026.find(e => e.dateStart > todayStr);

  // Trouver l'event qui vient de se terminer (récup)
  const justFinished = CALENDAR_2026.filter(e => e.dateEnd < todayStr).sort((a,b)=>b.dateEnd.localeCompare(a.dateEnd))[0];

  if (activeEvent) {
    // ON EST EN COURSE / TEST
    return {
      phase: activeEvent.type === 'test' ? 'taper' : 'race',
      event: activeEvent,
      nextEvent: nextEvent,
      daysTo: 0,
      daysAfter: 0,
      justFinished: null
    };
  }

  const daysAfterLast = justFinished ? diffDays(new Date(justFinished.dateEnd), today) : 999;

  // RÉCUPÉRATION : 0–3 jours après une course
  if (justFinished && daysAfterLast <= 3 && justFinished.type === 'race') {
    return {
      phase: 'recovery',
      event: nextEvent,
      justFinished: justFinished,
      daysTo: nextEvent ? diffDays(today, new Date(nextEvent.dateStart)) : null,
      daysAfter: daysAfterLast
    };
  }

  if (!nextEvent) {
    return { phase: 'training', event: null, nextEvent: null, daysTo: null, daysAfter: 0, justFinished: null };
  }

  const daysToNext = diffDays(today, new Date(nextEvent.dateStart));

  // JET LAG : si prochain event est long haul et dans moins de 14 jours + on vient de voyager
  const isLongHaul = LONG_HAUL.includes(nextEvent.country);

  // PRÉ-COURSE J-3 à J-1 : carb loading
  if (daysToNext <= 3 && daysToNext >= 0) {
    return { phase: 'prerace', event: nextEvent, daysTo: daysToNext, daysAfter: daysAfterLast, justFinished: null };
  }

  // TAPER J-7 à J-4 : réduction de charge
  if (daysToNext <= 7 && daysToNext >= 4) {
    return { phase: 'taper', event: nextEvent, daysTo: daysToNext, daysAfter: daysAfterLast, justFinished: null };
  }

  // JET LAG : alerte si long haul dans moins de 10 jours
  if (isLongHaul && daysToNext <= 10) {
    return { phase: 'jetlag', event: nextEvent, daysTo: daysToNext, daysAfter: daysAfterLast, justFinished: null };
  }

  // ENTRAÎNEMENT : phase normale
  return { phase: 'training', event: nextEvent, daysTo: daysToNext, daysAfter: daysAfterLast, justFinished: null };
}

// ============================================================
// DASHBOARD DYNAMIQUE
// ============================================================
function updateDashboard() {
  const p = getCurrentPhase();
  const banner = document.getElementById('phase-banner');
  const label = document.getElementById('phase-label');
  const title = document.getElementById('phase-title');
  const desc = document.getElementById('phase-desc');
  const meta = document.getElementById('phase-meta');

  // Reset classes
  banner.className = 'phase-banner ' + p.phase;

  const eventName = p.event ? p.event.event : (p.justFinished ? p.justFinished.event : '—');
  const champ = p.event ? p.event.championship : '';
  const country = p.event ? p.event.country : '';
  const isLongHaul = LONG_HAUL.includes(country);
  const jetlagInfo = JETLAG_INFO[country] || null;

  const phases = {
    training: {
      label: 'PHASE ENTRAÎNEMENT',
      getTitle: () => p.daysTo ? `J-${p.daysTo} avant ${eventName}` : 'Saison en cours',
      getDesc: () => p.daysTo
        ? `Programme training complet. ${p.daysTo > 14 ? 'Volume et intensité maximaux.' : 'Début de réduction progressive dans quelques jours.'} Nutrition : 2 800–3 200 kcal/j · 100% GF.`
        : 'Maintien de la condition physique entre les saisons.',
      getChips: () => `<span class="phase-chip" style="background:rgba(0,176,255,.1);border-color:rgba(0,176,255,.3);color:var(--blue);">💪 4–5 séances/sem</span><span class="phase-chip" style="background:rgba(0,230,118,.1);border-color:rgba(0,230,118,.3);color:var(--green);">🥗 2 800–3 200 kcal/j</span>${p.daysTo ? `<span class="phase-chip" style="background:rgba(255,193,7,.1);border-color:rgba(255,193,7,.3);color:var(--gold);">📅 ${champ} dans ${p.daysTo}j</span>` : ''}`
    },
    taper: {
      label: 'PHASE TAPER — RÉDUCTION DE CHARGE',
      getTitle: () => `J-${p.daysTo} — ${eventName}`,
      getDesc: () => `Réduire le volume d'entraînement de 40–50%. Maintenir l'intensité, baisser la durée. Corps frais = performance maximale. Privilégier sommeil +9h/nuit.`,
      getChips: () => `<span class="phase-chip" style="background:rgba(255,193,7,.1);border-color:rgba(255,193,7,.3);color:var(--gold);">⬇️ Volume –40%</span><span class="phase-chip" style="background:rgba(0,230,118,.1);border-color:rgba(0,230,118,.3);color:var(--green);">😴 Sommeil +9h priorité</span><span class="phase-chip" style="background:rgba(232,0,29,.1);border-color:rgba(232,0,29,.3);color:var(--red);">🏁 Course dans ${p.daysTo}j</span>`
    },
    prerace: {
      label: 'PHASE PRÉ-COURSE — CARB LOADING',
      getTitle: () => `J-${p.daysTo} — ${eventName}`,
      getDesc: () => p.daysTo <= 1
        ? `JOUR J ${p.daysTo === 1 ? 'DEMAIN' : "AUJOURD'HUI"}. Repas pré-course : riz blanc + œufs + banane. 750ml eau + électrolytes. Aucun gras ni fibres.`
        : `Carb loading 70% glucides. Riz blanc exclusif, pomme de terre, quinoa. Réduire fibres progressivement. Sodium-loading J-1.`,
      getChips: () => `<span class="phase-chip" style="background:rgba(232,0,29,.1);border-color:rgba(232,0,29,.3);color:var(--red);">🏎️ ${p.daysTo === 0 ? 'COURSE AUJOURD\'HUI' : `J-${p.daysTo}`}</span><span class="phase-chip" style="background:rgba(255,193,7,.1);border-color:rgba(255,193,7,.3);color:var(--gold);">🍚 Carb loading 70%</span><span class="phase-chip" style="background:rgba(0,230,118,.1);border-color:rgba(0,230,118,.3);color:var(--green);">💧 Sodium-loading J-1</span>`
    },
    race: {
      label: p.event && p.event.type === 'test' ? 'ESSAIS / TEST' : 'COURSE EN COURS 🏎️',
      getTitle: () => `${eventName}`,
      getDesc: () => p.event && p.event.type === 'test'
        ? `Journée d'essais. Hydratation 3–4L. Suppléments normaux. Focus sur les réglages et la performance.`
        : `Course en cours ! 60–90g glucides/heure. 500–800ml eau/heure selon température cockpit. Électrolytes obligatoires.`,
      getChips: () => `<span class="phase-chip" style="background:rgba(232,0,29,.1);border-color:rgba(232,0,29,.3);color:var(--red);">🏎️ ${champ}</span><span class="phase-chip" style="background:rgba(255,193,7,.1);border-color:rgba(255,193,7,.3);color:var(--gold);">⚡ 60–90g glucides/h</span><span class="phase-chip" style="background:rgba(0,176,255,.1);border-color:rgba(0,176,255,.3);color:var(--blue);">💧 800ml–1,2L/h</span>`
    },
    recovery: {
      label: 'PHASE RÉCUPÉRATION',
      getTitle: () => `J+${p.daysAfter} — Post ${p.justFinished ? p.justFinished.event : 'Course'}`,
      getDesc: () => p.daysAfter <= 1
        ? `Fenêtre anabolique prioritaire. Shake récup GF immédiat. Anti-inflammatoires naturels. Sommeil 9–10h. Surveiller HRV et poids.`
        : `Retour progressif à l'alimentation normale. Maintenir hydratation 4L/j. Éviter alcool 72h. Fruits rouges à chaque repas.`,
      getChips: () => `<span class="phase-chip" style="background:rgba(0,230,118,.1);border-color:rgba(0,230,118,.3);color:var(--green);">✓ J+${p.daysAfter} récupération</span><span class="phase-chip" style="background:rgba(0,176,255,.1);border-color:rgba(0,176,255,.3);color:var(--blue);">💧 4L/j hydratation</span><span class="phase-chip" style="background:rgba(206,147,216,.1);border-color:rgba(206,147,216,.3);color:var(--purple);">😴 Sommeil 9–10h</span>`
    },
    jetlag: {
      label: 'ALERTE JET LAG — LONG HAUL',
      getTitle: () => `${jetlagInfo ? jetlagInfo.flag : ''} ${eventName} — J-${p.daysTo}`,
      getDesc: () => `Prochain déplacement long-courrier (${jetlagInfo ? jetlagInfo.offset : ''}, niveau ${jetlagInfo ? jetlagInfo.severity : ''}). Commencer le protocole jet lag dès maintenant : mélatonine, ashwagandha, synchronisation lumière/alimentation.`,
      getChips: () => `<span class="phase-chip" style="background:rgba(206,147,216,.1);border-color:rgba(206,147,216,.3);color:var(--purple);">✈️ Décalage ${jetlagInfo ? jetlagInfo.offset : ''}</span><span class="phase-chip" style="background:rgba(232,0,29,.1);border-color:rgba(232,0,29,.3);color:var(--red);">⚠️ ${jetlagInfo ? jetlagInfo.severity : ''}</span><span class="phase-chip" style="background:rgba(255,193,7,.1);border-color:rgba(255,193,7,.3);color:var(--gold);">🌙 Mélatonine ce soir</span>`
    }
  };

  const info = phases[p.phase];
  label.textContent = info.label;
  title.textContent = info.getTitle();
  desc.textContent = info.getDesc();
  meta.innerHTML = info.getChips();

  // Stats row
  document.getElementById('stat-phase').textContent = {
    training: 'TRAINING', taper: 'TAPER', prerace: 'PRÉ-COURSE',
    race: 'COURSE', recovery: 'RÉCUP', jetlag: 'JET LAG'
  }[p.phase];

  const nextRace = CALENDAR_2026.filter(e => e.type === 'race' && e.dateStart > dateStr(getToday()))[0];
  document.getElementById('stat-nextrace').textContent = nextRace ? nextRace.event.replace('Francorchamps','SPA').substring(0,16) : '—';
  document.getElementById('stat-daysto').textContent = nextRace ? diffDays(getToday(), new Date(nextRace.dateStart)) + 'J' : '—';

  // Jet lag stat
  const nextLH = CALENDAR_2026.filter(e => LONG_HAUL.includes(e.country) && e.dateStart > dateStr(getToday()))[0];
  if (nextLH && JETLAG_INFO[nextLH.country]) {
    document.getElementById('stat-jetlag').textContent = JETLAG_INFO[nextLH.country].offset;
  } else {
    document.getElementById('stat-jetlag').textContent = '—';
  }

  // Hydratation objectif
  const hydraTargets = { training: '3,5 L/j training', taper: '3,5 L/j · Réduire 2j avant', prerace: '4–5 L/j + sodium-loading', race: '4–5 L/j · 800ml–1,2L/h cockpit', recovery: '4 L/j · Anti-inflammatoire', jetlag: '3,5 L/j + vol : 300ml/h' };
  document.getElementById('dash-hydra-target').textContent = 'Objectif : ' + (hydraTargets[p.phase] || '3,5 L/j');

  // Contenu nutrition dashboard
  updateDashNutrition(p);

  // Contenu training dashboard
  updateDashTraining(p);

  // Contenu suppléments dashboard
  updateDashSupps(p);

  // Checklists
  updateDashChecklist(p);

  // Alerte jet lag
  updateJetlagAlert(p);

  // Alert dans les onglets nutrition/training/supplements
  updatePageAlerts(p);
}

function updateDashNutrition(p) {
  const el = document.getElementById('dash-nutrition-content');
  const content = {
    training: `<div class="meal-card"><div class="meal-time">07:00</div><div class="meal-content"><div class="meal-name">Petit-déjeuner performance</div><div class="meal-desc">Porridge riz/quinoa + fruits rouges · 2–3 œufs · Avocat · Pain GF grillé</div></div><div class="meal-macros"><div class="macro-kcal">650</div><div>kcal</div></div></div><div class="meal-card"><div class="meal-time">13:00</div><div class="meal-content"><div class="meal-name">Déjeuner carb-focus</div><div class="meal-desc">Riz basmati 200g + saumon/poulet 150g + légumes vapeur · Tamari GF</div></div><div class="meal-macros"><div class="macro-kcal">720</div><div>kcal</div></div></div><div class="meal-card"><div class="meal-time">19:30</div><div class="meal-content"><div class="meal-name">Dîner protéines & légumes</div><div class="meal-desc">Bœuf ou thon + patate douce + brocolis + quinoa · Tisane récup</div></div><div class="meal-macros"><div class="macro-kcal">610</div><div>kcal</div></div></div>`,
    taper: `<div class="alert gold"><div class="alert-title">⬇️ Réduction de charge alimentaire</div>Maintenir les mêmes aliments GF, légèrement réduire les quantités. Éviter les aliments nouveaux ou fermentés.</div><div class="meal-card"><div class="meal-time">07:00</div><div class="meal-content"><div class="meal-name">Petit-déjeuner normal GF</div><div class="meal-desc">Porridge riz + œufs + banane · Rester sur les habitudes</div></div></div><div class="meal-card"><div class="meal-time">13:00</div><div class="meal-content"><div class="meal-name">Déjeuner carb modéré</div><div class="meal-desc">Riz blanc 150g + poulet 150g + légumes vapeur · Pas d'épices nouvelles</div></div></div><div class="meal-card"><div class="meal-time">19:30</div><div class="meal-content"><div class="meal-name">Dîner léger GF</div><div class="meal-desc">Riz blanc + protéine · Pas de légumineuses · Coucher tôt</div></div></div>`,
    prerace: `<div class="alert red"><div class="alert-title">🍚 Carb Loading 70% glucides</div>Riz blanc exclusif aujourd'hui. Zéro légumineuses, zéro lactose en excès. Réduire fibres.</div><div class="meal-card"><div class="meal-time">07:00</div><div class="meal-content"><div class="meal-name">Petit-déjeuner carb-loading</div><div class="meal-desc">Porridge riz blanc + confiture + pain GF · Jus d'orange · 2 œufs max</div></div><div class="meal-macros"><div class="macro-kcal">700</div><div>kcal</div></div></div><div class="meal-card"><div class="meal-time">12:00</div><div class="meal-content"><div class="meal-name">Déjeuner : riz blanc massif</div><div class="meal-desc">Riz blanc 300g + poulet vapeur + huile d'olive · Aucune sauce ni épice</div></div><div class="meal-macros"><div class="macro-kcal">850</div><div>kcal</div></div></div><div class="meal-card"><div class="meal-time">19:00</div><div class="meal-content"><div class="meal-name">Dîner de confirmation (≤19h)</div><div class="meal-desc">Riz blanc + poulet vapeur + huile d'olive · Pas d'aliment nouveau</div></div><div class="meal-macros"><div class="macro-kcal">680</div><div>kcal</div></div></div>`,
    race: `<div class="alert red"><div class="alert-title">🏎️ Protocole cockpit actif</div>60–90g glucides/heure · 800ml–1,2L eau/heure selon température.</div><div class="meal-card"><div class="meal-time">H-3</div><div class="meal-content"><div class="meal-name">Repas pré-course GF</div><div class="meal-desc">Riz blanc 200g + 2 œufs + banane + pain GF grillé · 750ml eau + électrolytes</div></div></div><div class="meal-card"><div class="meal-time">EN COURSE</div><div class="meal-content"><div class="meal-name">Gels GF toutes les 45 min</div><div class="meal-desc">Maurten 100 ou SiS Beta Fuel · Électrolytes + sel continus</div></div></div><div class="meal-card"><div class="meal-time">PIT STOP</div><div class="meal-content"><div class="meal-name">Ravitaillement complet</div><div class="meal-desc">500ml eau + électrolytes · Banane · 2 gélules de sel · Gel caféiné si nuit</div></div></div>`,
    recovery: `<div class="alert green"><div class="alert-title">✓ Fenêtre anabolique — Agir maintenant</div>0–30 min post-course = fenêtre critique. Anti-inflammatoires naturels toute la journée.</div><div class="meal-card"><div class="meal-time">IMMÉDIAT</div><div class="meal-content"><div class="meal-name">🥤 Shake récupération immédiate GF</div><div class="meal-desc">30g whey GF + banane + 200ml lait de coco + miel + électrolytes · 1g sel rose</div></div><div class="meal-macros"><div class="macro-kcal">420</div><div>kcal</div></div></div><div class="meal-card"><div class="meal-time">1–2h</div><div class="meal-content"><div class="meal-name">🍣 Repas anti-inflammatoire</div><div class="meal-desc">Saumon sauvage 180g + riz basmati + brocolis · 250ml jus cerise Montmorency</div></div><div class="meal-macros"><div class="macro-kcal">680</div><div>kcal</div></div></div>`,
    jetlag: `<div class="alert purple"><div class="alert-title">✈️ Nutrition Jet Lag — Commencer dès maintenant</div>Manger selon l'heure de destination dès J-3 du départ. Réduire glucides simples. Pas d'alcool 48h avant le vol.</div><div class="meal-card"><div class="meal-time">07:00</div><div class="meal-content"><div class="meal-name">Petit-déjeuner léger GF</div><div class="meal-desc">Œufs + légumes + avocat · Pas de céréales lourdes · Exposer au soleil 20 min</div></div></div><div class="meal-card"><div class="meal-time">13:00</div><div class="meal-content"><div class="meal-name">Déjeuner protéiné</div><div class="meal-desc">Poulet/saumon + légumes vapeur + riz · Pas d'alcool · Eau 3L/j</div></div></div><div class="meal-card"><div class="meal-time">19:30</div><div class="meal-content"><div class="meal-name">Dîner tôt (avant 19h)</div><div class="meal-desc">Dîner léger GF · Mélatonine 0,5mg 30 min avant sommeil · Limiter la lumière bleue</div></div></div>`
  };
  el.innerHTML = content[p.phase] || content.training;
}

function updateDashTraining(p) {
  const el = document.getElementById('dash-training-content');
  const content = {
    training: `<div class="exercise-item"><div class="ex-info"><div class="ex-name">Programme complet du jour</div><div class="ex-detail">Selon le jour de la semaine — voir onglet Entraînement</div></div></div><div class="alert blue"><div class="alert-title">💪 Aujourd'hui</div>Nuque + Core + Cardio Zone 2 selon planning semaine. 4–5 séances/semaine. Volume et intensité maximaux.</div>`,
    taper: `<div class="alert gold"><div class="alert-title">⬇️ Taper — Réduction de charge</div>Volume –40–50%. Maintenir intensité, baisser durée. Le corps doit être frais pour la course.</div><div class="exercise-item"><div class="ex-info"><div class="ex-name">Séance légère nuque</div><div class="ex-detail">2×10 reps · Charge légère · Activation seulement</div></div></div><div class="exercise-item"><div class="ex-info"><div class="ex-name">Mobilité & étirements</div><div class="ex-detail">20–30 min yoga/mobilité · Aucun effort musculaire intense</div></div></div><div class="exercise-item"><div class="ex-info"><div class="ex-name">Marche active 30 min</div><div class="ex-detail">FC &lt; 120 bpm · Air frais · Reconnaissance circuit si possible</div></div></div>`,
    prerace: `<div class="alert red"><div class="alert-title">🏁 J-${p.daysTo} — Repos quasi-complet</div>Zéro effort intense. Visualisation mentale. Sommeil +9h priorité absolue.</div><div class="exercise-item"><div class="ex-info"><div class="ex-name">Étirements légers 10 min</div><div class="ex-detail">Nuque, épaules, hanches · Pas de stretch intense</div></div></div><div class="exercise-item"><div class="ex-info"><div class="ex-name">Visualisation mentale</div><div class="ex-detail">15 min · Ferme les yeux · Conduis le circuit intégralement</div></div></div><div class="exercise-item"><div class="ex-info"><div class="ex-name">Marche courte</div><div class="ex-detail">15–20 min max · Reconnaître l'environnement · Calme</div></div></div>`,
    race: `<div class="alert red"><div class="alert-title">🏎️ JOUR DE COURSE — Protocole inter-relais</div>Mobilité légère uniquement entre les relais. Récupération active prioritaire.</div><div class="exercise-item"><div class="ex-info"><div class="ex-name">Échauffement nuque pré-relais</div><div class="ex-detail">5 min · Rotations cervicales · Isométrie 4 directions</div></div></div><div class="exercise-item"><div class="ex-info"><div class="ex-name">Étirements inter-relais</div><div class="ex-detail">Hip flexor, épaules, nuque · 5 min max · Récup, pas effort</div></div></div><div class="exercise-item"><div class="ex-info"><div class="ex-name">Respiration 4-7-8 pré-relais</div><div class="ex-detail">3–4 cycles · Réduit cortisol · Focus cockpit</div></div></div>`,
    recovery: `<div class="alert green"><div class="alert-title">✓ Récupération active — Pas d'effort intense</div>J+1 : natation douce 20–30 min. J+2–3 : retour progressif. Surveiller HRV chaque matin.</div><div class="exercise-item"><div class="ex-info"><div class="ex-name">Natation douce (si J+1)</div><div class="ex-detail">20–30 min · Crawl léger · Récupération active parfaite</div></div></div><div class="exercise-item"><div class="ex-info"><div class="ex-name">Mobilité & étirements</div><div class="ex-detail">Windshield Wiper · Pigeon Pose · Thread the Needle · Post-course obligatoire</div></div></div><div class="exercise-item"><div class="ex-info"><div class="ex-name">Massage (si J+1 ou +)</div><div class="ex-detail">Pas immédiatement post-course · Drainage lymphatique · Bain froid 10–15°C</div></div></div>`,
    jetlag: `<div class="alert purple"><div class="alert-title">✈️ Préparation physique voyage</div>Séances modérées pour ne pas arriver fatigué. Bain froid pour réinitialiser le système nerveux.</div><div class="exercise-item"><div class="ex-info"><div class="ex-name">Cardio Zone 2 léger</div><div class="ex-detail">30–40 min · Vélo ou natation · FC &lt; 140 bpm</div></div></div><div class="exercise-item"><div class="ex-info"><div class="ex-name">Nuque maintenance</div><div class="ex-detail">2×10 reps · Maintien uniquement</div></div></div><div class="exercise-item"><div class="ex-info"><div class="ex-name">Exposition solaire matin</div><div class="ex-detail">20 min après le réveil · Synchro horloge biologique pré-voyage</div></div></div>`
  };
  el.innerHTML = content[p.phase] || content.training;
}

function updateDashSupps(p) {
  const el = document.getElementById('dash-supps-content');
  const content = {
    training: `<div class="supp-card"><div class="supp-dot" style="background:var(--gold)"></div><div class="supp-info"><div class="supp-name">🌅 Matin : Stack de base</div><div class="supp-dose">Oméga-3 3g · D3+K2 · Magnésium 300mg · Vit C 500mg</div></div></div><div class="supp-card"><div class="supp-dot" style="background:var(--red)"></div><div class="supp-info"><div class="supp-name">⚡ Pré-séance : Créatine + Caféine</div><div class="supp-dose">Créatine 5g · Caféine 100mg + L-Théanine 100mg</div></div></div><div class="supp-card"><div class="supp-dot" style="background:var(--green)"></div><div class="supp-info"><div class="supp-name">🌙 Soir : Récupération</div><div class="supp-dose">Magnésium Glycinate 300mg · L-Théanine 200mg · Probiotiques</div></div></div>`,
    taper: `<div class="supp-card"><div class="supp-dot" style="background:var(--gold)"></div><div class="supp-info"><div class="supp-name">🌅 Matin : Stack de base maintenu</div><div class="supp-dose">Oméga-3 3g · D3+K2 · Magnésium · Vit C</div></div></div><div class="supp-card"><div class="supp-dot" style="background:var(--red)"></div><div class="supp-info"><div class="supp-name">⚡ Créatine continue</div><div class="supp-dose">Créatine 5g/j en continu · Arrêter Bêta-Alanine</div></div></div><div class="supp-card"><div class="supp-dot" style="background:var(--green)"></div><div class="supp-info"><div class="supp-name">🌙 Soir : Optimiser le sommeil</div><div class="supp-dose">Magnésium Glycinate 400mg · L-Théanine 200mg · Curcumine 1g</div></div></div>`,
    prerace: `<div class="alert red"><div class="alert-title">🏁 Suppléments pré-course</div>Seulement les produits testés et validés. Aucun nouveau supplément.</div><div class="supp-card"><div class="supp-dot" style="background:var(--gold)"></div><div class="supp-info"><div class="supp-name">🌅 Matin : Stack allégé</div><div class="supp-dose">Oméga-3 2g · Magnésium · Pas de nouveaux produits</div></div></div><div class="supp-card"><div class="supp-dot" style="background:var(--blue)"></div><div class="supp-info"><div class="supp-name">💧 Sodium-loading (J-1)</div><div class="supp-dose">Électrolytes + 1–2g sel rose · Retenir les fluides</div></div></div><div class="supp-card"><div class="supp-dot" style="background:var(--green)"></div><div class="supp-info"><div class="supp-name">🌙 Soir : Sommeil optimisé</div><div class="supp-dose">Magnésium Glycinate 400mg · L-Théanine 200mg · Coucher 22h max</div></div></div>`,
    race: `<div class="alert red"><div class="alert-title">🏎️ Kit cockpit actif</div>Gels GF toutes les 45 min. Électrolytes en continu. Caféine planifiée.</div><div class="supp-card"><div class="supp-dot" style="background:var(--gold)"></div><div class="supp-info"><div class="supp-name">En cockpit : Gels glucidiques GF</div><div class="supp-dose">Maurten 100 / SiS Beta Fuel · 1 gel / 45 min</div></div></div><div class="supp-card"><div class="supp-dot" style="background:var(--blue)"></div><div class="supp-info"><div class="supp-name">Électrolytes + SaltStick</div><div class="supp-dose">1 comprimé/h · 1–2 gélules sel/h si chaleur intense</div></div></div><div class="supp-card"><div class="supp-dot" style="background:var(--orange)"></div><div class="supp-info"><div class="supp-name">Caféine stratégique</div><div class="supp-dose">75–100mg max 3–4 fois/24h · Planifier aux creux de vigilance</div></div></div>`,
    recovery: `<div class="alert green"><div class="alert-title">✓ Protocole récupération actif</div>Anti-inflammatoires naturels en priorité. Microbiote à réparer.</div><div class="supp-card"><div class="supp-dot" style="background:var(--red)"></div><div class="supp-info"><div class="supp-name">🍒 Immédiat : Cerise Montmorency</div><div class="supp-dose">60ml concentré dans eau · Anti-inflammatoire + mélatonine naturelle</div></div></div><div class="supp-card"><div class="supp-dot" style="background:var(--gold)"></div><div class="supp-info"><div class="supp-name">Oméga-3 dose haute</div><div class="supp-dose">3g EPA+DHA · Curcumine 1g + Pipérine 10mg</div></div></div><div class="supp-card"><div class="supp-dot" style="background:var(--purple)"></div><div class="supp-info"><div class="supp-name">Probiotiques renforcés (double dose)</div><div class="supp-dose">20–30 milliards UFC · 2–3 jours · Réparer le microbiote</div></div></div>`,
    jetlag: `<div class="alert purple"><div class="alert-title">✈️ Protocole Jet Lag — Commencer maintenant</div>Ne pas attendre l'arrivée. Commencer 2–3 jours avant.</div><div class="supp-card"><div class="supp-dot" style="background:var(--purple)"></div><div class="supp-info"><div class="supp-name">🌙 Mélatonine 0,5mg</div><div class="supp-dose">30 min avant coucher · Heure locale destination · Pas le matin !</div></div></div><div class="supp-card"><div class="supp-dot" style="background:var(--red)"></div><div class="supp-info"><div class="supp-name">Ashwagandha KSM-66</div><div class="supp-dose">300–600mg/j · Régule le cortisol · Commence dès maintenant</div></div></div><div class="supp-card"><div class="supp-dot" style="background:var(--gold)"></div><div class="supp-info"><div class="supp-name">Magnésium + L-Théanine (soir)</div><div class="supp-dose">400mg Mg + 200mg L-Théanine · 1h avant coucher local</div></div></div>`
  };
  el.innerHTML = content[p.phase] || content.training;
}

function updateDashChecklist(p) {
  const physItems = {
    training: ['Séance core 25 min', 'Renforcement nuque (3×15 reps)', 'Cardio zone 2 – 30 min', 'Étirements & mobilité 15 min', 'Grip training (mains & avant-bras)'],
    taper: ['Nuque légère 2×10 reps', 'Mobilité 20 min', 'Marche active 30 min', 'HRV mesuré ce matin', 'Sommeil +8h prévu'],
    prerace: ['Étirements légers 10 min', 'Visualisation mentale 15 min', 'Marche courte (15 min)', 'Pas d\'effort intense', 'Sommeil 22h max'],
    race: ['Échauffement nuque pré-relais', 'Respiration 4-7-8 × 3 cycles', 'Étirements inter-relais (5 min)', 'Hydratation cockpit vérifiée', 'Récupération active entre relais'],
    recovery: ['Natation douce (si J+1)', 'Bain froid 10–15°C (dans 2h post-course)', 'Massage drainage (J+1, pas immédiat)', 'HRV mesuré ce matin', 'Étirements doux 10 min'],
    jetlag: ['Cardio Zone 2 léger 30 min', 'Nuque maintenance 2×10', 'Exposition solaire 20 min', 'HRV mesuré ce matin', 'Bain froid (reset système nerveux)']
  };
  const nutItems = {
    training: ['Petit-déj : riz + œufs + avocat', 'Snack pré-séance GF', 'Déjeuner : riz/pomme de terre + protéine', 'Suppléments matin pris', 'Suppléments soir pris', '3,5L eau atteints'],
    taper: ['Petit-déj GF habituel (pas de nouveauté)', 'Riz blanc + poulet le midi', 'Dîner léger (≤ 19h30)', 'Suppléments de base maintenus', 'Pas d\'aliment nouveau', '3,5L eau atteints'],
    prerace: ['Carb loading 70% glucides', 'Riz blanc exclusif', 'Zéro légumineuses', 'Sodium-loading électrolytes', 'Suppléments validés seulement', '4–5L eau atteints'],
    race: ['Repas pré-course H-3 GF', 'Gel GF H-1 + 300ml eau', 'Gels cockpit toutes les 45 min', 'Électrolytes continus', 'Banane à chaque pit stop', 'Shake récup post-arrivée'],
    recovery: ['Shake récup immédiat (0–30 min)', 'Jus cerise Montmorency 60ml', 'Repas anti-inflammatoire 1–2h', 'Oméga-3 dose haute (3g)', 'Probiotiques double dose', '4L eau/j maintenu'],
    jetlag: ['Repas selon heure destination', 'Pas d\'alcool 48h avant vol', 'Mélatonine 0,5mg ce soir', 'Électrolytes + hydratation 3,5L', 'Suppléments Ashwagandha', 'Exposition solaire matin faite']
  };

  const phys = physItems[p.phase] || physItems.training;
  const nut = nutItems[p.phase] || nutItems.training;

  document.getElementById('dash-checklist-physical-items').innerHTML =
    phys.map(i => `<div class="checklist-item" onclick="toggleCheck(this)"><div class="check-box"></div><span class="check-label">${i}</span></div>`).join('');
  document.getElementById('dash-checklist-nutrition-items').innerHTML =
    nut.map(i => `<div class="checklist-item" onclick="toggleCheck(this)"><div class="check-box"></div><span class="check-label">${i}</span></div>`).join('');
}

function updateJetlagAlert(p) {
  const el = document.getElementById('dash-jetlag-alert');
  const nextLH = CALENDAR_2026.filter(e => LONG_HAUL.includes(e.country) && e.dateStart > dateStr(getToday())).sort((a,b)=>a.dateStart.localeCompare(b.dateStart))[0];

  if (nextLH) {
    const ji = JETLAG_INFO[nextLH.country];
    const days = diffDays(getToday(), new Date(nextLH.dateStart));
    if (days <= 14) {
      el.style.display = 'block';
      el.innerHTML = `<div class="alert purple"><div class="alert-title">✈️ LONG HAUL DANS ${days} JOURS — ${nextLH.event}</div>Destination : ${nextLH.location} ${ji ? `(Décalage ${ji.offset}, niveau ${ji.severity})` : ''}. Commencer mélatonine + ashwagandha dès maintenant. Aller dans l'onglet Voyage pour le protocole complet.</div>`;
    } else {
      el.style.display = 'none';
    }
  } else {
    el.style.display = 'none';
  }
}

function updatePageAlerts(p) {
  const phaseNames = { training: 'Entraînement standard', taper: 'Taper — réduction de charge', prerace: 'Pré-course — carb loading', race: 'Course en cours', recovery: 'Récupération post-course', jetlag: 'Protocole jet lag actif' };
  const colors = { training: 'blue', taper: 'gold', prerace: 'red', race: 'red', recovery: 'green', jetlag: 'purple' };

  const name = phaseNames[p.phase] || 'Entraînement';
  const color = colors[p.phase] || 'blue';
  const msg = p.event ? ` — ${p.event.event} dans ${p.daysTo}j` : '';

  const nuAlert = document.getElementById('nutri-phase-alert');
  if (nuAlert) { nuAlert.className = `alert ${color}`; nuAlert.innerHTML = `<div class="alert-title">Phase actuelle : ${name}${msg}</div>Protocole nutritionnel adapté automatiquement selon ton calendrier.`; }

  const suppAlert = document.getElementById('supp-phase-alert');
  if (suppAlert) { suppAlert.className = `alert ${color}`; suppAlert.innerHTML = `<div class="alert-title">Phase actuelle : ${name}${msg}</div>Stack de suppléments adapté à ta phase de performance.`; }

  const trainAlert = document.getElementById('training-phase-alert');
  if (trainAlert) { trainAlert.className = `alert ${color}`; trainAlert.innerHTML = `<div class="alert-title">Phase actuelle : ${name}${msg}</div>Programme d'entraînement adapté. ${p.phase === 'taper' ? 'Volume –40%. Repos priorité.' : p.phase === 'race' ? 'Protocole inter-relais actif.' : p.phase === 'recovery' ? 'Récupération active uniquement.' : 'Programme complet actif.'}`; }

  // Travel alert
  const nextLH = CALENDAR_2026.filter(e => LONG_HAUL.includes(e.country) && e.dateStart > dateStr(getToday())).sort((a,b)=>a.dateStart.localeCompare(b.dateStart))[0];
  const travelAlert = document.getElementById('travel-next-alert');
  if (travelAlert && nextLH) {
    const ji = JETLAG_INFO[nextLH.country];
    const days = diffDays(getToday(), new Date(nextLH.dateStart));
    travelAlert.innerHTML = `<div class="alert ${ji && ji.severity === 'CRITIQUE' ? 'red' : ji && ji.severity === 'ÉLEVÉ' ? 'gold' : 'purple'}"><div class="alert-title">✈️ Prochain voyage long-courrier : ${nextLH.event}</div>${nextLH.location} · Dans ${days} jours · ${ji ? `Décalage ${ji.offset} · Niveau ${ji.severity}` : ''}</div>`;
  }
}

// ============================================================
// CALENDRIER UI
// ============================================================
let calCurrentDate = new Date();

function renderCalendar() {
  const year = calCurrentDate.getFullYear();
  const month = calCurrentDate.getMonth();

  document.getElementById('cal-month-title').textContent =
    calCurrentDate.toLocaleDateString('fr-FR', { month: 'long', year: 'numeric' });

  const header = document.getElementById('cal-header');
  const body = document.getElementById('cal-body');

  const days = ['LUN', 'MAR', 'MER', 'JEU', 'VEN', 'SAM', 'DIM'];
  header.innerHTML = days.map(d => `<div class="cal-header-cell">${d}</div>`).join('');

  const firstDay = new Date(year, month, 1);
  const lastDay = new Date(year, month + 1, 0);
  const startDow = (firstDay.getDay() + 6) % 7; // Monday = 0

  let cells = '';
  const today = dateStr(new Date());

  // Padding before
  for (let i = 0; i < startDow; i++) {
    const d = new Date(year, month, 1 - startDow + i);
    cells += `<div class="cal-day other-month"><div class="cal-day-num">${d.getDate()}</div></div>`;
  }

  for (let day = 1; day <= lastDay.getDate(); day++) {
    const d = new Date(year, month, day);
    const ds = dateStr(d);
    const isToday = ds === today;

    const events = CALENDAR_2026.filter(e => ds >= e.dateStart && ds <= e.dateEnd);
    const evHtml = events.map(e => `<div class="cal-event ${e.championship.toLowerCase().replace('-','')} ${e.type === 'test' ? 'test' : ''}" onclick="showEventDetail(${e.id})">${e.championship}</div>`).join('');

    cells += `<div class="cal-day${isToday ? ' today' : ''}" onclick="showDayDetail('${ds}')">
      <div class="cal-day-num">${day}</div>
      ${evHtml}
    </div>`;
  }

  // Padding after
  const remaining = (7 - (startDow + lastDay.getDate()) % 7) % 7;
  for (let i = 1; i <= remaining; i++) {
    cells += `<div class="cal-day other-month"><div class="cal-day-num">${i}</div></div>`;
  }

  body.innerHTML = cells;

  // Event list
  renderEventList(year, month);
  renderLongHaulList();
}

function renderEventList(year, month) {
  const monthStart = `${year}-${String(month+1).padStart(2,'0')}-01`;
  const monthEnd = `${year}-${String(month+1).padStart(2,'0')}-31`;

  const events = CALENDAR_2026.filter(e =>
    (e.dateStart >= monthStart && e.dateStart <= monthEnd) ||
    (e.dateEnd >= monthStart && e.dateEnd <= monthEnd)
  );

  const el = document.getElementById('cal-event-list');
  if (!events.length) { el.innerHTML = '<div class="alert blue"><div class="alert-title">Aucun événement ce mois</div></div>'; return; }

  el.innerHTML = events.map(e => {
    const ji = JETLAG_INFO[e.country];
    const isLH = LONG_HAUL.includes(e.country);
    const champClass = e.championship.toLowerCase().replace('-','');
    return `<div class="event-detail-card" onclick="showEventDetail(${e.id})" style="cursor:pointer;">
      <span class="event-champ-badge cal-event ${champClass}">${e.championship}</span>
      ${e.type === 'test' ? '<span class="tag tag-blue" style="margin-left:.5rem;">TEST</span>' : ''}
      ${isLH ? `<span class="tag tag-purple" style="margin-left:.5rem;">✈️ LONG HAUL</span>` : ''}
      ${e.duration === 24 ? '<span class="tag tag-red" style="margin-left:.5rem;">24H</span>' : ''}
      <div style="font-family:\'Barlow Condensed\';font-weight:900;font-size:1.1rem;color:#fff;margin:.4rem 0;">${e.event}</div>
      <div style="font-size:.8rem;color:var(--muted);">${e.location} · ${e.dateStart} → ${e.dateEnd}</div>
      ${ji ? `<div style="font-size:.75rem;color:var(--purple);margin-top:.3rem;">✈️ Décalage ${ji.offset} · Jet lag niveau ${ji.severity}</div>` : ''}
    </div>`;
  }).join('');
}

function renderLongHaulList() {
  const today = dateStr(new Date());
  const upcoming = CALENDAR_2026.filter(e => LONG_HAUL.includes(e.country) && e.dateStart >= today).slice(0, 6);
  const el = document.getElementById('cal-longhaul-list');
  el.innerHTML = upcoming.map(e => {
    const ji = JETLAG_INFO[e.country] || {};
    const days = diffDays(new Date(), new Date(e.dateStart));
    return `<div class="event-detail-card">
      <div style="display:flex;justify-content:space-between;align-items:center;">
        <div>
          <span class="tag tag-purple">✈️ ${ji.flag || ''} ${ji.offset || ''}</span>
          <div style="font-family:\'Barlow Condensed\';font-weight:700;font-size:1rem;color:#fff;margin:.4rem 0;">${e.event}</div>
          <div style="font-size:.8rem;color:var(--muted);">${e.location} · ${e.dateStart}</div>
        </div>
        <div style="text-align:right;">
          <div style="font-family:\'Barlow Condensed\';font-weight:900;font-size:2rem;color:${days <= 14 ? 'var(--red)' : 'var(--gold)'}">${days}</div>
          <div style="font-size:.65rem;color:var(--muted);">JOURS</div>
          <div style="font-size:.65rem;font-family:\'Share Tech Mono\';color:${ji.severity==='CRITIQUE'?'var(--red)':ji.severity==='ÉLEVÉ'?'var(--gold)':'var(--purple)'};">${ji.severity || ''}</div>
        </div>
      </div>
    </div>`;
  }).join('');
}

function showEventDetail(id) {
  const e = CALENDAR_2026.find(x => x.id === id);
  if (!e) return;
  const el = document.getElementById('cal-selected-event');
  const ji = JETLAG_INFO[e.country];
  const champClass = e.championship.toLowerCase().replace('-','');
  el.style.display = 'block';
  el.innerHTML = `<div class="card" style="border-color:rgba(255,193,7,.3);margin-top:1rem;">
    <div class="card-accent gold"></div>
    <span class="event-champ-badge cal-event ${champClass}">${e.championship}</span>
    <div style="font-family:\'Barlow Condensed\';font-weight:900;font-size:1.5rem;color:#fff;margin:.5rem 0;">${e.event}</div>
    <div style="font-size:.85rem;color:var(--muted);margin-bottom:1rem;">${e.location} · ${e.dateStart} → ${e.dateEnd} ${e.duration ? `· ${e.duration}H` : ''}</div>
    <div class="grid-2">
      <div>
        <div class="alert ${e.type === 'test' ? 'blue' : e.duration === 24 ? 'red' : 'gold'}">
          <div class="alert-title">🏁 Protocole course</div>
          ${e.duration === 24 ? 'Course 24h — Protocole multi-relais complet. Voir onglet Course > 24 heures.' : e.duration ? `Course ${e.duration}h — Protocole cockpit 60–90g glucides/h. Voir onglet Course > 3–6 heures.` : 'Test / Essais — Hydratation 3–4L. Suppléments de base.'}
        </div>
        ${ji ? `<div class="alert purple"><div class="alert-title">✈️ Jet Lag ${ji.flag}</div>Décalage ${ji.offset} · Niveau ${ji.severity}. Commencer mélatonine 2–3 jours avant le départ. Voir onglet Voyage.</div>` : ''}
      </div>
      <div>
        <div class="alert gold"><div class="alert-title">📅 Planning préparation</div>
          J-7 : Dernière séance intense<br>
          J-5 : Cardio léger<br>
          J-3 : ${e.duration ? 'Carb loading GF' : 'Repos + mobilité'}<br>
          J-1 : Repos complet · Sommeil +9h<br>
          ${ji ? `<strong style="color:var(--purple);">Jet lag : commencer protocole maintenant</strong>` : ''}
        </div>
      </div>
    </div>
  </div>`;
  el.scrollIntoView({ behavior: 'smooth', block: 'nearest' });
}

function showDayDetail(ds) {
  const events = CALENDAR_2026.filter(e => ds >= e.dateStart && ds <= e.dateEnd);
  if (!events.length) {
    document.getElementById('cal-selected-event').style.display = 'none';
    return;
  }
  showEventDetail(events[0].id);
}

function changeMonth(dir) {
  calCurrentDate.setMonth(calCurrentDate.getMonth() + dir);
  document.getElementById('cal-selected-event').style.display = 'none';
  renderCalendar();
}

// ============================================================
// NAVIGATION
// ============================================================
function showPage(pageId, btn) {
  document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
  document.querySelectorAll('.nav-tab').forEach(t => t.classList.remove('active'));
  document.getElementById('page-' + pageId).classList.add('active');
  if (btn) btn.classList.add('active');
  else {
    const tabs = document.querySelectorAll('.nav-tab');
    tabs.forEach(t => { if (t.getAttribute('onclick') && t.getAttribute('onclick').includes(pageId)) t.classList.add('active'); });
  }
}

function switchSection(prefix, sectionId, btn) {
  const all = document.querySelectorAll('[id^="' + prefix + '-"]');
  all.forEach(el => el.style.display = 'none');
  const target = document.getElementById(prefix + '-' + sectionId);
  if (target) target.style.display = '';
  btn.parentElement.querySelectorAll('.sel-btn').forEach(b => b.classList.remove('active'));
  btn.classList.add('active');
}

function toggleSection(header) {
  header.parentElement.classList.toggle('open');
}

// ============================================================
// HYDRATATION
// ============================================================
let hydrationCount = 0;
const TOTAL_UNITS = 14;

function initHydration() {
  const bar = document.getElementById('hydrationBar');
  bar.innerHTML = '';
  for (let i = 0; i < TOTAL_UNITS; i++) {
    const unit = document.createElement('div');
    unit.className = 'h-unit' + (i < hydrationCount ? ' filled' : '');
    unit.onclick = () => { hydrationCount = i + 1; updateHydration(); };
    bar.appendChild(unit);
  }
  document.getElementById('hydrationText').textContent = hydrationCount + ' / ' + TOTAL_UNITS + ' verres · 0 ml';
}

function updateHydration() {
  document.querySelectorAll('.h-unit').forEach((u, i) => u.classList.toggle('filled', i < hydrationCount));
  document.getElementById('hydrationText').textContent = hydrationCount + ' / ' + TOTAL_UNITS + ' verres · ' + (hydrationCount * 250) + ' ml';
}

function resetHydration() { hydrationCount = 0; updateHydration(); }

// ============================================================
// WEEK DAYS
// ============================================================
function initWeek() {
  const container = document.getElementById('weekDays');
  if (!container) return;
  const days = ['LUN', 'MAR', 'MER', 'JEU', 'VEN', 'SAM', 'DIM'];
  const today = new Date();
  const todayIdx = (today.getDay() + 6) % 7;
  days.forEach((d, i) => {
    const btn = document.createElement('div');
    btn.className = 'day-btn' + (i === todayIdx ? ' active' : '');
    const date = new Date();
    date.setDate(date.getDate() - todayIdx + i);
    btn.innerHTML = `<span class="day-name">${d}</span><span class="day-num">${date.getDate()}</span>`;
    btn.onclick = () => { document.querySelectorAll('.day-btn').forEach(b => b.classList.remove('active')); btn.classList.add('active'); };
    container.appendChild(btn);
  });
}

// ============================================================
// TIMEZONES
// ============================================================
function updateClocks() {
  function fmt(d) { return d.toLocaleTimeString('fr-FR', { hour: '2-digit', minute: '2-digit', hour12: false }); }
  const now = new Date();
  const tz = (zone) => new Date(now.toLocaleString('en-US', { timeZone: zone }));
  const set = (id, t) => { const el = document.getElementById(id); if (el) el.textContent = fmt(t); };
  set('tz-paris', tz('Europe/Brussels'));
  set('tz-tokyo', tz('Asia/Tokyo'));
  set('tz-ny', tz('America/New_York'));
  set('tz-dubai', tz('Asia/Dubai'));
}

// ============================================================
// CHECKLIST
// ============================================================
function toggleCheck(item) {
  item.classList.toggle('done');
  item.querySelector('.check-box').textContent = item.classList.contains('done') ? '✓' : '';
}

// ============================================================
// INIT
// ============================================================
initHydration();
initWeek();
updateClocks();
updateDashboard();
renderCalendar();
setInterval(updateClocks, 30000);
</script>

<!-- PWA -->

<script>
if ('serviceWorker' in navigator) {
  window.addEventListener('load', () => navigator.serviceWorker.register('./sw.js').catch(() => {}));
}
(function() {
  const isIOS = /iphone|ipad|ipod/i.test(navigator.userAgent);
  const isStandalone = window.navigator.standalone === true;
  const dismissed = sessionStorage.getItem('pwa-banner-dismissed');
  if (isIOS && !isStandalone && !dismissed) {
    const banner = document.createElement('div');
    banner.style.cssText = `position:fixed;bottom:0;left:0;right:0;z-index:9999;background:#1A1A20;border-top:1px solid rgba(232,0,29,0.4);padding:14px 18px 28px;display:flex;align-items:center;gap:14px;font-family:'Barlow',sans-serif;`;
    banner.innerHTML = `<div style="font-size:2rem;">🏎️</div><div style="flex:1;"><div style="font-family:'Barlow Condensed',sans-serif;font-weight:800;font-size:.95rem;letter-spacing:2px;text-transform:uppercase;color:#fff;margin-bottom:3px;">Installer GT PILOT</div><div style="font-size:.75rem;color:#55556A;line-height:1.4;">Appuie sur <strong style="color:#E8001D;">Partager</strong> ⬆️ puis <strong style="color:#E8001D;">"Sur l'écran d'accueil"</strong></div></div><button id="close-banner" style="background:transparent;border:1px solid rgba(255,255,255,.12);color:#55556A;font-size:.75rem;padding:5px 10px;border-radius:3px;cursor:pointer;font-family:'Barlow Condensed';letter-spacing:1px;">FERMER</button>`;
    document.body.appendChild(banner);
    document.getElementById('close-banner').onclick = () => { banner.remove(); sessionStorage.setItem('pwa-banner-dismissed','1'); };
  }
  window.addEventListener('beforeinstallprompt', e => {
    e.preventDefault();
    const btn = document.createElement('button');
    btn.style.cssText = `position:fixed;bottom:20px;right:20px;z-index:9999;background:#E8001D;color:#fff;border:none;border-radius:30px;padding:12px 20px;font-family:'Barlow Condensed',sans-serif;font-weight:700;font-size:.75rem;letter-spacing:2px;text-transform:uppercase;cursor:pointer;box-shadow:0 4px 24px rgba(232,0,29,.4);`;
    btn.textContent = '⬇️ INSTALLER L\'APP';
    btn.onclick = () => { e.prompt(); btn.remove(); };
    document.body.appendChild(btn);
  });
})();
</script>

<style>
@keyframes slideUp { from { transform: translateY(100%); opacity: 0; } to { transform: translateY(0); opacity: 1; } }
body { padding-bottom: env(safe-area-inset-bottom); }
nav { padding-top: env(safe-area-inset-top); height: calc(56px + env(safe-area-inset-top)); }
* { -webkit-tap-highlight-color: transparent; }
button, .nav-tab, .sel-btn, .checklist-item, .toggle-header, .h-unit, .day-btn, .exercise-item, .meal-card { -webkit-touch-callout: none; touch-action: manipulation; }
main { -webkit-overflow-scrolling: touch; }
</style>

</body>
</html>
