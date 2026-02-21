<!DOCTYPE html>
<html lang="hi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Aman Kumar — Earn 20K+ Monthly | iPreneurPlus</title>
<link href="https://fonts.googleapis.com/css2?family=Syne:wght@400;600;700;800&family=DM+Sans:wght@300;400;500;600&display=swap" rel="stylesheet">
<style>
:root {
  --gold: #F5C018;
  --gold2: #FFD95A;
  --dark: #080810;
  --dark2: #0F0F1A;
  --card: #12121F;
  --border: #1E1E30;
  --text: #EEEEF8;
  --muted: #6868A0;
  --green: #00E676;
  --accent: #7C3AED;
}
*{margin:0;padding:0;box-sizing:border-box;}
html{scroll-behavior:smooth;}
body{
  background:var(--dark);
  color:var(--text);
  font-family:'DM Sans',sans-serif;
  overflow-x:hidden;
}

/* ========== NOISE OVERLAY ========== */
body::after{
  content:'';position:fixed;inset:0;
  background-image:url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)' opacity='0.03'/%3E%3C/svg%3E");
  pointer-events:none;z-index:999;opacity:0.4;
}

/* ========== TIMER BANNER ========== */
.timer-bar{
  background: linear-gradient(90deg, #7C3AED, #4F46E5, #7C3AED);
  background-size:200% 100%;
  animation:shimmer 3s linear infinite;
  text-align:center;padding:10px 16px;
  font-size:13px;font-weight:600;letter-spacing:0.5px;
  position:sticky;top:0;z-index:100;
}
.timer-bar span{color:var(--gold2);font-weight:800;}
@keyframes shimmer{0%{background-position:0%}100%{background-position:200%}}

#countdown{display:inline-flex;gap:6px;align-items:center;margin-left:10px;}
.t-unit{
  background:rgba(0,0,0,0.3);border-radius:6px;
  padding:2px 8px;font-size:14px;font-weight:800;color:#fff;
  font-variant-numeric:tabular-nums;
}

/* ========== NAV ========== */
nav{
  display:flex;align-items:center;justify-content:space-between;
  padding:20px 32px;border-bottom:1px solid var(--border);
  position:sticky;top:42px;z-index:99;
  background:rgba(8,8,16,0.85);backdrop-filter:blur(20px);
}
.nav-logo{font-family:'Syne',sans-serif;font-weight:800;font-size:20px;letter-spacing:-0.5px;}
.nav-logo span{color:var(--gold);}
.nav-cta{
  background:var(--gold);color:#000;
  padding:10px 22px;border-radius:100px;
  font-weight:700;font-size:13px;text-decoration:none;
  transition:transform 0.2s,box-shadow 0.2s;
  box-shadow:0 0 20px rgba(245,192,24,0.3);
}
.nav-cta:hover{transform:scale(1.05);box-shadow:0 0 30px rgba(245,192,24,0.5);}

/* ========== HERO ========== */
.hero{
  min-height:100vh;display:flex;align-items:center;justify-content:center;
  text-align:center;padding:80px 20px;
  position:relative;overflow:hidden;
}
.hero-glow{
  position:absolute;top:50%;left:50%;transform:translate(-50%,-60%);
  width:800px;height:800px;
  background:radial-gradient(circle, rgba(124,58,237,0.18) 0%, rgba(245,192,24,0.08) 40%, transparent 70%);
  pointer-events:none;
}
.hero-badge{
  display:inline-flex;align-items:center;gap:8px;
  background:rgba(245,192,24,0.1);border:1px solid rgba(245,192,24,0.3);
  color:var(--gold);padding:8px 18px;border-radius:100px;
  font-size:12px;font-weight:600;letter-spacing:1px;text-transform:uppercase;
  margin-bottom:28px;
}
.pulse{width:8px;height:8px;background:var(--green);border-radius:50%;animation:pulse 1.5s infinite;}
@keyframes pulse{0%,100%{box-shadow:0 0 0 0 rgba(0,230,118,0.6)}50%{box-shadow:0 0 0 8px rgba(0,230,118,0)}}

.hero h1{
  font-family:'Syne',sans-serif;
  font-size:clamp(38px,7vw,80px);
  font-weight:800;line-height:1.05;
  letter-spacing:-2px;
  margin-bottom:24px;
}
.hero h1 em{font-style:normal;color:var(--gold);}
.hero p{
  max-width:560px;margin:0 auto 36px;
  font-size:17px;color:#A0A0C8;line-height:1.7;font-weight:400;
}

.hero-btns{display:flex;gap:14px;justify-content:center;flex-wrap:wrap;}
.btn-primary{
  background:var(--gold);color:#000;
  padding:16px 36px;border-radius:100px;
  font-weight:700;font-size:15px;text-decoration:none;
  box-shadow:0 0 30px rgba(245,192,24,0.35);
  transition:all 0.2s;display:inline-flex;align-items:center;gap:8px;
}
.btn-primary:hover{transform:translateY(-3px);box-shadow:0 8px 40px rgba(245,192,24,0.5);}
.btn-secondary{
  background:transparent;color:var(--text);
  border:1px solid var(--border);
  padding:16px 36px;border-radius:100px;
  font-weight:600;font-size:15px;text-decoration:none;
  transition:all 0.2s;
}
.btn-secondary:hover{border-color:var(--gold);color:var(--gold);}

.avatars{display:flex;align-items:center;gap:12px;justify-content:center;margin-top:40px;}
.avatar-stack{display:flex;}
.avatar-stack img{
  width:36px;height:36px;border-radius:50%;
  border:2px solid var(--dark);object-fit:cover;margin-left:-10px;
}
.avatar-stack img:first-child{margin-left:0;}
.avatar-text{font-size:13px;color:var(--muted);}
.avatar-text strong{color:var(--gold);}

/* ========== SECTION ========== */
section{padding:90px 20px;}
.container{max-width:1000px;margin:0 auto;}
.section-tag{
  display:inline-block;
  background:rgba(124,58,237,0.15);border:1px solid rgba(124,58,237,0.3);
  color:#A78BFA;padding:5px 14px;border-radius:100px;
  font-size:11px;font-weight:600;letter-spacing:2px;text-transform:uppercase;
  margin-bottom:16px;
}
.section-title{
  font-family:'Syne',sans-serif;font-weight:800;
  font-size:clamp(28px,5vw,46px);letter-spacing:-1px;
  line-height:1.1;margin-bottom:14px;
}
.section-sub{color:var(--muted);font-size:16px;max-width:520px;line-height:1.6;}

/* ========== STATS ROW ========== */
.stats{
  display:grid;grid-template-columns:repeat(auto-fit,minmax(160px,1fr));
  gap:2px;background:var(--border);border-radius:20px;overflow:hidden;
  margin:60px 0;
}
.stat{
  background:var(--card);padding:32px 24px;text-align:center;
  transition:background 0.2s;
}
.stat:hover{background:#1A1A2E;}
.stat-num{
  font-family:'Syne',sans-serif;font-size:42px;font-weight:800;
  color:var(--gold);letter-spacing:-2px;line-height:1;
}
.stat-label{font-size:13px;color:var(--muted);margin-top:6px;font-weight:500;}

/* ========== ABOUT ========== */
.about-grid{display:grid;grid-template-columns:1fr 1fr;gap:48px;align-items:center;}
@media(max-width:680px){.about-grid{grid-template-columns:1fr;}}
.about-img-wrap{position:relative;}
.about-img-wrap img{
  width:100%;border-radius:24px;object-fit:cover;aspect-ratio:4/5;
  border:1px solid var(--border);
}
.about-img-badge{
  position:absolute;bottom:20px;left:50%;transform:translateX(-50%);
  background:var(--gold);color:#000;
  padding:10px 20px;border-radius:100px;
  font-weight:800;font-size:13px;white-space:nowrap;
  box-shadow:0 8px 24px rgba(245,192,24,0.4);
}
.about-text .tag-row{margin-bottom:20px;}
.about-text h2{
  font-family:'Syne',sans-serif;font-size:clamp(26px,4vw,38px);
  font-weight:800;letter-spacing:-1px;margin-bottom:16px;line-height:1.15;
}
.about-text p{color:#A0A0C8;line-height:1.75;font-size:15px;margin-bottom:16px;}
.check-list{list-style:none;display:flex;flex-direction:column;gap:10px;margin-top:20px;}
.check-list li{
  display:flex;align-items:center;gap:12px;
  font-size:14px;font-weight:500;
}
.check-list li::before{
  content:'✓';width:22px;height:22px;
  background:rgba(0,230,118,0.15);color:var(--green);
  border-radius:50%;display:flex;align-items:center;justify-content:center;
  font-size:11px;font-weight:800;flex-shrink:0;
  text-align:center;line-height:22px;
}

/* ========== BENEFITS CARDS ========== */
.benefits-grid{
  display:grid;grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
  gap:16px;margin-top:48px;
}
.benefit-card{
  background:var(--card);border:1px solid var(--border);
  border-radius:20px;padding:28px;
  transition:transform 0.25s,border-color 0.25s;
  position:relative;overflow:hidden;
}
.benefit-card:hover{transform:translateY(-6px);border-color:rgba(245,192,24,0.3);}
.benefit-card::before{
  content:'';position:absolute;top:0;left:0;right:0;height:2px;
  background:linear-gradient(90deg,transparent,var(--gold),transparent);
  opacity:0;transition:opacity 0.3s;
}
.benefit-card:hover::before{opacity:1;}
.bc-icon{font-size:32px;margin-bottom:16px;}
.bc-title{font-family:'Syne',sans-serif;font-size:17px;font-weight:700;margin-bottom:10px;}
.bc-text{color:var(--muted);font-size:14px;line-height:1.65;}

/* ========== REQUIREMENTS ========== */
.req-box{
  background:linear-gradient(135deg,rgba(124,58,237,0.12),rgba(245,192,24,0.06));
  border:1px solid rgba(124,58,237,0.25);
  border-radius:24px;padding:48px;text-align:center;
  position:relative;overflow:hidden;
}
.req-box::before{
  content:'';position:absolute;inset:0;
  background:radial-gradient(circle at 50% 0%, rgba(124,58,237,0.15),transparent 60%);
}
.req-grid{
  display:grid;grid-template-columns:repeat(auto-fit,minmax(160px,1fr));
  gap:20px;margin:36px 0;
}
.req-item{
  background:rgba(255,255,255,0.04);border:1px solid var(--border);
  border-radius:16px;padding:24px 16px;
}
.req-item .req-icon{font-size:28px;margin-bottom:10px;}
.req-item p{font-size:14px;font-weight:600;}

/* ========== TESTIMONIALS ========== */
.testi-grid{
  display:grid;grid-template-columns:repeat(auto-fit,minmax(260px,1fr));
  gap:16px;margin-top:48px;
}
.testi-card{
  background:var(--card);border:1px solid var(--border);
  border-radius:20px;padding:24px;
  transition:border-color 0.25s;
}
.testi-card:hover{border-color:rgba(245,192,24,0.3);}
.testi-img{width:100%;border-radius:12px;margin-bottom:16px;aspect-ratio:4/3;object-fit:cover;}
.testi-name{font-weight:700;font-size:14px;color:var(--gold);}
.testi-label{font-size:12px;color:var(--muted);margin-top:2px;}

/* ========== EARNING PROOF ========== */
.proof-grid{
  display:grid;grid-template-columns:repeat(auto-fit,minmax(240px,1fr));
  gap:16px;margin-top:48px;
}
.proof-card{
  background:var(--card);border:1px solid var(--border);
  border-radius:20px;overflow:hidden;
  transition:transform 0.25s;
}
.proof-card:hover{transform:scale(1.02);}
.proof-card img{width:100%;aspect-ratio:4/3;object-fit:cover;}
.proof-label{padding:14px 16px;font-size:13px;font-weight:600;color:var(--muted);}

/* ========== LEGAL ========== */
.legal-box{
  display:flex;gap:32px;align-items:center;
  background:var(--card);border:1px solid var(--border);border-radius:20px;
  padding:36px;flex-wrap:wrap;
}
.legal-box img{width:140px;height:140px;object-fit:contain;border-radius:12px;flex-shrink:0;}
.legal-text h3{font-family:'Syne',sans-serif;font-size:22px;font-weight:800;margin-bottom:10px;}
.legal-text p{color:var(--muted);font-size:14px;line-height:1.7;}
.legal-badges{display:flex;gap:10px;flex-wrap:wrap;margin-top:16px;}
.lbadge{
  background:rgba(0,230,118,0.1);border:1px solid rgba(0,230,118,0.25);
  color:var(--green);padding:5px 14px;border-radius:100px;
  font-size:12px;font-weight:600;
}

/* ========== CONTACT ========== */
.contact-wrap{
  background:linear-gradient(135deg,var(--card),#0F0F20);
  border:1px solid var(--border);border-radius:24px;padding:48px;
  max-width:600px;margin:48px auto 0;
}
.contact-wrap h3{
  font-family:'Syne',sans-serif;font-size:28px;font-weight:800;
  margin-bottom:8px;text-align:center;
}
.contact-wrap p{color:var(--muted);text-align:center;margin-bottom:32px;font-size:15px;}
.form-group{margin-bottom:16px;}
.form-group input,
.form-group textarea{
  width:100%;background:rgba(255,255,255,0.04);
  border:1px solid var(--border);border-radius:12px;
  padding:14px 18px;color:var(--text);font-family:'DM Sans',sans-serif;
  font-size:14px;outline:none;transition:border-color 0.2s;resize:none;
}
.form-group input:focus,
.form-group textarea:focus{border-color:rgba(245,192,24,0.5);}
.form-group input::placeholder,
.form-group textarea::placeholder{color:var(--muted);}
.btn-submit{
  width:100%;background:var(--gold);color:#000;
  border:none;padding:16px;border-radius:12px;
  font-weight:800;font-size:15px;cursor:pointer;
  transition:all 0.2s;font-family:'DM Sans',sans-serif;
}
.btn-submit:hover{transform:translateY(-2px);box-shadow:0 8px 30px rgba(245,192,24,0.4);}
.success-msg{
  display:none;text-align:center;padding:20px;
  background:rgba(0,230,118,0.1);border:1px solid rgba(0,230,118,0.3);
  border-radius:12px;color:var(--green);font-weight:600;margin-top:16px;
}

/* ========== FOOTER ========== */
footer{
  border-top:1px solid var(--border);padding:32px 20px;
  text-align:center;color:var(--muted);font-size:13px;
}
footer strong{color:var(--gold);}
.disclaimer{
  max-width:700px;margin:16px auto 0;font-size:12px;
  color:#404060;line-height:1.6;
}

/* ========== WHATSAPP FLOAT ========== */
.wa-float{
  position:fixed;bottom:28px;right:28px;
  background:#25D366;color:#fff;
  width:58px;height:58px;border-radius:50%;
  display:flex;align-items:center;justify-content:center;
  text-decoration:none;font-size:28px;
  box-shadow:0 4px 20px rgba(37,211,102,0.5);
  z-index:200;animation:bounce 2s infinite;
}
@keyframes bounce{0%,100%{transform:translateY(0)}50%{transform:translateY(-8px)}}

/* ========== RESPONSIVE ========== */
@media(max-width:600px){
  nav{padding:14px 16px;}
  .req-box,
  .legal-box,
  .contact-wrap{padding:28px 20px;}
  .legal-box{flex-direction:column;}
}
</style>
</head>
<body>

<!-- TIMER BANNER -->
<div class="timer-bar">
  🔥 Limited Time Offer — Sirf <span>10 Slots</span> baaki hain! &nbsp;|&nbsp; Ends in:
  <div id="countdown">
    <span class="t-unit" id="ch">23</span>:
    <span class="t-unit" id="cm">59</span>:
    <span class="t-unit" id="cs">59</span>
  </div>
</div>

<!-- NAV -->
<nav>
  <div class="nav-logo">Aman<span>Kumar</span></div>
  <a href="https://alvo.chat/7cLH" class="nav-cta" target="_blank">💬 Message Now</a>
</nav>

<!-- HERO -->
<section class="hero">
  <div class="hero-glow"></div>
  <div class="container" style="position:relative;z-index:1;">
    <div class="hero-badge">
      <div class="pulse"></div>
      Live — Abhi Join Karo
    </div>
    <h1>
      Sirf <em>1–2 Ghante</em><br>
      Daily Mein Karao<br>
      <em>₹20,000+</em> Monthly
    </h1>
    <p>
      Main Aman Kumar hoon. Main teenagers, job persons aur housewives ko
      part-time income skills sikhata hoon aur earning start karwata hoon —
      bina kisi investment ke.
    </p>
    <div class="hero-btns">
      <a href="https://alvo.chat/7cLH" class="btn-primary" target="_blank">⚡ Abhi Shuru Karo</a>
      <a href="#proof" class="btn-secondary">Real Proof Dekho →</a>
    </div>
    <div class="avatars">
      <div class="avatar-stack">
        <img src="https://randomuser.me/api/portraits/men/32.jpg" alt="">
        <img src="https://randomuser.me/api/portraits/women/45.jpg" alt="">
        <img src="https://randomuser.me/api/portraits/men/76.jpg" alt="">
        <img src="https://randomuser.me/api/portraits/women/65.jpg" alt="">
      </div>
      <div class="avatar-text"><strong>50+ logon</strong> ko already train kar chuka hoon</div>
    </div>
  </div>
</section>

<!-- STATS -->
<div class="container">
  <div class="stats">
    <div class="stat">
      <div class="stat-num">₹50K+</div>
      <div class="stat-label">Total Earning</div>
    </div>
    <div class="stat">
      <div class="stat-num">50+</div>
      <div class="stat-label">Students Trained</div>
    </div>
    <div class="stat">
      <div class="stat-num">₹20K+</div>
      <div class="stat-label">Monthly Earn Possible</div>
    </div>
    <div class="stat">
      <div class="stat-num">1–2h</div>
      <div class="stat-label">Daily Time Enough</div>
    </div>
  </div>
</div>

<!-- ABOUT -->
<section id="about">
  <div class="container">
    <div class="about-grid">
      <div class="about-img-wrap">
        <img src="aman-photo.jpg" alt="Aman Kumar">
        <div class="about-img-badge">🏆 Six Figure Earner</div>
      </div>
      <div class="about-text">
        <div class="tag-row"><span class="section-tag">Mere Baare Mein</span></div>
        <h2>Main Aapko Sikhaunga <em style="color:var(--gold)">Asli Skills</em> Se Earn Karna</h2>
        <p>Main ek passionate affiliate marketer hoon jo iPreneurPlus jaise trusted platform par kaam kar raha hoon.</p>
        <p>Yahan main do tarike se earning karta hoon — high-quality digital products ko promote karke commission ke through, aur logon ko sahi skills sikhakar unki earning start karwakar.</p>
        <p>Mera focus sirf selling nahi, balki <strong>value dena aur long-term growth create karna</strong> hai.</p>
        <ul class="check-list">
          <li>Koi investment nahi chahiye shuru mein</li>
          <li>Sirf smartphone aur 1-2 ghante daily</li>
          <li>Step-by-step guidance mere saath</li>
          <li>Real skills jo life mein kaam aayein</li>
        </ul>
      </div>
    </div>
  </div>
</section>

<!-- BENEFITS -->
<section id="benefits" style="background:var(--dark2);">
  <div class="container">
    <div style="text-align:center;">
      <span class="section-tag">Kya Milega</span>
      <h2 class="section-title">iPreneurPlus Kyun Join Karein?</h2>
      <p class="section-sub" style="margin:0 auto;">Ye sirf earning platform nahi — ek complete growth system hai</p>
    </div>
    <div class="benefits-grid">
      <div class="benefit-card">
        <div class="bc-icon">🎯</div>
        <div class="bc-title">Skills + Practical Training</div>
        <div class="bc-text">Sirf theory nahi, balki real skills — affiliate marketing, digital selling aur online earning systems jo actually kaam karti hain.</div>
      </div>
      <div class="benefit-card">
        <div class="bc-icon">💰</div>
        <div class="bc-title">Skills ke Sath Earning</div>
        <div class="bc-text">Skills seekhte hi earning shuru hoti hai. Part-time kaam karke bhi log regular income generate kar rahe hain.</div>
      </div>
      <div class="benefit-card">
        <div class="bc-icon">✈️</div>
        <div class="bc-title">Trips & Meetups</div>
        <div class="bc-text">Performance ke basis par national trips, live meetups aur top leaders ke sath networking ka mauka milta hai.</div>
      </div>
      <div class="benefit-card">
        <div class="bc-icon">🎁</div>
        <div class="bc-title">Rewards & Gifts</div>
        <div class="bc-text">Achha performance karne par cash rewards, gadgets, gifts aur special recognitions bhi milte hain.</div>
      </div>
      <div class="benefit-card">
        <div class="bc-icon">🤝</div>
        <div class="bc-title">Full Support System</div>
        <div class="bc-text">Beginners ke liye full support — training, guidance aur step-by-step help mere aur team ke sath.</div>
      </div>
      <div class="benefit-card">
        <div class="bc-icon">🚀</div>
        <div class="bc-title">Long-Term Growth</div>
        <div class="bc-text">Sirf short-term earning nahi, balki long-term scalable income aur personal growth par focus.</div>
      </div>
    </div>
  </div>
</section>

<!-- REQUIREMENTS -->
<section>
  <div class="container">
    <div class="req-box">
      <span class="section-tag">Simple Requirements</span>
      <h2 class="section-title">Kaun Join Kar Sakta Hai?</h2>
      <p style="color:var(--muted);font-size:15px;position:relative;">Teenager ho, job karte ho, ya ghar par ho — sab ke liye hai</p>
      <div class="req-grid" style="position:relative;">
        <div class="req-item">
          <div class="req-icon">📱</div>
          <p>Smartphone</p>
        </div>
        <div class="req-item">
          <div class="req-icon">🌐</div>
          <p>Basic English</p>
        </div>
        <div class="req-item">
          <div class="req-icon">⏰</div>
          <p>Daily 1-2 Hours</p>
        </div>
        <div class="req-item">
          <div class="req-icon">📶</div>
          <p>Good Internet</p>
        </div>
      </div>
      <div style="position:relative;">
        <div style="background:rgba(245,192,24,0.1);border:1px solid rgba(245,192,24,0.3);display:inline-block;padding:8px 20px;border-radius:100px
