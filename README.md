<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Wyoming Premier Rental LLC — Natrona County Equipment Rental</title>
<meta name="description" content="Professional equipment rental serving Casper, Evansville, Mills, and Bar Nunn. Skid steer attachments, pressure washers, and more. Wyoming owned and operated.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Barlow:wght@300;400;500;600&family=Barlow+Condensed:wght@400;600;700&display=swap" rel="stylesheet">
<style>
:root {
  --gold: #C9A84C;
  --gold-dark: #9A7B2E;
  --dark: #111111;
  --dark2: #1C1C1C;
  --dark3: #242424;
  --mid: #333333;
  --light: #F5F0E8;
  --lighter: #FAF7F2;
  --text: #E8E0D0;
  --text-muted: #8A8070;
  --border: rgba(201,168,76,0.2);
}

* { box-sizing: border-box; margin: 0; padding: 0; }

html { scroll-behavior: smooth; }

body {
  font-family: 'Barlow', sans-serif;
  background: var(--dark);
  color: var(--text);
  overflow-x: hidden;
}

/* TOPBAR */
.topbar {
  background: #0A0A0A;
  padding: 8px 40px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  border-bottom: 1px solid rgba(201,168,76,0.15);
}
.topbar-left { font-size: 12px; color: var(--text-muted); letter-spacing: 2px; text-transform: uppercase; }
.topbar-right { display: flex; gap: 24px; }
.topbar-right a { font-size: 12px; color: var(--gold); text-decoration: none; letter-spacing: 1px; }
.topbar-right a:hover { color: #fff; }

/* NAV */
nav {
  background: var(--dark);
  padding: 0 40px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  border-bottom: 1px solid var(--border);
  position: sticky;
  top: 0;
  z-index: 100;
}
.nav-logo {
  display: flex;
  align-items: center;
  gap: 14px;
  padding: 16px 0;
  text-decoration: none;
}
.nav-logo-mark {
  width: 42px;
  height: 42px;
  background: var(--gold);
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: 'Bebas Neue', sans-serif;
  font-size: 18px;
  color: var(--dark);
  letter-spacing: 1px;
  clip-path: polygon(10% 0%, 90% 0%, 100% 10%, 100% 90%, 90% 100%, 10% 100%, 0% 90%, 0% 10%);
}
.nav-logo-text { display: flex; flex-direction: column; }
.nav-logo-name {
  font-family: 'Bebas Neue', sans-serif;
  font-size: 22px;
  color: #fff;
  letter-spacing: 3px;
  line-height: 1;
}
.nav-logo-name span { color: var(--gold); }
.nav-logo-sub { font-size: 10px; color: var(--text-muted); letter-spacing: 3px; text-transform: uppercase; margin-top: 2px; }
.nav-links { display: flex; gap: 0; }
.nav-link {
  font-family: 'Barlow Condensed', sans-serif;
  font-size: 13px;
  font-weight: 600;
  letter-spacing: 2px;
  text-transform: uppercase;
  color: var(--text-muted);
  text-decoration: none;
  padding: 20px 18px;
  border-bottom: 2px solid transparent;
  transition: color 0.2s, border-color 0.2s;
}
.nav-link:hover { color: #fff; border-bottom-color: var(--gold); }
.nav-cta {
  font-family: 'Barlow Condensed', sans-serif;
  font-size: 13px;
  font-weight: 700;
  letter-spacing: 2px;
  text-transform: uppercase;
  background: var(--gold);
  color: var(--dark);
  padding: 10px 20px;
  text-decoration: none;
  clip-path: polygon(6px 0%, 100% 0%, calc(100% - 6px) 100%, 0% 100%);
  transition: background 0.2s;
}
.nav-cta:hover { background: #E0B95C; }

/* HERO */
.hero {
  min-height: 85vh;
  background: var(--dark);
  display: flex;
  align-items: center;
  position: relative;
  overflow: hidden;
  padding: 80px 40px;
}
.hero-grid-bg {
  position: absolute;
  inset: 0;
  background-image:
    linear-gradient(rgba(201,168,76,0.05) 1px, transparent 1px),
    linear-gradient(90deg, rgba(201,168,76,0.05) 1px, transparent 1px);
  background-size: 60px 60px;
}
.hero-glow {
  position: absolute;
  top: -200px;
  right: -200px;
  width: 700px;
  height: 700px;
  background: radial-gradient(circle, rgba(201,168,76,0.08) 0%, transparent 70%);
  pointer-events: none;
}
.hero-content { position: relative; z-index: 1; max-width: 700px; }
.hero-eyebrow {
  display: inline-flex;
  align-items: center;
  gap: 10px;
  font-family: 'Barlow Condensed', sans-serif;
  font-size: 12px;
  font-weight: 600;
  letter-spacing: 4px;
  text-transform: uppercase;
  color: var(--gold);
  margin-bottom: 20px;
}
.hero-eyebrow::before {
  content: '';
  display: block;
  width: 30px;
  height: 1px;
  background: var(--gold);
}
.hero-title {
  font-family: 'Bebas Neue', sans-serif;
  font-size: clamp(60px, 10vw, 110px);
  line-height: 0.9;
  letter-spacing: 3px;
  color: #fff;
  margin-bottom: 24px;
}
.hero-title span { color: var(--gold); display: block; }
.hero-desc {
  font-size: 17px;
  font-weight: 300;
  color: var(--text-muted);
  line-height: 1.7;
  max-width: 520px;
  margin-bottom: 36px;
}
.hero-desc strong { color: var(--text); font-weight: 500; }
.hero-actions { display: flex; gap: 14px; align-items: center; flex-wrap: wrap; margin-bottom: 48px; }
.btn-primary {
  font-family: 'Barlow Condensed', sans-serif;
  font-size: 14px;
  font-weight: 700;
  letter-spacing: 3px;
  text-transform: uppercase;
  background: var(--gold);
  color: var(--dark);
  padding: 14px 32px;
  text-decoration: none;
  border: none;
  cursor: pointer;
  clip-path: polygon(8px 0%, 100% 0%, calc(100% - 8px) 100%, 0% 100%);
  transition: background 0.2s, transform 0.1s;
  display: inline-block;
}
.btn-primary:hover { background: #E0B95C; transform: translateY(-1px); }
.btn-outline {
  font-family: 'Barlow Condensed', sans-serif;
  font-size: 14px;
  font-weight: 600;
  letter-spacing: 3px;
  text-transform: uppercase;
  background: transparent;
  color: var(--text);
  padding: 13px 32px;
  text-decoration: none;
  border: 1px solid rgba(255,255,255,0.2);
  cursor: pointer;
  transition: border-color 0.2s, color 0.2s;
  display: inline-block;
}
.btn-outline:hover { border-color: var(--gold); color: var(--gold); }
.hero-stats {
  display: flex;
  gap: 40px;
  padding-top: 40px;
  border-top: 1px solid var(--border);
}
.hero-stat-num {
  font-family: 'Bebas Neue', sans-serif;
  font-size: 36px;
  color: var(--gold);
  letter-spacing: 2px;
  line-height: 1;
}
.hero-stat-label { font-size: 11px; color: var(--text-muted); letter-spacing: 2px; text-transform: uppercase; margin-top: 4px; }

/* SECTION STYLES */
.section { padding: 80px 40px; }
.section-dark { background: var(--dark2); }
.section-darker { background: #0D0D0D; }
.section-header { margin-bottom: 48px; }
.section-eyebrow {
  font-family: 'Barlow Condensed', sans-serif;
  font-size: 11px;
  font-weight: 600;
  letter-spacing: 4px;
  text-transform: uppercase;
  color: var(--gold);
  margin-bottom: 10px;
  display: flex;
  align-items: center;
  gap: 10px;
}
.section-eyebrow::before { content: ''; display: block; width: 20px; height: 1px; background: var(--gold); }
.section-title {
  font-family: 'Bebas Neue', sans-serif;
  font-size: clamp(36px, 5vw, 56px);
  letter-spacing: 2px;
  color: #fff;
  line-height: 1;
}
.section-sub { font-size: 15px; color: var(--text-muted); margin-top: 12px; max-width: 560px; line-height: 1.7; font-weight: 300; }

/* EQUIPMENT GRID */
.equip-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(280px, 1fr)); gap: 2px; }
.equip-card {
  background: var(--dark3);
  border: 1px solid var(--border);
  padding: 28px;
  position: relative;
  overflow: hidden;
  transition: border-color 0.3s, background 0.3s;
  cursor: pointer;
}
.equip-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 2px;
  background: var(--gold);
  transform: scaleX(0);
  transition: transform 0.3s;
  transform-origin: left;
}
.equip-card:hover { border-color: rgba(201,168,76,0.5); background: #2A2A2A; }
.equip-card:hover::before { transform: scaleX(1); }
.equip-number {
  font-family: 'Bebas Neue', sans-serif;
  font-size: 48px;
  color: rgba(201,168,76,0.08);
  position: absolute;
  top: 10px;
  right: 16px;
  line-height: 1;
  letter-spacing: 2px;
}
.equip-category {
  font-family: 'Barlow Condensed', sans-serif;
  font-size: 10px;
  font-weight: 600;
  letter-spacing: 3px;
  text-transform: uppercase;
  color: var(--gold);
  margin-bottom: 10px;
}
.equip-name {
  font-family: 'Bebas Neue', sans-serif;
  font-size: 24px;
  letter-spacing: 1px;
  color: #fff;
  margin-bottom: 8px;
  line-height: 1.1;
}
.equip-desc { font-size: 13px; color: var(--text-muted); line-height: 1.6; margin-bottom: 20px; font-weight: 300; }
.equip-footer { display: flex; justify-content: space-between; align-items: flex-end; }
.equip-price { }
.equip-price-num {
  font-family: 'Bebas Neue', sans-serif;
  font-size: 32px;
  color: var(--gold);
  letter-spacing: 1px;
  line-height: 1;
}
.equip-price-label { font-size: 11px; color: var(--text-muted); letter-spacing: 1px; margin-top: 2px; }
.equip-avail {
  font-family: 'Barlow Condensed', sans-serif;
  font-size: 11px;
  font-weight: 600;
  letter-spacing: 2px;
  text-transform: uppercase;
  padding: 4px 10px;
  border: 1px solid;
}
.avail-yes { color: #7EC8A0; border-color: rgba(126,200,160,0.3); background: rgba(126,200,160,0.05); }
.avail-request { color: var(--gold); border-color: rgba(201,168,76,0.3); background: rgba(201,168,76,0.05); }

/* HOW IT WORKS */
.how-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 0; }
.how-step {
  padding: 36px 32px;
  border-right: 1px solid var(--border);
  border-bottom: 1px solid var(--border);
  position: relative;
}
.how-step:last-child { border-right: none; }
.how-step-num {
  font-family: 'Bebas Neue', sans-serif;
  font-size: 72px;
  color: rgba(201,168,76,0.06);
  position: absolute;
  bottom: 10px;
  right: 20px;
  line-height: 1;
  letter-spacing: 3px;
}
.how-icon {
  width: 44px;
  height: 44px;
  border: 1px solid var(--border);
  display: flex;
  align-items: center;
  justify-content: center;
  margin-bottom: 16px;
  clip-path: polygon(6px 0%, 100% 0%, calc(100% - 6px) 100%, 0% 100%);
  background: var(--dark3);
}
.how-icon svg { width: 20px; height: 20px; stroke: var(--gold); fill: none; stroke-width: 1.5; }
.how-title {
  font-family: 'Barlow Condensed', sans-serif;
  font-size: 18px;
  font-weight: 700;
  letter-spacing: 1px;
  text-transform: uppercase;
  color: #fff;
  margin-bottom: 8px;
}
.how-desc { font-size: 13px; color: var(--text-muted); line-height: 1.6; font-weight: 300; }

/* PHOTO REQUIREMENT */
.photo-section {
  background: var(--dark3);
  border: 1px solid var(--border);
  padding: 32px;
  margin-top: 40px;
}
.photo-title {
  font-family: 'Bebas Neue', sans-serif;
  font-size: 24px;
  letter-spacing: 2px;
  color: var(--gold);
  margin-bottom: 16px;
}
.photo-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 10px; }
.photo-item {
  background: var(--dark);
  border: 1px solid var(--border);
  padding: 14px;
  display: flex;
  align-items: center;
  gap: 10px;
  font-size: 13px;
  color: var(--text-muted);
}
.photo-dot { width: 6px; height: 6px; background: var(--gold); flex-shrink: 0; }

/* CONTACT / BOOKING FORM */
.contact-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 48px; }
.contact-info { }
.contact-detail {
  display: flex;
  align-items: flex-start;
  gap: 14px;
  margin-bottom: 24px;
  padding-bottom: 24px;
  border-bottom: 1px solid var(--border);
}
.contact-detail:last-child { border-bottom: none; }
.contact-icon {
  width: 36px;
  height: 36px;
  border: 1px solid var(--border);
  display: flex;
  align-items: center;
  justify-content: center;
  flex-shrink: 0;
  background: var(--dark3);
}
.contact-icon svg { width: 16px; height: 16px; stroke: var(--gold); fill: none; stroke-width: 1.5; }
.contact-label { font-size: 10px; letter-spacing: 3px; text-transform: uppercase; color: var(--text-muted); margin-bottom: 4px; font-family: 'Barlow Condensed', sans-serif; font-weight: 600; }
.contact-value { font-size: 15px; color: #fff; font-weight: 400; }
.contact-value a { color: var(--gold); text-decoration: none; }
.contact-value a:hover { color: #fff; }

/* FORM */
.form { background: var(--dark3); border: 1px solid var(--border); padding: 32px; }
.form-title {
  font-family: 'Bebas Neue', sans-serif;
  font-size: 28px;
  letter-spacing: 2px;
  color: #fff;
  margin-bottom: 4px;
}
.form-sub { font-size: 13px; color: var(--text-muted); margin-bottom: 24px; font-weight: 300; }
.form-row { display: grid; grid-template-columns: 1fr 1fr; gap: 12px; margin-bottom: 12px; }
.form-group { display: flex; flex-direction: column; gap: 6px; margin-bottom: 12px; }
.form-label { font-size: 10px; letter-spacing: 3px; text-transform: uppercase; color: var(--text-muted); font-family: 'Barlow Condensed', sans-serif; font-weight: 600; }
.form-input {
  background: var(--dark);
  border: 1px solid rgba(255,255,255,0.08);
  color: #fff;
  padding: 11px 14px;
  font-family: 'Barlow', sans-serif;
  font-size: 14px;
  outline: none;
  transition: border-color 0.2s;
  width: 100%;
}
.form-input:focus { border-color: var(--gold); }
.form-input option { background: var(--dark2); }
.form-terms {
  display: flex;
  align-items: flex-start;
  gap: 10px;
  font-size: 12px;
  color: var(--text-muted);
  line-height: 1.5;
  margin-bottom: 20px;
}
.form-terms input { margin-top: 2px; accent-color: var(--gold); flex-shrink: 0; }
.form-submit {
  width: 100%;
  font-family: 'Barlow Condensed', sans-serif;
  font-size: 14px;
  font-weight: 700;
  letter-spacing: 3px;
  text-transform: uppercase;
  background: var(--gold);
  color: var(--dark);
  padding: 15px;
  border: none;
  cursor: pointer;
  clip-path: polygon(8px 0%, 100% 0%, calc(100% - 8px) 100%, 0% 100%);
  transition: background 0.2s;
}
.form-submit:hover { background: #E0B95C; }

/* SERVICE AREA BANNER */
.area-banner {
  background: var(--gold);
  padding: 28px 40px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-wrap: wrap;
  gap: 20px;
}
.area-banner-left { }
.area-banner-title {
  font-family: 'Bebas Neue', sans-serif;
  font-size: 28px;
  letter-spacing: 3px;
  color: var(--dark);
}
.area-banner-sub { font-size: 13px; color: rgba(17,17,17,0.6); margin-top: 2px; }
.area-tags { display: flex; gap: 8px; flex-wrap: wrap; }
.area-tag {
  background: rgba(17,17,17,0.15);
  color: var(--dark);
  padding: 6px 16px;
  font-family: 'Barlow Condensed', sans-serif;
  font-size: 13px;
  font-weight: 700;
  letter-spacing: 2px;
  text-transform: uppercase;
}

/* FOOTER */
footer {
  background: #0A0A0A;
  padding: 60px 40px 30px;
  border-top: 1px solid var(--border);
}
.footer-grid { display: grid; grid-template-columns: 2fr 1fr 1fr; gap: 48px; margin-bottom: 48px; }
.footer-brand { }
.footer-logo {
  font-family: 'Bebas Neue', sans-serif;
  font-size: 28px;
  letter-spacing: 3px;
  color: #fff;
  margin-bottom: 4px;
}
.footer-logo span { color: var(--gold); }
.footer-tagline { font-size: 12px; color: var(--text-muted); letter-spacing: 2px; text-transform: uppercase; margin-bottom: 16px; }
.footer-desc { font-size: 13px; color: var(--text-muted); line-height: 1.7; font-weight: 300; max-width: 280px; }
.footer-col-title { font-family: 'Barlow Condensed', sans-serif; font-size: 12px; font-weight: 700; letter-spacing: 3px; text-transform: uppercase; color: var(--gold); margin-bottom: 16px; }
.footer-item { font-size: 13px; color: var(--text-muted); margin-bottom: 8px; line-height: 1.5; }
.footer-item a { color: var(--text-muted); text-decoration: none; transition: color 0.2s; }
.footer-item a:hover { color: var(--gold); }
.footer-bottom {
  border-top: 1px solid var(--border);
  padding-top: 24px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  gap: 12px;
}
.footer-copy { font-size: 12px; color: var(--text-muted); letter-spacing: 1px; }
.footer-badge {
  font-family: 'Barlow Condensed', sans-serif;
  font-size: 11px;
  font-weight: 600;
  letter-spacing: 2px;
  text-transform: uppercase;
  color: var(--gold);
  border: 1px solid var(--border);
  padding: 4px 12px;
}

/* SUCCESS MESSAGE */
.success-msg {
  display: none;
  background: rgba(126,200,160,0.1);
  border: 1px solid rgba(126,200,160,0.3);
  padding: 16px 20px;
  margin-bottom: 20px;
  font-size: 14px;
  color: #7EC8A0;
}

/* RESPONSIVE */
@media (max-width: 768px) {
  .topbar { padding: 8px 20px; }
  nav { padding: 0 20px; }
  .nav-links { display: none; }
  .hero { padding: 60px 20px; min-height: auto; }
  .hero-stats { gap: 24px; flex-wrap: wrap; }
  .section { padding: 60px 20px; }
  .contact-grid { grid-template-columns: 1fr; }
  .footer-grid { grid-template-columns: 1fr; gap: 32px; }
  .area-banner { padding: 24px 20px; }
  .form-row { grid-template-columns: 1fr; }
  .photo-grid { grid-template-columns: 1fr 1fr; }
  footer { padding: 48px 20px 24px; }
  .how-step { border-right: none; }
}
</style>
</head>
<body>

<!-- TOPBAR -->
<div class="topbar">
  <div class="topbar-left">Natrona County, Wyoming</div>
  <div class="topbar-right">
    <a href="tel:3079005333">(307) 900-5333</a>
    <a href="mailto:wyomingpremierrental@gmail.com">wyomingpremierrental@gmail.com</a>
  </div>
</div>

<!-- NAV -->
<nav>
  <a href="#" class="nav-logo">
    <div class="nav-logo-mark">WPR</div>
    <div class="nav-logo-text">
      <div class="nav-logo-name">Wyoming <span>Premier</span> Rental</div>
      <div class="nav-logo-sub">Natrona County · Est. 2026</div>
    </div>
  </a>
  <div class="nav-links">
    <a href="#equipment" class="nav-link">Equipment</a>
    <a href="#how-it-works" class="nav-link">How It Works</a>
    <a href="#contact" class="nav-link">Contact</a>
  </div>
  <a href="#contact" class="nav-cta">Book Now</a>
</nav>

<!-- HERO -->
<section class="hero">
  <div class="hero-grid-bg"></div>
  <div class="hero-glow"></div>
  <div class="hero-content">
    <div class="hero-eyebrow">Natrona County Equipment Rental</div>
    <h1 class="hero-title">
      Built For
      <span>Wyoming</span>
      Work
    </h1>
    <p class="hero-desc">
      Professional grade skid steer attachments and equipment rental serving <strong>Casper, Evansville, Mills, and Bar Nunn.</strong> Wyoming owned and operated. Honest prices. No hassle booking.
    </p>
    <div class="hero-actions">
      <a href="#equipment" class="btn-primary">Browse Equipment</a>
      <a href="#contact" class="btn-outline">Book a Rental</a>
    </div>
    <div class="hero-stats">
      <div>
        <div class="hero-stat-num">10+</div>
        <div class="hero-stat-label">Items Available</div>
      </div>
      <div>
        <div class="hero-stat-num">100%</div>
        <div class="hero-stat-label">Wyoming Owned</div>
      </div>
      <div>
        <div class="hero-stat-num">24hr</div>
        <div class="hero-stat-label">Response Time</div>
      </div>
    </div>
  </div>
</section>

<!-- EQUIPMENT -->
<section class="section section-dark" id="equipment">
  <div class="section-header">
    <div class="section-eyebrow">Our Fleet</div>
    <h2 class="section-title">Equipment For Rent</h2>
    <p class="section-sub">All attachments fit standard skid steer loaders with auxiliary hydraulics. Inspect and document condition at every pickup and return.</p>
  </div>
  <div class="equip-grid">

    <div class="equip-card">
      <div class="equip-number">01</div>
      <div class="equip-category">Skid Steer Attachment</div>
      <div class="equip-name">Hydraulic Rock Rake</div>
      <p class="equip-desc">78" hydraulic rock rake. Ideal for clearing land, removing rocks and debris, grading and leveling soil.</p>
      <div class="equip-footer">
        <div class="equip-price">
          <div class="equip-price-num">$95</div>
          <div class="equip-price-label">Per day · Weekly rates available</div>
        </div>
        <div class="equip-avail avail-yes">Available</div>
      </div>
    </div>

    <div class="equip-card">
      <div class="equip-number">02</div>
      <div class="equip-category">Skid Steer Attachment</div>
      <div class="equip-name">4-In-1 Hydraulic Bucket</div>
      <p class="equip-desc">72" hydraulic 4-in-1 combination bucket. Scoop, clamp, grade, and spread. The most versatile attachment in the fleet.</p>
      <div class="equip-footer">
        <div class="equip-price">
          <div class="equip-price-num">$85</div>
          <div class="equip-price-label">Per day · Weekly rates available</div>
        </div>
        <div class="equip-avail avail-yes">Available</div>
      </div>
    </div>

    <div class="equip-card">
      <div class="equip-number">03</div>
      <div class="equip-category">Skid Steer Attachment</div>
      <div class="equip-name">Hydraulic Backhoe</div>
      <p class="equip-desc">Seated swivel backhoe with 12" bucket. Dig trenches, footings, utility lines, and more with precision control.</p>
      <div class="equip-footer">
        <div class="equip-price">
          <div class="equip-price-num">$175</div>
          <div class="equip-price-label">Per day · Weekly rates available</div>
        </div>
        <div class="equip-avail avail-yes">Available</div>
      </div>
    </div>

    <div class="equip-card">
      <div class="equip-number">04</div>
      <div class="equip-category">Skid Steer Attachment</div>
      <div class="equip-name">Hydraulic Stump Grinder</div>
      <p class="equip-desc">Heavy duty stump grinder attachment. Removes stumps quickly and efficiently without digging. Requires high flow hydraulics.</p>
      <div class="equip-footer">
        <div class="equip-price">
          <div class="equip-price-num">$150</div>
          <div class="equip-price-label">Per day · Weekly rates available</div>
        </div>
        <div class="equip-avail avail-yes">Available</div>
      </div>
    </div>

    <div class="equip-card">
      <div class="equip-number">05</div>
      <div class="equip-category">Skid Steer Attachment</div>
      <div class="equip-name">Posthole Digger</div>
      <p class="equip-desc">Hydraulic auger with 8", 12", and 16" bits included. Fence posts, sign posts, tree planting, and deck footings.</p>
      <div class="equip-footer">
        <div class="equip-price">
          <div class="equip-price-num">$125</div>
          <div class="equip-price-label">Per day · 3 auger sizes included</div>
        </div>
        <div class="equip-avail avail-yes">Available</div>
      </div>
    </div>

    <div class="equip-card">
      <div class="equip-number">06</div>
      <div class="equip-category">Skid Steer Attachment</div>
      <div class="equip-name">Flat Ripper Scarifier</div>
      <p class="equip-desc">70" hydraulic scarifier for breaking up hard packed soil, asphalt, and rocky ground before grading or landscaping.</p>
      <div class="equip-footer">
        <div class="equip-price">
          <div class="equip-price-num">$85</div>
          <div class="equip-price-label">Per day · Weekly rates available</div>
        </div>
        <div class="equip-avail avail-yes">Available</div>
      </div>
    </div>

    <div class="equip-card">
      <div class="equip-number">07</div>
      <div class="equip-category">Skid Steer Attachment</div>
      <div class="equip-name">Telescopic Boom</div>
      <p class="equip-desc">Extends reach for lifting and placing materials at height or over obstacles. Versatile tool for construction and landscaping.</p>
      <div class="equip-footer">
        <div class="equip-price">
          <div class="equip-price-num">$95</div>
          <div class="equip-price-label">Per day · Weekly rates available</div>
        </div>
        <div class="equip-avail avail-yes">Available</div>
      </div>
    </div>

    <div class="equip-card">
      <div class="equip-number">08</div>
      <div class="equip-category">Skid Steer Attachment</div>
      <div class="equip-name">Hydraulic Rototiller</div>
      <p class="equip-desc">72" hydraulic rototiller for soil preparation, garden beds, food plots, and seedbed preparation. Requires high flow.</p>
      <div class="equip-footer">
        <div class="equip-price">
          <div class="equip-price-num">$125</div>
          <div class="equip-price-label">Per day · Weekly rates available</div>
        </div>
        <div class="equip-avail avail-yes">Available</div>
      </div>
    </div>

    <div class="equip-card">
      <div class="equip-number">09</div>
      <div class="equip-category">Skid Steer Attachment</div>
      <div class="equip-name">Grapple Bucket</div>
      <p class="equip-desc">Hydraulic grapple bucket for handling brush, logs, debris, and loose materials. Essential for land clearing and cleanup.</p>
      <div class="equip-footer">
        <div class="equip-price">
          <div class="equip-price-num">$110</div>
          <div class="equip-price-label">Per day · Weekly rates available</div>
        </div>
        <div class="equip-avail avail-yes">Available</div>
      </div>
    </div>

    <div class="equip-card">
      <div class="equip-number">10</div>
      <div class="equip-category">Towable Equipment</div>
      <div class="equip-name">Pressure Washer Trailer</div>
      <p class="equip-desc">Commercial grade Hotsy pressure washer on tandem axle trailer with 500 gallon water tank and integrated hose reel.</p>
      <div class="equip-footer">
        <div class="equip-price">
          <div class="equip-price-num">$225</div>
          <div class="equip-price-label">Per day · $900 per week</div>
        </div>
        <div class="equip-avail avail-yes">Available</div>
      </div>
    </div>

    <div class="equip-card" style="border-color: rgba(201,168,76,0.4); grid-column: span 1;">
      <div class="equip-number">11</div>
      <div class="equip-category" style="color: #E0B95C;">Featured · Request To Book</div>
      <div class="equip-name">2024 Bobcat T76</div>
      <p class="equip-desc">2024 Bobcat T76 compact track loader. High flow hydraulics, Bluetooth, backup camera, 2-speed. One of the most capable machines in its class. Request to book — we confirm every T76 rental personally.</p>
      <div style="margin: 12px 0; padding: 10px 12px; border: 1px solid var(--border); background: var(--dark); font-size: 12px; color: var(--text-muted); line-height: 1.6;">
        Add any attachment at half price when bundled with T76 rental. Damage deposit required.
      </div>
      <div class="equip-footer">
        <div class="equip-price">
          <div class="equip-price-num">$375</div>
          <div class="equip-price-label">Per day · Weekly rates available</div>
        </div>
        <div class="equip-avail avail-request">Request</div>
      </div>
    </div>

  </div>

  <div style="margin-top: 24px; padding: 20px; border: 1px solid var(--border); background: var(--dark);">
    <p style="font-size: 13px; color: var(--text-muted); line-height: 1.6;">
      <strong style="color: var(--gold);">Compatibility note:</strong> Skid steer attachments require a loader with auxiliary hydraulics. Stump grinder and rototiller require high flow hydraulics. Not sure if your machine is compatible? Call us at (307) 900-5333 before booking.
    </p>
  </div>
</section>

<!-- HOW IT WORKS -->
<section class="section section-darker" id="how-it-works">
  <div class="section-header">
    <div class="section-eyebrow">The Process</div>
    <h2 class="section-title">How It Works</h2>
    <p class="section-sub">Simple, transparent, and documented at every step. Your equipment, your schedule.</p>
  </div>
  <div class="how-grid">
    <div class="how-step">
      <div class="how-step-num">01</div>
      <div class="how-icon">
        <svg viewBox="0 0 24 24"><rect x="3" y="4" width="18" height="18" rx="2"/><line x1="16" y1="2" x2="16" y2="6"/><line x1="8" y1="2" x2="8" y2="6"/><line x1="3" y1="10" x2="21" y2="10"/></svg>
      </div>
      <div class="how-title">Submit your request</div>
      <p class="how-desc">Fill out the booking form below with your equipment choice, dates, and contact info. We respond within 24 hours to confirm availability.</p>
    </div>
    <div class="how-step">
      <div class="how-step-num">02</div>
      <div class="how-icon">
        <svg viewBox="0 0 24 24"><line x1="12" y1="1" x2="12" y2="23"/><path d="M17 5H9.5a3.5 3.5 0 0 0 0 7h5a3.5 3.5 0 0 1 0 7H6"/></svg>
      </div>
      <div class="how-title">Confirm and pay</div>
      <p class="how-desc">Once confirmed, payment is collected via Stripe, Venmo, or cash on pickup. Your rental slot is held once payment is received.</p>
    </div>
    <div class="how-step">
      <div class="how-step-num">03</div>
      <div class="how-icon">
        <svg viewBox="0 0 24 24"><path d="M23 19a2 2 0 0 1-2 2H3a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h4l2-3h6l2 3h4a2 2 0 0 1 2 2z"/><circle cx="12" cy="13" r="4"/></svg>
      </div>
      <div class="how-title">Document at pickup</div>
      <p class="how-desc">Before leaving with the equipment, complete the required photo checklist documenting condition from all required angles.</p>
    </div>
    <div class="how-step">
      <div class="how-step-num">04</div>
      <div class="how-icon">
        <svg viewBox="0 0 24 24"><polyline points="20 6 9 17 4 12"/></svg>
      </div>
      <div class="how-title">Return and close out</div>
      <p class="how-desc">Return equipment by your scheduled time and complete the return photo checklist. Rental closes automatically when all photos are submitted.</p>
    </div>
  </div>

  <div class="photo-section">
    <div class="photo-title">Required Photo Documentation</div>
    <p style="font-size: 13px; color: var(--text-muted); margin-bottom: 16px; font-weight: 300;">All 6 photos required at pickup AND return. This protects both parties and ensures fair condition assessment.</p>
    <div class="photo-grid">
      <div class="photo-item"><div class="photo-dot"></div>Front of equipment</div>
      <div class="photo-item"><div class="photo-dot"></div>Rear of equipment</div>
      <div class="photo-item"><div class="photo-dot"></div>Left side</div>
      <div class="photo-item"><div class="photo-dot"></div>Right side</div>
      <div class="photo-item"><div class="photo-dot"></div>Hitch / connection point</div>
      <div class="photo-item"><div class="photo-dot"></div>Hour meter reading</div>
    </div>
  </div>
</section>

<!-- SERVICE AREA -->
<div class="area-banner">
  <div class="area-banner-left">
    <div class="area-banner-title">Serving All Of Natrona County</div>
    <div class="area-banner-sub">Pickup available at our Evansville location · Delivery available for select equipment</div>
  </div>
  <div class="area-tags">
    <div class="area-tag">Casper</div>
    <div class="area-tag">Evansville</div>
    <div class="area-tag">Mills</div>
    <div class="area-tag">Bar Nunn</div>
  </div>
</div>

<!-- CONTACT -->
<section class="section section-dark" id="contact">
  <div class="section-header">
    <div class="section-eyebrow">Get In Touch</div>
    <h2 class="section-title">Book Your Equipment</h2>
    <p class="section-sub">Submit a rental request and we'll confirm availability within 24 hours. Have questions? Call or text anytime.</p>
  </div>
  <div class="contact-grid">
    <div class="contact-info">
      <div class="contact-detail">
        <div class="contact-icon">
          <svg viewBox="0 0 24 24"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07A19.5 19.5 0 0 1 4.69 12 19.79 19.79 0 0 1 1.61 3.4 2 2 0 0 1 3.6 1.22h3a2 2 0 0 1 2 1.72c.127.96.361 1.903.7 2.81a2 2 0 0 1-.45 2.11L7.91 8.96a16 16 0 0 0 6 6l.92-.92a2 2 0 0 1 2.11-.45c.907.339 1.85.573 2.81.7A2 2 0 0 1 21.73 16.92z"/></svg>
        </div>
        <div>
          <div class="contact-label">Phone / Text</div>
          <div class="contact-value"><a href="tel:3079005333">(307) 900-5333</a></div>
        </div>
      </div>
      <div class="contact-detail">
        <div class="contact-icon">
          <svg viewBox="0 0 24 24"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"/><polyline points="22,6 12,13 2,6"/></svg>
        </div>
        <div>
          <div class="contact-label">Email</div>
          <div class="contact-value"><a href="mailto:wyomingpremierrental@gmail.com">wyomingpremierrental@gmail.com</a></div>
        </div>
      </div>
      <div class="contact-detail">
        <div class="contact-icon">
          <svg viewBox="0 0 24 24"><path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0 1 18 0z"/><circle cx="12" cy="10" r="3"/></svg>
        </div>
        <div>
          <div class="contact-label">Pickup Location</div>
          <div class="contact-value">Evansville, Wyoming 82636<br><span style="font-size: 13px; color: var(--text-muted);">Natrona County</span></div>
        </div>
      </div>
      <div class="contact-detail">
        <div class="contact-icon">
          <svg viewBox="0 0 24 24"><circle cx="12" cy="12" r="10"/><polyline points="12 6 12 12 16 14"/></svg>
        </div>
        <div>
          <div class="contact-label">Response Time</div>
          <div class="contact-value">Within 24 hours</div>
        </div>
      </div>
      <div style="padding: 20px; border: 1px solid var(--border); background: var(--dark3);">
        <div style="font-family: 'Barlow Condensed', sans-serif; font-size: 11px; font-weight: 600; letter-spacing: 3px; text-transform: uppercase; color: var(--gold); margin-bottom: 8px;">Payment Methods</div>
        <div style="font-size: 13px; color: var(--text-muted); line-height: 1.7;">Stripe (credit/debit card) · Venmo · Cash on pickup</div>
      </div>
    </div>

    <div class="form">
      <div class="form-title">Rental Request</div>
      <div class="form-sub">All fields required. We'll confirm availability and send payment instructions within 24 hours.</div>
      <div id="success-msg" class="success-msg">Your request has been submitted. We'll be in touch within 24 hours to confirm your rental.</div>
      <div class="form-row">
        <div class="form-group">
          <label class="form-label">First Name</label>
          <input class="form-input" type="text" placeholder="John" id="fname">
        </div>
        <div class="form-group">
          <label class="form-label">Last Name</label>
          <input class="form-input" type="text" placeholder="Smith" id="lname">
        </div>
      </div>
      <div class="form-row">
        <div class="form-group">
          <label class="form-label">Phone Number</label>
          <input class="form-input" type="tel" placeholder="(307) 555-0100" id="phone">
        </div>
        <div class="form-group">
          <label class="form-label">Email Address</label>
          <input class="form-input" type="email" placeholder="you@email.com" id="email">
        </div>
      </div>
      <div class="form-group">
        <label class="form-label">Equipment Requested</label>
        <select class="form-input" id="equipment">
          <option value="">Select equipment...</option>
          <option>Hydraulic Rock Rake 78" — $95/day</option>
          <option>4-In-1 Hydraulic Bucket 72" — $85/day</option>
          <option>Hydraulic Backhoe w/ 12" Bucket — $175/day</option>
          <option>Hydraulic Stump Grinder — $150/day</option>
          <option>Posthole Digger w/ 3 Auger Sizes — $125/day</option>
          <option>Flat Ripper Scarifier 70" — $85/day</option>
          <option>Telescopic Boom — $95/day</option>
          <option>Hydraulic Rototiller 72" — $125/day</option>
          <option>Grapple Bucket — $110/day</option>
          <option>2024 Bobcat T76 Skid Steer — $375/day (Request to book)</option>
          <option>2024 Bobcat T76 + Attachment Bundle — $375/day + half price attachment</option>
        </select>
      </div>
      <div class="form-row">
        <div class="form-group">
          <label class="form-label">Pickup Date</label>
          <input class="form-input" type="date" id="pickup">
        </div>
        <div class="form-group">
          <label class="form-label">Return Date</label>
          <input class="form-input" type="date" id="return">
        </div>
      </div>
      <div class="form-row">
        <div class="form-group">
          <label class="form-label">City</label>
          <select class="form-input" id="city">
            <option>Casper</option>
            <option>Evansville</option>
            <option>Mills</option>
            <option>Bar Nunn</option>
            <option>Other Natrona County</option>
          </select>
        </div>
        <div class="form-group">
          <label class="form-label">Preferred Payment</label>
          <select class="form-input" id="payment">
            <option>Stripe (credit/debit card)</option>
            <option>Venmo</option>
            <option>Cash on pickup</option>
          </select>
        </div>
      </div>
      <div class="form-group">
        <label class="form-label">Additional Notes (optional)</label>
        <textarea class="form-input" rows="3" placeholder="Project details, questions about compatibility, delivery needs..." id="notes" style="resize: vertical;"></textarea>
      </div>
      <div class="form-terms">
        <input type="checkbox" id="terms">
        <label for="terms">I understand that all required photos must be submitted at pickup and return, and that I am responsible for any damage beyond normal wear and tear during my rental period.</label>
      </div>
      <button class="form-submit" onclick="submitForm()">Submit Rental Request</button>
    </div>
  </div>
</section>

<!-- FOOTER -->
<footer>
  <div class="footer-grid">
    <div class="footer-brand">
      <div class="footer-logo">Wyoming <span>Premier</span> Rental</div>
      <div class="footer-tagline">Natrona County · Est. 2026</div>
      <p class="footer-desc">Wyoming owned and operated equipment rental serving Casper, Evansville, Mills, and Bar Nunn. Professional grade machines at honest prices.</p>
    </div>
    <div>
      <div class="footer-col-title">Equipment</div>
      <div class="footer-item">2024 Bobcat T76 Skid Steer</div>
      <div class="footer-item">Hydraulic Rock Rake</div>
      <div class="footer-item">4-In-1 Bucket</div>
      <div class="footer-item">Hydraulic Backhoe</div>
      <div class="footer-item">Stump Grinder</div>
      <div class="footer-item">Posthole Digger</div>
      <div class="footer-item">Pressure Washer Trailer</div>
    </div>
    <div>
      <div class="footer-col-title">Contact</div>
      <div class="footer-item"><a href="tel:3079005333">(307) 900-5333</a></div>
      <div class="footer-item"><a href="mailto:wyomingpremierrental@gmail.com">wyomingpremierrental@gmail.com</a></div>
      <div class="footer-item">Evansville, Wyoming 82636</div>
      <div class="footer-item" style="margin-top: 16px;">
        <a href="#equipment">Browse Equipment</a>
      </div>
      <div class="footer-item"><a href="#contact">Book a Rental</a></div>
    </div>
  </div>
  <div class="footer-bottom">
    <div class="footer-copy">© 2026 Wyoming Premier Rental LLC · All rights reserved</div>
    <div class="footer-badge">Wyoming LLC · Natrona County</div>
  </div>
</footer>

<script>
function submitForm() {
  const required = ['fname','lname','phone','email','equipment','pickup','return'];
  let valid = true;
  required.forEach(id => {
    const el = document.getElementById(id);
    if (!el.value) {
      el.style.borderColor = 'rgba(226,75,74,0.6)';
      valid = false;
    } else {
      el.style.borderColor = '';
    }
  });
  if (!document.getElementById('terms').checked) {
    alert('Please agree to the rental terms before submitting.');
    return;
  }
  if (!valid) {
    alert('Please fill in all required fields.');
    return;
  }
  const msg = document.getElementById('success-msg');
  msg.style.display = 'block';
  msg.scrollIntoView({ behavior: 'smooth', block: 'center' });
  ['fname','lname','phone','email','equipment','pickup','return','notes'].forEach(id => {
    document.getElementById(id).value = '';
  });
  document.getElementById('terms').checked = false;
}

document.querySelectorAll('a[href^="#"]').forEach(a => {
  a.addEventListener('click', e => {
    e.preventDefault();
    const target = document.querySelector(a.getAttribute('href'));
    if (target) target.scrollIntoView({ behavior: 'smooth' });
  });
});
</script>
</body>
</html>
