<!DOCTYPE html>
<!-- saved from url=(0055)file:///C:/Users/sebas/Downloads/serenum-app%20(3).html -->
<html lang="fr"><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">

<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Sérénum — Accompagnement émotionnel enfants &amp; adolescents</title>
<link href="./Sérénum — Accompagnement émotionnel enfants &amp; adolescents_files/css2" rel="stylesheet">
<style>
*{margin:0;padding:0;box-sizing:border-box}
:root{
  --sage:#7A9E7E;--sage-light:#B8D4BB;--sage-dark:#4A6B4E;
  --cream:#FAF7F2;--cream-dark:#F0EBE1;
  --sand:#C8B89A;--sand-dark:#9A8570;
  --teal:#4A8B8C;--teal-light:#A8CCCC;
  --rose:#C47B7B;--rose-light:#E8BBBB;
  --lavender:#7B7BAE;--lav-light:#BBBBDD;
  --gold:#C4A24A;--gold-light:#E8D4A0;
  --text:#2C2C2A;--text-muted:#666660;--text-light:#999990;
  --white:#FFFFFF;--border:#E0DDD5;
  --radius:12px;--radius-lg:20px;--radius-xl:28px;
}
body{font-family:'DM Sans',sans-serif;background:var(--cream);color:var(--text);min-height:100vh}
h1,h2,h3,h4{font-family:'Cormorant Garamond',serif}
.hidden{display:none!important}
.btn{padding:12px 28px;border:none;border-radius:50px;cursor:pointer;font-family:'DM Sans',sans-serif;font-size:14px;font-weight:500;transition:all .25s;letter-spacing:.3px}
.btn-primary{background:var(--sage);color:var(--white)}
.btn-primary:hover{background:var(--sage-dark);transform:translateY(-1px)}
.btn-outline{background:transparent;border:1.5px solid var(--sage);color:var(--sage)}
.btn-outline:hover{background:var(--sage);color:var(--white)}
.btn-sm{padding:8px 18px;font-size:13px}
.btn-gold{background:var(--gold);color:var(--white)}
.btn-gold:hover{background:#a8872a}
.btn-teal{background:var(--teal);color:var(--white)}
.btn-teal:hover{background:#3a6b6c}
.btn-rose{background:var(--rose);color:var(--white)}
.btn-rose:hover{background:#a46060}
.btn-lav{background:var(--lavender);color:var(--white)}
.btn-lav:hover{background:#606090}
.tag{display:inline-block;padding:4px 12px;border-radius:50px;font-size:12px;font-weight:500;letter-spacing:.4px}
.tag-sage{background:var(--sage-light);color:var(--sage-dark)}
.tag-gold{background:var(--gold-light);color:#7A6020}
.tag-teal{background:var(--teal-light);color:#2A5A5B}
.tag-rose{background:var(--rose-light);color:#7A4040}
.tag-lav{background:var(--lav-light);color:#4A4A80}
.card{background:var(--white);border-radius:var(--radius-lg);border:1px solid var(--border);padding:24px}
.nav{position:fixed;top:0;left:0;right:0;z-index:100;background:rgba(250,247,242,.95);backdrop-filter:blur(12px);border-bottom:1px solid var(--border);padding:0 40px;height:64px;display:flex;align-items:center;justify-content:space-between}
.nav-logo{font-family:'Cormorant Garamond',serif;font-size:26px;font-weight:300;color:var(--sage-dark);letter-spacing:1px;cursor:pointer}
.nav-logo span{color:var(--sage);font-style:italic}
.nav-links{display:flex;gap:8px;align-items:center}
.nav-link{padding:8px 16px;border-radius:50px;cursor:pointer;font-size:14px;color:var(--text-muted);transition:all .2s}
.nav-link:hover,.nav-link.active{background:var(--cream-dark);color:var(--text)}
/* PAGES */
.page{display:none;min-height:100vh;padding-top:64px}
.page.active{display:block}
/* HOME */
.hero{padding:80px 40px 60px;max-width:1100px;margin:0 auto;display:grid;grid-template-columns:1fr 1fr;gap:60px;align-items:center}
.hero-eyebrow{font-size:12px;letter-spacing:2px;text-transform:uppercase;color:var(--sage);margin-bottom:16px}
.hero-title{font-family:'Cormorant Garamond',serif;font-size:58px;font-weight:300;line-height:1.1;color:var(--text);margin-bottom:20px}
.hero-title em{font-style:italic;color:var(--sage)}
.hero-subtitle{font-size:16px;color:var(--text-muted);line-height:1.7;margin-bottom:28px;font-weight:300}
.hero-disclaimer{font-size:12px;color:var(--text-light);line-height:1.6;padding:12px 16px;background:var(--cream-dark);border-radius:8px;border-left:3px solid var(--sand)}
.hero-visual{position:relative;display:flex;align-items:center;justify-content:center}
.breathing-orb{width:280px;height:280px;border-radius:50%;background:radial-gradient(circle,var(--sage-light) 0%,var(--cream-dark) 70%);display:flex;align-items:center;justify-content:center;animation:breathe 4s ease-in-out infinite;position:relative}
.breathing-orb::before{content:'';position:absolute;inset:-20px;border-radius:50%;border:1px solid var(--sage-light);animation:breathe 4s ease-in-out infinite .5s}
.breathing-orb::after{content:'';position:absolute;inset:-40px;border-radius:50%;border:1px solid rgba(122,158,126,.2);animation:breathe 4s ease-in-out infinite 1s}
.orb-text{font-family:'Cormorant Garamond',serif;font-size:22px;font-weight:300;color:var(--sage-dark);text-align:center;font-style:italic}
@keyframes breathe{0%,100%{transform:scale(1)}50%{transform:scale(1.08)}}
.stats-row{display:grid;grid-template-columns:repeat(3,1fr);gap:20px;max-width:1100px;margin:0 auto 60px;padding:0 40px}
.stat-card{background:var(--white);border-radius:var(--radius);border:1px solid var(--border);padding:24px;text-align:center}
.stat-number{font-family:'Cormorant Garamond',serif;font-size:42px;font-weight:300;color:var(--sage)}
.stat-label{font-size:13px;color:var(--text-muted);line-height:1.5;margin-top:4px}
/* OFFRES */
.offres-header{text-align:center;padding:60px 40px 40px;max-width:800px;margin:0 auto}
.offres-header h2{font-size:48px;font-weight:300;color:var(--text);margin-bottom:12px}
.offres-grid{display:grid;grid-template-columns:repeat(2,1fr);gap:24px;max-width:1100px;margin:0 auto;padding:0 40px 60px}
.offre-card{background:var(--white);border-radius:var(--radius-xl);border:1px solid var(--border);overflow:hidden;transition:transform .3s,box-shadow .3s;cursor:pointer}
.offre-card:hover{transform:translateY(-4px);box-shadow:0 20px 60px rgba(0,0,0,.08)}
.offre-header{padding:28px 28px 20px;position:relative}
.offre-badge{position:absolute;top:20px;right:20px;font-size:11px;font-weight:500;letter-spacing:.8px;text-transform:uppercase;padding:5px 14px;border-radius:50px}
.offre-icon{width:52px;height:52px;border-radius:16px;display:flex;align-items:center;justify-content:center;font-size:24px;margin-bottom:16px}
.offre-name{font-family:'Cormorant Garamond',serif;font-size:26px;font-weight:400;margin-bottom:6px}
.offre-target{font-size:13px;color:var(--text-muted);margin-bottom:12px}
.offre-price{font-family:'Cormorant Garamond',serif;font-size:38px;font-weight:300;margin-bottom:4px}
.offre-price span{font-size:16px;font-weight:400;font-family:'DM Sans',sans-serif}
.offre-price-note{font-size:12px;color:var(--text-light)}
.offre-body{padding:0 28px 28px}
.offre-features{list-style:none;margin:16px 0}
.offre-features li{font-size:14px;color:var(--text-muted);padding:6px 0;border-bottom:1px solid var(--cream-dark);display:flex;align-items:center;gap:8px}
.offre-features li:last-child{border:none}
.check{color:var(--sage);font-weight:600;font-size:16px}
.offre-roles{display:flex;gap:8px;flex-wrap:wrap;margin:16px 0}
/* DASHBOARD */
.dash-layout{display:grid;grid-template-columns:240px 1fr;min-height:calc(100vh - 64px)}
.dash-sidebar{background:var(--white);border-right:1px solid var(--border);padding:28px 20px;position:sticky;top:64px;height:calc(100vh - 64px);overflow-y:auto}
.dash-sidebar-title{font-family:'Cormorant Garamond',serif;font-size:20px;font-weight:300;margin-bottom:20px;color:var(--text-muted)}
.dash-nav-item{display:flex;align-items:center;gap:10px;padding:10px 14px;border-radius:10px;cursor:pointer;margin-bottom:4px;font-size:14px;color:var(--text-muted);transition:all .2s}
.dash-nav-item:hover,.dash-nav-item.active{background:var(--cream-dark);color:var(--text)}
.dash-nav-item .icon{font-size:18px}
.dash-main{padding:32px;background:var(--cream);overflow-y:auto}
.dash-top{display:flex;justify-content:space-between;align-items:flex-start;margin-bottom:28px}
.dash-greeting h2{font-size:32px;font-weight:300;color:var(--text);margin-bottom:4px}
.dash-greeting p{font-size:14px;color:var(--text-muted)}
.dash-role-switcher{display:flex;gap:8px}
.role-btn{padding:8px 18px;border:1.5px solid var(--border);border-radius:50px;cursor:pointer;font-size:13px;font-family:'DM Sans',sans-serif;background:var(--white);color:var(--text-muted);transition:all .2s}
.role-btn.active{border-color:var(--sage);background:var(--sage);color:var(--white)}
.metrics-row{display:grid;grid-template-columns:repeat(4,1fr);gap:16px;margin-bottom:24px}
.metric{background:var(--white);border-radius:var(--radius);border:1px solid var(--border);padding:18px}
.metric-label{font-size:12px;color:var(--text-light);margin-bottom:6px;letter-spacing:.3px}
.metric-value{font-family:'Cormorant Garamond',serif;font-size:32px;font-weight:300;color:var(--text)}
.metric-sub{font-size:12px;color:var(--text-muted);margin-top:2px}
.dash-grid{display:grid;grid-template-columns:1fr 1fr;gap:20px;margin-bottom:20px}
.dash-full{grid-column:1/-1}
/* JOURNAL */
.journal-area{width:100%;min-height:140px;border:1px solid var(--border);border-radius:var(--radius);padding:16px;font-family:'DM Sans',sans-serif;font-size:15px;color:var(--text);background:var(--cream);resize:vertical;line-height:1.6}
.journal-area:focus{outline:none;border-color:var(--sage)}
.mood-picker{display:flex;gap:12px;margin:12px 0}
.mood-btn{width:48px;height:48px;border-radius:50%;border:2px solid var(--border);background:var(--white);font-size:24px;cursor:pointer;transition:all .2s;display:flex;align-items:center;justify-content:center}
.mood-btn.selected,.mood-btn:hover{border-color:var(--sage);transform:scale(1.1)}
/* CHART */
.chart-wrap{padding:8px 0}
.chart-bars{display:flex;align-items:flex-end;gap:8px;height:100px;padding:0 4px}
.bar-col{flex:1;display:flex;flex-direction:column;align-items:center;gap:4px}
.bar{border-radius:4px 4px 0 0;width:100%;transition:height .4s}
.bar-label{font-size:11px;color:var(--text-light)}
/* RESPIRATION */
.resp-circle{width:180px;height:180px;border-radius:50%;display:flex;align-items:center;justify-content:center;font-family:'Cormorant Garamond',serif;font-size:18px;font-weight:300;font-style:italic;transition:all 1s;position:relative;margin:0 auto}
.resp-circle.inhale{background:radial-gradient(circle,#B8D4BB,#7A9E7E);transform:scale(1.15)}
.resp-circle.hold{background:radial-gradient(circle,#BBBBDD,#7B7BAE)}
.resp-circle.exhale{background:radial-gradient(circle,#A8CCCC,#4A8B8C);transform:scale(.9)}
/* HARCELEMENT */
.signal-item{display:flex;align-items:flex-start;gap:12px;padding:14px;border-radius:10px;border:1px solid var(--border);margin-bottom:8px;cursor:pointer;transition:all .2s}
.signal-item.checked{background:rgba(122,158,126,.08);border-color:var(--sage)}
.signal-check{width:22px;height:22px;border-radius:6px;border:2px solid var(--border);flex-shrink:0;display:flex;align-items:center;justify-content:center;margin-top:1px;transition:all .2s}
.signal-item.checked .signal-check{background:var(--sage);border-color:var(--sage);color:var(--white)}
/* PAIEMENT */
.payment-overlay{position:fixed;inset:0;background:rgba(0,0,0,.5);z-index:200;display:flex;align-items:center;justify-content:center;padding:20px}
.payment-modal{background:var(--white);border-radius:var(--radius-xl);padding:40px;max-width:520px;width:100%;max-height:90vh;overflow-y:auto}
.payment-modal h3{font-size:28px;font-weight:300;margin-bottom:8px}
.legal-check{display:flex;align-items:flex-start;gap:12px;padding:14px;border:1px solid var(--border);border-radius:10px;margin-bottom:10px;cursor:pointer;transition:all .2s}
.legal-check:hover{border-color:var(--sage-light)}
.legal-check input[type=checkbox]{width:18px;height:18px;accent-color:var(--sage);flex-shrink:0;margin-top:2px;cursor:pointer}
.legal-check label{font-size:13px;color:var(--text-muted);line-height:1.5;cursor:pointer}
.legal-check label strong{color:var(--text)}
.disclaimer-box{background:var(--cream-dark);border-radius:10px;padding:16px;margin:16px 0;border-left:3px solid var(--rose)}
.disclaimer-box p{font-size:12px;color:var(--text-muted);line-height:1.6}
.price-row{display:flex;justify-content:space-between;align-items:center;padding:12px 0;border-top:1px solid var(--border);margin-top:16px}
.price-final{font-family:'Cormorant Garamond',serif;font-size:36px;font-weight:300}
.step-indicator{display:flex;gap:8px;margin-bottom:28px}
.step{flex:1;height:3px;border-radius:2px;background:var(--border)}
.step.done{background:var(--sage)}
.success-screen{text-align:center;padding:20px 0}
.success-icon{font-size:64px;margin-bottom:16px}
/* MENTIONS LÉGALES */
.legal-page{max-width:860px;margin:0 auto;padding:40px}
.legal-page h2{font-size:42px;font-weight:300;margin-bottom:8px}
.legal-section{margin:28px 0}
.legal-section h3{font-size:20px;font-weight:400;color:var(--text);margin-bottom:12px;padding-bottom:8px;border-bottom:1px solid var(--border);font-family:'Cormorant Garamond',serif}
.legal-section p,.legal-section li{font-size:14px;color:var(--text-muted);line-height:1.8;margin-bottom:8px}
.legal-section ul{padding-left:20px}
.highlight-box{background:var(--cream-dark);padding:16px;border-radius:10px;border-left:3px solid var(--sage);margin:12px 0}
/* TABS */
.tabs{display:flex;gap:4px;background:var(--cream-dark);border-radius:12px;padding:4px;margin-bottom:20px}
.tab{flex:1;padding:9px;border-radius:9px;border:none;cursor:pointer;font-family:'DM Sans',sans-serif;font-size:13px;font-weight:400;color:var(--text-muted);background:transparent;transition:all .2s;text-align:center}
.tab.active{background:var(--white);color:var(--text);font-weight:500;box-shadow:0 1px 4px rgba(0,0,0,.08)}
.tab-content{display:none}
.tab-content.active{display:block}
/* EXERCICES */
.ex-card{background:var(--white);border-radius:var(--radius);border:1px solid var(--border);padding:20px;margin-bottom:12px;cursor:pointer;transition:all .2s}
.ex-card:hover{border-color:var(--sage-light);background:rgba(184,212,187,.05)}
.ex-card h4{font-size:16px;font-weight:500;margin-bottom:4px}
.ex-card p{font-size:13px;color:var(--text-muted);line-height:1.5}
.ex-duration{font-size:12px;color:var(--text-light);margin-top:6px}
/* RESP player */
.resp-player{background:var(--white);border-radius:var(--radius-lg);border:1px solid var(--border);padding:24px;text-align:center}
.resp-phase{font-size:13px;letter-spacing:2px;text-transform:uppercase;color:var(--text-muted);margin-bottom:8px}
.resp-counter{font-family:'Cormorant Garamond',serif;font-size:48px;font-weight:300;color:var(--sage)}
.resp-progress{height:4px;background:var(--cream-dark);border-radius:2px;margin:16px 0;overflow:hidden}
.resp-bar{height:100%;border-radius:2px;background:var(--sage);transition:width 1s linear}
/* Journal enfant/ado spécial */
.journal-header{background:linear-gradient(135deg,var(--sage-light),var(--cream-dark));border-radius:var(--radius-lg);padding:24px;margin-bottom:20px}
.journal-header h3{font-size:26px;font-weight:300;margin-bottom:4px}
.journal-header p{font-size:14px;color:var(--text-muted)}
/* TIMELINE */
.timeline{position:relative;padding-left:24px}
.timeline::before{content:'';position:absolute;left:8px;top:0;bottom:0;width:1px;background:var(--border)}
.tl-item{position:relative;padding:12px 0 12px 24px;margin-bottom:4px}
.tl-item::before{content:'';position:absolute;left:-8px;top:18px;width:10px;height:10px;border-radius:50%;background:var(--sage);border:2px solid var(--white)}
.tl-time{font-size:11px;color:var(--text-light);margin-bottom:2px}
.tl-text{font-size:14px;color:var(--text-muted);line-height:1.5}
/* Alerts */
.alert{padding:12px 16px;border-radius:10px;font-size:13px;margin-bottom:8px;display:flex;align-items:flex-start;gap:10px}
.alert-warning{background:#FFF8E8;border:1px solid #F0D080;color:#806020}
.alert-info{background:#E8F4FF;border:1px solid #90C4EE;color:#204870}
.alert-danger{background:#FFEAEA;border:1px solid #F0A0A0;color:#702020}
.alert-success{background:#E8F5EA;border:1px solid #90C890;color:#204020}
/* Responsive */
@media(max-width:900px){
.hero{grid-template-columns:1fr;gap:40px}
.offres-grid{grid-template-columns:1fr}
.dash-layout{grid-template-columns:1fr}
.dash-sidebar{display:none}
.metrics-row{grid-template-columns:1fr 1fr}
.dash-grid{grid-template-columns:1fr}
}
</style>
</head>
<body>

<nav class="nav">
  <div class="nav-logo" onclick="showPage(&#39;home&#39;)">Séré<span>num</span></div>
  <div class="nav-links">
    <div class="nav-link" onclick="showPage(&#39;home&#39;)">Accueil</div>
    <div class="nav-link" onclick="showPage(&#39;offres&#39;)">Nos offres</div>
    <div class="nav-link" onclick="showPage(&#39;dashboard&#39;)">Espace membre</div>
    <div class="nav-link" onclick="showPage(&#39;legal&#39;)">Mentions légales</div>
  </div>
</nav>

<!-- PAGE ACCUEIL -->
<div id="page-home" class="page active">
  <div class="hero">
    <div>
      <h1 class="hero-title">Quand le stress<br>de l'école devient<br><em>trop lourd</em></h1>
      <p class="hero-subtitle">Sérénum accompagne enfants, adolescents et parents face à la pression scolaire, l'anxiété du quotidien, et les situations de harcèlement. Des outils concrets, accessibles, pensés pour chaque âge.</p>
      <div style="display:flex;gap:12px;margin-bottom:20px">
        <button class="btn btn-primary" onclick="showPage(&#39;offres&#39;)">Découvrir les offres</button>
        <button class="btn btn-outline" onclick="showPage(&#39;dashboard&#39;)">Espace membre</button>
      </div>
      <div class="hero-disclaimer">⚠️ <strong>Avertissement important</strong> — Je ne suis ni médecin, ni psychologue, ni thérapeute. Je suis un parent qui a cherché des solutions pour son enfant, et qui partage ce qui a fonctionné. Ces outils ne remplacent en aucun cas un avis médical ou un suivi thérapeutique professionnel. Aucun résultat de guérison n'est garanti ni promis.</div>
    </div>
    <div class="hero-visual">
      <div class="breathing-orb">
        <div class="orb-text">Inspire<br>doucement</div>
      </div>
    </div>
  </div>

  <div class="stats-row">
    <div class="stat-card">
      <div class="stat-number">1 / 5</div>
      <div class="stat-label">enfants souffre d'anxiété scolaire significative en France (INSERM, 2023)</div>
    </div>
    <div class="stat-card">
      <div class="stat-number">700 000</div>
      <div class="stat-label">élèves victimes de harcèlement scolaire chaque année (Éducation Nationale)</div>
    </div>
    <div class="stat-card">
      <div class="stat-number">67 %</div>
      <div class="stat-label">des parents déclarent se sentir démunis face au stress de leur enfant (Ifop 2022)</div>
    </div>
  </div>

  <!-- STORYTELLING -->
  <div style="max-width:860px;margin:0 auto 72px;padding:0 40px">
    <div style="position:relative;background:var(--white);border-radius:var(--radius-xl);border:1px solid var(--border);padding:48px 52px;overflow:hidden">
      <!-- Guillemet décoratif -->
      <div style="position:absolute;top:-10px;left:36px;font-family:&#39;Cormorant Garamond&#39;,serif;font-size:160px;font-weight:300;color:var(--sage-light);line-height:1;pointer-events:none;user-select:none;">"</div>
      <div style="position:relative">
        <div style="display:inline-block;font-size:11px;letter-spacing:2.5px;text-transform:uppercase;color:var(--sage);border-bottom:1px solid var(--sage-light);padding-bottom:6px;margin-bottom:28px">L'histoire qui a tout changé</div>

        <p style="font-family:&#39;Cormorant Garamond&#39;,serif;font-size:22px;font-weight:300;line-height:1.75;color:var(--text);margin-bottom:20px">
          Un jour, mon fils de 9 ans est rentré de l'école le visage fermé. Il avait eu une dictée surprise.
        </p>
        <p style="font-size:15px;color:var(--text-muted);line-height:1.8;margin-bottom:18px">
          Il m'a raconté qu'au moment où la maîtresse avait annoncé la dictée, son cœur s'était emballé. Les mots dans sa tête s'étaient brouillés. Il sentait la panique monter.
        </p>
        <p style="font-size:15px;color:var(--text-muted);line-height:1.8;margin-bottom:18px">
          Mais il a fait quelque chose que je ne lui avais pas demandé de faire. <strong style="color:var(--text);font-weight:500">Il s'est posé sur sa chaise. Il a fermé les yeux une seconde. Et il a pensé à moi.</strong> Il m'a dit : <em style="color:var(--sage-dark)">"J'ai fait la technique SOS qu'on faisait à la maison, papa."</em>
        </p>
        <p style="font-size:15px;color:var(--text-muted);line-height:1.8;margin-bottom:28px">
          Quelques respirations guidées par la mémoire de nos séances. Son rythme cardiaque s'est apaisé. Les mots sont revenus. La dictée s'est bien passée.
        </p>

        <div style="border-left:3px solid var(--sage);padding:16px 20px;background:rgba(184,212,187,.1);border-radius:0 10px 10px 0;margin-bottom:28px">
          <p style="font-family:&#39;Cormorant Garamond&#39;,serif;font-size:19px;font-weight:300;font-style:italic;color:var(--sage-dark);line-height:1.6">
            Ce jour-là, j'ai compris que la vraie victoire, ce n'est pas d'éliminer le stress de la vie de nos enfants. C'est de leur donner les outils pour y faire face, seuls, quand nous ne sommes pas là.
          </p>
        </div>

        <p style="font-size:14px;color:var(--text-muted);line-height:1.7;margin-bottom:28px">
          C'est pour ça que j'ai créé Sérénum. Pas pour promettre un miracle. Pas pour remplacer un médecin ou un psy — ces professionnels sont irremplaçables et je vous encourage à les consulter si votre enfant en a besoin. Mais pour mettre entre les mains de votre enfant, et dans les vôtres, des techniques concrètes, adaptées à chaque âge. Des outils qu'ils pourront utiliser seuls, en classe, dans le couloir du collège, avant un examen.
        </p>

        <div style="display:flex;align-items:center;gap:16px">
          <div style="width:48px;height:48px;border-radius:50%;background:var(--sage-light);display:flex;align-items:center;justify-content:center;font-size:22px;flex-shrink:0">👨‍👦</div>
          <div>
            <div style="font-weight:500;font-size:15px;color:var(--text)">Le fondateur de Sérénum</div>
            <div style="font-size:13px;color:var(--text-muted)">Parent avant tout — et fier de l'être.</div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <div style="max-width:1100px;margin:0 auto;padding:0 40px 80px">
    <h2 style="font-size:38px;font-weight:300;margin-bottom:32px;text-align:center">Comment fonctionne Sérénum</h2>
    <div style="display:grid;grid-template-columns:repeat(3,1fr);gap:24px">
      <div class="card" style="text-align:center">
        <div style="font-size:40px;margin-bottom:12px">🌱</div>
        <h3 style="font-size:20px;font-weight:400;margin-bottom:8px">Choisissez votre offre</h3>
        <p style="font-size:14px;color:var(--text-muted);line-height:1.6">Paiement unique, adapté à l'âge et au niveau de besoin. Zéro abonnement, zéro surprise.</p>
      </div>
      <div class="card" style="text-align:center">
        <div style="font-size:40px;margin-bottom:12px">🧘</div>
        <h3 style="font-size:20px;font-weight:400;margin-bottom:8px">Accédez à votre espace</h3>
        <p style="font-size:14px;color:var(--text-muted);line-height:1.6">Parent, enfant ou adolescent — chaque rôle a son interface, son journal, ses exercices.</p>
      </div>
      <div class="card" style="text-align:center">
        <div style="font-size:40px;margin-bottom:12px">📈</div>
        <h3 style="font-size:20px;font-weight:400;margin-bottom:8px">Suivez l'évolution</h3>
        <p style="font-size:14px;color:var(--text-muted);line-height:1.6">Tableau de bord journalier, graphiques d'humeur, alertes parentales, historique des exercices.</p>
      </div>
    </div>
  </div>
</div>

<!-- PAGE OFFRES -->
<div id="page-offres" class="page">
  <div class="offres-header">
    <div class="hero-eyebrow">Paiement unique · Sans abonnement</div>
    <h2>Nos 4 offres</h2>
    <p style="font-size:16px;color:var(--text-muted);line-height:1.6">Chaque offre contient des exercices, techniques et ressources <strong>100% exclusifs</strong>. Aucun contenu n'est partagé entre les offres.</p>
  </div>
  <div class="offres-grid">

    <!-- OFFRE 1 -->
    <div class="offre-card" onclick="openPayment(1)">
      <div class="offre-header" style="border-bottom:1px solid var(--border)">
        <div class="offre-badge tag-sage">Enfants · 6–11 ans</div>
        <div class="offre-icon" style="background:rgba(184,212,187,.3)">🌱</div>
        <div class="offre-name">Petites Pousses</div>
        <div class="offre-target">Pour les enfants de 6 à 11 ans</div>
        <div class="offre-price">49,99€ <span>TTC</span></div>
        <div class="offre-price-note">Paiement unique · Accès illimité</div>
      </div>
      <div class="offre-body">
        <div class="offre-roles">
          <span class="tag tag-sage">👨‍👩‍👧 Parent</span>
          <span class="tag tag-sage">🧒 Enfant</span>
        </div>
        <ul class="offre-features">
          <li><span class="check">✓</span>Cohérence cardiaque 3-6-5 (guidée enfant)</li>
          <li><span class="check">✓</span>Respiration "Bulle de savon"</li>
          <li><span class="check">✓</span>Respiration "Souffle du Lion"</li>
          <li><span class="check">✓</span>Technique "Ma tortue intérieure"</li>
          <li><span class="check">✓</span>Journal illustré des émotions (enfant)</li>
          <li><span class="check">✓</span>Dashboard parent avec alertes</li>
          <li><span class="check">✓</span>Suivi humeur journalier 7 jours</li>
        </ul>
        <button class="btn btn-primary" style="width:100%">Choisir Petites Pousses →</button>
      </div>
    </div>

    <!-- OFFRE 2 -->
    <div class="offre-card" onclick="openPayment(2)">
      <div class="offre-header" style="border-bottom:1px solid var(--border)">
        <div class="offre-badge tag-teal">Adolescents · 12–18 ans</div>
        <div class="offre-icon" style="background:rgba(168,204,204,.3)">🌊</div>
        <div class="offre-name">Cap Sérénité</div>
        <div class="offre-target">Pour les adolescents de 12 à 18 ans</div>
        <div class="offre-price">119€ <span>TTC</span></div>
        <div class="offre-price-note">Paiement unique · Accès illimité</div>
      </div>
      <div class="offre-body">
        <div class="offre-roles">
          <span class="tag tag-teal">👨‍👩‍👧 Parent</span>
          <span class="tag tag-teal">🧑 Adolescent</span>
        </div>
        <ul class="offre-features">
          <li><span class="check">✓</span>Respiration 4-7-8 anti-stress aigu</li>
          <li><span class="check">✓</span>Technique STOP (pleine conscience)</li>
          <li><span class="check">✓</span>Respiration physiologique (double expir.)</li>
          <li><span class="check">✓</span>Technique du "carnet des victoires"</li>
          <li><span class="check">✓</span>Journal émotionnel texte libre (ado)</li>
          <li><span class="check">✓</span>Dashboard parent discret (résumé)</li>
          <li><span class="check">✓</span>Graphique d'humeur 30 jours</li>
          <li><span class="check">✓</span>Tracker de stress scolaire</li>
        </ul>
        <button class="btn btn-teal" style="width:100%">Choisir Cap Sérénité →</button>
      </div>
    </div>

    <!-- OFFRE 3 -->
    <div class="offre-card" onclick="openPayment(3)">
      <div class="offre-header" style="border-bottom:1px solid var(--border)">
        <div class="offre-badge tag-gold">Famille · 6–18 ans</div>
        <div class="offre-icon" style="background:rgba(232,212,160,.3)">⭐</div>
        <div class="offre-name">Famille Unie</div>
        <div class="offre-target">Parents + enfants + adolescents (2 profils)</div>
        <div class="offre-price">189€ <span>TTC</span></div>
        <div class="offre-price-note">Paiement unique · Accès illimité · 2 enfants</div>
      </div>
      <div class="offre-body">
        <div class="offre-roles">
          <span class="tag tag-gold">👨‍👩‍👧 Parent</span>
          <span class="tag tag-gold">🧒 Enfant</span>
          <span class="tag tag-gold">🧑 Ado</span>
        </div>
        <ul class="offre-features">
          <li><span class="check">✓</span>Ancrage 5-4-3-2-1 (enfant + ado)</li>
          <li><span class="check">✓</span>Relaxation de Jacobson progressive</li>
          <li><span class="check">✓</span>Respiration "Vague de l'océan"</li>
          <li><span class="check">✓</span>Visualisation "Mon lieu de sécurité"</li>
          <li><span class="check">✓</span>Protocole dialogue parent-enfant</li>
          <li><span class="check">✓</span>Journal partagé famille (opt-in)</li>
          <li><span class="check">✓</span>Module harcèlement scolaire complet</li>
          <li><span class="check">✓</span>Dashboard famille avec 2 profils enfants</li>
          <li><span class="check">✓</span>Alertes comportementales avancées</li>
        </ul>
        <button class="btn btn-gold" style="width:100%">Choisir Famille Unie →</button>
      </div>
    </div>

    <!-- OFFRE 4 -->
    <div class="offre-card" onclick="openPayment(4)" style="border:2px solid var(--rose-light)">
      <div class="offre-header" style="border-bottom:1px solid var(--border)">
        <div class="offre-badge tag-rose">Programme complet · Anti-harcèlement</div>
        <div class="offre-icon" style="background:rgba(232,187,187,.3)">🛡️</div>
        <div class="offre-name">Intensif &amp; Harcèlement</div>
        <div class="offre-target" style="font-size:13px;color:var(--text-muted);line-height:1.5">Le programme le plus complet. Conçu pour les familles qui font face au harcèlement scolaire, aux crises d'anxiété sévères, et qui veulent donner à leur enfant les outils pour se reconstruire.</div>
        <div class="offre-price" style="margin-top:12px">269€ <span>TTC</span></div>
        <div class="offre-price-note">Paiement unique · Accès illimité · 4 profils enfants</div>
      </div>
      <div class="offre-body">
        <div class="offre-roles">
          <span class="tag tag-rose">👨‍👩‍👧 Parent</span>
          <span class="tag tag-rose">🧒 Enfant</span>
          <span class="tag tag-rose">🧑 Ado</span>
        </div>
        <ul class="offre-features">
          <li><span class="check">✓</span><strong>Protocole "Mon armure du matin"</strong> — routine 5 min avant l'école</li>
          <li><span class="check">✓</span><strong>Technique "La phrase qui coupe court"</strong> — désamorcer sans s'abaisser</li>
          <li><span class="check">✓</span><strong>Journal "Mes preuves de valeur"</strong> — reconstruire l'estime jour après jour</li>
          <li><span class="check">✓</span>Respiration box avancée 4-4-4-4</li>
          <li><span class="check">✓</span>Protocole crise immédiate (5 min)</li>
          <li><span class="check">✓</span>Détection harcèlement : checklist 10 signaux + analyse</li>
          <li><span class="check">✓</span>Scripts dialogue par âge (6-11 / 12-18 / cyber)</li>
          <li><span class="check">✓</span>Plan d'action harcèlement en 4 étapes</li>
          <li><span class="check">✓</span>Journal confidentiel ado (invisible aux parents)</li>
          <li><span class="check">✓</span>Dashboard intensif : 4 profils + alertes prioritaires</li>
          <li><span class="check">✓</span>Numéros d'urgence intégrés (3018, 119, 3114…)</li>
        </ul>
        <button class="btn btn-rose" style="width:100%;padding:14px;font-size:15px">Choisir ce programme →</button>
      </div>
    </div>
  </div>
</div>

<!-- PAGE DASHBOARD -->
<div id="page-dashboard" class="page">
  <div class="dash-layout">
    <aside class="dash-sidebar">
      <div class="dash-sidebar-title">Sérénum</div>
      <div class="dash-nav-item active" onclick="switchDashSection(&#39;overview&#39;,this)"><span class="icon">🏠</span> Tableau de bord</div>
      <div class="dash-nav-item" onclick="switchDashSection(&#39;journal&#39;,this)"><span class="icon">📓</span> Mon journal</div>
      <div class="dash-nav-item" onclick="switchDashSection(&#39;exercices&#39;,this)"><span class="icon">🧘</span> Exercices</div>
      <div class="dash-nav-item" onclick="switchDashSection(&#39;harcelement&#39;,this)"><span class="icon">🛡️</span> Harcèlement</div>
      <div class="dash-nav-item" onclick="switchDashSection(&#39;evolution&#39;,this)"><span class="icon">📈</span> Évolution</div>
      <div style="margin-top:auto;padding-top:20px;border-top:1px solid var(--border)">
        <div style="font-size:12px;color:var(--text-light);margin-bottom:8px">Offre active</div>
        <div class="tag tag-gold">⭐ Famille Unie</div>
      </div>
    </aside>
    <main class="dash-main">
      <div class="dash-top">
        <div class="dash-greeting">
          <h2 id="dash-greeting-text">Bonjour, Sophie 👋</h2>
          <p id="dash-date-text">Vendredi 29 mai 2026 · Voir comme :</p>
        </div>
        <div class="dash-role-switcher">
          <button class="role-btn active" onclick="switchRole(&#39;parent&#39;,this)">👨‍👩‍👧 Parent</button>
          <button class="role-btn" onclick="switchRole(&#39;enfant&#39;,this)">🧒 Enfant</button>
          <button class="role-btn" onclick="switchRole(&#39;ado&#39;,this)">🧑 Ado</button>
        </div>
      </div>

      <!-- SECTION OVERVIEW -->
      <div id="section-overview" class="tab-content active">
        <!-- PARENT VIEW -->
        <div id="view-parent" class="role-view">
          <div class="metrics-row">
            <div class="metric"><div class="metric-label">Score anxiété Emma</div><div class="metric-value" style="color:var(--rose)">6.4</div><div class="metric-sub">/10 · ↑ depuis hier</div></div>
            <div class="metric"><div class="metric-label">Score anxiété Léo</div><div class="metric-value" style="color:var(--gold)">4.2</div><div class="metric-sub">/10 · stable</div></div>
            <div class="metric"><div class="metric-label">Exercices cette semaine</div><div class="metric-value">12</div><div class="metric-sub">Emma: 8 · Léo: 4</div></div>
            <div class="metric"><div class="metric-label">Streak Emma</div><div class="metric-value" style="color:var(--sage)">7🔥</div><div class="metric-sub">jours consécutifs</div></div>
          </div>
          <div class="dash-grid">
            <div class="card">
              <h3 style="font-size:18px;font-weight:400;margin-bottom:16px">Alertes parentales</h3>
              <div class="alert alert-danger">⚠️ <div><strong>Emma (9 ans)</strong> — Score anxiété élevé (6.4/10). 3 jours consécutifs au-dessus de 6. Surveillance recommandée.</div></div>
              <div class="alert alert-warning">⏰ <div><strong>Léo (14 ans)</strong> — Journal non complété depuis 2 jours. Pensez à l'encourager.</div></div>
              <div class="alert alert-success">✅ <div><strong>Emma</strong> — A complété 3 exercices de respiration aujourd'hui. Excellent engagement !</div></div>
            </div>
            <div class="card">
              <h3 style="font-size:18px;font-weight:400;margin-bottom:16px">Humeur cette semaine</h3>
              <div style="margin-bottom:8px;font-size:12px;color:var(--text-muted)">Emma (bleu) · Léo (vert)</div>
              <div class="chart-wrap">
                <div class="chart-bars" id="mood-chart-parent">
                  <div class="bar-col"><div class="bar" style="height:60%;background:var(--teal-light)"></div><div class="bar" style="height:80%;background:var(--rose-light)"></div><div class="bar-label">Lun</div></div>
                  <div class="bar-col"><div class="bar" style="height:50%;background:var(--teal-light)"></div><div class="bar" style="height:40%;background:var(--rose-light)"></div><div class="bar-label">Mar</div></div>
                  <div class="bar-col"><div class="bar" style="height:70%;background:var(--teal-light)"></div><div class="bar" style="height:60%;background:var(--rose-light)"></div><div class="bar-label">Mer</div></div>
                  <div class="bar-col"><div class="bar" style="height:55%;background:var(--teal-light)"></div><div class="bar" style="height:50%;background:var(--rose-light)"></div><div class="bar-label">Jeu</div></div>
                  <div class="bar-col"><div class="bar" style="height:65%;background:var(--teal-light)"></div><div class="bar" style="height:75%;background:var(--rose-light)"></div><div class="bar-label">Ven</div></div>
                </div>
              </div>
              <div style="font-size:12px;color:var(--text-light);margin-top:8px;text-align:center">Plus haut = meilleure humeur</div>
            </div>
          </div>
          <div class="card dash-full">
            <h3 style="font-size:18px;font-weight:400;margin-bottom:16px">Activité récente</h3>
            <div class="timeline">
              <div class="tl-item"><div class="tl-time">Aujourd'hui · 16h32</div><div class="tl-text">Emma a complété "Bulle de savon" (3 cycles) — Humeur après : 😊</div></div>
              <div class="tl-item"><div class="tl-time">Aujourd'hui · 14h10</div><div class="tl-text">Emma a écrit dans son journal des émotions</div></div>
              <div class="tl-item"><div class="tl-time">Hier · 20h15</div><div class="tl-text">Léo a complété "Respiration 4-7-8" — Humeur après : 😐</div></div>
              <div class="tl-item"><div class="tl-time">Hier · 18h00</div><div class="tl-text">Emma a complété "Tortue intérieure" (5 min) — Humeur après : 😊</div></div>
              <div class="tl-item"><div class="tl-time">Mercredi · 21h30</div><div class="tl-text">Léo a consulté le module harcèlement</div></div>
            </div>
          </div>
        </div>

        <!-- ENFANT VIEW -->
        <div id="view-enfant" class="role-view hidden">
          <div style="background:linear-gradient(135deg,rgba(184,212,187,.3),rgba(250,247,242,.8));border-radius:var(--radius-xl);padding:28px;margin-bottom:20px;text-align:center">
            <div style="font-size:48px;margin-bottom:8px" id="enfant-mood-display">😊</div>
            <div style="font-family:&#39;Cormorant Garamond&#39;,serif;font-size:28px;font-weight:300;margin-bottom:4px">Bonjour Emma ! 🌟</div>
            <div style="font-size:14px;color:var(--text-muted)">Comment tu te sens aujourd'hui ?</div>
          </div>
          <div class="metrics-row" style="grid-template-columns:repeat(3,1fr)">
            <div class="metric"><div class="metric-label">Mon humeur</div><div class="metric-value">😊</div><div class="metric-sub">Aujourd'hui</div></div>
            <div class="metric"><div class="metric-label">Mon streak</div><div class="metric-value" style="color:var(--sage)">7🔥</div><div class="metric-sub">jours</div></div>
            <div class="metric"><div class="metric-label">Exercices faits</div><div class="metric-value">8</div><div class="metric-sub">cette semaine</div></div>
          </div>
          <div class="dash-grid">
            <div class="card">
              <h3 style="font-size:18px;font-weight:400;margin-bottom:12px">Ma bulle du jour 🫧</h3>
              <p style="font-size:14px;color:var(--text-muted);margin-bottom:16px">Fais une respiration "Bulle de savon" maintenant !</p>
              <button class="btn btn-primary" style="width:100%" onclick="switchDashSection(&#39;exercices&#39;,null);setTimeout(()=&gt;startResp(),300)">Commencer →</button>
            </div>
            <div class="card">
              <h3 style="font-size:18px;font-weight:400;margin-bottom:12px">Mes émotions 🎨</h3>
              <div class="mood-picker" style="justify-content:center">
                <button class="mood-btn" onclick="selectMoodEnfant(&#39;😄&#39;,this)">😄</button>
                <button class="mood-btn" onclick="selectMoodEnfant(&#39;😊&#39;,this)">😊</button>
                <button class="mood-btn" onclick="selectMoodEnfant(&#39;😐&#39;,this)">😐</button>
                <button class="mood-btn" onclick="selectMoodEnfant(&#39;😟&#39;,this)">😟</button>
                <button class="mood-btn" onclick="selectMoodEnfant(&#39;😢&#39;,this)">😢</button>
              </div>
              <button class="btn btn-outline btn-sm" style="width:100%;margin-top:8px" onclick="switchDashSection(&#39;journal&#39;,null)">Écrire dans mon journal →</button>
            </div>
          </div>
          <div class="card">
            <h3 style="font-size:18px;font-weight:400;margin-bottom:12px">Mon tableau de super-héros 🦸</h3>
            <div style="display:flex;gap:12px;flex-wrap:wrap">
              <div style="text-align:center;padding:12px;background:var(--cream-dark);border-radius:10px;min-width:80px"><div style="font-size:28px">🫁</div><div style="font-size:11px;color:var(--text-muted)">Respirations</div><div style="font-weight:500">24</div></div>
              <div style="text-align:center;padding:12px;background:var(--cream-dark);border-radius:10px;min-width:80px"><div style="font-size:28px">📓</div><div style="font-size:11px;color:var(--text-muted)">Journaux</div><div style="font-weight:500">7</div></div>
              <div style="text-align:center;padding:12px;background:var(--cream-dark);border-radius:10px;min-width:80px"><div style="font-size:28px">🌟</div><div style="font-size:11px;color:var(--text-muted)">Points</div><div style="font-weight:500">340</div></div>
              <div style="text-align:center;padding:12px;background:rgba(184,212,187,.2);border-radius:10px;min-width:80px;border:1px dashed var(--sage-light)"><div style="font-size:28px">🏆</div><div style="font-size:11px;color:var(--text-muted)">Niveau</div><div style="font-weight:500;color:var(--sage)">Or</div></div>
            </div>
          </div>
        </div>

        <!-- ADO VIEW -->
        <div id="view-ado" class="role-view hidden">
          <div style="background:linear-gradient(135deg,rgba(168,204,204,.2),rgba(250,247,242,.9));border-radius:var(--radius-xl);padding:28px;margin-bottom:20px">
            <div style="font-family:&#39;Cormorant Garamond&#39;,serif;font-size:32px;font-weight:300;margin-bottom:4px">Salut Léo.</div>
            <div style="font-size:15px;color:var(--text-muted)">Prends une minute pour toi aujourd'hui.</div>
          </div>
          <div class="metrics-row">
            <div class="metric"><div class="metric-label">Niveau de stress</div><div class="metric-value" style="color:var(--gold)">4.5</div><div class="metric-sub">/10 · en baisse 👍</div></div>
            <div class="metric"><div class="metric-label">Streak</div><div class="metric-value">4🔥</div><div class="metric-sub">jours</div></div>
            <div class="metric"><div class="metric-label">Exercices</div><div class="metric-value">4</div><div class="metric-sub">cette semaine</div></div>
            <div class="metric"><div class="metric-label">Journal</div><div class="metric-value" style="color:var(--rose)">2j</div><div class="metric-sub">sans écrire</div></div>
          </div>
          <div class="dash-grid">
            <div class="card">
              <h3 style="font-size:18px;font-weight:400;margin-bottom:12px">Aujourd'hui</h3>
              <div class="alert alert-info" style="margin-bottom:12px">📅 Contrôle de maths demain. Tu veux faire une technique anti-stress maintenant ?</div>
              <button class="btn btn-teal btn-sm" onclick="switchDashSection(&#39;exercices&#39;,null)">Voir les exercices →</button>
            </div>
            <div class="card">
              <h3 style="font-size:18px;font-weight:400;margin-bottom:12px">Mon humeur</h3>
              <div class="chart-bars" style="height:80px">
                <div class="bar-col"><div class="bar" style="height:60%;background:var(--teal-light)"></div><div class="bar-label">Lun</div></div>
                <div class="bar-col"><div class="bar" style="height:45%;background:var(--teal-light)"></div><div class="bar-label">Mar</div></div>
                <div class="bar-col"><div class="bar" style="height:70%;background:var(--teal-light)"></div><div class="bar-label">Mer</div></div>
                <div class="bar-col"><div class="bar" style="height:55%;background:var(--teal-light)"></div><div class="bar-label">Jeu</div></div>
                <div class="bar-col"><div class="bar" style="height:65%;background:var(--teal)"></div><div class="bar-label">Ven</div></div>
              </div>
            </div>
          </div>
        </div>
      </div>

      <!-- SECTION JOURNAL -->
      <div id="section-journal" class="tab-content">
        <!-- Parent journal -->
        <div id="journal-parent" class="role-view">
          <div class="journal-header">
            <h3>Journal parental 📔</h3>
            <p>Notez vos observations sur le comportement de vos enfants</p>
          </div>
          <div class="dash-grid">
            <div class="card">
              <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:12px">
                <h3 style="font-size:18px;font-weight:400">Observations du jour</h3>
                <span style="font-size:12px;color:var(--text-light)">29 mai 2026</span>
              </div>
              <div style="margin-bottom:12px">
                <label style="font-size:13px;color:var(--text-muted);margin-bottom:6px;display:block">Enfant observé</label>
                <select style="width:100%;padding:8px 12px;border:1px solid var(--border);border-radius:8px;font-family:&#39;DM Sans&#39;,sans-serif;background:var(--cream)">
                  <option>Emma (9 ans)</option>
                  <option>Léo (14 ans)</option>
                </select>
              </div>
              <textarea class="journal-area" placeholder="Qu&#39;avez-vous remarqué aujourd&#39;hui ? Comportement à l&#39;école, à la maison, appétit, sommeil..."></textarea>
              <div style="display:flex;justify-content:space-between;align-items:center;margin-top:12px">
                <div style="font-size:13px;color:var(--text-muted)">Humeur observée :</div>
                <div class="mood-picker" style="margin:0">
                  <button class="mood-btn" onclick="this.parentNode.querySelectorAll(&#39;.mood-btn&#39;).forEach(b=&gt;b.classList.remove(&#39;selected&#39;));this.classList.add(&#39;selected&#39;)">😄</button>
                  <button class="mood-btn" onclick="this.parentNode.querySelectorAll(&#39;.mood-btn&#39;).forEach(b=&gt;b.classList.remove(&#39;selected&#39;));this.classList.add(&#39;selected&#39;)">😊</button>
                  <button class="mood-btn" onclick="this.parentNode.querySelectorAll(&#39;.mood-btn&#39;).forEach(b=&gt;b.classList.remove(&#39;selected&#39;));this.classList.add(&#39;selected&#39;)">😐</button>
                  <button class="mood-btn" onclick="this.parentNode.querySelectorAll(&#39;.mood-btn&#39;).forEach(b=&gt;b.classList.remove(&#39;selected&#39;));this.classList.add(&#39;selected&#39;)">😟</button>
                  <button class="mood-btn" onclick="this.parentNode.querySelectorAll(&#39;.mood-btn&#39;).forEach(b=&gt;b.classList.remove(&#39;selected&#39;));this.classList.add(&#39;selected&#39;)">😢</button>
                </div>
              </div>
              <button class="btn btn-primary" style="width:100%;margin-top:12px" onclick="saveJournal(&#39;parent&#39;)">Enregistrer</button>
            </div>
            <div class="card">
              <h3 style="font-size:18px;font-weight:400;margin-bottom:12px">Entrées précédentes</h3>
              <div class="timeline">
                <div class="tl-item"><div class="tl-time">28 mai · Emma</div><div class="tl-text">Rentrée de l'école agitée. A pleuré pour les devoirs de math. S'est calmée après la respiration bulle.</div></div>
                <div class="tl-item"><div class="tl-time">27 mai · Emma</div><div class="tl-text">Très bonne journée. Souriante, mange bien. Aucune anxiété notable.</div></div>
                <div class="tl-item"><div class="tl-time">26 mai · Léo</div><div class="tl-text">Renfermé le soir. N'a pas voulu parler du collège. Inquiétude légère.</div></div>
              </div>
            </div>
          </div>
        </div>

        <!-- Enfant journal -->
        <div id="journal-enfant" class="role-view hidden">
          <div class="journal-header" style="background:linear-gradient(135deg,rgba(184,212,187,.4),rgba(250,247,242,.9))">
            <h3>Mon journal secret 🔒</h3>
            <p>C'est ton espace. Écris ce que tu ressens, dessine avec des mots !</p>
          </div>
          <div class="card" style="margin-bottom:20px">
            <div style="text-align:center;margin-bottom:16px">
              <div style="font-size:18px;font-weight:400;font-family:&#39;Cormorant Garamond&#39;,serif;margin-bottom:8px">Comment tu te sens aujourd'hui ?</div>
              <div class="mood-picker" style="justify-content:center">
                <button class="mood-btn" onclick="selectMoodEnfant(&#39;😄&#39;,this)">😄</button>
                <button class="mood-btn selected" onclick="selectMoodEnfant(&#39;😊&#39;,this)">😊</button>
                <button class="mood-btn" onclick="selectMoodEnfant(&#39;😐&#39;,this)">😐</button>
                <button class="mood-btn" onclick="selectMoodEnfant(&#39;😟&#39;,this)">😟</button>
                <button class="mood-btn" onclick="selectMoodEnfant(&#39;😢&#39;,this)">😢</button>
              </div>
            </div>
            <div style="display:grid;grid-template-columns:1fr 1fr;gap:12px;margin-bottom:16px">
              <div>
                <label style="font-size:13px;color:var(--text-muted);display:block;margin-bottom:6px">À l'école aujourd'hui ?</label>
                <select style="width:100%;padding:8px;border:1px solid var(--border);border-radius:8px;font-family:&#39;DM Sans&#39;,sans-serif;background:var(--cream)">
                  <option>C'était bien 😊</option>
                  <option>Ça allait 😐</option>
                  <option>C'était difficile 😟</option>
                  <option>C'était nul 😢</option>
                </select>
              </div>
              <div>
                <label style="font-size:13px;color:var(--text-muted);display:block;margin-bottom:6px">Avec mes amis ?</label>
                <select style="width:100%;padding:8px;border:1px solid var(--border);border-radius:8px;font-family:&#39;DM Sans&#39;,sans-serif;background:var(--cream)">
                  <option>Super bien 😄</option>
                  <option>Bien 😊</option>
                  <option>Comme ci comme ça 😐</option>
                  <option>Mal 😟</option>
                  <option>J'étais seul(e) 😢</option>
                </select>
              </div>
            </div>
            <label style="font-size:13px;color:var(--text-muted);display:block;margin-bottom:8px">Raconte ta journée (à toi seul, tes parents ne lisent pas ça 🔒)</label>
            <textarea class="journal-area" placeholder="Aujourd&#39;hui, j&#39;ai... Je me suis senti(e)... Ce qui m&#39;a rendu(e) heureux/heureuse c&#39;est... Ce qui était difficile c&#39;est..." style="min-height:120px"></textarea>
            <button class="btn btn-primary" style="width:100%;margin-top:12px" onclick="saveJournal(&#39;enfant&#39;)">Enregistrer mon journal 💚</button>
          </div>
          <div class="card">
            <h3 style="font-size:18px;font-weight:400;margin-bottom:12px">Mes émotions cette semaine 🌈</h3>
            <div class="chart-bars" style="height:80px">
              <div class="bar-col"><div class="bar" style="height:80%;background:var(--sage-light)"></div><div class="bar-label">Lun</div></div>
              <div class="bar-col"><div class="bar" style="height:50%;background:var(--rose-light)"></div><div class="bar-label">Mar</div></div>
              <div class="bar-col"><div class="bar" style="height:70%;background:var(--sage-light)"></div><div class="bar-label">Mer</div></div>
              <div class="bar-col"><div class="bar" style="height:60%;background:var(--gold-light)"></div><div class="bar-label">Jeu</div></div>
              <div class="bar-col"><div class="bar" style="height:85%;background:var(--sage)"></div><div class="bar-label">Ven</div></div>
            </div>
          </div>
        </div>

        <!-- Ado journal -->
        <div id="journal-ado" class="role-view hidden">
          <div class="journal-header" style="background:linear-gradient(135deg,rgba(168,204,204,.3),rgba(250,247,242,.9))">
            <h3>Mon espace privé 🔐</h3>
            <p>Journal confidentiel — tes parents ne voient pas le contenu, seulement que tu as écrit.</p>
          </div>
          <div class="card" style="margin-bottom:20px">
            <div style="display:grid;grid-template-columns:1fr 1fr 1fr;gap:12px;margin-bottom:16px">
              <div>
                <label style="font-size:12px;color:var(--text-light);display:block;margin-bottom:6px">NIVEAU DE STRESS</label>
                <input type="range" min="0" max="10" value="4" id="stress-slider" oninput="document.getElementById(&#39;stress-val&#39;).textContent=this.value" style="width:100%">
                <div style="font-size:24px;font-weight:300;font-family:&#39;Cormorant Garamond&#39;,serif;text-align:center" id="stress-val">4</div>
              </div>
              <div>
                <label style="font-size:12px;color:var(--text-light);display:block;margin-bottom:6px">HUMEUR GÉNÉRALE</label>
                <div class="mood-picker" style="justify-content:center;gap:6px;margin:8px 0">
                  <button class="mood-btn" onclick="this.parentNode.querySelectorAll(&#39;.mood-btn&#39;).forEach(b=&gt;b.classList.remove(&#39;selected&#39;));this.classList.add(&#39;selected&#39;)">😄</button>
                  <button class="mood-btn selected" onclick="this.parentNode.querySelectorAll(&#39;.mood-btn&#39;).forEach(b=&gt;b.classList.remove(&#39;selected&#39;));this.classList.add(&#39;selected&#39;)">😐</button>
                  <button class="mood-btn" onclick="this.parentNode.querySelectorAll(&#39;.mood-btn&#39;).forEach(b=&gt;b.classList.remove(&#39;selected&#39;));this.classList.add(&#39;selected&#39;)">😟</button>
                </div>
              </div>
              <div>
                <label style="font-size:12px;color:var(--text-light);display:block;margin-bottom:6px">SOMMEIL</label>
                <select style="width:100%;padding:8px;border:1px solid var(--border);border-radius:8px;font-family:&#39;DM Sans&#39;,sans-serif;background:var(--cream);font-size:13px;margin-top:6px">
                  <option>Bien dormi</option>
                  <option>Moyen</option>
                  <option>Mal dormi</option>
                  <option>Insomnie</option>
                </select>
              </div>
            </div>
            <div style="margin-bottom:12px">
              <label style="font-size:13px;color:var(--text-muted);display:block;margin-bottom:8px">Ce que j'ai envie de dire aujourd'hui</label>
              <textarea class="journal-area" placeholder="Libère-toi... Personne ne lira ça sauf toi. Tu peux parler de l&#39;école, des amis, de ce qui te pèse, de ce qui t&#39;a rendu heureux..." style="min-height:140px"></textarea>
            </div>
            <div style="background:var(--cream-dark);border-radius:8px;padding:12px;margin-bottom:12px">
              <div style="font-size:12px;color:var(--text-muted);margin-bottom:6px">Si tu traverses quelque chose de difficile, n'oublie pas :</div>
              <div style="font-size:13px;color:var(--text)">📞 3018 — Numéro anti-harcèlement (gratuit, anonyme) · 📱 Écris-nous : aide@serenum.fr</div>
            </div>
            <button class="btn btn-teal" style="width:100%" onclick="saveJournal(&#39;ado&#39;)">Sauvegarder en privé 🔐</button>
          </div>
        </div>
      </div>

      <!-- SECTION EXERCICES -->
      <div id="section-exercices" class="tab-content">
        <div class="tabs">
          <button class="tab active" onclick="switchTab(&#39;resp&#39;,&#39;exercices-tabs&#39;,this)">🫁 Respirations</button>
          <button class="tab" onclick="switchTab(&#39;relax&#39;,&#39;exercices-tabs&#39;,this)">🧘 Relaxation</button>
          <button class="tab" onclick="switchTab(&#39;cognitif&#39;,&#39;exercices-tabs&#39;,this)">🧠 Cognitif</button>
        </div>

        <div id="tab-resp" class="tab-content active">
          <div class="resp-player" id="resp-player" style="margin-bottom:20px">
            <div class="resp-phase" id="resp-phase">Prêt à commencer</div>
            <div class="resp-circle" id="resp-circle" style="background:radial-gradient(circle,var(--cream-dark),var(--cream));margin:20px auto">
              <span id="resp-count" style="font-size:48px;font-weight:300;font-family:&#39;Cormorant Garamond&#39;,serif">▶</span>
            </div>
            <div class="resp-progress"><div class="resp-bar" id="resp-bar" style="width:0%"></div></div>
            <div style="font-size:13px;color:var(--text-muted);margin-bottom:16px" id="resp-cycles">Cycles : 0 / 3</div>
            <div style="display:flex;gap:8px;justify-content:center;flex-wrap:wrap">
              <button class="btn btn-outline btn-sm" onclick="startResp(&#39;bulle&#39;)">🫧 Bulle de savon</button>
              <button class="btn btn-outline btn-sm" onclick="startResp(&#39;478&#39;)">4-7-8</button>
              <button class="btn btn-outline btn-sm" onclick="startResp(&#39;box&#39;)">📦 Box breathing</button>
              <button class="btn btn-outline btn-sm" onclick="startResp(&#39;lion&#39;)">🦁 Souffle du Lion</button>
            </div>
          </div>
          <div id="resp-desc" style="font-size:14px;color:var(--text-muted);text-align:center;padding:8px;background:var(--cream-dark);border-radius:8px;margin-bottom:16px"></div>
          <div class="ex-card" onclick="startResp(&#39;bulle&#39;)">
            <div style="display:flex;justify-content:space-between;align-items:flex-start">
              <div>
                <h4>🫧 Bulle de savon</h4>
                <p>Expire très doucement, comme si tu soufflais une bulle fragile. Parfait pour les enfants de 6 à 11 ans.</p>
                <div class="ex-duration">⏱ 3-5 minutes · 🧒 Enfants 6-11 ans · Offre Petites Pousses</div>
              </div>
              <span class="tag tag-sage">Débutant</span>
            </div>
          </div>
          <div class="ex-card" onclick="startResp(&#39;lion&#39;)">
            <div style="display:flex;justify-content:space-between;align-items:flex-start">
              <div>
                <h4>🦁 Souffle du Lion</h4>
                <p>Inspire profondément, expire en rugissant la bouche grande ouverte, langue tirée. Libère la tension immédiatement.</p>
                <div class="ex-duration">⏱ 2-3 minutes · 🧒 Enfants 6-11 ans · Offre Petites Pousses</div>
              </div>
              <span class="tag tag-sage">Amusant</span>
            </div>
          </div>
          <div class="ex-card" onclick="startResp(&#39;478&#39;)">
            <div style="display:flex;justify-content:space-between;align-items:flex-start">
              <div>
                <h4>🌙 Respiration 4-7-8</h4>
                <p>Inspire 4s, retiens 7s, expire 8s. Technique de relaxation profonde, idéale avant un contrôle ou le soir.</p>
                <div class="ex-duration">⏱ 4-8 minutes · 🧑 Adolescents · Offre Cap Sérénité</div>
              </div>
              <span class="tag tag-teal">Intermédiaire</span>
            </div>
          </div>
          <div class="ex-card" onclick="startResp(&#39;box&#39;)">
            <div style="display:flex;justify-content:space-between;align-items:flex-start">
              <div>
                <h4>📦 Box Breathing avancé</h4>
                <p>4 temps égaux (4-4-4-4) avec rétention. Technique des forces spéciales pour contrôler le stress intense et les crises.</p>
                <div class="ex-duration">⏱ 5-10 minutes · 🧑 Tous âges · Offre Intensif</div>
              </div>
              <span class="tag tag-rose">Avancé</span>
            </div>
          </div>
        </div>

        <div id="tab-relax" class="tab-content">
          <div class="ex-card">
            <h4>🐢 Ma tortue intérieure</h4>
            <p>Visualisation guidée pour les enfants : se retirer dans sa "carapace" imaginaire quand le monde devient trop intense. L'enfant apprend à créer un espace de sécurité intérieur.</p>
            <div class="ex-duration">⏱ 8 min · 🧒 Enfants 6-11 ans · Offre Petites Pousses</div>
          </div>
          <div class="ex-card">
            <h4>🌊 Relaxation de Jacobson progressive</h4>
            <p>Contraction-relâchement musculaire systématique de la tête aux pieds. Technique cliniquement validée pour l'anxiété chronique.</p>
            <div class="ex-duration">⏱ 15-20 min · 🧑 Tous âges · Offre Famille Unie</div>
          </div>
          <div class="ex-card">
            <h4>🏝️ Mon lieu de sécurité</h4>
            <p>Visualisation guidée d'un lieu imaginaire parfaitement sûr et apaisant. L'enfant ou l'ado crée mentalement un refuge qu'il peut "visiter" à tout moment.</p>
            <div class="ex-duration">⏱ 12 min · 🧒🧑 Tous âges · Offre Famille Unie</div>
          </div>
          <div class="ex-card">
            <h4>🛡️ Protocole "Mon armure du matin"</h4>
            <p>Routine de 5 minutes à faire avant l'école les jours difficiles : respiration box + visualisation d'un bouclier invisible + phrase de confiance que l'enfant se répète tout bas. Il arrive préparé, pas subi. Guidé étape par étape.</p>
            <div class="ex-duration">⏱ 5 min · 🧒🧑 Tous âges · Offre Intensif &amp; Harcèlement</div>
          </div>
        </div>

        <div id="tab-cognitif" class="tab-content">
          <div class="ex-card">
            <h4>🖐️ Ancrage 5-4-3-2-1</h4>
            <p>Reconnecte-toi au moment présent : 5 choses vues, 4 entendues, 3 touchées, 2 senties, 1 goûtée. Interrompt une spirale anxieuse immédiatement.</p>
            <div class="ex-duration">⏱ 3-5 min · 🧒🧑 Tous âges · Offre Famille Unie</div>
          </div>
          <div class="ex-card">
            <h4>⛔ Technique STOP</h4>
            <p>Stop — Take a breath — Observe — Proceed. Pleine conscience en 4 étapes pour interrompre les pensées automatiques anxieuses chez les ados.</p>
            <div class="ex-duration">⏱ 2-3 min · 🧑 Adolescents · Offre Cap Sérénité</div>
          </div>
          <div class="ex-card">
            <h4>🗣️ Technique "La phrase qui coupe court"</h4>
            <p>Apprendre à l'enfant ou l'ado UNE seule phrase neutre à dire face à un harceleur — ni agressive, ni soumise — pour désamorcer sans escalader. Exemples guidés par âge (6-11 ans / 12-18 ans), avec mises en situation parent-enfant à faire à la maison.</p>
            <div class="ex-duration">⏱ 15 min · 🧒🧑 Tous âges · Offre Intensif &amp; Harcèlement</div>
          </div>
          <div class="ex-card">
            <h4>📓 Journal "Mes preuves de valeur"</h4>
            <p>Un carnet structuré où l'enfant note chaque soir 3 preuves concrètes qu'il a de la valeur : un ami qui lui a souri, une bonne réponse en classe, un moment sympa. Contre-attaque directe contre les pensées négatives instillées par le harcèlement. Inclus : guide parent pour accompagner la démarche.</p>
            <div class="ex-duration">⏱ 5 min/jour · 🧒🧑 Tous âges · Offre Intensif &amp; Harcèlement</div>
          </div>
        </div>
      </div>

      <!-- SECTION HARCELEMENT -->
      <div id="section-harcelement" class="tab-content">
        <div style="margin-bottom:20px">
          <div style="background:linear-gradient(135deg,rgba(196,123,123,.15),rgba(250,247,242,.9));border-radius:var(--radius-lg);padding:24px;margin-bottom:20px">
            <h2 style="font-size:32px;font-weight:300;margin-bottom:8px">🛡️ Module harcèlement scolaire</h2>
            <p style="color:var(--text-muted);font-size:15px;line-height:1.6">Pour détecter les signes, ouvrir le dialogue, et agir. <strong>En cas d'urgence : appelez le 3018</strong> (numéro national, gratuit, 24h/24).</p>
          </div>
          <div class="tabs">
            <button class="tab active" onclick="switchTab(&#39;detection&#39;,&#39;harc-tabs&#39;,this)">🔍 Détection</button>
            <button class="tab" onclick="switchTab(&#39;dialogue&#39;,&#39;harc-tabs&#39;,this)">💬 Comment parler</button>
            <button class="tab" onclick="switchTab(&#39;action&#39;,&#39;harc-tabs&#39;,this)">📋 Plan d'action</button>
            <button class="tab" onclick="switchTab(&#39;urgence&#39;,&#39;harc-tabs&#39;,this)">🆘 Urgence</button>
          </div>

          <div id="tab-detection" class="tab-content active">
            <div class="card" style="margin-bottom:16px">
              <h3 style="font-size:18px;font-weight:400;margin-bottom:4px">Checklist des signaux d'alerte</h3>
              <p style="font-size:13px;color:var(--text-muted);margin-bottom:16px">Cochez les signaux que vous observez chez votre enfant :</p>
              <div id="signals-list">
                <div class="signal-item" onclick="toggleSignal(this)"><div class="signal-check">✓</div><div><strong style="font-size:14px">Refuse d'aller à l'école</strong><p style="font-size:12px;color:var(--text-muted);margin-top:2px">Inventions de maux de ventre, maux de tête le matin</p></div></div>
                <div class="signal-item" onclick="toggleSignal(this)"><div class="signal-check">✓</div><div><strong style="font-size:14px">Rentre systématiquement triste ou en colère</strong><p style="font-size:12px;color:var(--text-muted);margin-top:2px">Changement de comportement notable après l'école</p></div></div>
                <div class="signal-item" onclick="toggleSignal(this)"><div class="signal-check">✓</div><div><strong style="font-size:14px">Perd ses affaires ou arrive avec des objets abîmés</strong><p style="font-size:12px;color:var(--text-muted);margin-top:2px">Vêtements, cartable, matériel scolaire</p></div></div>
                <div class="signal-item" onclick="toggleSignal(this)"><div class="signal-check">✓</div><div><strong style="font-size:14px">Troubles du sommeil ou de l'alimentation</strong><p style="font-size:12px;color:var(--text-muted);margin-top:2px">Insomnies, cauchemars, perte d'appétit soudaine</p></div></div>
                <div class="signal-item" onclick="toggleSignal(this)"><div class="signal-check">✓</div><div><strong style="font-size:14px">Se replie sur lui-même, abandonne ses activités</strong><p style="font-size:12px;color:var(--text-muted);margin-top:2px">Arrête le sport, les amis, les loisirs</p></div></div>
                <div class="signal-item" onclick="toggleSignal(this)"><div class="signal-check">✓</div><div><strong style="font-size:14px">Réactions de peur aux notifications téléphone</strong><p style="font-size:12px;color:var(--text-muted);margin-top:2px">Cache l'écran, angoisse à la réception de messages</p></div></div>
                <div class="signal-item" onclick="toggleSignal(this)"><div class="signal-check">✓</div><div><strong style="font-size:14px">N'invite plus d'amis, évite les sorties</strong><p style="font-size:12px;color:var(--text-muted);margin-top:2px">Isolement social progressif et inexpliqué</p></div></div>
                <div class="signal-item" onclick="toggleSignal(this)"><div class="signal-check">✓</div><div><strong style="font-size:14px">Chute des résultats scolaires</strong><p style="font-size:12px;color:var(--text-muted);margin-top:2px">Difficultés de concentration, notes en baisse soudaine</p></div></div>
                <div class="signal-item" onclick="toggleSignal(this)"><div class="signal-check">✓</div><div><strong style="font-size:14px">Propos négatifs sur lui-même</strong><p style="font-size:12px;color:var(--text-muted);margin-top:2px">"Je suis nul", "Personne ne m'aime", "Je voudrais disparaître"</p></div></div>
                <div class="signal-item" onclick="toggleSignal(this)"><div class="signal-check">✓</div><div><strong style="font-size:14px">Marques inexpliquées, blessures légères</strong><p style="font-size:12px;color:var(--text-muted);margin-top:2px">Bleus, griffures, sans explication cohérente</p></div></div>
              </div>
              <div id="signal-result" style="margin-top:16px;padding:16px;border-radius:10px;display:none">
                <div id="signal-result-text"></div>
              </div>
              <button class="btn btn-primary btn-sm" style="margin-top:12px" onclick="analyzeSignals()">Analyser les signaux</button>
            </div>
          </div>

          <div id="tab-dialogue" class="tab-content">
            <div class="card" style="margin-bottom:16px">
              <h3 style="font-size:18px;font-weight:400;margin-bottom:12px">Comment amener votre enfant à parler</h3>
              <div class="alert alert-info" style="margin-bottom:16px">💡 <div>Le plus difficile n'est pas d'agir, c'est d'ouvrir la porte. Ces scripts vous donnent les mots exacts à utiliser selon l'âge.</div></div>
              <div class="tabs" style="margin-bottom:16px">
                <button class="tab active" onclick="switchTab(&#39;script-6&#39;,&#39;script-tabs&#39;,this)">6-11 ans</button>
                <button class="tab" onclick="switchTab(&#39;script-12&#39;,&#39;script-tabs&#39;,this)">12-18 ans</button>
                <button class="tab" onclick="switchTab(&#39;script-cyber&#39;,&#39;script-tabs&#39;,this)">Cyber-harcèlement</button>
              </div>
              <div id="tab-script-6" class="tab-content active">
                <div style="background:var(--cream-dark);padding:16px;border-radius:10px;margin-bottom:12px">
                  <div style="font-size:12px;color:var(--text-light);margin-bottom:8px;letter-spacing:.5px">PHRASE D'OUVERTURE (soir, calme, sans l'école en tête)</div>
                  <p style="font-size:14px;font-style:italic;color:var(--text)">"Tu sais, ma mission de parent préféré c'est d'être là pour toi, même pour les choses difficiles. Est-ce qu'il y a quelque chose qui te rend triste à l'école en ce moment ?"</p>
                </div>
                <div style="background:var(--cream-dark);padding:16px;border-radius:10px;margin-bottom:12px">
                  <div style="font-size:12px;color:var(--text-light);margin-bottom:8px;letter-spacing:.5px">SI L'ENFANT MINIMISE</div>
                  <p style="font-size:14px;font-style:italic;color:var(--text)">"J'ai remarqué que tu sembles moins heureux quand tu rentres de l'école. Je ne te juge pas, je veux juste comprendre. Tu peux tout me dire."</p>
                </div>
                <div style="background:var(--cream-dark);padding:16px;border-radius:10px">
                  <div style="font-size:12px;color:var(--text-light);margin-bottom:8px;letter-spacing:.5px">SI L'ENFANT AVOUE</div>
                  <p style="font-size:14px;font-style:italic;color:var(--text)">"Merci de me faire confiance. Tu as eu raison de me le dire. Ce n'est pas de ta faute. On va régler ça ensemble, je suis là."</p>
                </div>
              </div>
              <div id="tab-script-12" class="tab-content">
                <div style="background:var(--cream-dark);padding:16px;border-radius:10px;margin-bottom:12px">
                  <div style="font-size:12px;color:var(--text-light);margin-bottom:8px;letter-spacing:.5px">APPROCHE INDIRECTE (ne pas forcer)</div>
                  <p style="font-size:14px;font-style:italic;color:var(--text)">"Je ne veux pas t'envahir. Mais j'ai l'impression que quelque chose ne va pas. Je suis là si tu veux en parler, sans jugement, sans en faire tout un drame."</p>
                </div>
                <div style="background:var(--cream-dark);padding:16px;border-radius:10px;margin-bottom:12px">
                  <div style="font-size:12px;color:var(--text-light);margin-bottom:8px;letter-spacing:.5px">CRÉER DE LA DISTANCE EMOTIONNELLE</div>
                  <p style="font-size:14px;font-style:italic;color:var(--text)">"Imagine qu'un ami me raconte qu'il se fait embêter à l'école. Qu'est-ce que tu lui dirais, toi ?"</p>
                </div>
                <div style="background:var(--cream-dark);padding:16px;border-radius:10px">
                  <div style="font-size:12px;color:var(--text-light);margin-bottom:8px;letter-spacing:.5px">GARANTIR LA CONFIDENTIALITÉ (dans la limite du possible)</div>
                  <p style="font-size:14px;font-style:italic;color:var(--text)">"Ce que tu me dis reste entre nous, sauf si tu es en danger. Je ne vais pas appeler le proviseur sans t'en parler avant."</p>
                </div>
              </div>
              <div id="tab-script-cyber" class="tab-content">
                <div style="background:var(--cream-dark);padding:16px;border-radius:10px;margin-bottom:12px">
                  <div style="font-size:12px;color:var(--text-light);margin-bottom:8px;letter-spacing:.5px">OUVRIR LE SUJET SANS ACCUSER</div>
                  <p style="font-size:14px;font-style:italic;color:var(--text)">"J'ai lu que le cyber-harcèlement touche beaucoup d'ados en ce moment. Est-ce que tu reçois des messages qui te mettent mal à l'aise ?"</p>
                </div>
                <div style="background:var(--cream-dark);padding:16px;border-radius:10px;margin-bottom:12px">
                  <div style="font-size:12px;color:var(--text-light);margin-bottom:8px;letter-spacing:.5px">DÉDRAMATISER LA TECHNOLOGIE</div>
                  <p style="font-size:14px;font-style:italic;color:var(--text)">"Les captures d'écran, je peux t'aider à les sauvegarder. Ce n'est pas une honte d'en avoir reçu, c'est le problème de celui qui les envoie."</p>
                </div>
                <div class="alert alert-warning">⚠️ En cas de contenus sexuels impliquant un mineur : signalez immédiatement sur <strong>internet-signalement.gouv.fr</strong></div>
              </div>
            </div>
          </div>

          <div id="tab-action" class="tab-content">
            <div class="card">
              <h3 style="font-size:18px;font-weight:400;margin-bottom:12px">Plan d'action en 4 étapes</h3>
              <div style="display:grid;gap:16px">
                <div style="padding:16px;border:1px solid var(--border);border-radius:10px;border-left:4px solid var(--sage)">
                  <div style="font-weight:500;margin-bottom:6px">Étape 1 — Documenter</div>
                  <p style="font-size:13px;color:var(--text-muted)">Notez les dates, faits, témoins. Faites des captures d'écran si cyber. Conservez tout. Ne supprimez rien.</p>
                </div>
                <div style="padding:16px;border:1px solid var(--border);border-radius:10px;border-left:4px solid var(--teal)">
                  <div style="font-weight:500;margin-bottom:6px">Étape 2 — Contacter l'école</div>
                  <p style="font-size:13px;color:var(--text-muted)">Demandez un rendez-vous avec le directeur/proviseur ET le référent harcèlement (obligatoire depuis 2023 dans chaque établissement). Apportez vos documents.</p>
                </div>
                <div style="padding:16px;border:1px solid var(--border);border-radius:10px;border-left:4px solid var(--gold)">
                  <div style="font-weight:500;margin-bottom:6px">Étape 3 — Protection immédiate</div>
                  <p style="font-size:13px;color:var(--text-muted)">Contactez le 3018 pour un conseil juridique. En parallèle, renforcez le lien avec votre enfant et maintenez ses activités sociales hors école.</p>
                </div>
                <div style="padding:16px;border:1px solid var(--border);border-radius:10px;border-left:4px solid var(--rose)">
                  <div style="font-weight:500;margin-bottom:6px">Étape 4 — Suivi</div>
                  <p style="font-size:13px;color:var(--text-muted)">Si l'école ne réagit pas sous 15 jours, contactez l'Inspection Académique. En cas de violence physique, dépôt de plainte au commissariat.</p>
                </div>
              </div>
            </div>
          </div>

          <div id="tab-urgence" class="tab-content">
            <div class="alert alert-danger" style="margin-bottom:16px;font-size:15px">🆘 <div><strong>Si votre enfant est en danger immédiat : composez le 15 (SAMU) ou le 17 (Police).</strong></div></div>
            <div style="display:grid;gap:12px">
              <div class="card"><div style="font-size:28px;margin-bottom:8px">📞 3018</div><div style="font-weight:500;margin-bottom:4px">Numéro anti-harcèlement</div><p style="font-size:13px;color:var(--text-muted)">Gratuit · Anonyme · 7j/7 · 9h-23h. Écoute, conseil juridique, signalement.</p></div>
              <div class="card"><div style="font-size:28px;margin-bottom:8px">📞 119</div><div style="font-weight:500;margin-bottom:4px">Enfance en danger</div><p style="font-size:13px;color:var(--text-muted)">Gratuit · 24h/24 · 7j/7. Si votre enfant est en danger physique ou moral grave.</p></div>
              <div class="card"><div style="font-size:28px;margin-bottom:8px">💻 internet-signalement.gouv.fr</div><div style="font-weight:500;margin-bottom:4px">Cyber-harcèlement</div><p style="font-size:13px;color:var(--text-muted)">Signalement officiel de contenus illicites en ligne. Plateforme gouvernementale.</p></div>
              <div class="card"><div style="font-size:28px;margin-bottom:8px">📞 3114</div><div style="font-weight:500;margin-bottom:4px">Numéro national prévention suicide</div><p style="font-size:13px;color:var(--text-muted)">Si votre enfant tient des propos alarmants. Professionnels de santé. 24h/24.</p></div>
            </div>
          </div>
        </div>
      </div>

      <!-- SECTION ÉVOLUTION -->
      <div id="section-evolution" class="tab-content">
        <h2 style="font-size:28px;font-weight:300;margin-bottom:20px">Évolution sur 30 jours</h2>
        <div class="card" style="margin-bottom:20px">
          <h3 style="font-size:18px;font-weight:400;margin-bottom:12px">Score d'anxiété — Emma</h3>
          <div class="chart-bars" style="height:120px;gap:4px">
            <!-- 30 jours simulés -->
            <div class="bar-col"><div class="bar" style="height:70%;background:var(--rose-light)"></div></div>
            <div class="bar-col"><div class="bar" style="height:60%;background:var(--rose-light)"></div></div>
            <div class="bar-col"><div class="bar" style="height:80%;background:var(--rose-light)"></div></div>
            <div class="bar-col"><div class="bar" style="height:75%;background:var(--rose-light)"></div></div>
            <div class="bar-col"><div class="bar" style="height:65%;background:var(--gold-light)"></div></div>
            <div class="bar-col"><div class="bar" style="height:70%;background:var(--gold-light)"></div></div>
            <div class="bar-col"><div class="bar" style="height:55%;background:var(--gold-light)"></div></div>
            <div class="bar-col"><div class="bar" style="height:60%;background:var(--gold-light)"></div></div>
            <div class="bar-col"><div class="bar" style="height:50%;background:var(--sage-light)"></div></div>
            <div class="bar-col"><div class="bar" style="height:45%;background:var(--sage-light)"></div></div>
            <div class="bar-col"><div class="bar" style="height:40%;background:var(--sage-light)"></div></div>
            <div class="bar-col"><div class="bar" style="height:35%;background:var(--sage)"></div></div>
          </div>
          <div style="display:flex;gap:16px;margin-top:12px;font-size:12px">
            <div style="display:flex;align-items:center;gap:6px"><div style="width:12px;height:12px;border-radius:2px;background:var(--rose-light)"></div>Élevé (&gt;6)</div>
            <div style="display:flex;align-items:center;gap:6px"><div style="width:12px;height:12px;border-radius:2px;background:var(--gold-light)"></div>Modéré (4-6)</div>
            <div style="display:flex;align-items:center;gap:6px"><div style="width:12px;height:12px;border-radius:2px;background:var(--sage-light)"></div>Bas (&lt;4)</div>
          </div>
        </div>
        <div class="dash-grid">
          <div class="card">
            <h3 style="font-size:18px;font-weight:400;margin-bottom:12px">Exercices les plus efficaces</h3>
            <div style="display:flex;flex-direction:column;gap:10px">
              <div style="display:flex;justify-content:space-between;align-items:center"><span style="font-size:14px">🫧 Bulle de savon</span><div style="display:flex;align-items:center;gap:8px"><div style="width:80px;height:6px;border-radius:3px;background:var(--cream-dark);overflow:hidden"><div style="width:90%;height:100%;background:var(--sage)"></div></div><span style="font-size:12px;color:var(--text-muted)">9/10</span></div></div>
              <div style="display:flex;justify-content:space-between;align-items:center"><span style="font-size:14px">🐢 Ma tortue</span><div style="display:flex;align-items:center;gap:8px"><div style="width:80px;height:6px;border-radius:3px;background:var(--cream-dark);overflow:hidden"><div style="width:80%;height:100%;background:var(--sage)"></div></div><span style="font-size:12px;color:var(--text-muted)">8/10</span></div></div>
              <div style="display:flex;justify-content:space-between;align-items:center"><span style="font-size:14px">🦁 Souffle du Lion</span><div style="display:flex;align-items:center;gap:8px"><div style="width:80px;height:6px;border-radius:3px;background:var(--cream-dark);overflow:hidden"><div style="width:70%;height:100%;background:var(--gold)"></div></div><span style="font-size:12px;color:var(--text-muted)">7/10</span></div></div>
            </div>
          </div>
          <div class="card">
            <h3 style="font-size:18px;font-weight:400;margin-bottom:12px">Bilan du mois</h3>
            <div style="display:flex;flex-direction:column;gap:10px">
              <div style="display:flex;justify-content:space-between"><span style="font-size:14px;color:var(--text-muted)">Score moyen anxiété</span><span style="font-weight:500;color:var(--rose)">5.8/10</span></div>
              <div style="display:flex;justify-content:space-between"><span style="font-size:14px;color:var(--text-muted)">Total exercices</span><span style="font-weight:500">47</span></div>
              <div style="display:flex;justify-content:space-between"><span style="font-size:14px;color:var(--text-muted)">Entrées journal</span><span style="font-weight:500">22</span></div>
              <div style="display:flex;justify-content:space-between"><span style="font-size:14px;color:var(--text-muted)">Tendance générale</span><span style="font-weight:500;color:var(--sage)">↓ Amélioration</span></div>
            </div>
          </div>
        </div>
      </div>
    </main>
  </div>
</div>

<!-- PAGE MENTIONS LÉGALES -->
<div id="page-legal" class="page">
  <div class="legal-page">
    <div style="margin-bottom:32px">
      <div class="hero-eyebrow">Documents légaux</div>
      <h2>Mentions légales, CGV &amp; CNIL</h2>
      <p style="font-size:14px;color:var(--text-muted);margin-top:8px">Conformes au droit français · RGPD · Code de la consommation</p>
    </div>

    <div class="highlight-box" style="margin-bottom:24px">
      <strong style="font-size:14px">⚠️ Avertissement personnel — À lire avant toute chose</strong>
      <p style="margin-top:8px;font-size:13px">Je suis le créateur de Sérénum. Je ne suis ni médecin, ni psychologue, ni psychothérapeute, ni thérapeute d'aucune sorte. Je suis un parent qui a cherché des solutions concrètes pour aider son enfant face au stress scolaire, et qui partage aujourd'hui ce qu'il a découvert et mis en pratique. Les contenus, exercices et techniques proposés sur cette plateforme ne constituent pas un acte médical, psychologique ou thérapeutique. Ils ne remplacent en aucun cas une consultation médicale, un diagnostic, un traitement ou un suivi professionnel. Aucune guérison n'est promise, garantie ni sous-entendue. Je décline toute responsabilité quant aux résultats obtenus ou non obtenus par l'utilisation de ces outils. En cas de détresse psychologique sévère, de crise ou d'urgence, consultez immédiatement un médecin ou appelez le 15.</p>
    </div>

    <div class="legal-section">
      <h3>1. Identité de l'éditeur</h3>
      <p>Je suis le créateur et éditeur unique de la plateforme Sérénum. Je ne suis ni médecin, ni psychologue, ni thérapeute — je suis un parent qui partage des outils de gestion du stress scolaire.</p>
      <div class="highlight-box" style="margin:16px 0">
        <p><strong>Nom et prénom :</strong> Sébastien GARCIA</p>
        <p><strong>Forme juridique :</strong> Entrepreneur individuel — Micro-entreprise</p>
        <p><strong>SIREN :</strong> 990 963 852</p>
        <p><strong>SIRET :</strong> 990 963 852 00019</p>
        <p><strong>Code APE :</strong> 7022Z</p>
        <p><strong>Adresse du siège :</strong> 28 Rue du Maroc, 29270 Carhaix-Plouguer, France</p>
        <p><strong>Courriel :</strong> sebastien.garcia29@outlook.fr</p>
        <p><strong>Hébergeur :</strong> Vercel Inc., 340 Pine Street, Suite 701, San Francisco, CA 94104, États-Unis — vercel.com</p>
      </div>
      <p style="font-size:13px;color:var(--text-muted)">Conformément à l'article 6 de la loi n°2004-575 du 21 juin 2004 pour la Confiance dans l'Économie Numérique (LCEN).</p>
    </div>

    <div class="legal-section">
      <h3>2. Conditions Générales de Vente (CGV)</h3>
      <p>Les présentes CGV régissent les relations contractuelles entre moi, <strong>Sébastien GARCIA</strong>, entrepreneur individuel en micro-entreprise, exploitant la plateforme sous le nom commercial <strong>Sérénum</strong>, SIREN 990 963 852, SIRET 990 963 852 00019, domicilié au 28 Rue du Maroc, 29270 Carhaix-Plouguer (ci-après "le Vendeur"), et tout utilisateur ayant passé commande sur la plateforme Sérénum (ci-après "le Client"), conformément aux articles L.111-1 et suivants du Code de la consommation.</p>

      <p><strong>2.1 Offres et tarifs</strong></p>
      <ul>
        <li><strong>Petites Pousses</strong> — 49,99 € TTC (TVA 20% incluse, soit 41,66 € HT)</li>
        <li><strong>Cap Sérénité</strong> — 119,00 € TTC (99,17 € HT)</li>
        <li><strong>Famille Unie</strong> — 189,00 € TTC (157,50 € HT)</li>
        <li><strong>Intensif &amp; Harcèlement</strong> — 269,00 € TTC (224,17 € HT)</li>
      </ul>
      <p>Les prix sont indiqués en euros toutes taxes comprises. Paiement unique, sans abonnement récurrent. L'accès à la plateforme est illimité dans le temps pour l'offre choisie.</p>

      <p><strong>2.2 Processus de commande</strong></p>
      <ul>
        <li>1. Sélection de l'offre sur la plateforme</li>
        <li>2. Validation du panier et vérification des informations</li>
        <li>3. Acceptation obligatoire des CGV, mentions légales et CNIL (case à cocher)</li>
        <li>4. Renonciation expresse au droit de rétractation pour contenu numérique (case à cocher)</li>
        <li>5. Saisie des coordonnées bancaires via Stripe (prestataire agréé PCI-DSS)</li>
        <li>6. Confirmation de commande par email dans les 2 heures</li>
      </ul>

      <p><strong>2.3 Droit de rétractation — Article L.221-28 13° du Code de la consommation</strong></p>
      <div class="highlight-box">
        <p style="font-size:13px">Conformément à l'article L.221-28 alinéa 13° du Code de la consommation, le droit de rétractation de 14 jours prévu à l'article L.221-18 <strong>ne s'applique pas</strong> aux contenus numériques non fournis sur support matériel dont l'exécution a commencé avec l'accord exprès du consommateur, qui a par ailleurs renoncé expressément à son droit de rétractation. Cette renonciation est formalisée par la case à cocher obligatoire lors du paiement. Elle est parfaitement légale dès lors que (1) le Client y consent expressément AVANT le début d'exécution, (2) cette information lui a été fournie conformément à l'article L.221-5, et (3) la renonciation est consignée sur support durable.</p>
      </div>

      <p><strong>2.4 Responsabilité limitée</strong></p>
      <p>Je ne saurais être tenu responsable des dommages directs ou indirects résultant de l'utilisation ou de l'impossibilité d'utiliser les services proposés. Ma responsabilité est expressément exclue pour tout préjudice lié à l'état de santé mental ou physique du Client ou des membres de sa famille. Je rappelle que je ne suis ni médecin, ni psychologue, ni thérapeute — les outils proposés ne constituent pas des soins médicaux ou thérapeutiques.</p>

      <p><strong>2.5 Médiation</strong></p>
      <p>En cas de litige non résolu, vous pouvez recourir gratuitement au médiateur de la FEVAD (Fédération du E-Commerce et de la Vente à Distance) : mediateur@fevad.com. Plateforme européenne de règlement en ligne : <strong>ec.europa.eu/consumers/odr</strong></p>
    </div>

    <div class="legal-section">
      <h3>3. Politique de confidentialité &amp; RGPD</h3>
      <p>Conformément au Règlement Général sur la Protection des Données (UE) 2016/679 (RGPD) et à la loi Informatique et Libertés n°78-17 modifiée.</p>

      <p><strong>3.1 Données collectées</strong></p>
      <ul>
        <li>Données d'identification : nom, prénom, adresse email</li>
        <li>Données de paiement : traitées directement par Stripe (non stockées par Sérénum)</li>
        <li>Données d'utilisation : exercices réalisés, fréquence, durée</li>
        <li>Données du journal émotionnel : saisies volontaires, chiffrées en AES-256</li>
        <li>Données concernant les mineurs : soumises au consentement parental obligatoire (art. 8 RGPD — 15 ans minimum en France pour consentir seul)</li>
      </ul>

      <p><strong>3.2 Base légale et finalités</strong></p>
      <ul>
        <li>Exécution du contrat (art. 6.1.b RGPD) : fourniture des services commandés</li>
        <li>Consentement explicite (art. 9 RGPD) : traitement des données de santé (journaux émotionnels)</li>
        <li>Intérêt légitime (art. 6.1.f RGPD) : amélioration du service, sécurité</li>
        <li>Obligation légale (art. 6.1.c RGPD) : facturation, comptabilité</li>
      </ul>

      <p><strong>3.3 Durée de conservation</strong></p>
      <ul>
        <li>Données de compte : 3 ans après la dernière connexion</li>
        <li>Journaux émotionnels : durée de l'abonnement + 1 an</li>
        <li>Données de facturation : 10 ans (obligation comptable)</li>
        <li>Données de mineurs : suppression à la demande parentale ou à la majorité</li>
      </ul>

      <p><strong>3.4 Vos droits (art. 15 à 22 RGPD)</strong></p>
      <ul>
        <li>Droit d'accès à vos données personnelles</li>
        <li>Droit de rectification des données inexactes</li>
        <li>Droit à l'effacement ("droit à l'oubli")</li>
        <li>Droit à la limitation du traitement</li>
        <li>Droit à la portabilité de vos données</li>
        <li>Droit d'opposition au traitement</li>
        <li>Droit de retirer votre consentement à tout moment</li>
      </ul>
      <p>Pour exercer ces droits : <strong>dpo@serenum.fr</strong> ou courrier à l'adresse du siège. Délai de réponse : 1 mois (art. 12 RGPD). Droit de saisir la CNIL : <strong>www.cnil.fr</strong> — 3 place de Fontenoy, 75007 Paris.</p>

      <p><strong>3.5 Sous-traitants et transferts</strong></p>
      <ul>
        <li><strong>Vercel Inc.</strong> — Hébergement (USA, couvert par clauses contractuelles types UE)</li>
        <li><strong>Stripe Inc.</strong> — Paiement sécurisé (USA, couvert par clauses contractuelles types UE, certifié PCI-DSS niveau 1)</li>
      </ul>
      <p>Aucune donnée n'est vendue à des tiers à des fins commerciales.</p>

      <p><strong>3.6 Sécurité</strong></p>
      <p>Chiffrement TLS 1.3 en transit · Chiffrement AES-256 au repos pour les journaux · Authentification à deux facteurs disponible · Notification de violation de données dans les 72h (art. 33 RGPD) · Audit de sécurité annuel</p>

      <p><strong>3.7 Cookies</strong></p>
      <p>Sérénum utilise uniquement des cookies strictement nécessaires au fonctionnement de la plateforme (session, authentification). Aucun cookie publicitaire ou de pistage tiers n'est déposé. Conformément à la délibération CNIL n°2020-091, aucun consentement n'est requis pour ces cookies.</p>
    </div>

    <div class="legal-section">
      <h3>4. Propriété intellectuelle</h3>
      <p>L'ensemble des contenus que j'ai créés pour la plateforme Sérénum (textes, exercices, techniques, interfaces graphiques, logo) sont ma propriété exclusive en tant que Sébastien GARCIA, entrepreneur individuel (SIREN 990 963 852), et sont protégés par le Code de la propriété intellectuelle. Toute reproduction, représentation, modification ou exploitation non autorisée constitue une contrefaçon sanctionnée aux articles L.335-2 et suivants du Code de la propriété intellectuelle.</p>
    </div>

    <div style="text-align:center;padding:24px;background:var(--cream-dark);border-radius:var(--radius-lg);margin-top:32px">
      <p style="font-size:12px;color:var(--text-light)">Documents mis à jour le 29 mai 2026 · Sébastien GARCIA · Entrepreneur individuel · SIREN 990 963 852<br>28 Rue du Maroc, 29270 Carhaix-Plouguer · <span id="creator-email" style="cursor:pointer;text-decoration:underline;color:var(--text-light)" onclick="handleEmailClick()">sebastien.garcia29@outlook.fr</span></p>
    </div>
  </div>
</div>

<!-- MODAL PAIEMENT -->
<div id="payment-overlay" class="payment-overlay hidden" onclick="if(event.target===this)closePayment()">
  <div class="payment-modal">
    <div id="payment-step-1">
      <div style="text-align:center;margin-bottom:20px">
        <div style="font-size:36px;margin-bottom:8px" id="payment-icon">🌱</div>
        <h3 id="payment-title" style="font-size:26px;font-weight:300;margin-bottom:4px">Petites Pousses</h3>
        <p style="font-size:14px;color:var(--text-muted)" id="payment-subtitle">Accompagnement enfants 6-11 ans</p>
        <div style="font-family:&#39;Cormorant Garamond&#39;,serif;font-size:38px;font-weight:300;margin:12px 0" id="payment-price-display">49,99€ <span style="font-size:18px;font-family:&#39;DM Sans&#39;,sans-serif">TTC</span></div>
      </div>

      <div class="disclaimer-box">
        <p>⚠️ <strong>Rappel important :</strong> Je ne suis ni médecin, ni psychologue, ni thérapeute. Ces outils ne remplacent pas un suivi médical ou thérapeutique professionnel. Aucune guérison n'est garantie.</p>
      </div>

      <div class="legal-check" onclick="toggleCheck(&#39;check-cgv&#39;)">
        <input type="checkbox" id="check-cgv" onchange="checkLegal()">
        <label for="check-cgv" onclick="event.stopPropagation()"><strong>J'ai lu et j'accepte les CGV, les mentions légales et la politique de confidentialité (CNIL/RGPD)</strong> de Sérénum dans leur intégralité.</label>
      </div>

      <div class="legal-check" onclick="toggleCheck(&#39;check-retractation&#39;)">
        <input type="checkbox" id="check-retractation" onchange="checkLegal()">
        <label for="check-retractation" onclick="event.stopPropagation()"><strong>Cette case vaut acceptation et renonciation expresse à mon droit de rétractation de 14 jours</strong> (art. L.221-28 13° Code de la consommation), en demandant l'exécution immédiate du contenu numérique.</label>
      </div>

      <div id="legal-warning" style="font-size:12px;color:var(--rose);text-align:center;margin:8px 0;display:none">Vous devez cocher les deux cases pour continuer.</div>

      <div style="margin:20px 0 8px;padding:12px;background:var(--cream-dark);border-radius:8px;display:flex;align-items:center;gap:8px">
        <span style="font-size:18px">🔒</span>
        <span style="font-size:12px;color:var(--text-muted)">Paiement 100% sécurisé via <strong>Stripe</strong> · Certifié PCI-DSS · Vos données bancaires ne transitent pas par Sérénum.</span>
      </div>

      <button class="btn btn-primary" style="width:100%;margin-top:4px;font-size:15px;padding:14px;opacity:.4;cursor:not-allowed;transition:all .3s" id="btn-pay" disabled="" onclick="redirectToStripe()">
        Payer en sécurité via Stripe →
      </button>
      <button class="btn btn-outline" style="width:100%;margin-top:8px" onclick="closePayment()">Annuler</button>
    </div>
  </div>
</div>

<script>
const offresData=[
  {nom:'Petites Pousses',subtitle:'Accompagnement enfants 6-11 ans',prix:'49,99€',icon:'🌱',stripe:'https://buy.stripe.com/7sYfZi1jMcBD9643p2g7e0j'},
  {nom:'Cap Sérénité',subtitle:'Accompagnement adolescents 12-18 ans',prix:'119€',icon:'🌊',stripe:'https://buy.stripe.com/3cI7sM8Me0SVaa8aRug7e0g'},
  {nom:'Famille Unie',subtitle:'Famille complète · 2 profils enfants',prix:'189€',icon:'⭐',stripe:'https://buy.stripe.com/3cI28s5A2cBDcigbVyg7e0h'},
  {nom:'Intensif & Harcèlement',subtitle:'Crises sévères + module harcèlement · 4 profils',prix:'269€',icon:'🛡️',stripe:'https://buy.stripe.com/6oU8wQ4vY6dfgyw0cQg7e0k'}
];
let currentStripeUrl='';
let currentRole='parent';
let respTimer=null;
let respRunning=false;

function showPage(id){
  document.querySelectorAll('.page').forEach(p=>p.classList.remove('active'));
  document.querySelectorAll('.nav-link').forEach(l=>l.classList.remove('active'));
  document.getElementById('page-'+id).classList.add('active');
  window.scrollTo(0,0);
}

function switchRole(role,btn){
  currentRole=role;
  document.querySelectorAll('.role-btn').forEach(b=>b.classList.remove('active'));
  btn.classList.add('active');
  document.querySelectorAll('.role-view').forEach(v=>v.classList.add('hidden'));
  const views=document.querySelectorAll('[id^="view-"]');
  views.forEach(v=>{if(v.id==='view-'+role)v.classList.remove('hidden')});
  const jviews=document.querySelectorAll('[id^="journal-"]');
  jviews.forEach(v=>{if(v.id==='journal-'+role)v.classList.remove('hidden')});
  const g=document.getElementById('dash-greeting-text');
  if(role==='parent')g.textContent='Bonjour, Sophie 👋';
  else if(role==='enfant')g.textContent='Bonjour Emma ! 🌟';
  else g.textContent='Salut Léo. 👋';
}

function switchDashSection(section,el){
  document.querySelectorAll('[id^="section-"]').forEach(s=>s.classList.remove('active'));
  document.querySelectorAll('.dash-nav-item').forEach(i=>i.classList.remove('active'));
  const s=document.getElementById('section-'+section);
  if(s)s.classList.add('active');
  if(el)el.classList.add('active');
  else{
    const items=document.querySelectorAll('.dash-nav-item');
    items.forEach(i=>{if(i.textContent.includes(section==='exercices'?'Exercices':section==='harcelement'?'Harc':section==='journal'?'journal':section==='evolution'?'volution':'Tableau'))i.classList.add('active')});
  }
}

function switchTab(tab,group,btn){
  const parent=btn?btn.closest('.card')||btn.closest('.tab-content')||document.body:document.body;
  const tabs=btn?btn.parentNode.querySelectorAll('.tab'):document.querySelectorAll('.tab');
  const contents=document.querySelectorAll('[id^="tab-"]');
  if(btn){btn.parentNode.querySelectorAll('.tab').forEach(t=>t.classList.remove('active'));btn.classList.add('active');}
  document.getElementById('tab-'+tab).classList.add('active');
  const siblings=document.getElementById('tab-'+tab).parentNode.querySelectorAll('.tab-content');
  siblings.forEach(s=>{if(s.id!=='tab-'+tab)s.classList.remove('active')});
  document.getElementById('tab-'+tab).classList.add('active');
}

const respPatterns={
  bulle:{name:'🫧 Bulle de savon',desc:'Inspire doucement... et expire très lentement comme si tu soufflais une grosse bulle sans la faire éclater.',phases:[{label:'Inspire',dur:4,cls:'inhale'},{label:'Expire doucement',dur:6,cls:'exhale'}],cycles:3},
  '478':{name:'🌙 4-7-8',desc:'Technique de relaxation profonde. Idéale avant un examen ou pour s\'endormir.',phases:[{label:'Inspire',dur:4,cls:'inhale'},{label:'Retiens',dur:7,cls:'hold'},{label:'Expire',dur:8,cls:'exhale'}],cycles:4},
  box:{name:'📦 Box Breathing',desc:'4 temps égaux. Technique des forces spéciales pour contrôler une crise de stress.',phases:[{label:'Inspire',dur:4,cls:'inhale'},{label:'Retiens',dur:4,cls:'hold'},{label:'Expire',dur:4,cls:'exhale'},{label:'Pause',dur:4,cls:'hold'}],cycles:5},
  lion:{name:'🦁 Souffle du Lion',desc:'Inspire profondément par le nez, expire fort par la bouche en ouvrant grand yeux et bouche !',phases:[{label:'Inspire fort',dur:3,cls:'inhale'},{label:'Rugis !',dur:2,cls:'exhale'}],cycles:5}
};

let respPhaseIdx=0,respCycleCount=0,respCurrentPattern=null,respCountdown=null;

function startResp(type='bulle'){
  if(respTimer)clearInterval(respTimer);
  if(respCountdown)clearInterval(respCountdown);
  respCurrentPattern=respPatterns[type];
  respPhaseIdx=0;respCycleCount=0;
  document.getElementById('resp-desc').textContent=respCurrentPattern.desc;
  runRespPhase();
}

function runRespPhase(){
  const pattern=respCurrentPattern;
  const phase=pattern.phases[respPhaseIdx];
  const circ=document.getElementById('resp-circle');
  const phaseEl=document.getElementById('resp-phase');
  const countEl=document.getElementById('resp-count');
  const barEl=document.getElementById('resp-bar');
  const cyclesEl=document.getElementById('resp-cycles');
  phaseEl.textContent=phase.label;
  circ.className='resp-circle '+phase.cls;
  let sec=phase.dur;
  countEl.textContent=sec;
  barEl.style.width='100%';
  barEl.style.transition='none';
  setTimeout(()=>{barEl.style.transition='width '+phase.dur+'s linear';barEl.style.width='0%'},50);
  if(respCountdown)clearInterval(respCountdown);
  respCountdown=setInterval(()=>{
    sec--;
    countEl.textContent=Math.max(0,sec);
    if(sec<=0){
      clearInterval(respCountdown);
      respPhaseIdx++;
      if(respPhaseIdx>=pattern.phases.length){
        respPhaseIdx=0;
        respCycleCount++;
        cyclesEl.textContent='Cycles : '+respCycleCount+' / '+pattern.cycles;
        if(respCycleCount>=pattern.cycles){
          phaseEl.textContent='Terminé 🌿';
          circ.className='resp-circle';
          countEl.textContent='✓';
          barEl.style.width='100%';
          return;
        }
      }
      runRespPhase();
    }
  },1000);
}

function openPayment(num){
  const o=offresData[num-1];
  currentStripeUrl=o.stripe;
  document.getElementById('payment-icon').textContent=o.icon;
  document.getElementById('payment-title').textContent=o.nom;
  document.getElementById('payment-subtitle').textContent=o.subtitle;
  document.getElementById('payment-price-display').innerHTML=o.prix+' <span style="font-size:18px;font-family:\'DM Sans\',sans-serif">TTC</span>';
  document.getElementById('check-cgv').checked=false;
  document.getElementById('check-retractation').checked=false;
  document.getElementById('legal-warning').style.display='none';
  const btn=document.getElementById('btn-pay');
  btn.style.opacity='.4';btn.style.cursor='not-allowed';btn.disabled=true;
  document.getElementById('payment-overlay').classList.remove('hidden');
}

function closePayment(){document.getElementById('payment-overlay').classList.add('hidden');}

function toggleCheck(id){
  const cb=document.getElementById(id);
  cb.checked=!cb.checked;
  checkLegal();
}

function checkLegal(){
  const c1=document.getElementById('check-cgv').checked;
  const c2=document.getElementById('check-retractation').checked;
  const btn=document.getElementById('btn-pay');
  if(c1&&c2){
    btn.style.opacity='1';
    btn.style.cursor='pointer';
    btn.disabled=false;
    document.getElementById('legal-warning').style.display='none';
  } else {
    btn.style.opacity='.4';
    btn.style.cursor='not-allowed';
    btn.disabled=true;
  }
}

function redirectToStripe(){
  const c1=document.getElementById('check-cgv').checked;
  const c2=document.getElementById('check-retractation').checked;
  if(!c1||!c2){
    document.getElementById('legal-warning').style.display='block';
    return;
  }
  window.open(currentStripeUrl,'_blank');
  closePayment();
}

function toggleSignal(el){el.classList.toggle('checked');}

function analyzeSignals(){
  const checked=document.querySelectorAll('#signals-list .signal-item.checked').length;
  const res=document.getElementById('signal-result');
  const txt=document.getElementById('signal-result-text');
  res.style.display='block';
  if(checked<=2){res.style.background='#E8F5EA';res.style.border='1px solid #90C890';txt.innerHTML='<strong style="color:#204020">'+checked+' signal(s) détecté(s) — Vigilance normale</strong><br><span style="font-size:13px;color:#204020">Continuez à observer. Encouragez l\'expression des émotions au quotidien.</span>';}
  else if(checked<=5){res.style.background='#FFF8E8';res.style.border='1px solid #F0D080';txt.innerHTML='<strong style="color:#806020">'+checked+' signaux détectés — Attention recommandée</strong><br><span style="font-size:13px;color:#806020">Plusieurs indicateurs présents. Consultez l\'onglet "Comment parler" pour ouvrir le dialogue. Contactez l\'école si nécessaire.</span>';}
  else{res.style.background='#FFEAEA';res.style.border='1px solid #F0A0A0';txt.innerHTML='<strong style="color:#702020">'+checked+' signaux détectés — Risque élevé · Agissez maintenant</strong><br><span style="font-size:13px;color:#702020">Le nombre de signaux est préoccupant. Appelez le 3018 pour un conseil. Consultez immédiatement l\'onglet "Plan d\'action" et "Urgence".</span>';}
}

function selectMoodEnfant(emoji,btn){
  document.querySelectorAll('.mood-btn').forEach(b=>b.classList.remove('selected'));
  btn.classList.add('selected');
  document.getElementById('enfant-mood-display').textContent=emoji;
}

function saveJournal(role){
  const messages={
    parent:'✅ Observation enregistrée ! Visible dans votre tableau de bord.',
    enfant:'💚 Ton journal est sauvegardé ! Bravo pour avoir pris ce moment pour toi.',
    ado:'🔐 Journal sauvegardé de façon confidentielle.'
  };
  const div=document.createElement('div');
  div.className='alert alert-success';div.style.marginTop='12px';
  div.textContent=messages[role];
  const section=document.getElementById('section-journal');
  section.appendChild(div);
  setTimeout(()=>div.remove(),3000);
}

<!-- MODAL CRÉATEUR SECRET -->
<div id="creator-overlay" style="display:none;position:fixed;inset:0;background:rgba(0,0,0,.7);z-index:500;align-items:center;justify-content:center;padding:20px">
  <div style="background:var(--white);border-radius:var(--radius-xl);padding:40px;max-width:680px;width:100%;max-height:90vh;overflow-y:auto;position:relative">
    <div id="creator-pin-screen">
      <div style="text-align:center;margin-bottom:28px">
        <div style="font-size:36px;margin-bottom:8px">🔐</div>
        <h3 style="font-size:24px;font-weight:300;margin-bottom:4px">Accès créateur</h3>
        <p style="font-size:13px;color:var(--text-muted)">Entrez votre code PIN</p>
      </div>
      <div style="display:flex;gap:10px;justify-content:center;margin-bottom:20px">
        <input type="password" id="pin-input" maxlength="6" placeholder="••••" style="width:120px;text-align:center;font-size:24px;letter-spacing:8px;padding:12px;border:2px solid var(--border);border-radius:12px;font-family:'DM Sans',sans-serif" oninput="checkPin()" onkeydown="if(event.key==='Enter')checkPin(true)"/>
      </div>
      <div id="pin-error" style="text-align:center;font-size:13px;color:var(--rose);margin-bottom:12px;display:none">Code incorrect. Réessayez.</div>
      <div style="display:flex;gap:8px;justify-content:center">
        <button class="btn btn-primary" onclick="checkPin(true)">Entrer →</button>
        <button class="btn btn-outline" onclick="closeCreator()">Annuler</button>
      </div>
    </div>

    <div id="creator-dashboard" style="display:none">
      <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:24px">
        <div>
          <div style="font-size:11px;letter-spacing:2px;text-transform:uppercase;color:var(--sage);margin-bottom:4px">Mode créateur</div>
          <h3 style="font-size:26px;font-weight:300">Contenu complet de Sérénum</h3>
        </div>
        <button onclick="closeCreator()" style="background:none;border:none;font-size:20px;cursor:pointer;color:var(--text-muted)">✕</button>
      </div>

      <!-- OFFRE 1 -->
      <div style="border:1px solid var(--border);border-radius:var(--radius-lg);overflow:hidden;margin-bottom:16px">
        <div style="background:rgba(184,212,187,.2);padding:16px 20px;display:flex;justify-content:space-between;align-items:center;cursor:pointer" onclick="toggleSection('o1')">
          <div><span style="font-size:20px">🌱</span> <strong>Petites Pousses</strong> <span style="font-size:13px;color:var(--text-muted)">— 49,99€ · Enfants 6-11 ans</span></div>
          <span id="arrow-o1" style="color:var(--text-muted)">▼</span>
        </div>
        <div id="section-o1" style="padding:20px;display:none">
          <div style="display:grid;grid-template-columns:1fr 1fr;gap:16px">
            <div>
              <div style="font-size:11px;letter-spacing:1.5px;text-transform:uppercase;color:var(--sage);margin-bottom:10px">Respirations</div>
              <ul style="font-size:13px;color:var(--text-muted);line-height:2;padding-left:16px">
                <li><strong>Bulle de savon</strong> — expire très lentement comme souffler une bulle fragile. 4s inspire / 6s expire. 3 cycles.</li>
                <li><strong>Souffle du Lion</strong> — inspire profond, expire fort bouche grande ouverte langue tirée. Libère la tension. 5 cycles.</li>
                <li><strong>Cohérence cardiaque 3-6-5</strong> — 3 fois/jour, 6 respirations/min, 5 min. Inspire 5s / expire 5s.</li>
                <li><strong>Respiration Tortue</strong> — inspire lentement en rentrant la tête dans les épaules, expire en se détendant. 4 cycles.</li>
              </ul>
            </div>
            <div>
              <div style="font-size:11px;letter-spacing:1.5px;text-transform:uppercase;color:var(--sage);margin-bottom:10px">Exercices & techniques</div>
              <ul style="font-size:13px;color:var(--text-muted);line-height:2;padding-left:16px">
                <li><strong>Ma tortue intérieure</strong> — visualisation guidée 8 min. L'enfant crée une "carapace" imaginaire refuge.</li>
                <li><strong>Journal illustré des émotions</strong> — saisie quotidienne humeur + école + amis + texte libre. Privé, contrôle parental.</li>
                <li><strong>Tableau de super-héros</strong> — gamification : points, streaks, niveaux Bronze/Argent/Or pour motiver.</li>
              </ul>
              <div style="font-size:11px;letter-spacing:1.5px;text-transform:uppercase;color:var(--sage);margin:10px 0">Dashboard parent</div>
              <ul style="font-size:13px;color:var(--text-muted);line-height:2;padding-left:16px">
                <li>Score anxiété journalier /10</li>
                <li>Graphique humeur 7 jours</li>
                <li>Alertes comportementales</li>
                <li>Historique exercices + timeline activité</li>
              </ul>
            </div>
          </div>
        </div>
      </div>

      <!-- OFFRE 2 -->
      <div style="border:1px solid var(--border);border-radius:var(--radius-lg);overflow:hidden;margin-bottom:16px">
        <div style="background:rgba(168,204,204,.2);padding:16px 20px;display:flex;justify-content:space-between;align-items:center;cursor:pointer" onclick="toggleSection('o2')">
          <div><span style="font-size:20px">🌊</span> <strong>Cap Sérénité</strong> <span style="font-size:13px;color:var(--text-muted)">— 119€ · Adolescents 12-18 ans</span></div>
          <span id="arrow-o2" style="color:var(--text-muted)">▼</span>
        </div>
        <div id="section-o2" style="padding:20px;display:none">
          <div style="display:grid;grid-template-columns:1fr 1fr;gap:16px">
            <div>
              <div style="font-size:11px;letter-spacing:1.5px;text-transform:uppercase;color:var(--teal);margin-bottom:10px">Respirations</div>
              <ul style="font-size:13px;color:var(--text-muted);line-height:2;padding-left:16px">
                <li><strong>Respiration 4-7-8</strong> — inspire 4s, retiens 7s, expire 8s. Anti-stress aigu, idéal avant examen. 4 cycles.</li>
                <li><strong>Respiration physiologique</strong> — double inspiration nasale courte + longue expire. Réinitialise le système nerveux. 5 cycles.</li>
                <li><strong>Technique STOP</strong> — Stop / Take a breath / Observe / Proceed. Pleine conscience 4 étapes. 2-3 min.</li>
              </ul>
            </div>
            <div>
              <div style="font-size:11px;letter-spacing:1.5px;text-transform:uppercase;color:var(--teal);margin-bottom:10px">Exercices & techniques</div>
              <ul style="font-size:13px;color:var(--text-muted);line-height:2;padding-left:16px">
                <li><strong>Carnet des victoires</strong> — noter chaque soir 3 petites réussites de la journée pour reconstruire la confiance. Quotidien.</li>
                <li><strong>Journal émotionnel ado</strong> — slider stress /10, humeur, sommeil, texte libre confidentiel. Parents voient seulement "a écrit".</li>
                <li><strong>Tracker stress scolaire</strong> — suivi par matière/événement (contrôle, interro, exposé).</li>
                <li><strong>Graphique humeur 30 jours</strong> — évolution long terme visible parent + ado.</li>
              </ul>
            </div>
          </div>
        </div>
      </div>

      <!-- OFFRE 3 -->
      <div style="border:1px solid var(--border);border-radius:var(--radius-lg);overflow:hidden;margin-bottom:16px">
        <div style="background:rgba(232,212,160,.2);padding:16px 20px;display:flex;justify-content:space-between;align-items:center;cursor:pointer" onclick="toggleSection('o3')">
          <div><span style="font-size:20px">⭐</span> <strong>Famille Unie</strong> <span style="font-size:13px;color:var(--text-muted)">— 189€ · Famille complète · 2 profils</span></div>
          <span id="arrow-o3" style="color:var(--text-muted)">▼</span>
        </div>
        <div id="section-o3" style="padding:20px;display:none">
          <div style="display:grid;grid-template-columns:1fr 1fr;gap:16px">
            <div>
              <div style="font-size:11px;letter-spacing:1.5px;text-transform:uppercase;color:var(--gold);margin-bottom:10px">Respirations</div>
              <ul style="font-size:13px;color:var(--text-muted);line-height:2;padding-left:16px">
                <li><strong>Vague de l'océan</strong> — inspire en montant les bras comme une vague, expire en les descendant. Visualisation + mouvement. 6 cycles.</li>
                <li><strong>Respiration 4-4-4 famille</strong> — à faire ensemble parent + enfant. Synchronisation du souffle pour créer lien et calme partagé.</li>
              </ul>
              <div style="font-size:11px;letter-spacing:1.5px;text-transform:uppercase;color:var(--gold);margin:10px 0">Techniques cognitives</div>
              <ul style="font-size:13px;color:var(--text-muted);line-height:2;padding-left:16px">
                <li><strong>Ancrage 5-4-3-2-1</strong> — 5 choses vues / 4 entendues / 3 touchées / 2 senties / 1 goûtée. Interrompt spirale anxieuse. 3-5 min.</li>
                <li><strong>Relaxation de Jacobson</strong> — contraction-relâchement musculaire progressif tête-pieds. Cliniquement validé. 15-20 min.</li>
              </ul>
            </div>
            <div>
              <div style="font-size:11px;letter-spacing:1.5px;text-transform:uppercase;color:var(--gold);margin-bottom:10px">Outils famille</div>
              <ul style="font-size:13px;color:var(--text-muted);line-height:2;padding-left:16px">
                <li><strong>Mon lieu de sécurité</strong> — visualisation guidée 12 min. Création d'un refuge imaginaire personnalisé.</li>
                <li><strong>Protocole dialogue parent-enfant</strong> — scripts et postures de communication selon l'âge et la situation.</li>
                <li><strong>Journal partagé famille</strong> — opt-in. Parent + enfant peuvent choisir de partager certaines entrées.</li>
                <li><strong>Module harcèlement complet</strong> — checklist 10 signaux + analyse automatique + scripts dialogue + plan 4 étapes.</li>
                <li><strong>Dashboard 2 profils enfants</strong> — alertes avancées, comparaison évolution, graphiques croisés.</li>
              </ul>
            </div>
          </div>
        </div>
      </div>

      <!-- OFFRE 4 -->
      <div style="border:2px solid var(--rose-light);border-radius:var(--radius-lg);overflow:hidden;margin-bottom:16px">
        <div style="background:rgba(232,187,187,.2);padding:16px 20px;display:flex;justify-content:space-between;align-items:center;cursor:pointer" onclick="toggleSection('o4')">
          <div><span style="font-size:20px">⚡</span> <strong>Intensif & Harcèlement</strong> <span style="font-size:13px;color:var(--text-muted)">— 269€ · Crises sévères · 4 profils</span></div>
          <span id="arrow-o4" style="color:var(--text-muted)">▼</span>
        </div>
        <div id="section-o4" style="padding:20px;display:none">
          <div style="display:grid;grid-template-columns:1fr 1fr;gap:16px">
            <div>
              <div style="font-size:11px;letter-spacing:1.5px;text-transform:uppercase;color:var(--rose);margin-bottom:10px">Respirations avancées</div>
              <ul style="font-size:13px;color:var(--text-muted);line-height:2;padding-left:16px">
                <li><strong>Box Breathing 4-4-4-4</strong> — inspire 4s / retiens 4s / expire 4s / pause 4s. Technique forces spéciales. Crises intenses. 5-10 min.</li>
                <li><strong>Protocole crise 5 min</strong> — séquence d'urgence : box breathing 1 min + ancrage 54321 + phrase d'ancrage. Utilisable seul.</li>
              </ul>
              <div style="font-size:11px;letter-spacing:1.5px;text-transform:uppercase;color:var(--rose);margin:10px 0">3 techniques exclusives anti-harcèlement</div>
              <ul style="font-size:13px;color:var(--text-muted);line-height:2;padding-left:16px">
                <li><strong>🛡️ Protocole "Mon armure du matin"</strong> — respiration box + visualisation bouclier + phrase de confiance. 5 min avant l'école. Guidé étape par étape.</li>
                <li><strong>🗣️ Technique "La phrase qui coupe court"</strong> — 1 phrase neutre par âge pour désamorcer le harceleur sans s'abaisser ni escalader. Jeux de rôle parent-enfant inclus. 15 min.</li>
                <li><strong>📓 Journal "Mes preuves de valeur"</strong> — 3 preuves concrètes de valeur chaque soir. Contre-attaque directe contre les pensées négatives instillées par le harcèlement. Guide parent inclus.</li>
              </ul>
            </div>
            <div>
              <div style="font-size:11px;letter-spacing:1.5px;text-transform:uppercase;color:var(--rose);margin-bottom:10px">Module harcèlement renforcé</div>
              <ul style="font-size:13px;color:var(--text-muted);line-height:2;padding-left:16px">
                <li><strong>Checklist 10 signaux</strong> — analyse automatique risque (faible / modéré / élevé).</li>
                <li><strong>Scripts dialogue par âge</strong> — 6-11 ans / 12-18 ans / cyber-harcèlement. Phrases exactes à utiliser.</li>
                <li><strong>Plan d'action 4 étapes</strong> — Documenter / Contacter école / Protection immédiate / Suivi.</li>
                <li><strong>Journal confidentiel ado</strong> — totalement invisible aux parents. Même "a écrit" masqué.</li>
                <li><strong>Numéros intégrés</strong> — 3018 / 119 / 3114 / internet-signalement.gouv.fr.</li>
              </ul>
              <div style="font-size:11px;letter-spacing:1.5px;text-transform:uppercase;color:var(--rose);margin:10px 0">Dashboard intensif</div>
              <ul style="font-size:13px;color:var(--text-muted);line-height:2;padding-left:16px">
                <li>4 profils enfants simultanés</li>
                <li>Alertes prioritaires classées par urgence</li>
                <li>Évolution 30 jours avec tendances</li>
                <li>Efficacité par exercice (score ressenti avant/après)</li>
              </ul>
            </div>
          </div>
        </div>
      </div>

      <div style="text-align:center;padding-top:16px;border-top:1px solid var(--border);margin-top:8px">
        <p style="font-size:12px;color:var(--text-light)">Mode créateur · Sérénum · Sébastien Garcia</p>
        <button class="btn btn-outline btn-sm" style="margin-top:8px" onclick="closeCreator()">Fermer</button>
      </div>
    </div>
  </div>
</div>

<script>
// ── CRÉATEUR : 4 clics sur l'email ──
let emailClickCount=0;
let emailClickTimer=null;
function handleEmailClick(){
  emailClickCount++;
  clearTimeout(emailClickTimer);
  emailClickTimer=setTimeout(()=>{emailClickCount=0;},1800);
  if(emailClickCount>=4){
    emailClickCount=0;
    openCreator();
  }
}
function openCreator(){
  document.getElementById('creator-overlay').style.display='flex';
  document.getElementById('creator-pin-screen').style.display='block';
  document.getElementById('creator-dashboard').style.display='none';
  document.getElementById('pin-input').value='';
  document.getElementById('pin-error').style.display='none';
  setTimeout(()=>document.getElementById('pin-input').focus(),100);
}
function closeCreator(){
  document.getElementById('creator-overlay').style.display='none';
}
function checkPin(submit){
  const val=document.getElementById('pin-input').value;
  if(val==='1622'){
    document.getElementById('creator-pin-screen').style.display='none';
    document.getElementById('creator-dashboard').style.display='block';
    document.getElementById('pin-error').style.display='none';
  } else if(submit && val.length>0){
    document.getElementById('pin-error').style.display='block';
    document.getElementById('pin-input').value='';
  }
}
function toggleSection(id){
  const el=document.getElementById('section-'+id);
  const arrow=document.getElementById('arrow-'+id);
  const open=el.style.display==='block';
  el.style.display=open?'none':'block';
  arrow.textContent=open?'▼':'▲';
}
// Fermer en cliquant l'overlay
document.getElementById('creator-overlay').addEventListener('click',function(e){
  if(e.target===this)closeCreator();
});
</script>


</body></html>
