<!DOCTYPE html>
<!-- saved from url=(0051)file:///C:/Users/sebas/Downloads/serenum-final.html -->
<html lang="fr"><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">

<meta name="viewport" content="width=device-width,initial-scale=1.0">
<title>Sérénum — Gestion du stress scolaire</title>
<link href="./Sérénum — Accompagnement émotionnel enfants &amp; adolescents_files/css2" rel="stylesheet">
<style>
*{margin:0;padding:0;box-sizing:border-box}
:root{
  --sage:#7A9E7E;--sage-l:#B8D4BB;--sage-d:#4A6B4E;
  --cream:#FAF7F2;--cream-d:#F0EBE1;
  --sand:#C8B89A;--sand-d:#9A8570;
  --teal:#4A8B8C;--teal-l:#A8CCCC;
  --rose:#C47B7B;--rose-l:#E8BBBB;
  --lav:#7B7BAE;--lav-l:#BBBBDD;
  --gold:#C4A24A;--gold-l:#E8D4A0;
  --text:#2C2C2A;--text-m:#666660;--text-l:#999990;
  --white:#FFF;--border:#E0DDD5;
  --r:12px;--rl:20px;--rxl:28px;
}
body{font-family:'DM Sans',sans-serif;background:var(--cream);color:var(--text);min-height:100vh}
h1,h2,h3,h4{font-family:'Cormorant Garamond',serif}
.hidden{display:none!important}
/* BUTTONS */
.btn{padding:11px 26px;border:none;border-radius:50px;cursor:pointer;font-family:'DM Sans',sans-serif;font-size:14px;font-weight:500;transition:all .2s;letter-spacing:.3px;display:inline-flex;align-items:center;gap:6px}
.btn-sage{background:var(--sage);color:#fff}.btn-sage:hover{background:var(--sage-d);transform:translateY(-1px)}
.btn-teal{background:var(--teal);color:#fff}.btn-teal:hover{background:#3a6b6c;transform:translateY(-1px)}
.btn-gold{background:var(--gold);color:#fff}.btn-gold:hover{background:#a8872a;transform:translateY(-1px)}
.btn-rose{background:var(--rose);color:#fff}.btn-rose:hover{background:#a46060;transform:translateY(-1px)}
.btn-out{background:transparent;border:1.5px solid var(--sage);color:var(--sage)}.btn-out:hover{background:var(--sage);color:#fff}
.btn-sm{padding:7px 16px;font-size:13px}
.btn:disabled{opacity:.4;cursor:not-allowed;transform:none!important}
/* NAV */
.nav{position:fixed;top:0;left:0;right:0;z-index:100;background:rgba(250,247,242,.96);backdrop-filter:blur(12px);border-bottom:1px solid var(--border);padding:0 40px;height:64px;display:flex;align-items:center;justify-content:space-between}
.nav-logo{font-family:'Cormorant Garamond',serif;font-size:26px;font-weight:300;color:var(--sage-d);letter-spacing:1px;cursor:pointer}
.nav-logo em{color:var(--sage);font-style:italic}
.nav-links{display:flex;gap:4px;align-items:center}
.nav-link{padding:8px 16px;border-radius:50px;cursor:pointer;font-size:14px;color:var(--text-m);transition:all .2s}
.nav-link:hover,.nav-link.active{background:var(--cream-d);color:var(--text)}
/* PAGES */
.page{display:none;min-height:100vh;padding-top:64px}
.page.active{display:block}
/* HERO */
.hero{padding:80px 40px 60px;max-width:1100px;margin:0 auto;display:grid;grid-template-columns:1fr 1fr;gap:60px;align-items:center}
.hero-tag{font-size:11px;letter-spacing:2.5px;text-transform:uppercase;color:var(--sage);margin-bottom:16px}
.hero-title{font-size:58px;font-weight:300;line-height:1.1;margin-bottom:20px}
.hero-title em{font-style:italic;color:var(--sage)}
.hero-sub{font-size:16px;color:var(--text-m);line-height:1.7;margin-bottom:28px;font-weight:300}
.disclaimer{font-size:12px;color:var(--text-l);line-height:1.6;padding:12px 16px;background:var(--cream-d);border-radius:8px;border-left:3px solid var(--sand)}
.orb{width:280px;height:280px;border-radius:50%;background:radial-gradient(circle,var(--sage-l) 0%,var(--cream-d) 70%);display:flex;align-items:center;justify-content:center;animation:breathe 4s ease-in-out infinite;position:relative;margin:0 auto}
.orb::before{content:'';position:absolute;inset:-20px;border-radius:50%;border:1px solid var(--sage-l);animation:breathe 4s ease-in-out infinite .5s}
.orb-text{font-family:'Cormorant Garamond',serif;font-size:20px;font-weight:300;color:var(--sage-d);text-align:center;font-style:italic}
@keyframes breathe{0%,100%{transform:scale(1)}50%{transform:scale(1.08)}}
/* STATS */
.stats{display:grid;grid-template-columns:repeat(3,1fr);gap:20px;max-width:1100px;margin:0 auto 60px;padding:0 40px}
.stat{background:var(--white);border-radius:var(--r);border:1px solid var(--border);padding:24px;text-align:center}
.stat-n{font-family:'Cormorant Garamond',serif;font-size:42px;font-weight:300;color:var(--sage)}
.stat-l{font-size:13px;color:var(--text-m);line-height:1.5;margin-top:4px}
/* STORY */
.story{max-width:860px;margin:0 auto 72px;padding:0 40px}
.story-inner{position:relative;background:var(--white);border-radius:var(--rxl);border:1px solid var(--border);padding:48px 52px;overflow:hidden}
.story-quote{position:absolute;top:-10px;left:36px;font-family:'Cormorant Garamond',serif;font-size:160px;font-weight:300;color:var(--sage-l);line-height:1;pointer-events:none}
.story-tag{display:inline-block;font-size:11px;letter-spacing:2.5px;text-transform:uppercase;color:var(--sage);border-bottom:1px solid var(--sage-l);padding-bottom:6px;margin-bottom:28px}
/* HOW IT WORKS */
.how{max-width:1100px;margin:0 auto;padding:0 40px 80px}
.how-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:24px}
.how-card{background:var(--white);border-radius:var(--rl);border:1px solid var(--border);padding:28px;text-align:center}
/* OFFRES */
.offres-head{text-align:center;padding:60px 40px 40px;max-width:800px;margin:0 auto}
.offres-grid{display:grid;grid-template-columns:repeat(2,1fr);gap:24px;max-width:1100px;margin:0 auto;padding:0 40px 60px}
.offre-card{background:var(--white);border-radius:var(--rxl);border:1px solid var(--border);overflow:hidden;transition:transform .3s,box-shadow .3s;cursor:pointer}
.offre-card:hover{transform:translateY(-4px);box-shadow:0 20px 60px rgba(0,0,0,.08)}
.offre-card.featured{border:2px solid var(--rose-l)}
.offre-head{padding:28px 28px 20px;border-bottom:1px solid var(--border)}
.offre-badge{display:inline-block;font-size:11px;font-weight:500;letter-spacing:.8px;text-transform:uppercase;padding:5px 14px;border-radius:50px;margin-bottom:12px}
.badge-sage{background:var(--sage-l);color:var(--sage-d)}
.badge-teal{background:var(--teal-l);color:#2A5A5B}
.badge-gold{background:var(--gold-l);color:#7A6020}
.badge-rose{background:var(--rose-l);color:#7A4040}
.offre-icon{width:52px;height:52px;border-radius:16px;display:flex;align-items:center;justify-content:center;font-size:26px;margin-bottom:14px}
.offre-name{font-size:26px;font-weight:400;margin-bottom:6px}
.offre-desc{font-size:13px;color:var(--text-m);line-height:1.5;margin-bottom:14px}
.offre-price{font-family:'Cormorant Garamond',serif;font-size:38px;font-weight:300;margin-bottom:2px}
.offre-price span{font-size:16px;font-weight:400;font-family:'DM Sans',sans-serif}
.offre-note{font-size:12px;color:var(--text-l)}
.offre-body{padding:0 28px 28px}
.roles{display:flex;gap:8px;flex-wrap:wrap;margin:16px 0 12px}
.role-tag{display:inline-block;padding:4px 12px;border-radius:50px;font-size:12px;font-weight:500}
.features{list-style:none;margin-bottom:16px}
.features li{font-size:13px;color:var(--text-m);padding:7px 0;border-bottom:1px solid var(--cream-d);display:flex;align-items:flex-start;gap:8px;line-height:1.4}
.features li:last-child{border:none}
.check{color:var(--sage);font-weight:700;font-size:15px;flex-shrink:0;margin-top:1px}
.plus-value{background:var(--cream-d);border-radius:10px;padding:10px 14px;margin-bottom:16px;font-size:12px;color:var(--text-m);border-left:3px solid var(--sage)}
/* DASHBOARD */
.dash-wrap{display:grid;grid-template-columns:240px 1fr;min-height:calc(100vh - 64px)}
.sidebar{background:var(--white);border-right:1px solid var(--border);padding:24px 16px;position:sticky;top:64px;height:calc(100vh - 64px);overflow-y:auto;display:flex;flex-direction:column}
.sidebar-title{font-family:'Cormorant Garamond',serif;font-size:20px;font-weight:300;margin-bottom:20px;color:var(--text-m);padding:0 8px}
.s-nav{display:flex;flex-direction:column;gap:2px;flex:1}
.s-item{display:flex;align-items:center;gap:10px;padding:10px 12px;border-radius:10px;cursor:pointer;font-size:14px;color:var(--text-m);transition:all .2s;border:none;background:none;width:100%;text-align:left;font-family:'DM Sans',sans-serif}
.s-item:hover,.s-item.active{background:var(--cream-d);color:var(--text)}
.s-item .ico{font-size:18px;width:22px;text-align:center}
.s-lock{display:flex;align-items:center;gap:10px;padding:10px 12px;border-radius:10px;font-size:13px;color:var(--text-l);cursor:default;opacity:.6}
.s-lock .ico{font-size:16px}
.s-offre{margin-top:auto;padding:12px;background:var(--cream-d);border-radius:10px}
.s-offre-label{font-size:11px;color:var(--text-l);margin-bottom:4px}
.dash-main{padding:32px;background:var(--cream);overflow-y:auto}
/* ROLE SWITCHER */
.dash-top{display:flex;justify-content:space-between;align-items:flex-start;margin-bottom:28px}
.greeting h2{font-size:32px;font-weight:300}
.greeting p{font-size:14px;color:var(--text-m);margin-top:2px}
.role-sw{display:flex;gap:8px}
.r-btn{padding:8px 18px;border:1.5px solid var(--border);border-radius:50px;cursor:pointer;font-size:13px;font-family:'DM Sans',sans-serif;background:var(--white);color:var(--text-m);transition:all .2s}
.r-btn.active{border-color:var(--sage);background:var(--sage);color:#fff}
.r-btn.locked{opacity:.4;cursor:not-allowed}
/* METRICS */
.metrics{display:grid;grid-template-columns:repeat(4,1fr);gap:16px;margin-bottom:24px}
.metric{background:var(--white);border-radius:var(--r);border:1px solid var(--border);padding:18px}
.metric-l{font-size:12px;color:var(--text-l);margin-bottom:6px;letter-spacing:.3px}
.metric-v{font-family:'Cormorant Garamond',serif;font-size:32px;font-weight:300}
.metric-s{font-size:12px;color:var(--text-m);margin-top:2px}
.grid2{display:grid;grid-template-columns:1fr 1fr;gap:20px;margin-bottom:20px}
.full{grid-column:1/-1}
.card{background:var(--white);border-radius:var(--rl);border:1px solid var(--border);padding:24px}
.card-title{font-size:18px;font-weight:400;margin-bottom:16px}
/* CHART */
.bars{display:flex;align-items:flex-end;gap:8px;height:90px}
.bar-col{flex:1;display:flex;flex-direction:column;align-items:center;gap:4px}
.bar{border-radius:4px 4px 0 0;width:100%;transition:height .5s}
.bar-lbl{font-size:11px;color:var(--text-l)}
/* MOOD */
.mood-row{display:flex;gap:10px;margin:10px 0}
.mood-btn{width:46px;height:46px;border-radius:50%;border:2px solid var(--border);background:var(--white);font-size:22px;cursor:pointer;transition:all .2s;display:flex;align-items:center;justify-content:center}
.mood-btn.sel,.mood-btn:hover{border-color:var(--sage);transform:scale(1.12);background:rgba(184,212,187,.1)}
/* JOURNAL */
.journal-box{width:100%;min-height:130px;border:1px solid var(--border);border-radius:var(--r);padding:14px;font-family:'DM Sans',sans-serif;font-size:14px;color:var(--text);background:var(--cream);resize:vertical;line-height:1.6;transition:border .2s}
.journal-box:focus{outline:none;border-color:var(--sage)}
/* EXERCICES */
.ex-tabs{display:flex;gap:4px;background:var(--cream-d);border-radius:12px;padding:4px;margin-bottom:20px}
.ex-tab{flex:1;padding:9px;border-radius:9px;border:none;cursor:pointer;font-family:'DM Sans',sans-serif;font-size:13px;color:var(--text-m);background:transparent;transition:all .2s;text-align:center}
.ex-tab.active{background:var(--white);color:var(--text);font-weight:500;box-shadow:0 1px 4px rgba(0,0,0,.08)}
.ex-panel{display:none}.ex-panel.active{display:block}
.ex-card{background:var(--white);border-radius:var(--r);border:1px solid var(--border);padding:20px;margin-bottom:10px;cursor:pointer;transition:all .2s;position:relative}
.ex-card:hover{border-color:var(--sage-l)}
.ex-card.locked{opacity:.55;cursor:not-allowed}
.ex-card.locked::after{content:'🔒 Offre supérieure requise';position:absolute;inset:0;background:rgba(250,247,242,.85);display:flex;align-items:center;justify-content:center;border-radius:var(--r);font-size:13px;color:var(--text-m);font-weight:500}
.ex-card h4{font-size:15px;font-weight:500;margin-bottom:4px}
.ex-card p{font-size:13px;color:var(--text-m);line-height:1.5}
.ex-dur{font-size:12px;color:var(--text-l);margin-top:6px}
.ex-tag{display:inline-block;padding:3px 10px;border-radius:50px;font-size:11px;font-weight:500;margin-bottom:8px}
/* RESPIRATION */
.resp-player{background:var(--white);border-radius:var(--rl);border:1px solid var(--border);padding:28px;text-align:center;margin-bottom:20px}
.resp-circle{width:180px;height:180px;border-radius:50%;display:flex;align-items:center;justify-content:center;margin:0 auto 16px;transition:all 1s;position:relative}
.resp-circle.inhale{background:radial-gradient(circle,#B8D4BB,#7A9E7E);transform:scale(1.15)}
.resp-circle.hold{background:radial-gradient(circle,#BBBBDD,#7B7BAE)}
.resp-circle.exhale{background:radial-gradient(circle,#A8CCCC,#4A8B8C);transform:scale(.88)}
.resp-circle.idle{background:radial-gradient(circle,var(--cream-d),var(--cream))}
.resp-phase{font-size:12px;letter-spacing:2px;text-transform:uppercase;color:var(--text-m);margin-bottom:8px}
.resp-count{font-family:'Cormorant Garamond',serif;font-size:56px;font-weight:300;color:var(--sage);line-height:1}
.resp-prog{height:4px;background:var(--cream-d);border-radius:2px;margin:14px 0 10px;overflow:hidden}
.resp-bar{height:100%;border-radius:2px;background:var(--sage);width:0%}
.resp-cycles{font-size:13px;color:var(--text-m);margin-bottom:16px}
.resp-btns{display:flex;gap:8px;justify-content:center;flex-wrap:wrap}
/* HARCÈLEMENT */
.harc-tabs{display:flex;gap:4px;background:var(--cream-d);border-radius:12px;padding:4px;margin-bottom:20px}
.h-tab{flex:1;padding:9px;border-radius:9px;border:none;cursor:pointer;font-family:'DM Sans',sans-serif;font-size:12px;color:var(--text-m);background:transparent;transition:all .2s;text-align:center}
.h-tab.active{background:var(--white);color:var(--text);font-weight:500;box-shadow:0 1px 4px rgba(0,0,0,.08)}
.h-panel{display:none}.h-panel.active{display:block}
.signal-item{display:flex;align-items:flex-start;gap:12px;padding:12px;border-radius:10px;border:1px solid var(--border);margin-bottom:8px;cursor:pointer;transition:all .2s}
.signal-item.checked{background:rgba(122,158,126,.08);border-color:var(--sage)}
.sig-check{width:22px;height:22px;min-width:22px;border-radius:6px;border:2px solid var(--border);display:flex;align-items:center;justify-content:center;transition:all .2s;font-size:13px;color:transparent}
.signal-item.checked .sig-check{background:var(--sage);border-color:var(--sage);color:#fff}
.script-box{background:var(--cream-d);padding:14px 18px;border-radius:10px;margin-bottom:10px}
.script-label{font-size:11px;color:var(--text-l);letter-spacing:.8px;text-transform:uppercase;margin-bottom:6px}
.script-text{font-size:14px;font-style:italic;color:var(--text);line-height:1.6}
.action-step{padding:14px;border:1px solid var(--border);border-radius:10px;margin-bottom:10px;border-left:4px solid var(--sage)}
/* ÉVOLUTION */
.evo-profile{display:flex;gap:8px;margin-bottom:20px}
.evo-btn{padding:8px 18px;border:1.5px solid var(--border);border-radius:50px;cursor:pointer;font-size:13px;font-family:'DM Sans',sans-serif;background:var(--white);color:var(--text-m);transition:all .2s}
.evo-btn.active{border-color:var(--teal);background:var(--teal);color:#fff}
/* TIMELINE */
.timeline{position:relative;padding-left:24px}
.timeline::before{content:'';position:absolute;left:8px;top:0;bottom:0;width:1px;background:var(--border)}
.tl-item{position:relative;padding:10px 0 10px 20px;margin-bottom:2px}
.tl-item::before{content:'';position:absolute;left:-8px;top:16px;width:10px;height:10px;border-radius:50%;background:var(--sage);border:2px solid var(--white)}
.tl-time{font-size:11px;color:var(--text-l);margin-bottom:2px}
.tl-text{font-size:14px;color:var(--text-m);line-height:1.5}
/* ALERTS */
.alert{padding:12px 14px;border-radius:10px;font-size:13px;margin-bottom:8px;display:flex;align-items:flex-start;gap:10px;line-height:1.5}
.alert-r{background:#FFEAEA;border:1px solid #F0A0A0;color:#702020}
.alert-y{background:#FFF8E8;border:1px solid #F0D080;color:#806020}
.alert-g{background:#E8F5EA;border:1px solid #90C890;color:#204020}
.alert-b{background:#E8F4FF;border:1px solid #90C4EE;color:#204870}
/* LOCK OVERLAY */
.lock-overlay{text-align:center;padding:60px 40px;background:var(--white);border-radius:var(--rl);border:1px solid var(--border)}
.lock-overlay h3{font-size:28px;font-weight:300;margin-bottom:8px}
.lock-overlay p{font-size:14px;color:var(--text-m);margin-bottom:20px;line-height:1.6}
/* PAYMENT MODAL */
.modal-bg{position:fixed;inset:0;background:rgba(0,0,0,.5);z-index:200;display:flex;align-items:center;justify-content:center;padding:20px}
.modal{background:var(--white);border-radius:var(--rxl);padding:40px;max-width:500px;width:100%;max-height:90vh;overflow-y:auto}
.legal-ck{display:flex;align-items:flex-start;gap:12px;padding:14px;border:1px solid var(--border);border-radius:10px;margin-bottom:10px;transition:all .2s}
.legal-ck:hover{border-color:var(--sage-l)}
.legal-ck input{width:20px;height:20px;min-width:20px;accent-color:var(--sage);flex-shrink:0;margin-top:2px;cursor:pointer}
.legal-ck label{font-size:13px;color:var(--text-m);line-height:1.5;cursor:pointer}
.legal-ck label strong{color:var(--text)}
.warn-box{background:var(--cream-d);border-radius:10px;padding:14px;border-left:3px solid var(--rose);margin:14px 0}
.warn-box p{font-size:12px;color:var(--text-m);line-height:1.6}
/* LEGAL */
.legal-wrap{max-width:860px;margin:0 auto;padding:40px}
.hl-box{background:var(--cream-d);padding:16px;border-radius:10px;border-left:3px solid var(--sage);margin:12px 0}
.legal-sec h3{font-size:20px;font-weight:400;color:var(--text);margin-bottom:12px;padding-bottom:8px;border-bottom:1px solid var(--border);font-family:'Cormorant Garamond',serif}
.legal-sec p,.legal-sec li{font-size:14px;color:var(--text-m);line-height:1.8;margin-bottom:6px}
.legal-sec ul{padding-left:20px}
/* CREATOR */
.creator-modal{background:var(--white);border-radius:var(--rxl);padding:40px;max-width:720px;width:100%;max-height:90vh;overflow-y:auto}
.creator-offre{border:1px solid var(--border);border-radius:var(--rl);overflow:hidden;margin-bottom:14px}
.creator-offre-head{padding:14px 18px;display:flex;justify-content:space-between;align-items:center;cursor:pointer;font-weight:500}
.creator-offre-body{padding:20px;display:none;border-top:1px solid var(--border)}
.creator-section{margin-bottom:14px}
.creator-section-title{font-size:11px;letter-spacing:1.5px;text-transform:uppercase;color:var(--sage);margin-bottom:8px}
.creator-item{font-size:13px;color:var(--text-m);padding:6px 0;border-bottom:1px solid var(--cream-d);line-height:1.5}
.creator-item:last-child{border:none}
.creator-item strong{color:var(--text)}
/* PROGRESS BAR */
.prog-wrap{margin-bottom:8px}
.prog-label{display:flex;justify-content:space-between;font-size:13px;color:var(--text-m);margin-bottom:4px}
.prog-bg{height:6px;background:var(--cream-d);border-radius:3px;overflow:hidden}
.prog-fill{height:100%;border-radius:3px;background:var(--sage);transition:width .6s}
/* STREAKS */
.streak-grid{display:grid;grid-template-columns:repeat(7,1fr);gap:6px;margin-top:8px}
.streak-day{height:32px;border-radius:6px;display:flex;align-items:center;justify-content:center;font-size:11px;color:var(--text-l)}
.streak-day.done{background:var(--sage);color:#fff}
.streak-day.today{background:var(--sage-d);color:#fff;font-weight:500}
/* SCORE RING */
.score-ring{width:80px;height:80px;margin:0 auto 12px}
.score-ring svg{transform:rotate(-90deg)}
/* RESPONSIVE */
@media(max-width:900px){
  .hero{grid-template-columns:1fr}.offres-grid{grid-template-columns:1fr}
  .dash-wrap{grid-template-columns:1fr}.sidebar{display:none}
  .metrics{grid-template-columns:1fr 1fr}.grid2{grid-template-columns:1fr}
}
input,select,textarea{font-family:'DM Sans',sans-serif}
select{padding:8px 12px;border:1px solid var(--border);border-radius:8px;background:var(--cream);color:var(--text);font-size:14px}
</style>
</head>
<body>

<!-- NAV -->
<nav class="nav">
  <div class="nav-logo" onclick="goPage(&#39;home&#39;)">Séré<em>num</em></div>
  <div class="nav-links">
    <div class="nav-link" onclick="goPage(&#39;home&#39;)">Accueil</div>
    <div class="nav-link" onclick="goPage(&#39;offres&#39;)">Nos offres</div>
    <div class="nav-link" onclick="goPage(&#39;dash&#39;)">Espace membre</div>
    <div class="nav-link" onclick="goPage(&#39;legal&#39;)">Mentions légales</div>
  </div>
</nav>

<!-- ═══════════════ PAGE ACCUEIL ═══════════════ -->
<div id="page-home" class="page active">
  <div class="hero">
    <div>
      <div class="hero-tag">Gestion du stress scolaire · Paiement unique</div>
      <h1 class="hero-title">Quand l'école<br>devient<br><em>trop lourde</em></h1>
      <p class="hero-sub">Des outils concrets pour aider vos enfants à gérer l'anxiété scolaire, la pression des notes, et le harcèlement. Pensés par un parent, pour des parents.</p>
      <div style="display:flex;gap:12px;margin-bottom:20px">
        <button class="btn btn-sage" onclick="goPage(&#39;offres&#39;)">Découvrir les offres</button>
        <button class="btn btn-out" onclick="goPage(&#39;dash&#39;)">Espace membre</button>
      </div>
      <div class="disclaimer">⚠️ <strong>Important :</strong> Je ne suis ni médecin, ni psychologue, ni thérapeute. Je suis un parent qui partage ce qui a fonctionné pour son fils. Ces outils ne remplacent aucun suivi médical ou thérapeutique. Aucune guérison n'est garantie.</div>
    </div>
    <div><div class="orb"><div class="orb-text">Inspire<br>doucement</div></div></div>
  </div>

  <div class="stats">
    <div class="stat"><div class="stat-n">1/5</div><div class="stat-l">enfants souffre d'anxiété scolaire significative (INSERM 2023)</div></div>
    <div class="stat"><div class="stat-n">700 000</div><div class="stat-l">élèves victimes de harcèlement chaque année (Éducation Nationale)</div></div>
    <div class="stat"><div class="stat-n">67%</div><div class="stat-l">des parents se sentent démunis face au stress de leur enfant (Ifop 2022)</div></div>
  </div>

  <div class="story">
    <div class="story-inner">
      <div class="story-quote">"</div>
      <div style="position:relative">
        <div class="story-tag">L'histoire qui a tout changé</div>
        <p style="font-family:&#39;Cormorant Garamond&#39;,serif;font-size:22px;font-weight:300;line-height:1.75;margin-bottom:18px">Un jour, mon fils de 9 ans est rentré de l'école le visage fermé. Il avait eu une dictée surprise.</p>
        <p style="font-size:15px;color:var(--text-m);line-height:1.8;margin-bottom:16px">Il m'a raconté qu'au moment où la maîtresse avait annoncé la dictée, son cœur s'était emballé. Les mots dans sa tête s'étaient brouillés. Il sentait la panique monter.</p>
        <p style="font-size:15px;color:var(--text-m);line-height:1.8;margin-bottom:16px">Mais il a fait quelque chose que je ne lui avais pas demandé. <strong style="color:var(--text)">Il s'est posé sur sa chaise. Il a fermé les yeux une seconde. Et il a pensé à moi.</strong> Il m'a dit : <em style="color:var(--sage-d)">"J'ai fait la technique SOS qu'on faisait à la maison, papa."</em></p>
        <p style="font-size:15px;color:var(--text-m);line-height:1.8;margin-bottom:24px">Quelques respirations guidées. Son rythme cardiaque s'est apaisé. La dictée s'est bien passée.</p>
        <div style="border-left:3px solid var(--sage);padding:14px 18px;background:rgba(184,212,187,.1);border-radius:0 10px 10px 0;margin-bottom:24px">
          <p style="font-family:&#39;Cormorant Garamond&#39;,serif;font-size:19px;font-weight:300;font-style:italic;color:var(--sage-d);line-height:1.6">La vraie victoire, ce n'est pas d'éliminer le stress de la vie de nos enfants. C'est de leur donner les outils pour y faire face seuls, quand nous ne sommes pas là.</p>
        </div>
        <p style="font-size:14px;color:var(--text-m);line-height:1.7;margin-bottom:24px">C'est pour ça que j'ai créé Sérénum. Pas pour promettre un miracle, pas pour remplacer un médecin ou un psy. Mais pour mettre entre les mains de votre enfant des techniques concrètes, adaptées à son âge, qu'il pourra utiliser seul.</p>
        <div style="display:flex;align-items:center;gap:14px">
          <div style="width:46px;height:46px;border-radius:50%;background:var(--sage-l);display:flex;align-items:center;justify-content:center;font-size:20px;flex-shrink:0">👨‍👦</div>
          <div><div style="font-weight:500;font-size:15px">Sébastien GARCIA</div><div style="font-size:13px;color:var(--text-m)">Fondateur de Sérénum · Parent avant tout</div></div>
        </div>
      </div>
    </div>
  </div>

  <div class="how">
    <h2 style="font-size:38px;font-weight:300;margin-bottom:32px;text-align:center">Comment ça fonctionne</h2>
    <div class="how-grid">
      <div class="how-card"><div style="font-size:40px;margin-bottom:12px">🌱</div><h3 style="font-size:20px;font-weight:400;margin-bottom:8px">Choisissez votre offre</h3><p style="font-size:14px;color:var(--text-m);line-height:1.6">Paiement unique, adapté à l'âge et au besoin. Zéro abonnement, zéro surprise.</p></div>
      <div class="how-card"><div style="font-size:40px;margin-bottom:12px">🧘</div><h3 style="font-size:20px;font-weight:400;margin-bottom:8px">Accédez à votre espace</h3><p style="font-size:14px;color:var(--text-m);line-height:1.6">Parent, enfant ou ado — chaque rôle a son interface, son journal et ses exercices exclusifs.</p></div>
      <div class="how-card"><div style="font-size:40px;margin-bottom:12px">📈</div><h3 style="font-size:20px;font-weight:400;margin-bottom:8px">Suivez l'évolution</h3><p style="font-size:14px;color:var(--text-m);line-height:1.6">Dashboard journalier, graphiques d'humeur, alertes parentales, historique complet.</p></div>
    </div>
  </div>
</div>

<!-- ═══════════════ PAGE OFFRES ═══════════════ -->
<div id="page-offres" class="page">
  <div class="offres-head">
    <div class="hero-tag" style="display:block;margin-bottom:12px">Paiement unique · Sans abonnement · Accès illimité</div>
    <h2 style="font-size:46px;font-weight:300;margin-bottom:12px">Choisissez votre programme</h2>
    <p style="font-size:15px;color:var(--text-m);line-height:1.6">Chaque offre contient des exercices <strong>100% exclusifs</strong>. Plus vous montez en gamme, plus les outils sont spécialisés et complets.</p>
  </div>
  <div class="offres-grid">

    <!-- O1 -->
    <div class="offre-card" onclick="openPay(0)">
      <div class="offre-head">
        <div class="offre-badge badge-sage">🧒 Enfants · 6–11 ans</div>
        <div class="offre-icon" style="background:rgba(184,212,187,.3)">🌱</div>
        <div class="offre-name">Petites Pousses</div>
        <div class="offre-desc">Le premier programme de respiration et de gestion des émotions pensé spécialement pour les enfants de primaire.</div>
        <div class="offre-price">49€ <span>TTC</span></div>
        <div class="offre-note">Paiement unique · 1 profil enfant</div>
      </div>
      <div class="offre-body">
        <div class="roles"><span class="role-tag badge-sage">👨‍👩‍👧 Parent</span><span class="role-tag badge-sage">🧒 Enfant</span></div>
        <div class="plus-value">✦ Idéal pour : premier contact avec la gestion du stress, enfants 6-11 ans, parents qui cherchent une base solide.</div>
        <ul class="features">
          <li><span class="check">✓</span>Cohérence cardiaque guidée 3-6-5 (voix enfant)</li>
          <li><span class="check">✓</span>Respiration "Bulle de savon" (expire 6s sans éclater)</li>
          <li><span class="check">✓</span>Respiration "Souffle du Lion" (évacuation tension)</li>
          <li><span class="check">✓</span>Technique "Ma tortue intérieure" (visualisation 8min)</li>
          <li><span class="check">✓</span>Journal illustré des émotions (privé, enfant)</li>
          <li><span class="check">✓</span>Dashboard parent : score anxiété + alertes</li>
          <li><span class="check">✓</span>Graphique humeur 7 jours + streak</li>
        </ul>
        <button class="btn btn-sage" style="width:100%">Choisir Petites Pousses →</button>
      </div>
    </div>

    <!-- O2 -->
    <div class="offre-card" onclick="openPay(1)">
      <div class="offre-head">
        <div class="offre-badge badge-teal">🧑 Adolescents · 12–18 ans</div>
        <div class="offre-icon" style="background:rgba(168,204,204,.3)">🌊</div>
        <div class="offre-name">Cap Sérénité</div>
        <div class="offre-desc">Un programme complet pour les ados face à la pression des examens, des notes et des relations sociales complexes.</div>
        <div class="offre-price">119€ <span>TTC</span></div>
        <div class="offre-note">Paiement unique · 1 profil ado</div>
      </div>
      <div class="offre-body">
        <div class="roles"><span class="role-tag badge-teal">👨‍👩‍👧 Parent</span><span class="role-tag badge-teal">🧑 Ado</span></div>
        <div class="plus-value">✦ En plus de Petites Pousses : techniques avancées pour les ados, tracker stress scolaire, journal confidentiel, suivi 30 jours.</div>
        <ul class="features">
          <li><span class="check">✓</span>Respiration 4-7-8 (anti-stress avant examen)</li>
          <li><span class="check">✓</span>Respiration physiologique (double expir. — réinitialise SN)</li>
          <li><span class="check">✓</span>Technique STOP — pleine conscience en 4 étapes</li>
          <li><span class="check">✓</span>Carnet des victoires (3 réussites/soir — confiance)</li>
          <li><span class="check">✓</span>Journal émotionnel ado (slider stress, sommeil, confidentiel)</li>
          <li><span class="check">✓</span>Tracker stress par matière (maths, exposé, interro…)</li>
          <li><span class="check">✓</span>Graphique humeur 30 jours + analyse tendances</li>
          <li><span class="check">✓</span>Dashboard parent discret (résumés, pas le contenu)</li>
        </ul>
        <button class="btn btn-teal" style="width:100%">Choisir Cap Sérénité →</button>
      </div>
    </div>

    <!-- O3 -->
    <div class="offre-card" onclick="openPay(2)">
      <div class="offre-head">
        <div class="offre-badge badge-gold">👨‍👩‍👧 Famille · Tous âges</div>
        <div class="offre-icon" style="background:rgba(232,212,160,.3)">⭐</div>
        <div class="offre-name">Famille Unie</div>
        <div class="offre-desc">Pour toute la famille : enfants ET ados, avec des outils de communication parent-enfant et un premier module anti-harcèlement.</div>
        <div class="offre-price">189€ <span>TTC</span></div>
        <div class="offre-note">Paiement unique · 2 profils enfants</div>
      </div>
      <div class="offre-body">
        <div class="roles"><span class="role-tag badge-gold">👨‍👩‍👧 Parent</span><span class="role-tag badge-gold">🧒 Enfant</span><span class="role-tag badge-gold">🧑 Ado</span></div>
        <div class="plus-value">✦ En plus des offres précédentes : outils famille, ancrage corporel, relaxation clinique, module harcèlement, 2 profils enfants simultanés.</div>
        <ul class="features">
          <li><span class="check">✓</span>Ancrage sensoriel 5-4-3-2-1 (interrompt crise)</li>
          <li><span class="check">✓</span>Relaxation de Jacobson (contraction-relâchement clinique)</li>
          <li><span class="check">✓</span>Respiration "Vague de l'océan" (corps + souffle)</li>
          <li><span class="check">✓</span>Visualisation "Mon lieu de sécurité" (refuge mental)</li>
          <li><span class="check">✓</span>Protocole dialogue parent-enfant (scripts par âge)</li>
          <li><span class="check">✓</span>Journal partagé famille (opt-in, enfant choisit)</li>
          <li><span class="check">✓</span>Module harcèlement : détection + scripts dialogue</li>
          <li><span class="check">✓</span>Dashboard 2 profils + alertes avancées croisées</li>
          <li><span class="check">✓</span>Plan d'action harcèlement 4 étapes</li>
        </ul>
        <button class="btn btn-gold" style="width:100%">Choisir Famille Unie →</button>
      </div>
    </div>

    <!-- O4 -->
    <div class="offre-card featured" onclick="openPay(3)">
      <div class="offre-head">
        <div class="offre-badge badge-rose">🛡️ Programme complet · Anti-harcèlement</div>
        <div class="offre-icon" style="background:rgba(232,187,187,.3)">🛡️</div>
        <div class="offre-name">Intensif &amp; Harcèlement</div>
        <div class="offre-desc">Le programme le plus complet. Pour les familles qui font face au harcèlement scolaire actif et aux crises d'anxiété sévères. Outils de reconstruction de l'estime et de défense concrète.</div>
        <div class="offre-price">269€ <span>TTC</span></div>
        <div class="offre-note">Paiement unique · 4 profils enfants · Module harcèlement complet</div>
      </div>
      <div class="offre-body">
        <div class="roles"><span class="role-tag badge-rose">👨‍👩‍👧 Parent</span><span class="role-tag badge-rose">🧒 Enfant</span><span class="role-tag badge-rose">🧑 Ado</span></div>
        <div class="plus-value" style="border-color:var(--rose)">✦ EXCLUSIF à cette offre : 3 techniques anti-harcèlement inédites + protocole crise + journal confidentiel total (invisible aux parents) + 4 profils.</div>
        <ul class="features">
          <li><span class="check">✓</span><strong>🛡️ "Mon armure du matin"</strong> — routine 5min avant l'école</li>
          <li><span class="check">✓</span><strong>🗣️ "La phrase qui coupe court"</strong> — désamorcer sans s'abaisser</li>
          <li><span class="check">✓</span><strong>📓 "Mes preuves de valeur"</strong> — reconstruire l'estime/jour</li>
          <li><span class="check">✓</span>Respiration Box 4-4-4-4 (protocole forces spéciales)</li>
          <li><span class="check">✓</span>Protocole crise immédiate 5 min (utilisable seul)</li>
          <li><span class="check">✓</span>Checklist 10 signaux harcèlement + analyse risque auto</li>
          <li><span class="check">✓</span>Scripts dialogue par âge (6-11 / 12-18 / cyber)</li>
          <li><span class="check">✓</span>Journal confidentiel ado (INVISIBLE aux parents)</li>
          <li><span class="check">✓</span>Dashboard intensif 4 profils + alertes prioritaires</li>
          <li><span class="check">✓</span>Numéros urgence intégrés (3018, 119, 3114)</li>
        </ul>
        <button class="btn btn-rose" style="width:100%;padding:14px;font-size:15px">Choisir ce programme →</button>
      </div>
    </div>
  </div>
</div>

<!-- ═══════════════ PAGE DASHBOARD ═══════════════ -->
<div id="page-dash" class="page">
  <div class="dash-wrap">
    <aside class="sidebar">
      <div class="sidebar-title">Sérénum</div>
      <div class="s-nav" id="sidebar-nav"><button class="s-item active"><span class="ico">🏠</span>Tableau de bord</button><button class="s-item"><span class="ico">📓</span>Mon journal</button><button class="s-item"><span class="ico">🫁</span>Exercices</button><button class="s-item"><span class="ico">🛡️</span>Harcèlement</button><button class="s-item"><span class="ico">📈</span>Évolution</button><div class="s-lock"><span class="ico">🔒</span>Armure du matin (Intensif)</div></div>
      <div class="s-offre">
        <div class="s-offre-label">Offre active</div>
        <div id="sidebar-offre-badge" style="font-weight:500;font-size:14px">⭐ Famille Unie</div>
      </div>
    </aside>
    <main class="dash-main" id="dash-main"><div class="dash-top">
    <div class="greeting"><h2>Bonjour, Sébastien 👋</h2><p>Vendredi 29 mai 2026</p></div>
    <div class="role-sw"><button class="r-btn active" data-role="parent">👨‍👩‍👧 Parent</button><button class="r-btn" data-role="enfant">🧒 Enfant</button><button class="r-btn" data-role="ado">🧑 Ado</button></div>
  </div>
  <div class="metrics">
    <div class="metric"><div class="metric-l">Score anxiété Emma</div><div class="metric-v" style="color:#C47B7B">6.4</div><div class="metric-s">/10 · ↑ depuis hier</div></div>
    <div class="metric"><div class="metric-l">Score anxiété Léo</div><div class="metric-v" style="color:#C4A24A">4.2</div><div class="metric-s">/10 · stable</div></div>
    <div class="metric"><div class="metric-l">Exercices cette semaine</div><div class="metric-v">12</div><div class="metric-s">Emma: 8 · Léo: 4</div></div>
    <div class="metric"><div class="metric-l">Streak Emma</div><div class="metric-v" style="color:var(--sage)">7🔥</div><div class="metric-s">jours consécutifs</div></div>
  </div>
  <div class="grid2">
    <div class="card">
      <div class="card-title">Alertes parentales</div>
      <div class="alert alert-r">⚠️ <div><strong>Emma (9 ans)</strong> — Anxiété élevée (6.4/10) depuis 3 jours. Surveillance recommandée.</div></div>
      <div class="alert alert-y">⏰ <div><strong>Léo (14 ans)</strong> — Journal non complété depuis 2 jours.</div></div>
      <div class="alert alert-g">✅ <div><strong>Emma</strong> — 3 exercices complétés aujourd'hui. Excellent !</div></div>
    </div>
    <div class="card">
      <div class="card-title">Humeur cette semaine</div>
      <div style="font-size:12px;color:var(--text-m);margin-bottom:8px">Emma (rose) · Léo (teal)</div>
      <div class="bars">
        <div class="bar-col">
          <div class="bar" style="height:45%;background:var(--teal-l)"></div>
          <div class="bar" style="height:54%;background:var(--rose-l)"></div>
          <div class="bar-lbl">Lun</div>
        </div><div class="bar-col">
          <div class="bar" style="height:36%;background:var(--teal-l)"></div>
          <div class="bar" style="height:45%;background:var(--rose-l)"></div>
          <div class="bar-lbl">Mar</div>
        </div><div class="bar-col">
          <div class="bar" style="height:54%;background:var(--teal-l)"></div>
          <div class="bar" style="height:63%;background:var(--rose-l)"></div>
          <div class="bar-lbl">Mer</div>
        </div><div class="bar-col">
          <div class="bar" style="height:45%;background:var(--teal-l)"></div>
          <div class="bar" style="height:54%;background:var(--rose-l)"></div>
          <div class="bar-lbl">Jeu</div>
        </div><div class="bar-col">
          <div class="bar" style="height:63%;background:var(--teal-l)"></div>
          <div class="bar" style="height:81%;background:var(--rose-l)"></div>
          <div class="bar-lbl">Ven</div>
        </div><div class="bar-col">
          <div class="bar" style="height:54%;background:var(--teal-l)"></div>
          <div class="bar" style="height:63%;background:var(--rose-l)"></div>
          <div class="bar-lbl">Sam</div>
        </div><div class="bar-col">
          <div class="bar" style="height:45%;background:var(--teal-l)"></div>
          <div class="bar" style="height:72%;background:var(--rose-l)"></div>
          <div class="bar-lbl">Dim</div>
        </div>
      </div>
      <div style="font-size:11px;color:var(--text-l);text-align:center;margin-top:6px">Plus haut = meilleure humeur</div>
    </div>
  </div>
  <div class="card full">
    <div class="card-title">Activité récente</div>
    <div class="timeline">
      <div class="tl-item"><div class="tl-time">Aujourd'hui · 16h32</div><div class="tl-text">Emma a complété "Bulle de savon" (3 cycles) — Humeur après : 😊</div></div>
      <div class="tl-item"><div class="tl-time">Aujourd'hui · 14h10</div><div class="tl-text">Emma a écrit dans son journal des émotions</div></div>
      <div class="tl-item"><div class="tl-time">Hier · 20h15</div><div class="tl-text">Léo a complété "Respiration 4-7-8" — Humeur après : 😐</div></div>
      <div class="tl-item"><div class="tl-time">Hier · 18h00</div><div class="tl-text">Emma a complété "Cohérence cardiaque" (5 min)</div></div>
    </div>
  </div></main>
  </div>
</div>

<!-- ═══════════════ PAGE LEGAL ═══════════════ -->
<div id="page-legal" class="page">
  <div class="legal-wrap">
    <div style="margin-bottom:32px">
      <div class="hero-tag" style="display:block;margin-bottom:8px">Documents légaux · Conformes droit français · RGPD</div>
      <h2 style="font-size:44px;font-weight:300;margin-bottom:6px">Mentions légales, CGV &amp; CNIL</h2>
    </div>
    <div class="hl-box" style="border-color:var(--rose);margin-bottom:28px">
      <p style="font-size:13px"><strong>⚠️ Avertissement personnel :</strong> Je suis le créateur de Sérénum. Je ne suis ni médecin, ni psychologue, ni psychothérapeute, ni thérapeute d'aucune sorte. Je suis un parent qui partage des outils de gestion du stress scolaire. Ces contenus ne constituent pas un acte médical, psychologique ou thérapeutique. Ils ne remplacent en aucun cas une consultation professionnelle. Aucune guérison n'est promise. Je décline toute responsabilité quant aux résultats. En cas d'urgence : médecin ou 15.</p>
    </div>
    <div class="legal-sec" style="margin-bottom:24px">
      <h3>1. Identité de l'éditeur</h3>
      <div class="hl-box">
        <p><strong>Nom et prénom :</strong> Sébastien GARCIA</p>
        <p><strong>Forme juridique :</strong> Entrepreneur individuel — Micro-entreprise</p>
        <p><strong>SIREN :</strong> 990 963 852</p>
        <p><strong>SIRET :</strong> 990 963 852 00019</p>
        <p><strong>Code APE :</strong> 7022Z</p>
        <p><strong>Adresse du siège :</strong> 28 Rue du Maroc, 29270 Carhaix-Plouguer, France</p>
        <p><strong>Courriel :</strong> <span id="legal-email" style="cursor:pointer;text-decoration:underline" onclick="handleEmailClick()">sebastien.garcia29@outlook.fr</span></p>
        <p><strong>Hébergeur :</strong> Vercel Inc., 340 Pine Street Suite 701, San Francisco CA 94104, USA — vercel.com</p>
        <p><strong>Paiement :</strong> Stripe Inc., 354 Oyster Point Blvd, South San Francisco CA 94080, USA — certifié PCI-DSS niveau 1</p>
      </div>
      <p style="font-size:13px;color:var(--text-m);margin-top:8px">Conformément à l'article 6 de la loi n°2004-575 du 21 juin 2004 (LCEN).</p>
    </div>
    <div class="legal-sec" style="margin-bottom:24px">
      <h3>2. Conditions Générales de Vente</h3>
      <p>Les présentes CGV régissent les relations contractuelles entre moi, <strong>Sébastien GARCIA</strong>, entrepreneur individuel (SIREN 990 963 852, SIRET 990 963 852 00019), domicilié au 28 Rue du Maroc, 29270 Carhaix-Plouguer (ci-après "le Vendeur"), et tout utilisateur ayant passé commande (ci-après "le Client"), conformément aux articles L.111-1 et suivants du Code de la consommation.</p>
      <p style="margin-top:10px"><strong>Tarifs TTC :</strong> Petites Pousses 49€ · Cap Sérénité 119€ · Famille Unie 189€ · Intensif &amp; Harcèlement 269€. Paiement unique, sans abonnement, accès illimité.</p>
      <div class="hl-box" style="margin-top:12px">
        <p style="font-size:13px"><strong>Droit de rétractation — art. L.221-28 13° Code de la consommation :</strong> Conformément à cet article, le droit de rétractation de 14 jours ne s'applique pas aux contenus numériques dont l'exécution a commencé avec l'accord exprès du consommateur, qui a renoncé expressément à ce droit. Cette renonciation est formalisée par la case à cocher obligatoire lors du paiement.</p>
      </div>
      <p style="margin-top:10px"><strong>Responsabilité :</strong> Je ne saurais être tenu responsable des dommages directs ou indirects résultant de l'utilisation des services. Je ne suis ni médecin, ni psychologue, ni thérapeute. Les outils proposés ne constituent pas des soins médicaux ou thérapeutiques.</p>
      <p style="margin-top:10px"><strong>Médiation :</strong> En cas de litige non résolu : médiateur FEVAD — mediateur@fevad.com. Plateforme UE : ec.europa.eu/consumers/odr</p>
    </div>
    <div class="legal-sec" style="margin-bottom:24px">
      <h3>3. Politique de confidentialité &amp; RGPD</h3>
      <p>Conformément au RGPD (UE) 2016/679 et à la loi Informatique et Libertés n°78-17.</p>
      <p style="margin-top:8px"><strong>Données collectées :</strong> identification (nom, email), données d'utilisation (exercices, fréquence), journaux émotionnels (chiffrés AES-256, traitement fondé sur consentement explicite art. 9 RGPD), données concernant les mineurs (consentement parental obligatoire art. 8 RGPD).</p>
      <p style="margin-top:8px"><strong>Vos droits (art. 15-22 RGPD) :</strong> accès, rectification, effacement, limitation, portabilité, opposition, retrait du consentement. Contact : sebastien.garcia29@outlook.fr. Délai : 1 mois. Recours CNIL : www.cnil.fr</p>
      <p style="margin-top:8px"><strong>Sous-traitants :</strong> Vercel Inc. (hébergement, CCT UE) · Stripe Inc. (paiement, PCI-DSS niveau 1, CCT UE). Aucune donnée vendue à des tiers.</p>
      <p style="margin-top:8px"><strong>Sécurité :</strong> TLS 1.3 en transit · AES-256 au repos · Notification violation 72h (art. 33 RGPD).</p>
      <p style="margin-top:8px"><strong>Cookies :</strong> Uniquement les cookies strictement nécessaires au fonctionnement. Aucun cookie publicitaire ou de pistage (délibération CNIL n°2020-091).</p>
    </div>
    <div class="legal-sec" style="margin-bottom:24px">
      <h3>4. Propriété intellectuelle</h3>
      <p>L'ensemble des contenus que j'ai créés pour Sérénum sont ma propriété exclusive en tant que Sébastien GARCIA (SIREN 990 963 852), protégés par le Code de la propriété intellectuelle. Toute reproduction non autorisée constitue une contrefaçon (art. L.335-2 et suivants).</p>
    </div>
    <div style="text-align:center;padding:24px;background:var(--cream-d);border-radius:var(--rl);margin-top:24px">
      <p style="font-size:12px;color:var(--text-l)">Mis à jour le 29 mai 2026 · Sébastien GARCIA · Entrepreneur individuel · SIREN 990 963 852<br>28 Rue du Maroc, 29270 Carhaix-Plouguer · <span onclick="handleEmailClick()" style="cursor:pointer;text-decoration:underline">sebastien.garcia29@outlook.fr</span></p>
    </div>
  </div>
</div>

<!-- ═══════════════ MODAL PAIEMENT ═══════════════ -->
<div id="pay-bg" class="modal-bg hidden" onclick="if(event.target===this)closePay()">
  <div class="modal">
    <div style="text-align:center;margin-bottom:20px">
      <div style="font-size:40px;margin-bottom:8px" id="pay-icon">🌱</div>
      <h3 style="font-size:26px;font-weight:300;margin-bottom:4px" id="pay-name">Petites Pousses</h3>
      <p style="font-size:14px;color:var(--text-m)" id="pay-sub">Enfants 6-11 ans</p>
      <div style="font-family:&#39;Cormorant Garamond&#39;,serif;font-size:40px;font-weight:300;margin:12px 0" id="pay-price">49€ <span style="font-size:18px;font-family:&#39;DM Sans&#39;,sans-serif">TTC</span></div>
    </div>
    <div class="warn-box"><p>⚠️ <strong>Rappel :</strong> Je ne suis ni médecin, ni psychologue, ni thérapeute. Ces outils ne remplacent pas un suivi professionnel. Aucune guérison n'est garantie.</p></div>
    <div class="legal-ck">
      <input type="checkbox" id="ck1" onchange="checkPay()">
      <label for="ck1"><strong>J'ai lu et j'accepte les CGV, les mentions légales et la politique de confidentialité (CNIL/RGPD)</strong> de Sérénum dans leur intégralité.</label>
    </div>
    <div class="legal-ck">
      <input type="checkbox" id="ck2" onchange="checkPay()">
      <label for="ck2"><strong>Cette case vaut acceptation et renonciation expresse à mon droit de rétractation de 14 jours</strong> (art. L.221-28 13° Code de la consommation), en demandant l'exécution immédiate du contenu numérique.</label>
    </div>
    <div id="pay-warn" style="font-size:12px;color:var(--rose);text-align:center;margin:8px 0;display:none">Cochez les deux cases pour continuer.</div>
    <div style="margin:16px 0 8px;padding:12px;background:var(--cream-d);border-radius:8px;display:flex;align-items:center;gap:8px">
      <span>🔒</span><span style="font-size:12px;color:var(--text-m)">Paiement sécurisé via <strong>Stripe</strong> · PCI-DSS · Vos données bancaires ne transitent pas par Sérénum.</span>
    </div>
    <button class="btn btn-sage" id="pay-btn" style="width:100%;font-size:15px;padding:14px;justify-content:center" disabled="" onclick="doPay()">Payer en sécurité via Stripe →</button>
    <button class="btn btn-out" style="width:100%;margin-top:8px;justify-content:center" onclick="closePay()">Annuler</button>
  </div>
</div>

<!-- ═══════════════ MODAL CREATOR ═══════════════ -->
<div id="creator-bg" style="display:none;position:fixed;inset:0;background:rgba(0,0,0,.7);z-index:500;align-items:center;justify-content:center;padding:20px" onclick="if(event.target===this)closeCreator()">
  <div class="creator-modal">
    <div id="creator-pin-screen">
      <div style="text-align:center;margin-bottom:24px">
        <div style="font-size:40px;margin-bottom:8px">🔐</div>
        <h3 style="font-size:24px;font-weight:300;margin-bottom:4px">Accès créateur</h3>
        <p style="font-size:13px;color:var(--text-m)">Code PIN requis</p>
      </div>
      <div style="display:flex;gap:8px;justify-content:center;margin-bottom:16px">
        <input type="password" id="pin-inp" maxlength="6" placeholder="••••" style="width:130px;text-align:center;font-size:24px;letter-spacing:8px;padding:12px;border:2px solid var(--border);border-radius:12px" oninput="tryPin()" onkeydown="if(event.key===&#39;Enter&#39;)tryPin(true)">
      </div>
      <div id="pin-err" style="text-align:center;font-size:13px;color:var(--rose);margin-bottom:12px;display:none">Code incorrect.</div>
      <div style="display:flex;gap:8px;justify-content:center">
        <button class="btn btn-sage btn-sm" onclick="tryPin(true)">Entrer</button>
        <button class="btn btn-out btn-sm" onclick="closeCreator()">Annuler</button>
      </div>
    </div>
    <div id="creator-content" style="display:none">
      <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:24px">
        <div><div style="font-size:11px;letter-spacing:2px;text-transform:uppercase;color:var(--sage);margin-bottom:4px">Mode créateur</div><h3 style="font-size:24px;font-weight:300">Contenu détaillé de Sérénum</h3></div>
        <button onclick="closeCreator()" style="background:none;border:none;font-size:22px;cursor:pointer;color:var(--text-m)">✕</button>
      </div>
      <div class="creator-offre">
        <div class="creator-offre-head" style="background:rgba(184,212,187,.15)" onclick="toggleC(&#39;c1&#39;)">🌱 Petites Pousses — 49€ <span id="c1-arrow">▼</span></div>
        <div class="creator-offre-body" id="c1">
          <div class="creator-section"><div class="creator-section-title">Respirations (4 exclusives)</div>
            <div class="creator-item"><strong>Cohérence cardiaque 3-6-5</strong> — 3x/jour, 6 resp/min, 5 min. Inspire 5s expire 5s. Voix guidée enfant.</div>
            <div class="creator-item"><strong>Bulle de savon</strong> — Inspire 4s, expire 6s très doucement. Ne pas faire éclater la bulle imaginaire. 3 cycles.</div>
            <div class="creator-item"><strong>Souffle du Lion</strong> — Inspire profond par le nez, expire fort bouche grande ouverte langue tirée. 5 cycles. Évacue la tension physique.</div>
            <div class="creator-item"><strong>Respiration Tortue</strong> — Inspire en rentrant la tête dans les épaules, expire en se détendant. 4 cycles.</div>
          </div>
          <div class="creator-section"><div class="creator-section-title">Exercices (3 exclusifs)</div>
            <div class="creator-item"><strong>Ma tortue intérieure</strong> — Visualisation guidée 8 min. L'enfant crée une carapace imaginaire refuge.</div>
            <div class="creator-item"><strong>Journal illustré des émotions</strong> — Humeur (5 émojis), école, amis, texte libre. Privé (parent ne lit pas le contenu). Streak affiché.</div>
            <div class="creator-item"><strong>Tableau de super-héros</strong> — Gamification : points, niveaux Bronze/Argent/Or. Motivation enfant.</div>
          </div>
          <div class="creator-section"><div class="creator-section-title">Dashboard parent</div>
            <div class="creator-item">Score anxiété /10 · Graphique humeur 7j · Alertes comportementales · Timeline exercices · Streak enfant</div>
          </div>
        </div>
      </div>
      <div class="creator-offre">
        <div class="creator-offre-head" style="background:rgba(168,204,204,.15)" onclick="toggleC(&#39;c2&#39;)">🌊 Cap Sérénité — 119€ <span id="c2-arrow">▼</span></div>
        <div class="creator-offre-body" id="c2">
          <div class="creator-section"><div class="creator-section-title">Respirations (3 exclusives — différentes O1)</div>
            <div class="creator-item"><strong>Respiration 4-7-8</strong> — Inspire 4s, retiens 7s, expire 8s. Anti-stress aigu, avant examen, pour dormir. 4 cycles.</div>
            <div class="creator-item"><strong>Respiration physiologique</strong> — Double inspiration nasale courte + longue expire. Réinitialise le SN en 30s. 5 cycles.</div>
            <div class="creator-item"><strong>Technique STOP</strong> — Stop / Take a breath / Observe / Proceed. Pleine conscience 4 étapes. 2-3 min.</div>
          </div>
          <div class="creator-section"><div class="creator-section-title">Exercices (4 exclusifs — différents O1)</div>
            <div class="creator-item"><strong>Carnet des victoires</strong> — 3 preuves de réussite/soir. Reconstruire la confiance face aux échecs scolaires. Quotidien.</div>
            <div class="creator-item"><strong>Journal émotionnel ado</strong> — Slider stress /10, humeur, sommeil, texte libre. Confidentiel (parents voient seulement "a écrit")</div>
            <div class="creator-item"><strong>Tracker stress scolaire</strong> — Suivi par matière et type d'événement (contrôle, exposé, interro). Identification des déclencheurs.</div>
            <div class="creator-item"><strong>Analyse tendances</strong> — Corrélation exercices pratiqués / niveau de stress. Montre ce qui fonctionne le mieux.</div>
          </div>
          <div class="creator-section"><div class="creator-section-title">Dashboard parent (plus discret)</div>
            <div class="creator-item">Résumé hebdo · Graphique humeur 30j · Nombre d'exercices · Pas d'accès au contenu du journal</div>
          </div>
        </div>
      </div>
      <div class="creator-offre">
        <div class="creator-offre-head" style="background:rgba(232,212,160,.15)" onclick="toggleC(&#39;c3&#39;)">⭐ Famille Unie — 189€ <span id="c3-arrow">▼</span></div>
        <div class="creator-offre-body" id="c3">
          <div class="creator-section"><div class="creator-section-title">Respirations (2 exclusives — différentes O1+O2)</div>
            <div class="creator-item"><strong>Vague de l'océan</strong> — Inspire en montant les bras comme une vague, expire en les descendant. Mouvement + respiration. 6 cycles.</div>
            <div class="creator-item"><strong>Respiration en duo</strong> — Parent + enfant synchronisent leur respiration. Crée le lien, apaise les deux. 5 min ensemble.</div>
          </div>
          <div class="creator-section"><div class="creator-section-title">Exercices (5 exclusifs — différents O1+O2)</div>
            <div class="creator-item"><strong>Ancrage 5-4-3-2-1</strong> — 5 vus / 4 entendus / 3 touchés / 2 sentis / 1 goûté. Interrompt spirale anxieuse en 3 min. Tous âges.</div>
            <div class="creator-item"><strong>Relaxation de Jacobson</strong> — Contraction-relâchement musculaire progressif tête-pieds. Validé cliniquement. 15-20 min.</div>
            <div class="creator-item"><strong>Mon lieu de sécurité</strong> — Visualisation guidée 12 min. Création d'un refuge mental personnalisé.</div>
            <div class="creator-item"><strong>Protocole dialogue parent-enfant</strong> — Scripts de communication selon âge et situation. Comment parler sans braquer.</div>
            <div class="creator-item"><strong>Journal partagé famille</strong> — Opt-in. L'enfant choisit ce qu'il veut montrer. Lien parent-enfant.</div>
          </div>
          <div class="creator-section"><div class="creator-section-title">Module harcèlement (version famille)</div>
            <div class="creator-item">Checklist 10 signaux · Scripts dialogue 6-11 ans et 12-18 ans · Plan action 4 étapes · Numéros utiles</div>
          </div>
          <div class="creator-section"><div class="creator-section-title">Dashboard famille (2 profils)</div>
            <div class="creator-item">2 enfants simultanés · Alertes croisées · Comparaison évolution · Graphiques croisés famille</div>
          </div>
        </div>
      </div>
      <div class="creator-offre" style="border:2px solid var(--rose-l)">
        <div class="creator-offre-head" style="background:rgba(232,187,187,.15)" onclick="toggleC(&#39;c4&#39;)">🛡️ Intensif &amp; Harcèlement — 269€ <span id="c4-arrow">▼</span></div>
        <div class="creator-offre-body" id="c4">
          <div class="creator-section"><div class="creator-section-title" style="color:var(--rose)">3 techniques EXCLUSIVES anti-harcèlement (nulle part ailleurs)</div>
            <div class="creator-item"><strong>🛡️ Mon armure du matin</strong> — Routine 5 min avant l'école : box breathing 1 min + visualisation bouclier invisible + phrase de confiance personnalisée choisie par l'enfant. À faire les jours difficiles. L'enfant arrive préparé, pas subi.</div>
            <div class="creator-item"><strong>🗣️ La phrase qui coupe court</strong> — UNE phrase neutre par âge (6-11 / 12-18) à dire face au harceleur, ni agressive ni soumise. Désamorce sans escalader. Jeux de rôle parent-enfant guidés (15 min). Ex 6-11 ans : "C'est ton opinion." et partir. Ex 12-18 ans : "OK." + silence.</div>
            <div class="creator-item"><strong>📓 Mes preuves de valeur</strong> — Journal structuré : 3 preuves concrètes de valeur chaque soir (ami qui a souri, bonne réponse, moment sympa). Contre-attaque directe contre les pensées négatives instillées par le harcèlement. Guide parent pour accompagner.</div>
          </div>
          <div class="creator-section"><div class="creator-section-title">Respirations avancées (2 exclusives — différentes O1+O2+O3)</div>
            <div class="creator-item"><strong>Box Breathing 4-4-4-4</strong> — Inspire 4s / retiens 4s / expire 4s / pause 4s. Technique forces spéciales. Crises intenses. 5-10 min.</div>
            <div class="creator-item"><strong>Protocole crise 5 min</strong> — Séquence d'urgence : box 1 min + ancrage 54321 + phrase d'ancrage. Utilisable seul par l'enfant.</div>
          </div>
          <div class="creator-section"><div class="creator-section-title">Module harcèlement renforcé (vs Famille Unie)</div>
            <div class="creator-item">Checklist + analyse automatique risque (faible/modéré/élevé) · Scripts cyber-harcèlement (absent O3) · Journal confidentiel ado TOTAL (même "a écrit" masqué) · Numéros urgence intégrés dans l'app</div>
          </div>
          <div class="creator-section"><div class="creator-section-title">Dashboard intensif (4 profils)</div>
            <div class="creator-item">4 enfants simultanés · Alertes classées par urgence · Évolution 30 jours · Efficacité par exercice (avant/après)</div>
          </div>
        </div>
      </div>
      <div style="text-align:center;padding-top:16px;border-top:1px solid var(--border)">
        <button class="btn btn-out btn-sm" onclick="closeCreator()">Fermer</button>
      </div>
    </div>
  </div>
</div>

<script>
// ═══════════ DATA ═══════════
const OFFRES=[
  {name:'Petites Pousses',sub:'Enfants 6-11 ans',prix:'49€',icon:'🌱',color:'sage',stripe:'https://buy.stripe.com/7sYfZi1jMcBD9643p2g7e0j',
   roles:['parent','enfant'],profiles:1,
   nav:[{id:'overview',ico:'🏠',label:'Tableau de bord'},{id:'journal',ico:'📓',label:'Mon journal'},{id:'exercices',ico:'🫁',label:'Exercices'},{id:'evolution',ico:'📈',label:'Évolution'}]},
  {name:'Cap Sérénité',sub:'Adolescents 12-18 ans',prix:'119€',icon:'🌊',color:'teal',stripe:'https://buy.stripe.com/3cI7sM8Me0SVaa8aRug7e0g',
   roles:['parent','ado'],profiles:1,
   nav:[{id:'overview',ico:'🏠',label:'Tableau de bord'},{id:'journal',ico:'📓',label:'Mon journal'},{id:'exercices',ico:'🫁',label:'Exercices'},{id:'tracker',ico:'📊',label:'Tracker stress'},{id:'evolution',ico:'📈',label:'Évolution'}]},
  {name:'Famille Unie',sub:'Famille complète · 2 profils',prix:'189€',icon:'⭐',color:'gold',stripe:'https://buy.stripe.com/3cI28s5A2cBDcigbVyg7e0h',
   roles:['parent','enfant','ado'],profiles:2,
   nav:[{id:'overview',ico:'🏠',label:'Tableau de bord'},{id:'journal',ico:'📓',label:'Mon journal'},{id:'exercices',ico:'🫁',label:'Exercices'},{id:'harcelement',ico:'🛡️',label:'Harcèlement'},{id:'evolution',ico:'📈',label:'Évolution'}]},
  {name:'Intensif & Harcèlement',sub:'Crises sévères · Anti-harcèlement · 4 profils',prix:'269€',icon:'🛡️',color:'rose',stripe:'https://buy.stripe.com/6oU8wQ4vY6dfgyw0cQg7e0k',
   roles:['parent','enfant','ado'],profiles:4,
   nav:[{id:'overview',ico:'🏠',label:'Tableau de bord'},{id:'journal',ico:'📓',label:'Mon journal'},{id:'exercices',ico:'🫁',label:'Exercices'},{id:'harcelement',ico:'🛡️',label:'Harcèlement'},{id:'armure',ico:'🛡️',label:'Armure du matin'},{id:'evolution',ico:'📈',label:'Évolution'}]}
];

// Données humeur simulées par rôle/profil
const moodData={
  enfant:{week:[7,5,8,6,9,7,8],month:[6,7,5,8,6,9,7,8,7,6,8,9,7,8,6,7,5,8,9,7,6,8,7,9,8,7,6,8,7,8]},
  ado:{week:[5,4,6,5,7,6,5],month:[5,4,6,5,7,6,5,4,6,7,5,6,4,5,7,6,5,4,6,5,7,6,7,5,4,6,5,7,6,5]},
  emma:{week:[6,5,7,6,9,7,8],name:'Emma',age:9},
  leo:{week:[5,4,6,5,7,6,5],name:'Léo',age:14}
};

const jours=['Lun','Mar','Mer','Jeu','Ven','Sam','Dim'];

// State
let currentOffre=2; // Famille Unie par défaut démo
let currentRole='parent';
let currentSection='overview';
let currentMood=null;
let moodHistory={enfant:[],ado:[]};
let journalEntries={parent:[],enfant:[],ado:[]};
let stressData={maths:6,francais:4,anglais:3,histoire:5,science:4};
let signalsChecked=new Set();
let respRunning=false,respTimer=null,respCount=0,respPhaseIdx=0,respCycleCount=0,currentResp=null;

// ═══════════ NAVIGATION ═══════════
function goPage(id){
  document.querySelectorAll('.page').forEach(p=>p.classList.remove('active'));
  document.querySelectorAll('.nav-link').forEach(l=>l.classList.remove('active'));
  document.getElementById('page-'+id).classList.add('active');
  if(id==='dash') initDash();
  window.scrollTo(0,0);
}

// ═══════════ DASHBOARD ═══════════
function initDash(){
  const o=OFFRES[currentOffre];
  // Sidebar
  const nav=document.getElementById('sidebar-nav');
  nav.innerHTML='';
  o.nav.forEach(item=>{
    const btn=document.createElement('button');
    btn.className='s-item'+(item.id===currentSection?' active':'');
    btn.innerHTML=`<span class="ico">${item.ico}</span>${item.label}`;
    btn.onclick=()=>switchSection(item.id,btn);
    nav.appendChild(btn);
  });
  // Locked items based on offre
  if(currentOffre<3){
    const lock=document.createElement('div');
    lock.className='s-lock';
    lock.innerHTML=`<span class="ico">🔒</span>Armure du matin (Intensif)`;
    nav.appendChild(lock);
  }
  if(currentOffre<2){
    ['Harcèlement','Tracker stress'].forEach(l=>{
      const lock=document.createElement('div');
      lock.className='s-lock';
      lock.innerHTML=`<span class="ico">🔒</span>${l}`;
      nav.appendChild(lock);
    });
  }
  // Badge
  document.getElementById('sidebar-offre-badge').textContent=o.icon+' '+o.name;
  // Role switcher
  renderRoles();
  renderSection();
}

function switchSection(id,btn){
  currentSection=id;
  document.querySelectorAll('.s-item').forEach(i=>i.classList.remove('active'));
  if(btn)btn.classList.add('active');
  renderSection();
}

function switchRole(role){
  currentRole=role;
  document.querySelectorAll('.r-btn').forEach(b=>{
    b.classList.toggle('active',b.dataset.role===role);
  });
  renderSection();
}

function renderRoles(){
  const o=OFFRES[currentOffre];
  const sw=document.querySelector('.role-sw');
  if(!sw)return;
  sw.innerHTML='';
  const roleLabels={parent:'👨‍👩‍👧 Parent',enfant:'🧒 Enfant',ado:'🧑 Ado'};
  ['parent','enfant','ado'].forEach(r=>{
    const btn=document.createElement('button');
    btn.className='r-btn'+(r===currentRole?' active':'')+(o.roles.includes(r)?'':' locked');
    btn.dataset.role=r;
    btn.textContent=roleLabels[r];
    if(o.roles.includes(r)) btn.onclick=()=>switchRole(r);
    else btn.title='Non inclus dans cette offre';
    sw.appendChild(btn);
  });
}

function renderSection(){
  const main=document.getElementById('dash-main');
  const o=OFFRES[currentOffre];
  const greetings={parent:'Bonjour, Sébastien 👋',enfant:'Bonjour Emma ! 🌟',ado:'Salut Léo 👋'};
  const top=`<div class="dash-top">
    <div class="greeting"><h2>${greetings[currentRole]}</h2><p>Vendredi 29 mai 2026</p></div>
    <div class="role-sw"></div>
  </div>`;
  let content='';
  if(currentSection==='overview') content=renderOverview();
  else if(currentSection==='journal') content=renderJournal();
  else if(currentSection==='exercices') content=renderExercices();
  else if(currentSection==='harcelement') content=renderHarcelement();
  else if(currentSection==='tracker') content=renderTracker();
  else if(currentSection==='armure') content=renderArmure();
  else if(currentSection==='evolution') content=renderEvolution();
  main.innerHTML=top+content;
  renderRoles();
  // Re-init interactive elements
  if(currentSection==='exercices') initExTabs();
  if(currentSection==='harcelement') initHarcTabs();
}

// ═══════════ OVERVIEW ═══════════
function renderOverview(){
  const o=OFFRES[currentOffre];
  if(currentRole==='parent') return renderOverviewParent();
  if(currentRole==='enfant') return renderOverviewEnfant();
  if(currentRole==='ado') return renderOverviewAdo();
  return '';
}

function renderOverviewParent(){
  const o=OFFRES[currentOffre];
  const multi=o.profiles>1;
  return `
  <div class="metrics">
    <div class="metric"><div class="metric-l">Score anxiété${multi?' Emma':''}</div><div class="metric-v" style="color:#C47B7B">6.4</div><div class="metric-s">/10 · ↑ depuis hier</div></div>
    ${multi?`<div class="metric"><div class="metric-l">Score anxiété Léo</div><div class="metric-v" style="color:#C4A24A">4.2</div><div class="metric-s">/10 · stable</div></div>`:''}
    <div class="metric"><div class="metric-l">Exercices cette semaine</div><div class="metric-v">12</div><div class="metric-s">${multi?'Emma: 8 · Léo: 4':'cette semaine'}</div></div>
    <div class="metric"><div class="metric-l">Streak${multi?' Emma':''}</div><div class="metric-v" style="color:var(--sage)">7🔥</div><div class="metric-s">jours consécutifs</div></div>
  </div>
  <div class="grid2">
    <div class="card">
      <div class="card-title">Alertes parentales</div>
      <div class="alert alert-r">⚠️ <div><strong>Emma (9 ans)</strong> — Anxiété élevée (6.4/10) depuis 3 jours. Surveillance recommandée.</div></div>
      <div class="alert alert-y">⏰ <div>${multi?'<strong>Léo (14 ans)</strong> — Journal non complété depuis 2 jours.':'Journal non complété depuis 2 jours. Encouragez votre enfant.'}</div></div>
      <div class="alert alert-g">✅ <div><strong>${multi?'Emma':'Votre enfant'}</strong> — 3 exercices complétés aujourd'hui. Excellent !</div></div>
    </div>
    <div class="card">
      <div class="card-title">Humeur cette semaine</div>
      ${multi?'<div style="font-size:12px;color:var(--text-m);margin-bottom:8px">Emma (rose) · Léo (teal)</div>':''}
      <div class="bars">
        ${jours.map((j,i)=>`<div class="bar-col">
          ${multi?`<div class="bar" style="height:${moodData.leo.week[i]*9}%;background:var(--teal-l)"></div>`:''}
          <div class="bar" style="height:${moodData.emma.week[i]*9}%;background:var(--rose-l)"></div>
          <div class="bar-lbl">${j}</div>
        </div>`).join('')}
      </div>
      <div style="font-size:11px;color:var(--text-l);text-align:center;margin-top:6px">Plus haut = meilleure humeur</div>
    </div>
  </div>
  <div class="card full">
    <div class="card-title">Activité récente</div>
    <div class="timeline">
      <div class="tl-item"><div class="tl-time">Aujourd'hui · 16h32</div><div class="tl-text">${multi?'Emma a':'A'} complété "Bulle de savon" (3 cycles) — Humeur après : 😊</div></div>
      <div class="tl-item"><div class="tl-time">Aujourd'hui · 14h10</div><div class="tl-text">${multi?'Emma a':'A'} écrit dans son journal des émotions</div></div>
      ${multi?`<div class="tl-item"><div class="tl-time">Hier · 20h15</div><div class="tl-text">Léo a complété "Respiration 4-7-8" — Humeur après : 😐</div></div>`:''}
      <div class="tl-item"><div class="tl-time">Hier · 18h00</div><div class="tl-text">${multi?'Emma a':'A'} complété "Cohérence cardiaque" (5 min)</div></div>
    </div>
  </div>`;
}

function renderOverviewEnfant(){
  const saved=currentMood||'😊';
  return `
  <div style="background:linear-gradient(135deg,rgba(184,212,187,.3),rgba(250,247,242,.8));border-radius:var(--rxl);padding:28px;margin-bottom:20px;text-align:center">
    <div style="font-size:52px;margin-bottom:8px" id="enfant-mood-big">${saved}</div>
    <h2 style="font-size:28px;font-weight:300;margin-bottom:4px">Comment tu te sens aujourd'hui ?</h2>
    <div class="mood-row" style="justify-content:center">
      ${['😄','😊','😐','😟','😢'].map(e=>`<button class="mood-btn${e===saved?' sel':''}" onclick="setMoodEnfant('${e}',this)">${e}</button>`).join('')}
    </div>
  </div>
  <div class="metrics" style="grid-template-columns:repeat(3,1fr)">
    <div class="metric"><div class="metric-l">Mon humeur</div><div class="metric-v">${saved}</div><div class="metric-s">Aujourd'hui</div></div>
    <div class="metric"><div class="metric-l">Mon streak</div><div class="metric-v" style="color:var(--sage)">7🔥</div><div class="metric-s">jours</div></div>
    <div class="metric"><div class="metric-l">Exercices</div><div class="metric-v">8</div><div class="metric-s">cette semaine</div></div>
  </div>
  <div class="grid2">
    <div class="card">
      <div class="card-title">Ma bulle du jour 🫧</div>
      <p style="font-size:14px;color:var(--text-m);margin-bottom:14px">Fais une respiration maintenant pour te sentir mieux !</p>
      <button class="btn btn-sage" style="width:100%" onclick="currentSection='exercices';renderSection()">Commencer un exercice →</button>
    </div>
    <div class="card">
      <div class="card-title">Mes émotions 🌈</div>
      <div class="bars" style="height:70px">
        ${jours.map((j,i)=>`<div class="bar-col"><div class="bar" style="height:${moodData.enfant.week[i]*10}%;background:var(--sage-l)"></div><div class="bar-lbl">${j.slice(0,2)}</div></div>`).join('')}
      </div>
    </div>
  </div>
  <div class="card">
    <div class="card-title">Mon tableau de super-héros 🦸</div>
    <div style="display:flex;gap:12px;flex-wrap:wrap">
      <div style="text-align:center;padding:12px;background:var(--cream-d);border-radius:10px;min-width:80px"><div style="font-size:26px">🫁</div><div style="font-size:11px;color:var(--text-m)">Respirations</div><div style="font-weight:500">24</div></div>
      <div style="text-align:center;padding:12px;background:var(--cream-d);border-radius:10px;min-width:80px"><div style="font-size:26px">📓</div><div style="font-size:11px;color:var(--text-m)">Journaux</div><div style="font-weight:500">7</div></div>
      <div style="text-align:center;padding:12px;background:var(--cream-d);border-radius:10px;min-width:80px"><div style="font-size:26px">🌟</div><div style="font-size:11px;color:var(--text-m)">Points</div><div style="font-weight:500">340</div></div>
      <div style="text-align:center;padding:12px;background:rgba(184,212,187,.2);border-radius:10px;min-width:80px;border:1px dashed var(--sage-l)"><div style="font-size:26px">🏆</div><div style="font-size:11px;color:var(--text-m)">Niveau</div><div style="font-weight:500;color:var(--sage)">Or</div></div>
    </div>
  </div>`;
}

function renderOverviewAdo(){
  return `
  <div style="background:linear-gradient(135deg,rgba(168,204,204,.2),rgba(250,247,242,.9));border-radius:var(--rxl);padding:28px;margin-bottom:20px">
    <h2 style="font-size:32px;font-weight:300;margin-bottom:4px">Prends une minute pour toi.</h2>
    <p style="font-size:15px;color:var(--text-m)">Comment tu te sens aujourd'hui, vraiment ?</p>
    <div class="mood-row" style="margin-top:12px">
      ${['😄','😊','😐','😟','😢'].map(e=>`<button class="mood-btn${e===currentMood?' sel':''}" onclick="setMoodAdo('${e}',this)">${e}</button>`).join('')}
    </div>
  </div>
  <div class="metrics">
    <div class="metric"><div class="metric-l">Niveau de stress</div><div class="metric-v" style="color:var(--gold)">4.5</div><div class="metric-s">/10 · en baisse 👍</div></div>
    <div class="metric"><div class="metric-l">Streak</div><div class="metric-v">4🔥</div><div class="metric-s">jours</div></div>
    <div class="metric"><div class="metric-l">Exercices</div><div class="metric-v">4</div><div class="metric-s">cette semaine</div></div>
    <div class="metric"><div class="metric-l">Journal</div><div class="metric-v" style="color:var(--rose)">2j</div><div class="metric-s">sans écrire</div></div>
  </div>
  <div class="grid2">
    <div class="card">
      <div class="card-title">Aujourd'hui</div>
      <div class="alert alert-b" style="margin-bottom:12px">📅 Contrôle de maths demain. Tu veux faire une technique anti-stress ?</div>
      <button class="btn btn-teal btn-sm" onclick="currentSection='exercices';renderSection()">Voir les exercices →</button>
    </div>
    <div class="card">
      <div class="card-title">Mon humeur</div>
      <div class="bars" style="height:70px">
        ${jours.map((j,i)=>`<div class="bar-col"><div class="bar" style="height:${moodData.ado.week[i]*12}%;background:var(--teal-l)"></div><div class="bar-lbl">${j.slice(0,2)}</div></div>`).join('')}
      </div>
    </div>
  </div>`;
}

// ═══════════ JOURNAL ═══════════
function renderJournal(){
  if(currentRole==='parent') return renderJournalParent();
  if(currentRole==='enfant') return renderJournalEnfant();
  if(currentRole==='ado') return renderJournalAdo();
  return '';
}

function renderJournalParent(){
  const entries=journalEntries.parent;
  return `
  <div style="background:linear-gradient(135deg,rgba(184,212,187,.3),rgba(250,247,242,.9));border-radius:var(--rxl);padding:24px;margin-bottom:20px">
    <h3 style="font-size:26px;font-weight:300;margin-bottom:4px">Journal parental 📔</h3>
    <p style="font-size:14px;color:var(--text-m)">Notez vos observations pour garder une trace de l'évolution</p>
  </div>
  <div class="grid2">
    <div class="card">
      <div class="card-title">Observation du jour</div>
      <select id="j-enfant" style="width:100%;margin-bottom:12px">${OFFRES[currentOffre].profiles>1?'<option>Emma (9 ans)</option><option>Léo (14 ans)</option>':'<option>Votre enfant</option>'}</select>
      <div style="margin-bottom:10px">
        <div style="font-size:13px;color:var(--text-m);margin-bottom:6px">Humeur observée :</div>
        <div class="mood-row">
          ${['😄','😊','😐','😟','😢'].map(e=>`<button class="mood-btn" onclick="this.parentNode.querySelectorAll('.mood-btn').forEach(b=>b.classList.remove('sel'));this.classList.add('sel')">${e}</button>`).join('')}
        </div>
      </div>
      <textarea class="journal-box" id="j-parent-text" placeholder="Comportement à l'école, appétit, sommeil, remarques importantes..."></textarea>
      <button class="btn btn-sage" style="width:100%;margin-top:12px;justify-content:center" onclick="saveJournalEntry('parent')">Enregistrer l'observation</button>
    </div>
    <div class="card">
      <div class="card-title">Entrées précédentes</div>
      ${entries.length===0?`<div class="timeline">
        <div class="tl-item"><div class="tl-time">28 mai · Emma</div><div class="tl-text">Rentrée agitée. Pleurs pour les devoirs de maths. Calmée après la respiration bulle.</div></div>
        <div class="tl-item"><div class="tl-time">27 mai · Emma</div><div class="tl-text">Très bonne journée. Souriante, appétit normal.</div></div>
        <div class="tl-item"><div class="tl-time">26 mai · Léo</div><div class="tl-text">Renfermé le soir. N'a pas voulu parler du collège.</div></div>
      </div>`:entries.map(e=>`<div class="tl-item"><div class="tl-time">${e.date}</div><div class="tl-text">${e.mood} ${e.text}</div></div>`).join('')}
      <div id="j-parent-saved" style="display:none" class="alert alert-g" style="margin-top:12px">✅ Observation enregistrée !</div>
    </div>
  </div>`;
}

function renderJournalEnfant(){
  const entries=journalEntries.enfant;
  return `
  <div style="background:linear-gradient(135deg,rgba(184,212,187,.4),rgba(250,247,242,.9));border-radius:var(--rxl);padding:24px;margin-bottom:20px">
    <h3 style="font-size:26px;font-weight:300;margin-bottom:4px">Mon journal secret 🔒</h3>
    <p style="font-size:14px;color:var(--text-m)">C'est ton espace. Tes parents ne lisent pas ce que tu écris ici.</p>
  </div>
  <div class="card" style="margin-bottom:20px">
    <div style="text-align:center;margin-bottom:16px">
      <div style="font-size:18px;font-weight:400;font-family:'Cormorant Garamond',serif;margin-bottom:10px">Comment tu te sens aujourd'hui ?</div>
      <div class="mood-row" style="justify-content:center">
        ${['😄','😊','😐','😟','😢'].map(e=>`<button class="mood-btn" onclick="this.parentNode.querySelectorAll('.mood-btn').forEach(b=>b.classList.remove('sel'));this.classList.add('sel')">${e}</button>`).join('')}
      </div>
    </div>
    <div style="display:grid;grid-template-columns:1fr 1fr;gap:12px;margin-bottom:14px">
      <div><label style="font-size:13px;color:var(--text-m);display:block;margin-bottom:6px">À l'école aujourd'hui ?</label>
        <select style="width:100%"><option>C'était bien 😊</option><option>Ça allait 😐</option><option>C'était difficile 😟</option><option>C'était nul 😢</option></select></div>
      <div><label style="font-size:13px;color:var(--text-m);display:block;margin-bottom:6px">Avec mes amis ?</label>
        <select style="width:100%"><option>Super bien 😄</option><option>Bien 😊</option><option>Comme ci comme ça 😐</option><option>Mal 😟</option><option>J'étais seul(e) 😢</option></select></div>
    </div>
    <textarea class="journal-box" id="j-enfant-text" placeholder="Raconte ta journée... Ce qui s'est passé, ce que tu as ressenti, ce qui t'a rendu heureux ou triste..." style="min-height:120px"></textarea>
    <button class="btn btn-sage" style="width:100%;margin-top:12px;justify-content:center" onclick="saveJournalEntry('enfant')">Sauvegarder mon journal 💚</button>
    <div id="j-enfant-saved" style="display:none;margin-top:10px" class="alert alert-g">💚 Ton journal est sauvegardé ! Bien joué !</div>
  </div>
  <div class="card">
    <div class="card-title">Mes émotions cette semaine 🌈</div>
    <div class="bars" style="height:80px">
      ${jours.map((j,i)=>`<div class="bar-col"><div class="bar" style="height:${moodData.enfant.week[i]*10}%;background:var(--sage-l)"></div><div class="bar-lbl">${j.slice(0,2)}</div></div>`).join('')}
    </div>
    <div style="display:grid;grid-template-columns:repeat(7,1fr);gap:4px;margin-top:12px">
      ${jours.map((j,i)=>`<div class="streak-day${i<6?' done':' today'}" style="${i<6?'':'font-weight:600'}">${i<6?'✓':'★'}</div>`).join('')}
    </div>
  </div>`;
}

function renderJournalAdo(){
  const o=OFFRES[currentOffre];
  const isPrivate=currentOffre===3;
  return `
  <div style="background:linear-gradient(135deg,rgba(168,204,204,.3),rgba(250,247,242,.9));border-radius:var(--rxl);padding:24px;margin-bottom:20px">
    <h3 style="font-size:26px;font-weight:300;margin-bottom:4px">Mon espace ${isPrivate?'confidentiel 🔐':'privé 🔒'}</h3>
    <p style="font-size:14px;color:var(--text-m)">${isPrivate?'Journal confidentiel — tes parents ne voient pas le contenu, ni même que tu as écrit.':'Journal privé — tes parents voient seulement que tu as écrit, pas le contenu.'}</p>
  </div>
  <div class="card" style="margin-bottom:20px">
    <div style="display:grid;grid-template-columns:1fr 1fr 1fr;gap:16px;margin-bottom:16px">
      <div>
        <div style="font-size:12px;color:var(--text-l);margin-bottom:8px;text-transform:uppercase;letter-spacing:.5px">Niveau de stress</div>
        <input type="range" min="0" max="10" value="4" id="stress-slider" oninput="document.getElementById('stress-val').textContent=this.value" style="width:100%"/>
        <div style="font-size:32px;font-weight:300;font-family:'Cormorant Garamond',serif;text-align:center" id="stress-val">4</div>
        <div style="font-size:11px;color:var(--text-l);text-align:center">/10</div>
      </div>
      <div>
        <div style="font-size:12px;color:var(--text-l);margin-bottom:8px;text-transform:uppercase;letter-spacing:.5px">Humeur</div>
        <div class="mood-row" style="flex-wrap:wrap;gap:6px;justify-content:center">
          ${['😄','😐','😟'].map(e=>`<button class="mood-btn" onclick="this.parentNode.querySelectorAll('.mood-btn').forEach(b=>b.classList.remove('sel'));this.classList.add('sel')">${e}</button>`).join('')}
        </div>
      </div>
      <div>
        <div style="font-size:12px;color:var(--text-l);margin-bottom:8px;text-transform:uppercase;letter-spacing:.5px">Sommeil</div>
        <select style="width:100%;margin-top:4px"><option>Bien dormi</option><option>Moyen</option><option>Mal dormi</option><option>Insomnie</option></select>
      </div>
    </div>
    <textarea class="journal-box" id="j-ado-text" placeholder="Libère-toi... Écris ce que tu veux, personne ne lira ça sauf toi. Tu peux parler de l'école, des amis, de ce qui te pèse, de tes rêves..." style="min-height:140px"></textarea>
    <div style="background:var(--cream-d);border-radius:8px;padding:10px 14px;margin:12px 0;font-size:12px;color:var(--text-m)">
      Si tu traverses quelque chose de difficile : <strong>📞 3018</strong> (harcèlement, gratuit, anonyme) · <strong>📞 3114</strong> (mal-être, 24h/24)
    </div>
    <button class="btn btn-teal" style="width:100%;justify-content:center" onclick="saveJournalEntry('ado')">Sauvegarder en privé 🔐</button>
    <div id="j-ado-saved" style="display:none;margin-top:10px" class="alert alert-b">🔐 Sauvegardé de façon confidentielle.</div>
  </div>`;
}

function saveJournalEntry(role){
  const el=document.getElementById('j-'+role+'-saved');
  const txt=document.getElementById('j-'+role+'-text');
  if(el){el.style.display='flex';setTimeout(()=>el.style.display='none',3000);}
  if(txt&&txt.value){
    journalEntries[role].unshift({date:'Aujourd\'hui',text:txt.value.slice(0,60)+'...',mood:'😊'});
    txt.value='';
  }
}

// ═══════════ EXERCICES ═══════════
const RESP_PATTERNS={
  bulle:{name:'🫧 Bulle de savon',desc:'Expire très doucement, comme si tu soufflais une bulle fragile. Ne la fais pas éclater !',phases:[{l:'Inspire',d:4,cls:'inhale'},{l:'Expire doucement',d:6,cls:'exhale'}],cycles:3,offre:0},
  lion:{name:'🦁 Souffle du Lion',desc:'Inspire profondément par le nez. Expire fort, bouche grande ouverte, langue sortie !',phases:[{l:'Inspire fort',d:3,cls:'inhale'},{l:'Rugis !',d:2,cls:'exhale'}],cycles:5,offre:0},
  coeur:{name:'💚 Cohérence cardiaque',desc:'3 fois par jour, 6 respirations par minute, 5 minutes. La technique la plus efficace.',phases:[{l:'Inspire',d:5,cls:'inhale'},{l:'Expire',d:5,cls:'exhale'}],cycles:6,offre:0},
  '478':{name:'🌙 Respiration 4-7-8',desc:'Technique puissante pour calmer le système nerveux avant un examen ou pour dormir.',phases:[{l:'Inspire',d:4,cls:'inhale'},{l:'Retiens',d:7,cls:'hold'},{l:'Expire',d:8,cls:'exhale'}],cycles:4,offre:1},
  physio:{name:'⚡ Respiration physiologique',desc:'Double inspiration + longue expiration. Réinitialise le système nerveux en 30 secondes.',phases:[{l:'Inspire court',d:2,cls:'inhale'},{l:'Encore',d:1,cls:'inhale'},{l:'Expire long',d:7,cls:'exhale'}],cycles:5,offre:1},
  vague:{name:'🌊 Vague de l\'océan',desc:'Monte les bras avec l\'inspiration comme une vague, descends à l\'expiration.',phases:[{l:'Monte les bras',d:4,cls:'inhale'},{l:'Descends',d:4,cls:'exhale'}],cycles:6,offre:2},
  box:{name:'📦 Box Breathing 4-4-4-4',desc:'Technique des forces spéciales. Pour les crises intenses. 4 temps égaux.',phases:[{l:'Inspire',d:4,cls:'inhale'},{l:'Retiens',d:4,cls:'hold'},{l:'Expire',d:4,cls:'exhale'},{l:'Pause',d:4,cls:'hold'}],cycles:5,offre:3}
};

function renderExercices(){
  return `
  <div class="ex-tabs">
    <button class="ex-tab active" data-panel="resp" onclick="switchExTab(this,'resp')">🫁 Respirations</button>
    <button class="ex-tab" data-panel="relax" onclick="switchExTab(this,'relax')">🧘 Relaxation</button>
    <button class="ex-tab" data-panel="cognitif" onclick="switchExTab(this,'cognitif')">🧠 Cognitif</button>
  </div>
  <div id="ex-resp" class="ex-panel active">
    <div class="resp-player">
      <div class="resp-phase" id="resp-phase">Choisissez une technique ci-dessous</div>
      <div class="resp-circle idle" id="resp-circ">
        <div style="text-align:center"><div id="resp-count" style="font-family:'Cormorant Garamond',serif;font-size:52px;font-weight:300;color:var(--sage)">▶</div></div>
      </div>
      <div class="resp-prog"><div class="resp-bar" id="resp-bar"></div></div>
      <div class="resp-cycles" id="resp-cycles">Sélectionnez une technique</div>
      <div class="resp-btns">
        ${Object.entries(RESP_PATTERNS).map(([k,p])=>{
          const locked=p.offre>currentOffre;
          return `<button class="btn btn-sm ${locked?'btn-out':'btn-sage'}" ${locked?'disabled title="Offre supérieure requise 🔒"':''} onclick="startResp('${k}')">${p.name}</button>`;
        }).join('')}
        <button class="btn btn-out btn-sm" onclick="stopResp()">⏹ Arrêter</button>
      </div>
    </div>
    <div id="resp-desc-box" style="font-size:14px;color:var(--text-m);text-align:center;padding:10px;background:var(--cream-d);border-radius:8px;margin-bottom:16px;display:none"></div>
    ${Object.entries(RESP_PATTERNS).map(([k,p])=>{
      const locked=p.offre>currentOffre;
      const offreName=OFFRES[p.offre].name;
      return `<div class="ex-card${locked?' locked':''}" onclick="${locked?'showLockMsg()':'startResp(\''+k+'\')'}">
        <span class="ex-tag ${locked?'badge-rose':'badge-sage'}">${locked?'🔒 '+offreName:'✓ Inclus'}</span>
        <h4>${p.name}</h4>
        <p>${p.desc}</p>
        <div class="ex-dur">⏱ ${p.cycles * p.phases.reduce((a,ph)=>a+ph.d,0)}s par cycle · ${p.cycles} cycles</div>
      </div>`;
    }).join('')}
  </div>
  <div id="ex-relax" class="ex-panel">
    ${renderRelaxExercices()}
  </div>
  <div id="ex-cognitif" class="ex-panel">
    ${renderCognitifExercices()}
  </div>`;
}

function renderRelaxExercices(){
  const exs=[
    {name:'🐢 Ma tortue intérieure',desc:"Visualisation guidée 8 min. L'enfant crée une carapace imaginaire refuge où il se sent en sécurité.",dur:'8 min',offre:0},
    {name:'🏝️ Mon lieu de sécurité',desc:"Visualisation guidée 12 min. Création d'un refuge mental personnalisé, riche en détails sensoriels.",dur:'12 min',offre:2},
    {name:'💪 Relaxation de Jacobson',desc:"Contraction-relâchement musculaire progressif de la tête aux pieds. Cliniquement validé pour l'anxiété.",dur:'15-20 min',offre:2},
    {name:'🛡️ Mon armure du matin',desc:"Routine 5 min avant l'école. Box breathing + visualisation bouclier + phrase de confiance. Pour les jours difficiles.",dur:'5 min',offre:3},
    {name:'📓 Mes preuves de valeur',desc:"3 preuves concrètes de valeur chaque soir. Reconstruit l'estime face au harcèlement. Guide parent inclus.",dur:'5 min/soir',offre:3}
  ];
  return exs.map(e=>{
    const locked=e.offre>currentOffre;
    return `<div class="ex-card${locked?' locked':''}" onclick="${locked?'showLockMsg()':'\'\''}">
      <span class="ex-tag ${locked?'badge-rose':'badge-sage'}">${locked?'🔒 '+OFFRES[e.offre].name:'✓ Inclus'}</span>
      <h4>${e.name}</h4>
      <p>${e.desc}</p>
      <div class="ex-dur">⏱ ${e.dur}</div>
    </div>`;
  }).join('');
}

function renderCognitifExercices(){
  const exs=[
    {name:'🖐️ Ancrage 5-4-3-2-1',desc:"5 choses vues / 4 entendues / 3 touchées / 2 senties / 1 goûtée. Interrompt une spirale anxieuse en 3 min.",dur:'3-5 min',offre:2},
    {name:'⛔ Technique STOP',desc:"Stop / Take a breath / Observe / Proceed. Pleine conscience en 4 étapes pour les ados.",dur:'2-3 min',offre:1},
    {name:'📖 Carnet des victoires',desc:"Écrire 3 petites réussites chaque soir. Reconstruire la confiance face aux échecs scolaires.",dur:'5 min/soir',offre:1},
    {name:'🗣️ La phrase qui coupe court',desc:"UNE phrase neutre par âge (6-11 / 12-18) pour désamorcer le harceleur sans s'abaisser. Jeux de rôle guidés.",dur:'15 min',offre:3}
  ];
  return exs.map(e=>{
    const locked=e.offre>currentOffre;
    return `<div class="ex-card${locked?' locked':''}" onclick="${locked?'showLockMsg()':'\'\''}">
      <span class="ex-tag ${locked?'badge-rose':'badge-sage'}">${locked?'🔒 '+OFFRES[e.offre].name:'✓ Inclus'}</span>
      <h4>${e.name}</h4>
      <p>${e.desc}</p>
      <div class="ex-dur">⏱ ${e.dur}</div>
    </div>`;
  }).join('');
}

function switchExTab(btn,panel){
  document.querySelectorAll('.ex-tab').forEach(t=>t.classList.remove('active'));
  document.querySelectorAll('.ex-panel').forEach(p=>p.classList.remove('active'));
  btn.classList.add('active');
  document.getElementById('ex-'+panel).classList.add('active');
}

function initExTabs(){}

function showLockMsg(){
  const div=document.createElement('div');
  div.className='alert alert-r';
  div.style.cssText='position:fixed;bottom:24px;right:24px;z-index:300;max-width:320px;animation:fadeIn .3s';
  div.innerHTML='🔒 Cet exercice nécessite une offre supérieure. <button onclick="this.parentNode.remove();goPage(\'offres\')" style="margin-left:8px;text-decoration:underline;background:none;border:none;cursor:pointer;color:inherit;font-family:\'DM Sans\',sans-serif">Voir les offres →</button>';
  document.body.appendChild(div);
  setTimeout(()=>div.remove(),4000);
}

// ═══════ RESPIRATION ENGINE ═══════
function startResp(key){
  if(respTimer)clearInterval(respTimer);
  const p=RESP_PATTERNS[key];
  if(!p||p.offre>currentOffre){showLockMsg();return;}
  currentResp=p;respPhaseIdx=0;respCycleCount=0;respRunning=true;
  document.getElementById('resp-desc-box').style.display='block';
  document.getElementById('resp-desc-box').textContent=p.desc;
  runRespPhase();
}

function runRespPhase(){
  if(!currentResp||!respRunning)return;
  const phase=currentResp.phases[respPhaseIdx];
  const circ=document.getElementById('resp-circ');
  const phEl=document.getElementById('resp-phase');
  const cntEl=document.getElementById('resp-count');
  const barEl=document.getElementById('resp-bar');
  const cycEl=document.getElementById('resp-cycles');
  if(!circ)return;
  phEl.textContent=phase.l;
  circ.className='resp-circle '+phase.cls;
  barEl.style.transition='none';barEl.style.width='100%';
  setTimeout(()=>{barEl.style.transition='width '+phase.d+'s linear';barEl.style.width='0%'},50);
  let sec=phase.d;cntEl.textContent=sec;
  if(respTimer)clearInterval(respTimer);
  respTimer=setInterval(()=>{
    sec--;cntEl.textContent=Math.max(0,sec);
    if(sec<=0){
      clearInterval(respTimer);
      respPhaseIdx++;
      if(respPhaseIdx>=currentResp.phases.length){
        respPhaseIdx=0;respCycleCount++;
        cycEl.textContent='Cycles : '+respCycleCount+' / '+currentResp.cycles;
        if(respCycleCount>=currentResp.cycles){
          phEl.textContent='Terminé 🌿';
          circ.className='resp-circle idle';
          cntEl.textContent='✓';
          barEl.style.width='100%';
          respRunning=false;
          return;
        }
      }
      runRespPhase();
    }
  },1000);
}

function stopResp(){
  if(respTimer)clearInterval(respTimer);
  respRunning=false;
  const circ=document.getElementById('resp-circ');
  const phEl=document.getElementById('resp-phase');
  const cntEl=document.getElementById('resp-count');
  if(circ){circ.className='resp-circle idle';phEl.textContent='Choisissez une technique';cntEl.textContent='▶';}
}

// ═══════════ HARCELEMENT ═══════════
function renderHarcelement(){
  return `
  <div style="background:linear-gradient(135deg,rgba(196,123,123,.15),rgba(250,247,242,.9));border-radius:var(--rxl);padding:24px;margin-bottom:20px">
    <h2 style="font-size:30px;font-weight:300;margin-bottom:6px">🛡️ Module harcèlement</h2>
    <p style="color:var(--text-m);font-size:14px">Pour détecter, ouvrir le dialogue et agir. <strong>Urgence : 3018</strong> (gratuit, anonyme, 24h/24)</p>
  </div>
  <div class="harc-tabs">
    <button class="h-tab active" onclick="switchHTab(this,'h-detect')">🔍 Détection</button>
    <button class="h-tab" onclick="switchHTab(this,'h-dialogue')">💬 Comment parler</button>
    <button class="h-tab" onclick="switchHTab(this,'h-action')">📋 Plan d'action</button>
    ${currentOffre>=3?'<button class="h-tab" onclick="switchHTab(this,\'h-cyber\')">💻 Cyber</button>':''}
    <button class="h-tab" onclick="switchHTab(this,'h-urgence')">🆘 Urgences</button>
  </div>
  <div id="h-detect" class="h-panel active">
    <div class="card">
      <div class="card-title">Checklist des 10 signaux d'alerte</div>
      <p style="font-size:13px;color:var(--text-m);margin-bottom:14px">Cochez les signaux que vous observez chez votre enfant :</p>
      ${[
        ['Refuse d\'aller à l\'école','Maux de ventre/tête répétés le matin, inventions'],
        ['Rentre systématiquement triste ou en colère','Changement de comportement notable après l\'école'],
        ['Perd ses affaires ou rentre avec des objets abîmés','Cartable, matériel, vêtements endommagés'],
        ['Troubles du sommeil ou de l\'alimentation','Insomnies, cauchemars, perte d\'appétit soudaine'],
        ['Se replie, abandonne ses activités','Arrête le sport, les amis, les loisirs progressivement'],
        ['Réactions de peur aux notifications','Cache l\'écran, angoisse à la réception de messages'],
        ['N\'invite plus d\'amis, évite les sorties','Isolement social inexpliqué et progressif'],
        ['Chute des résultats scolaires','Difficultés de concentration, notes en baisse soudaine'],
        ['Propos négatifs sur lui-même','Je suis nul, personne ne m\'aime, je voudrais disparaître'],
        ['Marques inexpliquées','Bleus, griffures, blessures légères sans explication']
      ].map((s,i)=>`
        <div class="signal-item" id="sig-${i}" onclick="toggleSignal(${i})">
          <div class="sig-check" id="sig-chk-${i}">✓</div>
          <div><strong style="font-size:14px">${s[0]}</strong><p style="font-size:12px;color:var(--text-m);margin-top:2px">${s[1]}</p></div>
        </div>`).join('')}
      <div id="sig-result" style="display:none;margin-top:14px;padding:14px;border-radius:10px"></div>
      <button class="btn btn-sage btn-sm" style="margin-top:12px" onclick="analyzeSignals()">Analyser les signaux</button>
    </div>
  </div>
  <div id="h-dialogue" class="h-panel">
    <div class="card">
      <div class="card-title">Scripts de dialogue par âge</div>
      <div class="harc-tabs" style="margin-bottom:16px">
        <button class="h-tab active" onclick="switchHTab(this,'s-611',this.closest('.card'))">6-11 ans</button>
        <button class="h-tab" onclick="switchHTab(this,'s-1218',this.closest('.card'))">12-18 ans</button>
      </div>
      <div id="s-611" class="h-panel active">
        <div class="script-box"><div class="script-label">Phrase d'ouverture (soir, calme)</div><div class="script-text">"Tu sais, ma mission de parent c'est d'être là pour toi, même pour les choses difficiles. Est-ce qu'il y a quelque chose qui te rend triste à l'école en ce moment ?"</div></div>
        <div class="script-box"><div class="script-label">Si l'enfant minimise</div><div class="script-text">"J'ai remarqué que tu sembles moins heureux quand tu rentres. Je ne te juge pas, je veux juste comprendre. Tu peux tout me dire."</div></div>
        <div class="script-box"><div class="script-label">S'il avoue quelque chose</div><div class="script-text">"Merci de me faire confiance. Tu as bien fait de me le dire. Ce n'est pas de ta faute. On va régler ça ensemble, je suis là."</div></div>
      </div>
      <div id="s-1218" class="h-panel">
        <div class="script-box"><div class="script-label">Approche indirecte (ne pas forcer)</div><div class="script-text">"Je ne veux pas t'envahir. Mais j'ai l'impression que quelque chose ne va pas. Je suis là si tu veux en parler, sans jugement, sans en faire tout un drame."</div></div>
        <div class="script-box"><div class="script-label">Créer une distance émotionnelle</div><div class="script-text">"Imagine qu'un ami me raconte qu'il se fait embêter à l'école. Qu'est-ce que tu lui dirais, toi ?"</div></div>
        <div class="script-box"><div class="script-label">Garantir la confidentialité</div><div class="script-text">"Ce que tu me dis reste entre nous, sauf si tu es en danger. Je ne vais pas appeler le proviseur sans t'en parler avant."</div></div>
      </div>
    </div>
  </div>
  <div id="h-action" class="h-panel">
    <div class="card">
      <div class="card-title">Plan d'action en 4 étapes</div>
      <div class="action-step"><strong>Étape 1 — Documenter</strong><p style="font-size:13px;color:var(--text-m);margin-top:4px">Notez dates, faits, témoins. Captures d'écran si cyber. Conservez tout. Ne supprimez rien.</p></div>
      <div class="action-step" style="border-color:var(--teal)"><strong>Étape 2 — Contacter l'école</strong><p style="font-size:13px;color:var(--text-m);margin-top:4px">Demandez un RDV avec le directeur/proviseur ET le référent harcèlement (obligatoire depuis 2023). Apportez vos documents.</p></div>
      <div class="action-step" style="border-color:var(--gold)"><strong>Étape 3 — Protection immédiate</strong><p style="font-size:13px;color:var(--text-m);margin-top:4px">Contactez le 3018 pour un conseil juridique. Renforcez le lien avec votre enfant. Maintenez ses activités sociales hors école.</p></div>
      <div class="action-step" style="border-color:var(--rose)"><strong>Étape 4 — Suivi</strong><p style="font-size:13px;color:var(--text-m);margin-top:4px">Si l'école ne réagit pas sous 15 jours → Inspection Académique. Violence physique → dépôt de plainte au commissariat.</p></div>
    </div>
  </div>
  ${currentOffre>=3?`<div id="h-cyber" class="h-panel">
    <div class="card">
      <div class="card-title">Cyber-harcèlement 💻</div>
      <div class="script-box"><div class="script-label">Ouvrir le sujet sans accuser</div><div class="script-text">"J'ai lu que le cyber-harcèlement touche beaucoup d'ados. Est-ce que tu reçois des messages qui te mettent mal à l'aise ?"</div></div>
      <div class="script-box"><div class="script-label">Dédramatiser la technologie</div><div class="script-text">"Les captures d'écran, je peux t'aider à les sauvegarder. Ce n'est pas une honte d'en avoir reçu — c'est le problème de celui qui les envoie."</div></div>
      <div class="alert alert-y" style="margin-top:12px">⚠️ Contenus sexuels impliquant un mineur → signalez immédiatement sur <strong>internet-signalement.gouv.fr</strong></div>
    </div>
  </div>`:''}
  <div id="h-urgence" class="h-panel">
    <div style="display:grid;gap:12px">
      <div class="card" style="display:flex;align-items:center;gap:16px"><div style="font-size:36px">📞</div><div><div style="font-weight:500;font-size:16px">3018 — Anti-harcèlement</div><p style="font-size:13px;color:var(--text-m)">Gratuit · Anonyme · 9h-23h · Conseil juridique · Signalement</p></div></div>
      <div class="card" style="display:flex;align-items:center;gap:16px"><div style="font-size:36px">📞</div><div><div style="font-weight:500;font-size:16px">119 — Enfance en danger</div><p style="font-size:13px;color:var(--text-m)">Gratuit · 24h/24 · 7j/7 · Danger physique ou moral grave</p></div></div>
      <div class="card" style="display:flex;align-items:center;gap:16px"><div style="font-size:36px">📞</div><div><div style="font-weight:500;font-size:16px">3114 — Prévention suicide</div><p style="font-size:13px;color:var(--text-m)">Gratuit · 24h/24 · Si votre enfant tient des propos alarmants</p></div></div>
      <div class="card" style="display:flex;align-items:center;gap:16px"><div style="font-size:36px">💻</div><div><div style="font-weight:500;font-size:16px">internet-signalement.gouv.fr</div><p style="font-size:13px;color:var(--text-m)">Signalement officiel de contenus illicites en ligne</p></div></div>
    </div>
  </div>`;
}

function switchHTab(btn,panelId,scope){
  const container=scope||document;
  container.querySelectorAll('.h-tab').forEach(t=>t.classList.remove('active'));
  container.querySelectorAll('.h-panel').forEach(p=>p.classList.remove('active'));
  btn.classList.add('active');
  const panel=document.getElementById(panelId);
  if(panel)panel.classList.add('active');
}
function initHarcTabs(){
  // Re-init signal items
  signalsChecked.forEach(i=>{
    const item=document.getElementById('sig-'+i);
    if(item)item.classList.add('checked');
  });
}
function toggleSignal(i){
  const item=document.getElementById('sig-'+i);
  if(!item)return;
  if(signalsChecked.has(i)){signalsChecked.delete(i);item.classList.remove('checked');}
  else{signalsChecked.add(i);item.classList.add('checked');}
}
function analyzeSignals(){
  const n=signalsChecked.size;
  const res=document.getElementById('sig-result');
  if(!res)return;
  res.style.display='block';
  if(n<=2){res.style.cssText='display:block;background:#E8F5EA;border:1px solid #90C890;border-radius:10px;padding:14px';res.innerHTML=`<strong style="color:#204020">${n} signal(s) — Vigilance normale</strong><br><span style="font-size:13px;color:#204020">Continuez à observer. Encouragez l'expression des émotions au quotidien.</span>`;}
  else if(n<=5){res.style.cssText='display:block;background:#FFF8E8;border:1px solid #F0D080;border-radius:10px;padding:14px';res.innerHTML=`<strong style="color:#806020">${n} signaux — Attention recommandée</strong><br><span style="font-size:13px;color:#806020">Plusieurs indicateurs. Consultez l'onglet "Comment parler" pour ouvrir le dialogue.</span>`;}
  else{res.style.cssText='display:block;background:#FFEAEA;border:1px solid #F0A0A0;border-radius:10px;padding:14px';res.innerHTML=`<strong style="color:#702020">${n} signaux — Risque élevé · Agissez maintenant</strong><br><span style="font-size:13px;color:#702020">Appelez le 3018 maintenant. Consultez "Plan d'action" et "Urgences".</span>`;}
}

// ═══════════ ARMURE DU MATIN ═══════════
function renderArmure(){
  if(currentOffre<3) return `<div class="lock-overlay"><div style="font-size:48px;margin-bottom:12px">🔒</div><h3>Offre Intensif & Harcèlement requise</h3><p>Le protocole "Mon armure du matin" est exclusif à l'offre Intensif & Harcèlement (269€).</p><button class="btn btn-rose" onclick="goPage('offres')">Voir les offres →</button></div>`;
  return `
  <div style="background:linear-gradient(135deg,rgba(196,123,123,.15),rgba(250,247,242,.9));border-radius:var(--rxl);padding:24px;margin-bottom:20px">
    <h2 style="font-size:30px;font-weight:300;margin-bottom:6px">🛡️ Mon armure du matin</h2>
    <p style="color:var(--text-m);font-size:14px">Routine de 5 minutes à faire AVANT l'école les jours difficiles. À faire avec votre enfant.</p>
  </div>
  <div style="display:grid;gap:16px">
    <div class="card" style="border-left:4px solid var(--teal)">
      <div style="font-size:11px;letter-spacing:1.5px;text-transform:uppercase;color:var(--teal);margin-bottom:8px">Étape 1 · 1 minute</div>
      <h3 style="font-size:20px;font-weight:400;margin-bottom:8px">🫁 Box Breathing</h3>
      <p style="font-size:14px;color:var(--text-m);margin-bottom:12px">Inspire 4s · Retiens 4s · Expire 4s · Pause 4s. Répétez 4 fois ensemble.</p>
      <button class="btn btn-teal btn-sm" onclick="startResp('box')">Lancer la respiration →</button>
    </div>
    <div class="card" style="border-left:4px solid var(--sage)">
      <div style="font-size:11px;letter-spacing:1.5px;text-transform:uppercase;color:var(--sage);margin-bottom:8px">Étape 2 · 2 minutes</div>
      <h3 style="font-size:20px;font-weight:400;margin-bottom:8px">🛡️ Visualisation du bouclier</h3>
      <p style="font-size:14px;color:var(--text-m)">Fermez les yeux. Imaginez un bouclier invisible autour de vous. Choisissez sa couleur. Il est solide. Les mots méchants glissent dessus sans entrer. Sentez-le vous protéger.</p>
    </div>
    <div class="card" style="border-left:4px solid var(--gold)">
      <div style="font-size:11px;letter-spacing:1.5px;text-transform:uppercase;color:var(--gold);margin-bottom:8px">Étape 3 · 2 minutes</div>
      <h3 style="font-size:20px;font-weight:400;margin-bottom:8px">💬 Ma phrase de confiance</h3>
      <p style="font-size:14px;color:var(--text-m);margin-bottom:12px">L'enfant choisit UNE phrase qu'il se répète tout bas aujourd'hui :</p>
      <div style="display:grid;gap:8px">
        ${["Je suis plus fort(e) que leurs mots.","Ce qu'ils disent ne me définit pas.","J'ai des gens qui m'aiment.","Je gère.","Je suis à ma place ici."].map(p=>`<div style="padding:10px 14px;background:var(--cream-d);border-radius:8px;font-size:14px;font-style:italic;cursor:pointer;transition:all .2s" onclick="this.style.background='rgba(184,212,187,.3)';this.style.fontWeight='500'">"${p}"</div>`).join('')}
      </div>
    </div>
  </div>`;
}

// ═══════════ TRACKER STRESS ═══════════
function renderTracker(){
  if(currentOffre<1) return `<div class="lock-overlay"><div style="font-size:48px;margin-bottom:12px">🔒</div><h3>Offre Cap Sérénité requise</h3><p>Le tracker de stress scolaire est disponible à partir de l'offre Cap Sérénité (119€).</p><button class="btn btn-teal" onclick="goPage('offres')">Voir les offres →</button></div>`;
  return `
  <div style="background:linear-gradient(135deg,rgba(168,204,204,.2),rgba(250,247,242,.9));border-radius:var(--rxl);padding:24px;margin-bottom:20px">
    <h2 style="font-size:30px;font-weight:300;margin-bottom:6px">📊 Tracker de stress scolaire</h2>
    <p style="color:var(--text-m);font-size:14px">Identifier les déclencheurs pour mieux les anticiper</p>
  </div>
  <div class="grid2">
    <div class="card">
      <div class="card-title">Ajouter un événement stressant</div>
      <div style="display:grid;gap:10px">
        <select id="t-matiere" style="width:100%"><option>Mathématiques</option><option>Français</option><option>Anglais</option><option>Histoire-Géo</option><option>Sciences</option><option>EPS</option><option>Autre</option></select>
        <select id="t-type" style="width:100%"><option>Contrôle surprise</option><option>Contrôle annoncé</option><option>Exposé oral</option><option>Interro</option><option>Devoir maison</option><option>Note reçue</option></select>
        <div>
          <label style="font-size:13px;color:var(--text-m)">Niveau de stress ressenti</label>
          <input type="range" min="1" max="10" value="5" id="t-stress" oninput="document.getElementById('t-sv').textContent=this.value" style="width:100%;margin-top:6px"/>
          <div style="display:flex;justify-content:space-between;font-size:12px;color:var(--text-l)"><span>Peu stressé</span><span id="t-sv" style="font-weight:500;color:var(--text)">5</span><span>Très stressé</span></div>
        </div>
        <textarea class="journal-box" id="t-note" placeholder="Note (optionnel) : ce qui a déclenché ce stress..." style="min-height:70px"></textarea>
        <button class="btn btn-teal btn-sm" style="justify-content:center" onclick="addTracker()">Enregistrer</button>
      </div>
    </div>
    <div class="card">
      <div class="card-title">Stress par matière</div>
      ${Object.entries(stressData).map(([m,v])=>`
        <div class="prog-wrap">
          <div class="prog-label"><span>${m.charAt(0).toUpperCase()+m.slice(1)}</span><span>${v}/10</span></div>
          <div class="prog-bg"><div class="prog-fill" style="width:${v*10}%;background:${v>7?'var(--rose)':v>4?'var(--gold)':'var(--sage)'}"></div></div>
        </div>`).join('')}
    </div>
  </div>
  <div class="card" id="tracker-history">
    <div class="card-title">Événements récents</div>
    <div class="timeline">
      <div class="tl-item"><div class="tl-time">Aujourd'hui</div><div class="tl-text">Contrôle surprise en Maths — Stress : 8/10</div></div>
      <div class="tl-item"><div class="tl-time">Hier</div><div class="tl-text">Note reçue en Français (12/20) — Stress : 5/10</div></div>
      <div class="tl-item"><div class="tl-time">Lundi</div><div class="tl-text">Exposé oral en Histoire — Stress : 7/10</div></div>
    </div>
  </div>`;
}

function addTracker(){
  const m=document.getElementById('t-matiere')?.value;
  const t=document.getElementById('t-type')?.value;
  const s=document.getElementById('t-stress')?.value;
  if(!m)return;
  const h=document.getElementById('tracker-history');
  const tl=h?.querySelector('.timeline');
  if(tl){
    const item=document.createElement('div');
    item.className='tl-item';
    item.innerHTML=`<div class="tl-time">Maintenant</div><div class="tl-text">${t} en ${m} — Stress : ${s}/10</div>`;
    tl.insertBefore(item,tl.firstChild);
  }
  stressData[m.toLowerCase()]=(parseInt(stressData[m.toLowerCase()]||5)+parseInt(s))/2|0;
  const card=document.querySelector('#tracker-history').previousElementSibling.previousElementSibling;
  if(card) card.querySelector('.card-title').nextElementSibling && (card.innerHTML='<div class="card-title">Stress par matière</div>'+Object.entries(stressData).map(([m,v])=>`<div class="prog-wrap"><div class="prog-label"><span>${m.charAt(0).toUpperCase()+m.slice(1)}</span><span>${v}/10</span></div><div class="prog-bg"><div class="prog-fill" style="width:${v*10}%;background:${v>7?'var(--rose)':v>4?'var(--gold)':'var(--sage)'}"></div></div></div>`).join(''));
}

// ═══════════ ÉVOLUTION ═══════════
function renderEvolution(){
  const data30=moodData.enfant.month;
  const avg=(data30.reduce((a,b)=>a+b,0)/data30.length).toFixed(1);
  return `
  <div class="grid2" style="margin-bottom:20px">
    <div class="metric full" style="grid-column:auto"><div class="metric-l">Moyenne humeur 30 jours</div><div class="metric-v" style="color:var(--sage)">${avg}/10</div><div class="metric-s">↑ Amélioration vs mois dernier</div></div>
    <div class="metric"><div class="metric-l">Total exercices</div><div class="metric-v">47</div><div class="metric-s">ce mois</div></div>
    <div class="metric"><div class="metric-l">Jours avec journal</div><div class="metric-v">22</div><div class="metric-s">sur 30</div></div>
    <div class="metric"><div class="metric-l">Streak max</div><div class="metric-v">9🔥</div><div class="metric-s">jours consécutifs</div></div>
  </div>
  <div class="card" style="margin-bottom:20px">
    <div class="card-title">Humeur sur 30 jours</div>
    <div class="bars" style="height:120px;gap:3px">
      ${data30.map((v,i)=>`<div class="bar-col" style="gap:2px">
        <div class="bar" style="height:${v*10}%;background:${v>=7?'var(--sage)':v>=5?'var(--gold)':'var(--rose)'}"></div>
      </div>`).join('')}
    </div>
    <div style="display:flex;gap:16px;margin-top:10px;font-size:12px">
      <div style="display:flex;align-items:center;gap:5px"><div style="width:10px;height:10px;border-radius:2px;background:var(--rose)"></div>Difficile</div>
      <div style="display:flex;align-items:center;gap:5px"><div style="width:10px;height:10px;border-radius:2px;background:var(--gold)"></div>Moyen</div>
      <div style="display:flex;align-items:center;gap:5px"><div style="width:10px;height:10px;border-radius:2px;background:var(--sage)"></div>Bien</div>
    </div>
  </div>
  <div class="grid2">
    <div class="card">
      <div class="card-title">Exercices les plus efficaces</div>
      ${[['🫧 Bulle de savon',90],['🐢 Ma tortue',80],['💚 Cohérence cardiaque',75],['🦁 Souffle du Lion',60]].map(([n,v])=>`
        <div class="prog-wrap">
          <div class="prog-label"><span>${n}</span><span>${v}%</span></div>
          <div class="prog-bg"><div class="prog-fill" style="width:${v}%"></div></div>
        </div>`).join('')}
      <p style="font-size:12px;color:var(--text-l);margin-top:8px">Basé sur l'humeur déclarée avant/après</p>
    </div>
    <div class="card">
      <div class="card-title">Streak des 7 derniers jours</div>
      <div style="font-size:13px;color:var(--text-m);margin-bottom:10px">Journal complété :</div>
      <div class="streak-grid">
        ${jours.map((j,i)=>`<div><div class="streak-day${i<6?' done':' today'}">${i<6?'✓':'★'}</div><div style="text-align:center;font-size:10px;color:var(--text-l);margin-top:3px">${j.slice(0,2)}</div></div>`).join('')}
      </div>
    </div>
  </div>`;
}

// ═══════════ MOOD ═══════════
function setMoodEnfant(emoji,btn){
  currentMood=emoji;
  document.querySelectorAll('.mood-btn').forEach(b=>b.classList.remove('sel'));
  btn.classList.add('sel');
  const big=document.getElementById('enfant-mood-big');
  if(big)big.textContent=emoji;
}
function setMoodAdo(emoji,btn){
  currentMood=emoji;
  document.querySelectorAll('.mood-btn').forEach(b=>b.classList.remove('sel'));
  btn.classList.add('sel');
}

// ═══════════ PAYMENT ═══════════
let currentPayIdx=0;
function openPay(idx){
  currentPayIdx=idx;
  const o=OFFRES[idx];
  document.getElementById('pay-icon').textContent=o.icon;
  document.getElementById('pay-name').textContent=o.name;
  document.getElementById('pay-sub').textContent=o.sub;
  document.getElementById('pay-price').innerHTML=o.prix+' <span style="font-size:18px;font-family:\'DM Sans\',sans-serif">TTC</span>';
  document.getElementById('ck1').checked=false;
  document.getElementById('ck2').checked=false;
  document.getElementById('pay-warn').style.display='none';
  document.getElementById('pay-btn').disabled=true;
  document.getElementById('pay-bg').classList.remove('hidden');
}
function closePay(){document.getElementById('pay-bg').classList.add('hidden');}
function checkPay(){
  const ok=document.getElementById('ck1').checked&&document.getElementById('ck2').checked;
  document.getElementById('pay-btn').disabled=!ok;
  if(ok)document.getElementById('pay-warn').style.display='none';
}
function doPay(){
  if(!document.getElementById('ck1').checked||!document.getElementById('ck2').checked){document.getElementById('pay-warn').style.display='block';return;}
  window.open(OFFRES[currentPayIdx].stripe,'_blank');
  closePay();
}

// ═══════════ CREATOR ═══════════
let emailClicks=0,emailTimer=null;
function handleEmailClick(){
  emailClicks++;
  clearTimeout(emailTimer);
  emailTimer=setTimeout(()=>emailClicks=0,1800);
  if(emailClicks>=4){emailClicks=0;openCreator();}
}
function openCreator(){
  document.getElementById('creator-bg').style.display='flex';
  document.getElementById('creator-pin-screen').style.display='block';
  document.getElementById('creator-content').style.display='none';
  document.getElementById('pin-inp').value='';
  document.getElementById('pin-err').style.display='none';
  setTimeout(()=>document.getElementById('pin-inp').focus(),100);
}
function closeCreator(){document.getElementById('creator-bg').style.display='none';}
function tryPin(submit){
  const v=document.getElementById('pin-inp').value;
  if(v==='1622'){
    document.getElementById('creator-pin-screen').style.display='none';
    document.getElementById('creator-content').style.display='block';
    document.getElementById('pin-err').style.display='none';
  }else if(submit&&v.length>0){
    document.getElementById('pin-err').style.display='block';
    document.getElementById('pin-inp').value='';
  }
}
function toggleC(id){
  const el=document.getElementById(id);
  const arrow=document.getElementById(id+'-arrow');
  const open=el.style.display==='block';
  el.style.display=open?'none':'block';
  if(arrow)arrow.textContent=open?'▼':'▲';
}

// ═══════════ DÉMO OFFRE SWITCHER ═══════════
// Barre de démo pour tester les offres dans le dashboard
function addDemoBar(){
  const bar=document.createElement('div');
  bar.id='demo-bar';
  bar.style.cssText='position:fixed;bottom:0;left:0;right:0;background:rgba(44,44,42,.9);padding:8px 20px;display:flex;align-items:center;gap:12px;z-index:150;font-size:13px;color:#fff;backdrop-filter:blur(8px)';
  bar.innerHTML=`<span style="opacity:.6">Mode démo — Simuler une offre :</span>${OFFRES.map((o,i)=>`<button onclick="currentOffre=${i};currentRole='parent';currentSection='overview';if(document.getElementById('page-dash').classList.contains('active'))initDash()" style="padding:5px 14px;border-radius:50px;border:1px solid rgba(255,255,255,.3);background:${i===currentOffre?'#7A9E7E':'transparent'};color:#fff;cursor:pointer;font-family:'DM Sans',sans-serif;font-size:12px" id="demo-btn-${i}">${o.icon} ${o.name}</button>`).join('')}`;
  document.body.appendChild(bar);
}
addDemoBar();

// Init
document.addEventListener('DOMContentLoaded',()=>{
  initDash();
});
initDash();
</script><div id="demo-bar" style="position: fixed; bottom: 0px; left: 0px; right: 0px; background: rgba(44, 44, 42, 0.9); padding: 8px 20px; display: flex; align-items: center; gap: 12px; z-index: 150; font-size: 13px; color: rgb(255, 255, 255); backdrop-filter: blur(8px);"><span style="opacity:.6">Mode démo — Simuler une offre :</span><button onclick="currentOffre=0;currentRole=&#39;parent&#39;;currentSection=&#39;overview&#39;;if(document.getElementById(&#39;page-dash&#39;).classList.contains(&#39;active&#39;))initDash()" style="padding:5px 14px;border-radius:50px;border:1px solid rgba(255,255,255,.3);background:transparent;color:#fff;cursor:pointer;font-family:&#39;DM Sans&#39;,sans-serif;font-size:12px" id="demo-btn-0">🌱 Petites Pousses</button><button onclick="currentOffre=1;currentRole=&#39;parent&#39;;currentSection=&#39;overview&#39;;if(document.getElementById(&#39;page-dash&#39;).classList.contains(&#39;active&#39;))initDash()" style="padding:5px 14px;border-radius:50px;border:1px solid rgba(255,255,255,.3);background:transparent;color:#fff;cursor:pointer;font-family:&#39;DM Sans&#39;,sans-serif;font-size:12px" id="demo-btn-1">🌊 Cap Sérénité</button><button onclick="currentOffre=2;currentRole=&#39;parent&#39;;currentSection=&#39;overview&#39;;if(document.getElementById(&#39;page-dash&#39;).classList.contains(&#39;active&#39;))initDash()" style="padding:5px 14px;border-radius:50px;border:1px solid rgba(255,255,255,.3);background:#7A9E7E;color:#fff;cursor:pointer;font-family:&#39;DM Sans&#39;,sans-serif;font-size:12px" id="demo-btn-2">⭐ Famille Unie</button><button onclick="currentOffre=3;currentRole=&#39;parent&#39;;currentSection=&#39;overview&#39;;if(document.getElementById(&#39;page-dash&#39;).classList.contains(&#39;active&#39;))initDash()" style="padding:5px 14px;border-radius:50px;border:1px solid rgba(255,255,255,.3);background:transparent;color:#fff;cursor:pointer;font-family:&#39;DM Sans&#39;,sans-serif;font-size:12px" id="demo-btn-3">🛡️ Intensif &amp; Harcèlement</button></div>


</body></html>
