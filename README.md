[index.html](https://github.com/user-attachments/files/27397633/index.html)
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Sidebar Services — Court Filing & Document Running in New York</title>
<meta name="description" content="Fast, reliable court filing and document running for law firms and solo attorneys throughout New York.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,500;0,600;1,300;1,400&family=Jost:wght@300;400;500&display=swap" rel="stylesheet">
<style>
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
:root{--beige:#f5f0e8;--beige-mid:#ede6d6;--beige-dark:#e0d5c0;--beige-deep:#c9bda3;--brown:#6b5b45;--brown-dark:#4a3f30;--ink:#2c2419;--muted:#9a8e7e;--white:#faf8f4;--accent:#7a6248}
html{scroll-behavior:smooth}
body{font-family:'Jost',sans-serif;background:var(--beige);color:var(--ink);font-size:16px;line-height:1.6;overflow-x:hidden}

/* NAV */
nav{position:fixed;top:0;left:0;right:0;z-index:100;display:flex;justify-content:space-between;align-items:center;padding:1rem 4rem;background:rgba(245,240,232,0.97);border-bottom:1px solid var(--beige-dark);backdrop-filter:blur(8px)}
.logo{display:flex;align-items:center;gap:.75rem;text-decoration:none}
.logo img{height:44px;width:auto}
.logo-text{display:flex;flex-direction:column;line-height:1.15}
.logo-name{font-family:'Cormorant Garamond',serif;font-size:1.15rem;font-weight:600;color:var(--brown-dark);letter-spacing:.04em}
.logo-tagline{font-size:.58rem;font-weight:400;letter-spacing:.18em;text-transform:uppercase;color:var(--muted)}
.nav-links{display:flex;gap:2.5rem;list-style:none;align-items:center}
.nav-links a{color:var(--brown);text-decoration:none;font-size:.78rem;letter-spacing:.1em;text-transform:uppercase;font-weight:400;transition:color .2s}
.nav-links a:hover{color:var(--ink)}
.nav-cta{padding:.6rem 1.4rem!important;background:var(--brown-dark)!important;color:var(--beige)!important;border-radius:2px;font-weight:500!important;transition:background .2s!important}
.nav-cta:hover{background:var(--ink)!important}

/* HERO */
.hero{min-height:100vh;display:grid;grid-template-columns:1fr 1fr;align-items:center;padding:8rem 4rem 4rem;gap:4rem}
.hero-badge{display:inline-flex;align-items:center;gap:.5rem;font-size:.7rem;letter-spacing:.2em;text-transform:uppercase;color:var(--brown);background:var(--beige-mid);border:1px solid var(--beige-dark);padding:.4rem .9rem;border-radius:2px;margin-bottom:1.75rem}
.hero-badge::before{content:'';width:6px;height:6px;border-radius:50%;background:var(--brown);opacity:.6}
.hero h1{font-family:'Cormorant Garamond',serif;font-size:clamp(3rem,5vw,4.5rem);font-weight:300;line-height:1.15;color:var(--ink);margin-bottom:1.5rem}
.hero h1 em{font-style:italic;color:var(--brown)}
.hero-sub{font-size:1rem;font-weight:300;color:var(--muted);max-width:420px;margin-bottom:2.5rem;line-height:1.75}
.hero-cta{display:flex;gap:1rem;flex-wrap:wrap;align-items:center}
.btn-primary{display:inline-block;padding:.85rem 2rem;background:var(--brown-dark);color:var(--beige);text-decoration:none;font-size:.78rem;font-weight:500;letter-spacing:.1em;text-transform:uppercase;border-radius:2px;transition:background .2s;border:none;cursor:pointer;font-family:'Jost',sans-serif}
.btn-primary:hover{background:var(--ink)}
.btn-outline{display:inline-block;padding:.85rem 2rem;border:1px solid var(--beige-deep);color:var(--brown);text-decoration:none;font-size:.78rem;font-weight:400;letter-spacing:.1em;text-transform:uppercase;border-radius:2px;transition:border-color .2s,color .2s}
.btn-outline:hover{border-color:var(--brown);color:var(--ink)}
.hero-right{display:flex;justify-content:center;align-items:center}
.hero-emblem{width:min(360px,100%);aspect-ratio:1;background:var(--white);border:1px solid var(--beige-dark);border-radius:50%;display:flex;flex-direction:column;align-items:center;justify-content:center;gap:.6rem;padding:3rem;box-shadow:0 8px 48px rgba(107,91,69,0.08)}
.hero-emblem img{width:160px;height:auto}
.emblem-rule{width:40px;height:1px;background:var(--beige-deep)}
.emblem-sub{font-size:.62rem;letter-spacing:.25em;text-transform:uppercase;color:var(--muted)}

/* STATS */
.stats-bar{background:var(--brown-dark);display:grid;grid-template-columns:repeat(3,1fr)}
.stat{padding:2rem;text-align:center;border-right:1px solid rgba(255,255,255,0.08)}
.stat:last-child{border-right:none}
.stat-num{font-family:'Cormorant Garamond',serif;font-size:2.5rem;font-weight:300;color:var(--beige);line-height:1}
.stat-label{font-size:.7rem;letter-spacing:.15em;text-transform:uppercase;color:rgba(245,240,232,0.5);margin-top:.4rem}

/* SERVICES */
.services{padding:6rem 4rem;background:var(--white)}
.section-label{font-size:.68rem;letter-spacing:.25em;text-transform:uppercase;color:var(--brown);margin-bottom:.6rem}
.section-title{font-family:'Cormorant Garamond',serif;font-size:clamp(2rem,4vw,3rem);font-weight:300;color:var(--ink);line-height:1.2;margin-bottom:3rem}
.services-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(240px,1fr));gap:1.5rem}
.service-card{background:var(--beige);border:1px solid var(--beige-dark);border-radius:4px;padding:2rem;transition:box-shadow .2s,transform .2s}
.service-card:hover{box-shadow:0 4px 24px rgba(107,91,69,0.1);transform:translateY(-2px)}
.service-num{font-family:'Cormorant Garamond',serif;font-size:2.5rem;color:var(--beige-deep);line-height:1;margin-bottom:.75rem;font-weight:300}
.service-name{font-family:'Cormorant Garamond',serif;font-size:1.3rem;font-weight:500;color:var(--ink);margin-bottom:.6rem}
.service-desc{font-size:.88rem;font-weight:300;color:var(--muted);line-height:1.7}

