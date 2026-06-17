<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Trendancy | Customer Insight Consultancy</title>
<style>
@import url('https://fonts.googleapis.com/css2?family=Raleway:wght@300;400;500;600;700;800&family=Lora:wght@400;500&display=swap');
*{box-sizing:border-box;margin:0;padding:0;}
:root{
  --black:#000000;
  --grey-20:#333333;
  --grey-40:#666666;
  --grey-60:#999999;
  --grey-80:#CCCCCC;
  --white:#FFFFFF;
  --green-light:#00CCAA;
  --green-medium:#009980;
  --green-dark:#006655;
  --rose:#FF3355;
}
.hp{font-family:'Lora',serif;max-width:100%;overflow-x:hidden;background:var(--black);}
.nav{background:var(--black);padding:0 2.5rem;display:flex;align-items:center;justify-content:space-between;height:80px;border-bottom:0.5px solid var(--grey-20);}
.nav-brand{display:flex;align-items:center;gap:14px;}
.nav-logo-wrap{display:flex;align-items:center;gap:12px;}
.nav-logo-img{width:44px;height:44px;object-fit:contain;}
.nav-brand-text{display:flex;flex-direction:column;gap:2px;}
.nav-wordmark{font-family:'Raleway',sans-serif;font-weight:800;font-size:18px;color:var(--white);letter-spacing:0.1em;text-transform:uppercase;line-height:1;}
.nav-tagline{font-family:'Raleway',sans-serif;font-size:10px;font-weight:700;color:var(--green-light);letter-spacing:0.14em;text-transform:uppercase;line-height:1;}
.nav-links{display:flex;gap:2.25rem;}
.nav-links a{font-family:'Raleway',sans-serif;font-size:12px;font-weight:600;color:var(--grey-60);text-decoration:none;letter-spacing:0.08em;text-transform:uppercase;}
.nav-links a:hover{color:var(--white);}
.nav-cta{background:var(--green-dark);color:var(--white);font-family:'Raleway',sans-serif;font-size:12px;font-weight:700;border:none;border-radius:4px;padding:10px 22px;cursor:pointer;letter-spacing:0.08em;text-transform:uppercase;}
.nav-cta:hover{background:var(--green-medium);}
.hero{position:relative;min-height:540px;display:flex;align-items:center;justify-content:center;text-align:center;overflow:hidden;background:url('https://static.wixstatic.com/media/b621b9_15d5508a613f4a418909599603b9d8b0~mv2.jpg') no-repeat center center;background-size:cover;}
.hero-overlay{position:absolute;inset:0;background:rgba(0,0,0,0.72);}
.hero-content{position:relative;z-index:2;padding:5rem 2.5rem;}
.hero-eyebrow{font-family:'Raleway',sans-serif;font-size:14px;font-weight:700;letter-spacing:0.2em;text-transform:uppercase;color:var(--green-light);margin-bottom:1.5rem;}
.hero-h1{font-family:'Raleway',sans-serif;font-size:clamp(34px,5vw,60px);font-weight:800;color:var(--white);line-height:1.05;letter-spacing:0.04em;margin-bottom:1.5rem;max-width:740px;margin-left:auto;margin-right:auto;text-transform:uppercase;}
.hero-h1 span{color:var(--green-light);}
.hero-sub{font-family:'Lora',serif;font-size:18px;font-weight:400;color:var(--grey-80);line-height:1.8;max-width:580px;margin:0 auto 2.75rem;}
.hero-actions{display:flex;gap:14px;justify-content:center;flex-wrap:wrap;}
.btn-primary{background:var(--green-medium);color:var(--white);font-family:'Raleway',sans-serif;font-size:12px;font-weight:700;border:none;border-radius:4px;padding:14px 30px;cursor:pointer;letter-spacing:0.1em;text-transform:uppercase;}
.btn-ghost{background:transparent;color:var(--grey-80);font-family:'Raleway',sans-serif;font-size:12px;font-weight:600;border:1px solid var(--grey-40);border-radius:4px;padding:14px 30px;cursor:pointer;letter-spacing:0.1em;text-transform:uppercase;}
.problem{background:var(--grey-20);padding:5rem 2.5rem;text-align:center;}
.section-label{font-family:'Raleway',sans-serif;font-size:13px;font-weight:700;letter-spacing:0.2em;text-transform:uppercase;color:var(--green-light);margin-bottom:1.1rem;}
.problem-h2{font-family:'Raleway',sans-serif;font-size:clamp(20px,3vw,34px);font-weight:800;color:var(--white);line-height:1.1;margin-bottom:1.25rem;max-width:620px;margin-left:auto;margin-right:auto;text-transform:uppercase;letter-spacing:0.04em;}
.problem-body{font-family:'Lora',serif;font-size:17px;font-weight:400;color:var(--grey-80);line-height:1.85;max-width:580px;margin:0 auto;}
.services{background:var(--black);padding:5rem 2.5rem;}
.services-inner{max-width:1000px;margin:0 auto;}
.services-header{text-align:center;margin-bottom:2.75rem;}
.services-h2{font-family:'Raleway',sans-serif;font-size:clamp(20px,3vw,34px);font-weight:800;color:var(--white);line-height:1.1;margin-bottom:0.75rem;text-transform:uppercase;letter-spacing:0.04em;}
.services-h2 span{color:var(--green-light);display:block;}
.services-sub{font-family:'Lora',serif;font-size:16px;color:var(--grey-60);line-height:1.8;max-width:480px;margin:0 auto;}
.services-grid{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:1.5rem;}
.svc-card{background:var(--grey-20);border-radius:6px;padding:2rem 1.75rem 2.25rem;border:0.5px solid var(--grey-40);}
.svc-num{font-family:'Raleway',sans-serif;font-size:12px;font-weight:700;letter-spacing:0.16em;text-transform:uppercase;color:var(--green-medium);margin-bottom:0.75rem;}
.svc-title{font-family:'Raleway',sans-serif;font-size:16px;font-weight:800;color:var(--white);margin-bottom:0.75rem;text-transform:uppercase;letter-spacing:0.06em;}
.svc-body{font-family:'Lora',serif;font-size:14px;color:var(--grey-80);line-height:1.75;}
.svc-tags{display:flex;flex-wrap:wrap;gap:6px;margin-top:1.25rem;}
.svc-tag{font-family:'Raleway',sans-serif;font-size:10px;font-weight:700;letter-spacing:0.06em;background:var(--green-dark);color:var(--grey-80);padding:4px 10px;border-radius:3px;text-transform:uppercase;}
.how{background:var(--grey-20);padding:5rem 2.5rem;text-align:center;}
.how-h2{font-family:'Raleway',sans-serif;font-size:clamp(20px,3vw,34px);font-weight:800;color:var(--white);line-height:1.1;margin-bottom:0.75rem;text-transform:uppercase;letter-spacing:0.04em;}
.how-sub{font-family:'Lora',serif;font-size:16px;color:var(--grey-60);line-height:1.8;max-width:460px;margin:0 auto 2.75rem;}
.how-steps{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:1.25rem;max-width:680px;margin:0 auto;}
.how-step{background:var(--black);border:0.5px solid var(--grey-40);border-radius:6px;padding:1.75rem 1.5rem;text-align:left;}
.step-n{font-family:'Raleway',sans-serif;font-size:12px;font-weight:700;letter-spacing:0.16em;text-transform:uppercase;color:var(--green-medium);margin-bottom:0.6rem;}
.step-title{font-family:'Raleway',sans-serif;font-size:15px;font-weight:800;color:var(--white);margin-bottom:0.5rem;text-transform:uppercase;letter-spacing:0.06em;}
.step-body{font-family:'Lora',serif;font-size:13px;color:var(--grey-60);line-height:1.7;}
.cta-band{background:var(--green-dark);padding:5rem 2.5rem;text-align:center;}
.cta-h2{font-family:'Raleway',sans-serif;font-size:clamp(20px,3vw,34px);font-weight:800;color:var(--white);line-height:1.1;margin-bottom:0.85rem;text-transform:uppercase;letter-spacing:0.04em;}
.cta-sub{font-family:'Lora',serif;font-size:17px;color:rgba(255,255,255,0.75);line-height:1.8;max-width:500px;margin:0 auto 2.25rem;}
.btn-white{background:var(--white);color:var(--black);font-family:'Raleway',sans-serif;font-size:12px;font-weight:700;border:none;border-radius:4px;padding:14px 32px;cursor:pointer;letter-spacing:0.1em;text-transform:uppercase;}
.footer{background:var(--black);padding:2.5rem 2.5rem;display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;gap:20px;border-top:0.5px solid var(--grey-20);}
.footer-brand{display:flex;align-items:center;gap:14px;}
.footer-logo-wrap{display:flex;align-items:center;gap:12px;}
.footer-logo-img{width:44px;height:44px;object-fit:contain;}
.footer-brand-text{display:flex;flex-direction:column;gap:2px;}
.footer-wordmark{font-family:'Raleway',sans-serif;font-weight:800;font-size:14px;color:var(--white);letter-spacing:0.12em;text-transform:uppercase;line-height:1;}
.footer-tagline{font-family:'Raleway',sans-serif;font-size:10px;font-weight:700;color:var(--green-light);letter-spacing:0.14em;text-transform:uppercase;line-height:1;margin-top:3px;}
.footer-desc{font-family:'Raleway',sans-serif;font-size:11px;font-weight:400;color:var(--grey-40);margin-top:4px;letter-spacing:0.06em;text-transform:uppercase;}
.footer-links{display:flex;gap:2rem;}
.footer-links a{font-family:'Raleway',sans-serif;font-size:12px;font-weight:500;color:var(--grey-40);text-decoration:none;letter-spacing:0.06em;text-transform:uppercase;}
.footer-links a:hover{color:var(--green-light);}
.footer-copy{font-family:'Raleway',sans-serif;font-size:11px;color:var(--grey-40);letter-spacing:0.04em;width:100%;padding-top:1.5rem;border-top:0.5px solid var(--grey-20);}
</style>
</head>
<body>
<div class="hp">

  <nav class="nav">
    <div class="nav-brand">
      <div class="nav-logo-wrap">
        <img class="nav-logo-img" src="https://static.wixstatic.com/media/b621b9_0b095878efb2403da3f5f615b24cc232~mv2.png" alt="Trendancy logo">
        <div class="nav-brand-text">
          <span class="nav-wordmark">Trendancy</span>
          <span class="nav-tagline">Grow Smarter</span>
        </div>
      </div>
    </div>
    <div class="nav-links">
      <a href="#">Services</a>
      <a href="#">About</a>
      <a href="#">Contact</a>
    </div>
    <button class="nav-cta">Get started</button>
  </nav>

  <section class="hero">
    <div class="hero-overlay"></div>
    <div class="hero-content">
      <p class="hero-eyebrow">Customer insight consultancy</p>
      <h1 class="hero-h1">Grow Smarter<br>With <span>Advanced</span> Customer Insight</h1>
      <p class="hero-sub">We help small and mid-size businesses<br>identify their most valuable customers,<br>understand them and find more just like them.</p>
      <div class="hero-actions">
        <button class="btn-primary">Start your discovery</button>
        <button class="btn-ghost">Learn how it works</button>
      </div>
    </div>
  </section>

  <section class="problem">
    <p class="section-label">The challenge</p>
    <h2 class="problem-h2">Most businesses are sitting on valuable data they cannot use</h2>
    <p class="problem-body">Small and mid-size businesses collect customer data every day but without the right tools or expertise, it just sits there. Trendancy turns that raw data into clear insight so you can stop guessing and start growing.</p>
  </section>

  <section class="services">
    <div class="services-inner">
      <div class="services-header">
        <p class="section-label">What we do</p>
        <h2 class="services-h2">Three services. One goal.<span>Smarter growth.</span></h2>
        <p class="services-sub">Our core services work together to give you a complete picture of your customers and where to find more of them.</p>
      </div>
      <div class="services-grid">
        <div class="svc-card">
          <p class="svc-num">01 Segment</p>
          <h3 class="svc-title">Customer segmentation</h3>
          <p class="svc-body">We use machine learning to cluster your customers into meaningful groups based on behavior, value, and characteristics so you know exactly who your best customers are.</p>
          <div class="svc-tags"><span class="svc-tag">Purchase history</span><span class="svc-tag">Engagement</span><span class="svc-tag">Demographics</span></div>
        </div>
        <div class="svc-card">
          <p class="svc-num">02 Understand</p>
          <h3 class="svc-title">Consumer insight</h3>
          <p class="svc-body">We enrich your first-party data by matching it with third-party consumer profiles, revealing income, interests, life events, and purchase intent you never had before.</p>
          <div class="svc-tags"><span class="svc-tag">Identity matching</span><span class="svc-tag">Life events</span><span class="svc-tag">Intent data</span></div>
        </div>
        <div class="svc-card">
          <p class="svc-num">03 Expand</p>
          <h3 class="svc-title">Audience expansion</h3>
          <p class="svc-body">Using lookalike modeling, we find new prospective customers who share the characteristics of your most valuable ones, extending your reach and improving return on ad spend.</p>
          <div class="svc-tags"><span class="svc-tag">Lookalike modeling</span><span class="svc-tag">ROAS</span><span class="svc-tag">Campaign reach</span></div>
        </div>
      </div>
    </div>
  </section>

  <section class="how">
    <p class="section-label">How it works</p>
    <h2 class="how-h2">From raw data to real growth</h2>
    <p class="how-sub">A simple, structured process that delivers actionable results without requiring an in-house data team.</p>
    <div class="how-steps">
      <div class="how-step">
        <p class="step-n">Step 01</p>
        <p class="step-title">Discovery</p>
        <p class="step-body">We learn about your business, goals, and the data you have available.</p>
      </div>
      <div class="how-step">
        <p class="step-n">Step 02</p>
        <p class="step-title">Segmentation</p>
        <p class="step-body">We analyze your customer data to identify your most valuable segments.</p>
      </div>
      <div class="how-step">
        <p class="step-n">Step 03</p>
        <p class="step-title">Enrichment</p>
        <p class="step-body">We match your data with third-party profiles for richer consumer insight.</p>
      </div>
      <div class="how-step">
        <p class="step-n">Step 04</p>
        <p class="step-title">Expansion</p>
        <p class="step-body">We build lookalike audiences to help you acquire new high-value customers.</p>
      </div>
    </div>
  </section>

  <section class="cta-band">
    <h2 class="cta-h2">Ready to understand your customers better?</h2>
    <p class="cta-sub">Fill out our short discovery questionnaire and we will be in touch to talk through how Trendancy can help your business grow.</p>
    <button class="btn-white">Start the questionnaire</button>
  </section>

  <footer class="footer">
    <div class="footer-brand">
      <div class="footer-logo-wrap">
        <img class="footer-logo-img" src="https://static.wixstatic.com/media/b621b9_0b095878efb2403da3f5f615b24cc232~mv2.png" alt="Trendancy logo">
        <div class="footer-brand-text">
          <p class="footer-wordmark">Trendancy</p>
          <p class="footer-tagline">Grow Smarter</p>
          <p class="footer-desc">Customer insight consultancy</p>
        </div>
      </div>
    </div>
    <div class="footer-links">
      <a href="https://www.trendancy.com">trendancy.com</a>
      <a href="https://www.linkedin.com/company/Trendancy">LinkedIn</a>
      <a href="https://www.youtube.com/@Trendancy">YouTube</a>
    </div>
    <p class="footer-copy">© 2025 Trendancy. All rights reserved.</p>
  </footer>
</div>
</body>
</html>