/* WHY */
.why{padding:6rem 4rem;background:var(--beige-mid)}
.why-grid{display:grid;grid-template-columns:1fr 1fr;gap:5rem;align-items:center}
.why-points{list-style:none;margin-top:2rem}
.why-points li{padding:1rem 0;border-bottom:1px solid var(--beige-dark);font-size:.92rem;font-weight:300;color:var(--brown-dark);display:flex;gap:1rem;align-items:flex-start;line-height:1.6}
.why-check{width:18px;height:18px;border-radius:50%;background:var(--brown-dark);display:flex;align-items:center;justify-content:center;flex-shrink:0;margin-top:2px}
.why-check svg{width:9px;height:9px}
.why-right-card{background:var(--white);border:1px solid var(--beige-dark);border-radius:4px;padding:3rem}
.why-right-card blockquote{font-family:'Cormorant Garamond',serif;font-size:1.5rem;font-weight:300;font-style:italic;color:var(--brown-dark);line-height:1.5;margin-bottom:1.5rem}
.quote-attr{font-size:.75rem;letter-spacing:.12em;text-transform:uppercase;color:var(--muted)}
.clients{margin-top:2rem;padding-top:2rem;border-top:1px solid var(--beige-dark)}
.clients-label{font-size:.68rem;letter-spacing:.2em;text-transform:uppercase;color:var(--muted);margin-bottom:1rem}
.client-pills{display:flex;flex-wrap:wrap;gap:.5rem}
.pill{padding:.35rem .85rem;background:var(--beige-mid);border:1px solid var(--beige-dark);border-radius:20px;font-size:.75rem;color:var(--brown)}

/* CONTACT */
.contact{padding:6rem 4rem;background:var(--white);display:grid;grid-template-columns:1fr 1fr;gap:5rem;align-items:start}
.contact-left h2{font-family:'Cormorant Garamond',serif;font-size:clamp(2rem,3.5vw,3rem);font-weight:300;color:var(--ink);margin-bottom:1rem}
.contact-left p{font-size:.92rem;font-weight:300;color:var(--muted);max-width:360px;line-height:1.75}
.contact-details{margin-top:2.5rem;display:flex;flex-direction:column;gap:1.25rem}
.cd-row{display:flex;flex-direction:column;gap:.2rem}
.cd-label{font-size:.65rem;letter-spacing:.2em;text-transform:uppercase;color:var(--muted)}
.cd-val{font-size:.92rem;color:var(--brown-dark);text-decoration:none;font-weight:400}
.cd-val:hover{color:var(--ink)}
.contact-form{display:flex;flex-direction:column;gap:1.1rem}
.form-row{display:grid;grid-template-columns:1fr 1fr;gap:1rem}
.form-group{display:flex;flex-direction:column;gap:.4rem}
.form-label{font-size:.65rem;letter-spacing:.15em;text-transform:uppercase;color:var(--muted)}
.form-input,.form-textarea{background:var(--beige);border:1px solid var(--beige-dark);color:var(--ink);padding:.8rem 1rem;font-family:'Jost',sans-serif;font-size:.9rem;font-weight:300;outline:none;border-radius:2px;transition:border-color .2s;width:100%}
.form-input:focus,.form-textarea:focus{border-color:var(--brown)}
.form-textarea{resize:vertical;min-height:120px}
.form-input::placeholder,.form-textarea::placeholder{color:var(--beige-deep)}

/* FOOTER */
footer{background:var(--ink);padding:2.5rem 4rem;display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;gap:1rem}
.footer-logo{display:flex;align-items:center;gap:.75rem}
.footer-logo img{height:32px;width:auto;filter:brightness(0) invert(1) opacity(.7)}
.footer-logo-name{font-family:'Cormorant Garamond',serif;font-size:1rem;font-weight:500;color:var(--beige);letter-spacing:.04em}
.footer-copy{font-size:.72rem;color:rgba(245,240,232,0.35);letter-spacing:.05em}

/* MOBILE */
@media(max-width:768px){
  nav{padding:1rem 1.5rem}
  .nav-links{display:none}
  .hero{grid-template-columns:1fr;padding:6rem 1.5rem 3rem}
  .hero-right{display:none}
  .services,.why,footer{padding-left:1.5rem;padding-right:1.5rem}
  .contact{grid-template-columns:1fr;padding:4rem 1.5rem;gap:2.5rem}
  .why-grid{grid-template-columns:1fr;gap:2.5rem}
  .stats-bar{grid-template-columns:1fr}
  .stat{border-right:none;border-bottom:1px solid rgba(255,255,255,0.08)}
  .form-row{grid-template-columns:1fr}
}
</style>
</head>
<body>

<nav>
  <a class="logo" href="#home">
    <img src="data:image/png;base64,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" alt="Sidebar Services Logo">
    <div class="logo-text">
      <span class="logo-name">Sidebar Services</span>
      <span class="logo-tagline">Court Filing &amp; Document Running</span>
    </div>
  </a>
  <ul class="nav-links">
    <li><a href="#services">Services</a></li>
    <li><a href="#why">Why Us</a></li>
    <li><a href="#contact" class="nav-cta">Get in Touch</a></li>
  </ul>
</nav>

<section class="hero" id="home">
  <div class="hero-left">
    <div class="hero-badge">New York Court Filing Specialists</div>
    <h1>Your Filing<br>Deadline is <em>Safe</em><br>With Us.</h1>
    <p class="hero-sub">Sidebar Services handles court filing and document running for law firms and solo attorneys throughout New York — so you can stay focused on your clients.</p>
    <div class="hero-cta">
      <a href="#contact" class="btn-primary">Get in Touch</a>
      <a href="#services" class="btn-outline">Our Services</a>
    </div>
  </div>
  <div class="hero-right">
    <div class="hero-emblem">
      <img src="data:image/png;base64,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" alt="Sidebar Services">
      <div class="emblem-rule"></div>
      <div class="emblem-sub">Est. New York</div>
    </div>
  </div>
</section>

<div class="stats-bar">
  <div class="stat"><div class="stat-num">Same</div><div class="stat-label">Day Filing Available</div></div>
  <div class="stat"><div class="stat-num">All</div><div class="stat-label">NY State &amp; Federal Courts</div></div>
  <div class="stat"><div class="stat-num">Zero</div><div class="stat-label">Missed Deadlines</div></div>
</div>

<section class="services" id="services">
  <p class="section-label">What We Do</p>
  <h2 class="section-title">Our Services</h2>
  <div class="services-grid">
    <div class="service-card">
      <div class="service-num">01</div>
      <div class="service-name">Court Filing</div>
      <p class="service-desc">Same-day filing at all New York state and federal courts. Your deadlines are never in question.</p>
    </div>
    <div class="service-card">
      <div class="service-num">02</div>
      <div class="service-name">Document Running</div>
      <p class="service-desc">Time-sensitive deliveries between courts, firms, and agencies — handled with urgency and precision.</p>
    </div>
    <div class="service-card">
      <div class="service-num">03</div>
      <div class="service-name">Rush &amp; After-Hours</div>
      <p class="service-desc">Deadlines don't keep business hours. Rush and after-hours service available for urgent matters.</p>
    </div>
    <div class="service-card">
      <div class="service-num">04</div>
      <div class="service-name">Docket Retrieval</div>
      <p class="service-desc">Filed copies, docket sheets, case records — retrieved quickly and delivered accurately.</p>
    </div>
  </div>
</section>

<section class="why" id="why">
  <div class="why-grid">
    <div>
      <p class="section-label">Why Sidebar</p>
      <h2 class="section-title">The Professional Standard<br>for Court Running<br>in New York.</h2>
      <ul class="why-points">
        <li><div class="why-check"><svg viewBox="0 0 9 9" fill="none"><path d="M2 4.5 L3.8 6.5 L7 3" stroke="#e0d5c0" stroke-width="1.2" stroke-linecap="round" stroke-linejoin="round"/></svg></div>Deep familiarity with New York state and federal court procedures</li>
        <li><div class="why-check"><svg viewBox="0 0 9 9" fill="none"><path d="M2 4.5 L3.8 6.5 L7 3" stroke="#e0d5c0" stroke-width="1.2" stroke-linecap="round" stroke-linejoin="round"/></svg></div>Trusted by large law firms and solo practitioners alike</li>
        <li><div class="why-check"><svg viewBox="0 0 9 9" fill="none"><path d="M2 4.5 L3.8 6.5 L7 3" stroke="#e0d5c0" stroke-width="1.2" stroke-linecap="round" stroke-linejoin="round"/></svg></div>Real-time status updates so you're never left waiting</li>
        <li><div class="why-check"><svg viewBox="0 0 9 9" fill="none"><path d="M2 4.5 L3.8 6.5 L7 3" stroke="#e0d5c0" stroke-width="1.2" stroke-linecap="round" stroke-linejoin="round"/></svg></div>Transparent, flat-rate pricing — no surprise fees</li>
        <li><div class="why-check"><svg viewBox="0 0 9 9" fill="none"><path d="M2 4.5 L3.8 6.5 L7 3" stroke="#e0d5c0" stroke-width="1.2" stroke-linecap="round" stroke-linejoin="round"/></svg></div>Founded by legal professionals who understand the stakes</li>
      </ul>
    </div>
    <div class="why-right-card">
      <blockquote>"When a filing deadline is on the line, you need someone who knows the courts as well as you know the law."</blockquote>
      <p class="quote-attr">— The Sidebar Services Standard</p>
      <div class="clients">
        <p class="clients-label">We Serve</p>
        <div class="client-pills">
          <span class="pill">Large Law Firms</span>
          <span class="pill">Solo Attorneys</span>
          <span class="pill">Boutique Practices</span>
          <span class="pill">In-House Counsel</span>
          <span class="pill">Legal Departments</span>
        </div>
      </div>
    </div>
  </div>
</section>

<section class="contact" id="contact">
  <div class="contact-left">
    <p class="section-label">Get in Touch</p>
    <h2>Ready to Get<br>Started?</h2>
    <p>Reach out and we'll respond promptly to discuss your needs and how we can help.</p>
    <div class="contact-details">
      <div class="cd-row">
        <span class="cd-label">Phone</span>
        <a href="tel:+19295297760" class="cd-val">+1 (929) 529-7760</a>
      </div>
      <div class="cd-row">
        <span class="cd-label">Email</span>
        <a href="mailto:info@sidebarservices.com" class="cd-val">info@sidebarservices.com</a>
      </div>
      <div class="cd-row">
        <span class="cd-label">Service Area</span>
        <span class="cd-val">New York City &amp; Surrounding Courts</span>
      </div>
    </div>
  </div>
  <div class="contact-form">
    <div class="form-row">
      <div class="form-group">
        <label class="form-label">First Name</label>
        <input class="form-input" type="text" placeholder="Jane">
      </div>
      <div class="form-group">
        <label class="form-label">Last Name</label>
        <input class="form-input" type="text" placeholder="Smith">
      </div>
    </div>
    <div class="form-group">
      <label class="form-label">Firm / Organization</label>
      <input class="form-input" type="text" placeholder="Smith &amp; Associates LLP">
    </div>
    <div class="form-group">
      <label class="form-label">Email</label>
      <input class="form-input" type="email" placeholder="jane@yourfirm.com">
    </div>
    <div class="form-group">
      <label class="form-label">How Can We Help?</label>
      <textarea class="form-textarea" placeholder="Tell us about your filing needs..."></textarea>
    </div>
    <button class="btn-primary">Send Message</button>
  </div>
</section>

<footer>
  <div class="footer-logo">
    <img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAARgAAABQCAYAAADC8mo5AAAACXBIWXMAAC4jAAAuIwF4pT92AAAiDElEQVR4nO2de3xcV3Xvf2vtc0aSLduxQyxLdmLq2pKjQCAI0pDX2JbsGEIL5d5xaIH0E7ixSUjLLaW0FNKRgPQBtxcKSUoCLQEKvfWUeyEkRMQvjQPcQBEkQEQky87LlvyInYcf0szZe63+cc7Ier9sOQ7s7+czH9kze++zzz7nrL32Xo9DAAhTQ6dY3uPxeDwej+f0Qhe8+sr5kyrIRlUq6ekFx44in7cz3TGPx/PyJ4gK5bsnV1SVOKLze8xbnwEeAjIGyLmZ7Z7H43k5ExDTpDQYACBmiGg4kx3yeDy/PgRQHbZpqwIlBZQAGvSbxt8Ry5ntosfjebnCiK1IAx8iY8iYgEyQ/B34hGRMoIJAFZROHyRVkOqUrVAej+c3hODkP1WJDKm4PyPSn6mQIdYheyzKQFi0PyOCAnlLXrR4PJ5xGCRgoCAiUveDfV1tPxqv0pa7muYFqYgA4Hifo9kHzNHVLd6y5PF4hhIM/0IpqIwtRDAABjSYdPog5fML9et/2zvXWftTFT7HidrK8jLTVxW9FcBDmzdnzIYN3rLk8XhiRggYIpHY/JzBYDN0WxuICDpv3pWA4twgoDliFcYQGN6y5PF4RsLTqaRAZK2qSvJXyYcPeDyeEUxLwBCBiEAo/fV4PJ5RmJaA8Xg8nsngBYzH45kxRmzynkFGW1r5vRyP59eIMy1gGOk0I79KgJbRQg4YmQzh4EFCfqECOcFoQiednny/83kBIFOuN6SNhQrkdKCdiZjucUZj4UJFbsCaR0inzam1Va9jjP1UiK9jibGv58R1p8Lp67/nDHEGBUwSfZ3PC5AH0ungvEMoFxdRxfHFdu/e+gLQIsjlJm5quukiTkeaiXQ6QD7vMJ62NXPpLPS0tZ3JmEGCa6pIIrgT8qdQd1oQkGEfzX/2c6YEDAE5V13fdAE5ug7QNPbjQgCLoGFKZh0p1NT+4DCo8RlV6iTCr0jpp076frG/+/uHhjdWvbJxIyGoglqFklFSIiKFAEpKpKQgWCbDVt0D+zu3/gQAVa9svHHCelABACEog/oAfU6J94oWuw505p88+YCPna5iEv0TECZ8OIhNCHX79j2+9YsAcMEFV86PKlI3kZIBGEpiiEhV4/ZVk7YxKICVoAQSAY6D+Sk4PN7b9eDjiXAhTGlZmmWgRWvqVteyKXuHdZELTGgkct/u2bXlUWSzhJYxtQsGIFUr177KgH8/GRtWUiYlBQNJ/weuQan/ACmpngDTU6rmsZ7O73XGY59lr82c3cy0gBmYaWrqmj5Ewh8jY+YRMaztLwDUSYQXFZSC6hLm8ApjwitUIqgIjKk8Ul275sO9Xdv/OdEcLACQ0ieCsoqFpXIDlBTvxIbOJgXX/0IBwE+ADJM+N3E9iv9jABAIqgpxRQBhX03d2l8A+A8X4SsH9uQOjnWDT9Q/Igbx+CsdTZ4xV7S7AHwRAGxFuNAE5bcRMaA6UGbIsYmBgSCx2I9ARQCJ5aKSszUr1/5UBJ/f37XlX3FyL2xiQZPpIOQgAH+UTerdRhXMKTg6fimAa9HSMfbSJ51m5PPC0MuC1KyPqxRjMTjqOZiBXhExVAQiNpaGaqOalet+pM7+795dLf8PieCasO+el4QZFjBZAlpcTV3j3xuT+rCTCOpsvyqyYvmeA3u2HBwo2rAxXHJsz0qncgtBN4pqf2CCBXB45fBWldybo6hvFlx0LoG/ClAFoApSIQ6N2OK9AH2GYYOQw864Vk6UVk9cT/WzwmRItYLAdSC6lomamKgCRJcSmUsB+8Hq2qZbe7tavlSa1THoAR2zf1AlNuyk+BMiug+qDKKhD0fyHQE14GAjgMPJLxT2y1OFWVGarFOQeSMx3QZ1DkoGpA4UGCD6pDrZzoxAYSpVtZ4Iv0/Ev6PxUxoQmUuDgL9WU9f4Oz2d2/540DmMByOXc+fVpxfB4a22eCKCqlrnCESNS3573fK9u3PdY2oV8bISaoNvF8yJbo6cJeB9ZILrVCIHJUasqkSkuEFVewhUpoZWktL1RPQGEYlACInoSg5TV1bXNn26t2vrh70mc/YycwImkzHItbiqusZVxOGHrSsUDIcpEfvF3q6tn0pKUSKEgPa7o73ALwBsqqlt6mHmZhUnStw/vOnex3e0A8Dy5evnnmBLIAQAFEqOiAKF7t3fte37w6rppOrt2v7QoDoPAPhsTW3jdSD+ElTLVYtKzIvYhF+srmuq7+1s+eDw5dK4x2ETqLqHezm33jbe8FXXrltpCJtAJ72kn3oq3w9gJwDUXNiUInCgCgLFChcRGQE/2rtr6+Bz+A6Q/XTNyh/8ExuzUZx1KhaqJBykbllc19i2r7PlmxPuySQaSCipP2QTzBUbWRCFUFhjwjJRewOAjyLdxsiPqlEoAOzvbj0EoA0AFtU2vikgClQJpXOAQsoibXvyie0Hknpb6+szdz/vnt9MJniruqjUfzVB6s+X1DU+urez5eunuKfkmSFmfA/GKN1Cyc2lsc6+Bel0gGPHCO3t0aCZM1lOAT1duZbquqa3B0HFxXAnRlG7MwYATugL85LEWEN+JVAZkDFYfjRAd2sRA9rFFOpdMsfi4EECgJ78tn+vqm3SwJh/V1FRVVEbOROk/rS6tulgb1fu74YKmQmOozorsTQFAAY2besPLeTDh58Plyw5Ujz4Ip0HDo04O3dI5fpMCh1w6l6spNFWWYLZJ899jkX9YwYdLcXyYtOH+wKXIeb5SZIxVVUR0A0AvomJ9tbzedfQ0BD2HtP3qjgBJedFYBUHJbm+6uK1f3Mgv+UExt/bISxfn0L3HEs4UjZagQJoHpB5FtjDqF9GHR254uLl628BbBOIZiWDKKpOVOmDAL6BXM5rMGchM+VoR8jl3PLly8sAbVAVghITEQA5D/m8RWWliVXbwXsAOYd0/FCT0leI6DkBjo1sPidAzplAxpqx4rYW9w2z9kyhXi7nkM9b5PMODQ3hga6tm0XsduKAoaogBOKKjog/UbVy7avitjNmcschSfaTbHIMi3zednTkigcObDne3t4eRXDPqou203ATzUVwQM7FQamjNi0nzz3n0NFRBEB79mx9AaRd8R6TCkgZKkyqr0SyCY+xXmGTyRgA2nN8wWpiU69QBgbEG6s4ZzhcwkX9PQA6gSldB/o2hhAyRpLf2x06ckUAvK+7da9Cf0lsKN64IVYRBrCiatna85K2vOPoWcaMajAngqWVUJqvUBCUVUQVfEvNysZv9+S3HR54djIZE/u+rBLkWxwA6qkufu6CI6kvlxVsH4CZNP1OhKKyUgEQK91DwJrkqSAolAMTqIv+HMAfxQHo0zoGAdCqC6+5KGCz0BXkl/t3tf4KQOOQfpwipBj+4A/ZOxqT+noFABLZREEIEXcnAe8EaF6pukIB0U0A/i32i5mS6XoCMgTkCKDnhstAJYQIMPs0HsxzGplRiR+E5aJIsuIRsaoDE10CpfbFdU1/Fc/8WR7QFuKNungGzOfd07+4/7lk3+GlJfbbUBg8LGJtbOaAgsAiFlBcu3Rp+pxBpt8JUB5YIqXTAZavTyGdDtjZvzUcbodxqwAQ6jOpRMubPMoMZAz2VRggY1BfnwKgVcvWLgSoTkUUIAYQEQekwH8C0JKWMrLBLKOlRarq0q8E87XOFY6gsvzPofows1GoOhAZFafEfFXNirWvja9jZnwz2ZTIJYJQFwzpIkEIOGrp+LOlsz99x/ScDmZUwDz9i2NHCThIIE18M0jVCREvJRPeZlQfran7waM1dWvvXnxh07tr6q6pA0CJtqLJQ3g2RGvHM/jRY3tVdX/JlA2AoaLMfK4Lw9fEX2UmHFMlOpEsi/qRz1t0txaQz1sQPafihJQiABovh6ZoHWEcB3IO3a2F0hJpyZLLKoIQt5MxcwARAMQmVSbOHgwkvA0AxR6yo5BuYwAwGrw7CCrKSPGN3vb7Tijhaxh8bRSOOWBlvTEehin1egjOcSwc0WBiIQuprm+6AOBXqziN7fBaZA5ZFA8e7vzh0bEFpOelZKaWSFryWyFtbCNjVqp1EQgpgFhVRK1IbDLlVxGbV0H1RoW1NXVNHUT0Hbb2y8/kd+xGLATPihtn796H+6prmw6BaEm8UUoUW4Y4cCS1APJIH6SxVwfKqgICXV5T1/TRATN18leB16oKq7jpzP7xXrroJdUr1hxmRiCKeQR+jZBeR8wXJg+nAeiYiNvpbPThnt07dicb0aMJMkI+75YsuaxCgPc61y8E/SIAmovZ974ox/cymyXxXjFMos1dt6R+3a17c7kjmLIjX0wZ9IVkj8ahox3Ll68vO+7sHcRcoc5GIArZpMpEik+y449gPAHpeUmZuT2YeB1OLPK/nLXvJBPMUecikBqAGBQLDlWnakXiV6JQQMwXE5mLxdAHqmvXfqK3a8unRvM1OcOUNhCFSE8M+i6GCMw4b8JWiFjFwnB4KQepS4f/7Gw/VB2YR7UPTdQ4qzgYE/41hWV/DZTUU4K4IuKxRwTgQQD/0vP4g9+J62UMQKNvRsdLVesq56wPTGqptf3beru2/7yhoSFsb7/3aE1d078Sm78sTRYQcSZInSsu2gDgC6X6Uz2RQoDV1SvW7IPRCha+6ATZP2I2r1FxIBOEKq4oYnOICh/p2f3QMwDI+8GcnczgJm+LAOBnunfsXrR81e8aTn2Zg/C3VFzsgaqwiVBJ/EQIAFTFJdZTVAZh6u+ra5vm9Ha13PrSv0kyC6AFYz2MSpg4baiqkAnYif2xFO29o2gwG4xJXezETuM8VYgMO2dzZIu/ABNDdRaAFQBdxSZ4hUjEAL0F0FWLV657TFTu7O3MfQNjefMmm7Uk8j4YgoK/AAB9fcsIaAdg7hFn/yzx84l1KBUosBHI3p1s2E+W2HpIFJqw/N+QeCArCUgFKs4BtE9FbrdF+erBk34y3pP3LGam/WAEyPL+7pb8kiWXvV5nV75PgT8A0avYBEHJ3X1A4JDyIO1GnI2EmT9Ws2LtN3t25R55aT02Y38dVQSj5pkQ6Zu4DRIiZoX9YW/nthGOdtV1TbXJknE6glTjoZOv9nRuu2/wD0vr04siQTNxsEnFKYjOAdEVhsMrquuaruldFL03iYiO2wFQGuuqC1dfRGqabNTX44IFrUDGdHTAoaEh7Gn/XldNbeMONuE6cVFps1eY+JJFK3545f5d2DmFiUEBEFSds4XPQalPSRs59kCOYiGm1SC+MQjoIICvDA4f8ZydnIFgxxZFJmOSNfnfAPi7mvq1F4vYK1RxFUHfAKJlbIIg1m6cJFYOTmZ8iEbXA3hkHC/Rmaa0l0AEnTvoO4CUEG/H7Jt0Y8Md7fZVGCzuc+jV+cSGlaafRF1EzxnSdn6hPtWR2w/gfdW1TYuNMW8R56ySJVVIEJZfX92jT/SipXmIMIjjjsAuuMGkylijvs8c6sid9ElqLwVr0qdUtWlgPBRChpnFbgKwc6qmewUckd7W07n1MICP1dQ13UMmuF4lEoBCAlZQmLqnZsWaQk9++/956TVbz3icCcckHTDfxje+9HRseaTn8S139HZueccsF9Qr6PXiireqyuPEwclNXVKKtRt9HQCchjD/U2LZsqa5UCyKA/RKEYXEok7JoQNAsqyYiGGOdt2tReTzVkzwESfRGjjTBgDJxuWUrGjE6oa0jZxDw8YQAJHqP8bmsMRRjsg4VxQQ3bJg+fq5g5ztCLmcW7o0fQ5B3u1cEQq8q6auaWdNXdNDyd+dNXVNOxX6SVXHA1GiBBOvZvDWxcvTS5JrP0VTu7yilFOngFm3iNi9RIYAiKpzKk7A/Nl5r0mfA0x9jDxnjhkXMFUXr519wauvnY+T5mcCsokfSMZ0d7cWeh9/sL2nc9snw/7oEjj5ArGhJFQ40RJoftLcye/OKFkCQP2sy2D4XI1d7QmAEDFU9YlZCDvi7yYMGhwNBYADv/reY/se++6OJF4HA35Bp0r73Q6ARil5QpwrAlwS4gxVIqZzy1SXx4UzXPLEjcqDt3OQWihi+6F6IaBXAPpGQC9PPlcQ6PUK9A26LARVyyacLRy+CwCmmmDKuFg41tfXh4c77z3KoE8m94QCZFRE2IRVs/vMnwAtgszErgGel4YZvDCxoxX36+3iaHdV3Zo0AIpvhhYZmF1LAqehIXzqqXx/hZj/qc7tBzNDS6bTITH9Z96SFPuCKAytYQ4ImiwPFBK7ruPr3d2theTBPIX+ZTnx5yAANH9Z07ylr0mfM2VnuzHgKBCQjuyfAmrsSctVHPlMqnoj4vcEv6sg4XnH++25BcyeX/r0RbSgX4JzWfiNCvQPtEZgVQdA31Nfn0mVIqmnSkfHRQ7IcoUz9zgbdcXarToQjIpVJf5A1cVrFyZxSF7InIWciYsyhw3PN0pvB6DYs2f4MeMUiO3tEQDu7m4tKPAEEUPjmBMF0BMXPZ3eoZMly3HKzIwB6L0qgngTWh0xB+KiA9Doc4g1tFNcwrVI8rDo0qXpsooQPyj2hXsWv7qtJikwveuVTjOQZTI4nzkoKznbIYk/hcoJy8HeuOxBAqBLVqx7gzGpy1xU6NzfueBbR7pbX3zhqfzzhzvvPVr6PLdn6wtHultf3LfrwUcJ2socaCJ8WcUJm3DF83JkHYBSPNMUySnQQd3drQUIWohjaQeAVESMCRdwv34Isd+VFzBnITN+UQhQcUUF8buqatf+Ftrbo9g78+RMHX/SQRxzkmWCVpeSslEcIdkKoHTzAw0NAdLpwJqxNqkHueIPPsep1EuWcPEyJedq6p77BLO5UMU6KITABiCIyg29XflnEw9emdxxEq3t0EKOtZPBnwwDWS4W57AC5xLTfGcHslMRjh4NkE4HqqP7yqiQGXEOSRgGid6cvMYqCSBSy2wIRDufffx7vUDG4Mm4z8LuRg5SANFXkT6YhC0Mvl7Jp6EhjPuj9wCgeH8HcXIKAKq4CYDiZ0eDQcGtcd+URr3/nEl+r68P4sDRLPdeMv/fnbU/IxOYWIshFhcJEd1Uc9G68wEg6aMXNGcRM29FYoWKOhDmMfDNqrr02w905J4cWTA2N9bUrr2ZTPBKEdfPJigXGz2dKtjYLb2kasfaDsySyw7JrMoRKv+AK/6gVAjTrXdefXpRaMOPEPGfiIuKIATMgVGVEyruhv1d2x8YYcmY6DigItAi6EBxrGHr7cWJmrlNRagKsSm14dDa6gCA6xqfH+3yMdPzw8+hZmXjuQr+CIOuE2dt7GkPSyYMVdwxUvkLlCKqn4JbsHz9XJC7zhb7jpjjxz6D/MNjm4KTc+0Fvl1d1/gIc/BaFRsLALFK4KaquvQrD3S2PlmaJ5BP4svqmo6PaI+gfDw8hPyDJ4+Z6WDkco5XNN0K4L6TJeE4CCpdVPwr5PM3jdlHz0vGGTBTU6UJUoGN+sBsLiFJPVyzsumfyOJ7xVT0pCtWnAjKixWBpWUQvg6EmxF7pJaruIPO2A09T+WfH/wQL6pbs4kpXChqKxUICJrkoSWoOCHg8pq6po+yCQLr7P2lnLyL6tZsnLBebeOtiZNaBUAr1eFqDsL5qg4cpFIqDqKuNXL2Lw/t2vHoaGbSsfsHEmeFSN9WXdd0YeKiP8aejTKAVyhQEBcxEAsKUdzEClJQbZwLs5TDljTOjyLX19Q2XjJwDooVULrcsFkkYkHMQcngIyo/B8n7ejq3/xwAV9Vds9QQ3q1qLyIylSJ2t86e9ac1K9cF1rl/Pbhr2x4Mdf8nAFpdu+ZtxoSvErHHY8cmUpAqlISYAiPh7Uvq3/Qj56IfG8u7UcbvFBc5AKtV3OB9NoKCZbZ8rGbl2udU5fnezgV3IpdzyGTMvlzu/praxp1kgqvikAGwuMgRcP3i2sbDxEGhKNG3D3bF5wPvgPeSM4MCJjYfksqnXFQ4AOAKFbeMTVjFHDQLu+ZQCKGJHCJj2ITgwEBcBBF3Qp39tnH21gPdbbsTp6+Bh5jBHw9SFQvVRRAZObkaTl1KxJeyScHZF/qQ5ORlPDdxPTaxC7/GXqniIjgbHSbgSSXsBPAfPZ1bfhjXGN0HY6L+MQXnE/H5E42giABqIVGybDG0MNDUJ4jjnLwiNtkPSg4LgE2YIeKToYZJOZFIoHRCSfaq6k9BdG+P3fMtdHcX0LAxRPvdEZOuCFKzPq6uAHEOxoTLyZjbiEOgcOwRAHuGZPPPZOJIeNB7TGrW76LYB4WCjBnep2tNWHGtiwr/ooz7g7CymbgQe+qqDC4PApg5+FNig6h4om/58qN3d3fDlZJ/iZFbDShPJhjsKzSLTfBR5hS4cPQQgJ+XMvBNNMaemWWmQwWwr3P7DgA76uszqRfs0ZVOooucK9ZBsZSIqqCYpVARWzzsgCeI6TEr8lAyW2I0710leVMU9c2GjcA8/BwCRCgqK9lALIUcdsff50RpzcT1olJ6CVZmWMfuKDs50NOVf3ZQ4VKqzzHCBsbrH6AgtcwT3vxGyAiplBUK+wAgeOHYk25W5VVQIQ0MmRFBkQGsFoXc0GRUZMiS6nHDwaGnq/oPDfV+zTLaWywA9Bflx6C+qxVFMhoa1UidsxbGUpgq+2VpHAeqJlnkiPEhKZ74tFXHRpmHrkwDWOl3BFEH2heWlz0nxeNXW+dUGWZkecDayCIIoar93XFGwoF8QPt/tWNnzcrGy0m4AuQGtD/rXBQYSxpRZ1LeO9+dBVBNXVNykVSIA4ZEa2KhMHR2Vo0T1N9355XzAwS7DdN8K2orykzQ3x+tWf/+nTs2b86YDRuGz+hZjr1Cp+ptmeXEdf3smYXS6SB5CdvL/ObNmNjDdowX253dTCtC2/PScCZCBSRxFY9n/SS/SPyWPiBeSnXE1qGSlSifn+BNgVkeqDMhgx+iqdQrUa8DkdyTjnuZznHGY7BAm66pfuA84vZGd98fyIs8Sh/GEUalSWScw8cCLR7HTIYnHz4wQpjr+GPwshSav7acyVfHxjf4eLFEk86yON2AxzMVKDmTx5lR7Wma2tnAJDI2g38/5ez/L3cN8jcH7zPg8XhmDC9gPB7PjOEFjMfjmTHOyB6Mailb2eQ330p1Sky27uB6U6kzvOxo341aN8lAPZnjjHPspKnJlR/8/+mM6VTqeDynwoxqMApQNgsmgk71pi7VmWrdwXU2b56cxWWEcMHkhAsATFe4lPqWHGdKfZ3quJzKdfB4ToVpaTAKFQUEUFGoGB7d3Z0ARQv0gbuuqgaA8h4+tLplYlNvNgtuqEkvqEA4CwCcLeiL5y3qGeljM7Lela9onI8UzXbHjh1bvyF3ZOJzAW29q2nu2k1bXxjc7+9/6fI50TNh33j93bw5Y847eLBi9S35Ud4+Oc4xFUQUn0vrHVedTyfKj1yzITcyLmcY0x2X6V4Hj+dUmbIGE/RZIqU5FWUBp0KTmlUWsNWhgkrjSBTaclfTvAfuSH89RcE/hwj+qW8h/Y2ejMQdQTYb5z15wzlX14UOP3Iu+pyq+xxgPhXuOzin1PZY9d5Yk651xv5IxH6mbO6s/9t6R/q2+PfRz1OzYCjgXPSVB+9YlS71677bVy89Vgi/dbRmTimCeNTjzTmw/zX9TN8Yq1+jn2OsSdx/59Vv2nLX6q3MwWd4ns213n71nyHRNE7XuEz3Ong8p4tJazAl1brsdWUv9v9KmgpFCSJx2tcPcnCPAEAmE7uOtzWnzeqWvG290/4PAmY3btzxZgD47j+un1tK7TzescKQ5yqwZ/3NbW8bqx+jYSM3L6DgmWtubvtvO76cLtcIna13pb+2flP+8WwW3NIy1AenDWleTXnbeifaBHoDEk+cwOi7VKjz9zbdd2JHNh2MNdtTgEAV88Y7l8Fks1luaWmR1s+lVyroDnXyh+tuzj+85fON5yrJurs2NgSbWuLo5NMxLqd6HTyeU2XKS6TVq/MWwEOj/Va6yVcheTexyk+J+Ybtd635hLL+/8YbW7+LD0xmY1QLAFU9cPvqDWWBUr+loz86tKN1uIAYTsihVdWybbevXuosVRHkgPTrMQBoboa2tAwtv6o579ACGBd8zbF99313Xjn/LTd//zlVfXNAesuQcxkFEVJiTHqpsQpt3AKIGrwDitZ1788//JO7GsLXb9p2GMC/TdzC1Mbl1K+Dx3NqjFw6qCaq88GRyYUSlXrz5owZ/NFhqja1tIgqaP37d+5wIjcQKTH4Qw/cuep79971llnQUiq10XHkRFXngfUyJbqMWF970UWZUqakcdR6KSj0t62Rf4DifgDffPMH8ns3b86Y0Wb40kbw2j/edphAjwccrHvwi1dfCIVde/POn2k2y9QygVfuJJdGg2HQPAWe3bEjHcztP4937EhPStBPdVxO9Tp4PKfKiBubDOL3QmPsTcCJNhWBk9rMm9+/8z8Rv2AdrXemfxm6o5cTYevmzRmDMdphpnIIPbL+5rYPjmh3nBmXGOUQevSam9r++/2fb6xlxte3fKXxS2s35I5MZHZW1a+pw7vU8WVQ+SYAtKFt3JwiKqRsMGm39UMXLYzfrUTyn6R80+rV+b9GEkq8+R8uq8DD5xc3jONGP51xOZXr4PGcKiMEjAjNu+DVV863URkHYWHg4SI2qlJJTy84dnSioL/NmYzZkMu5B+5cdU1ZyI3ForSnUry8UHQWgTymACGTG/PBZWJxhEseuD39B8RKUHb9x4rffdtf/PAoxommdZGGMLwgFibbulrvWLXDHnefBvCeXG703C0bNuRcNgt+ceHCLXOePfS3AiwLgtQFAKi0hBqzn9BQwfPHLjH6scoO0Ob+KmS2fGHVN6zSt0KmFdbJkhczuEU3jy0Ipzoup3odPJ5TZdASKX63MZS/ERXKd6tQd1Qo3136FPuC3TaKdp/fY94Ylx/bb+Ox+pwCgIPdBeBZJb0EAFJl/NY3bXqoFxh9U7K5uVkBgKLgCUC/DKbXEfgSkL4uVc7lAEqpeketZ2CfYujniaDZLBip/r8D0D56GolB9ZHFhg05Z4g+CtIPrN209YXSq+1HLZ8czwbB0wz9/Fjtjlq3Bbq6JW/fdHPb7xP0u4bQoCp9AfEnx+rjdMdlutfB4zldDMoHM/DVGKtyBXEA2ELjvq4d26f7Rr2Xw8biy6GPp8pvwjl6XnqCYe8cQpxjcTTHOVVACTRxJraBGtkst9fcN6Dp7Jm/TJDJyUQbi83NoN+taRiiIX2np901N4//QDQ3Z2nVqjZetSrJZtacpbtr7jMbN7ZPytLT1pw2XTXHCBvb7WQ2P0ccbwo0N4NWrUrznK5jBAANPW9xaB7/pW3THRc0Z2k618HjGYtJe7ovvvCaSc5isQYjxcLanl3btvp3Ans8nokIINGayRZWBoLywiPx/8bfHFQFbb27aW6Qivws6fH8uvEkjk0m3CRIknJPh1E1n5I5+FufTc+rKLM/0SKd4ywUpF7QeDwvcwiQ8pTh6Dz3NgDfn8iAEkw9x+vkcp5WVBYYUflvzakIObIK8uLF43nZI6qYXRHg2T5bMZnyweneRxmIWVpe9mLfY5o+VigG1sftejy/NggBZZX0CHAy/tDj8XjOODO6cJlsEiWPx/PyIrMhJ96PyuPxeDwej8fj8Xg8Ho/H4/F4PB6Px+PxeDwej8fj8Xg8Ho/H4/F4PB6Px+PxeDwej8fj8fzm8l9Yc3tYpxwMJQAAAABJRU5ErkJggg==" alt="Sidebar Services">
    <span class="footer-logo-name">Sidebar Services</span>
  </div>
  <p class="footer-copy">&copy; 2026 Sidebar Services. New York, NY. All rights reserved.</p>
</footer>

</body>
</html>
