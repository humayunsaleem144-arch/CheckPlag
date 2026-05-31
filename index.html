<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta http-equiv="Cache-Control" content="no-cache, no-store, must-revalidate">
<meta http-equiv="Pragma" content="no-cache">
<meta http-equiv="Expires" content="0">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>CheckPlag — Plagiarism Report Service</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Fraunces:opsz,wght@9..144,400;9..144,500;9..144,600;9..144,700;9..144,900&family=Plus+Jakarta+Sans:wght@400;500;600;700;800&display=swap" rel="stylesheet">
<script src="https://cdn.jsdelivr.net/npm/@supabase/supabase-js@2"></script>
<style>
:root {
  /* Premium indigo-navy primary palette (mapped to blue-* names for compatibility) */
  --blue-50: #eef2ff;
  --blue-100: #e0e7ff;
  --blue-200: #c7d2fe;
  --blue-300: #a5b4fc;
  --blue-400: #818cf8;
  --blue-500: #6366f1;
  --blue-600: #4f46e5;
  --blue-700: #4338ca;
  --blue-800: #3730a3;
  --blue-900: #1e1b4b;
  --white: #ffffff;
  /* Warm-tinted neutrals for a refined, less sterile feel */
  --gray-50: #f9fafb;
  --gray-100: #f3f4f6;
  --gray-200: #e5e7eb;
  --gray-300: #d1d5db;
  --gray-400: #9ca3af;
  --gray-500: #6b7280;
  --gray-600: #4b5563;
  --gray-700: #374151;
  --gray-800: #1f2937;
  --gray-900: #111827;
  --green-500: #10b981;
  --green-600: #059669;
  --green-50: #ecfdf5;
  --amber-500: #f59e0b;
  --amber-600: #d97706;
  --red-500: #ef4444;
  --red-600: #dc2626;
  --red-50: #fef2f2;
  --red-200: #fecaca;
  /* Signature accent — refined teal */
  --accent: #0d9488;
  --accent-light: #14b8a6;
  --ink: #14152e;
  --radius: 14px;
  --radius-lg: 20px;
  --shadow-sm: 0 1px 2px rgba(20,21,46,0.04);
  --shadow: 0 1px 3px rgba(20,21,46,0.08), 0 1px 2px rgba(20,21,46,0.04);
  --shadow-md: 0 4px 16px -2px rgba(20,21,46,0.08), 0 2px 6px -2px rgba(20,21,46,0.05);
  --shadow-lg: 0 12px 32px -6px rgba(20,21,46,0.12), 0 4px 12px -4px rgba(20,21,46,0.06);
  --shadow-xl: 0 24px 48px -12px rgba(20,21,46,0.18), 0 8px 16px -8px rgba(20,21,46,0.08);
  --shadow-glow: 0 0 0 1px rgba(79,70,229,0.08), 0 8px 24px -6px rgba(79,70,229,0.2);
}

* { margin: 0; padding: 0; box-sizing: border-box; }

body {
  font-family: 'Plus Jakarta Sans', -apple-system, sans-serif;
  background: var(--gray-50);
  color: var(--gray-800);
  min-height: 100vh;
  overflow-x: hidden;
  -webkit-font-smoothing: antialiased;
  text-rendering: optimizeLegibility;
}

h1, h2, h3, h4, h5 {
  font-family: 'Fraunces', Georgia, serif;
  letter-spacing: -0.02em;
  font-optical-sizing: auto;
}

.hidden { display: none !important; }

::selection { background: var(--blue-200); color: var(--blue-900); }

/* Refined scrollbar */
::-webkit-scrollbar { width: 10px; height: 10px; }
::-webkit-scrollbar-track { background: transparent; }
::-webkit-scrollbar-thumb { background: var(--gray-300); border-radius: 10px; border: 2px solid var(--gray-50); }
::-webkit-scrollbar-thumb:hover { background: var(--gray-400); }

/* ==================== LANDING PAGE ==================== */
.landing-page { min-height: 100vh; }

.landing-nav {
  display: flex; align-items: center; justify-content: space-between;
  padding: 18px 44px; background: rgba(255,255,255,0.8);
  backdrop-filter: blur(16px) saturate(180%);
  border-bottom: 1px solid var(--gray-200);
  position: sticky; top: 0; z-index: 100;
}

.logo-group { display: flex; align-items: center; gap: 11px; }

.logo-svg { width: 40px; height: 40px; }

.logo-text { font-family: 'Fraunces', serif; font-weight: 600; font-size: 24px; color: var(--ink); letter-spacing: -0.02em; }

.nav-actions { display: flex; align-items: center; gap: 12px; }

.lang-toggle {
  background: var(--gray-100); border: 1px solid var(--gray-200);
  padding: 7px 15px; border-radius: 100px; cursor: pointer;
  font-size: 13px; font-weight: 600; color: var(--gray-600);
  transition: all 0.2s;
}
.lang-toggle:hover { background: var(--blue-50); color: var(--blue-600); border-color: var(--blue-200); }

.btn {
  padding: 11px 24px; border-radius: 10px; border: none;
  font-weight: 600; font-size: 14px; cursor: pointer;
  font-family: 'Plus Jakarta Sans', sans-serif; letter-spacing: 0.01em;
  transition: transform 0.2s cubic-bezier(0.16,1,0.3,1), box-shadow 0.2s, background 0.2s, border-color 0.2s;
}

.btn-outline {
  background: transparent; color: var(--blue-600);
  border: 1.5px solid var(--blue-200);
}
.btn-outline:hover { background: var(--blue-50); border-color: var(--blue-400); }

.btn-primary {
  background: linear-gradient(135deg, var(--blue-600), var(--blue-700)); color: var(--white);
  box-shadow: 0 2px 8px -1px rgba(79,70,229,0.4), inset 0 1px 0 rgba(255,255,255,0.15);
}
.btn-primary:hover { transform: translateY(-2px); box-shadow: 0 8px 20px -4px rgba(79,70,229,0.5), inset 0 1px 0 rgba(255,255,255,0.15); }

.btn-sm { padding: 8px 16px; font-size: 13px; border-radius: 8px; }
.btn-lg { padding: 15px 34px; font-size: 16px; border-radius: 12px; }
.btn-danger { background: var(--red-500); color: white; box-shadow: 0 2px 8px -1px rgba(239,68,68,0.35); }
.btn-danger:hover { background: var(--red-600); transform: translateY(-2px); box-shadow: 0 8px 18px -4px rgba(239,68,68,0.45); }
.btn-success { background: linear-gradient(135deg, var(--green-500), var(--green-600)); color: white; box-shadow: 0 2px 8px -1px rgba(16,185,129,0.35); }
.btn-success:hover { transform: translateY(-2px); box-shadow: 0 8px 18px -4px rgba(16,185,129,0.45); }
.btn-ghost { background: transparent; color: var(--gray-600); }
.btn-ghost:hover { background: var(--gray-100); }
.btn-white { background: white; color: var(--blue-700); border: 1.5px solid var(--gray-200); }
.btn-white:hover { border-color: var(--blue-300); background: var(--blue-50); }
.btn-full { width: 100%; }

.hero {
  padding: 110px 40px 120px; text-align: center;
  background:
    radial-gradient(ellipse 80% 60% at 50% -20%, rgba(20,184,166,0.25), transparent 60%),
    radial-gradient(circle at 15% 80%, rgba(99,102,241,0.3), transparent 50%),
    linear-gradient(165deg, #1e1b4b 0%, #312e81 45%, #1e1b4b 100%);
  color: white; position: relative; overflow: hidden;
}

.hero::before {
  content: ''; position: absolute; inset: 0;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='200' height='200'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='3'/%3E%3C/filter%3E%3Crect width='200' height='200' filter='url(%23n)' opacity='0.04'/%3E%3C/svg%3E");
  pointer-events: none;
}

.hero::after {
  content: ''; position: absolute; left: 0; right: 0; bottom: 0; height: 1px;
  background: linear-gradient(90deg, transparent, rgba(255,255,255,0.2), transparent);
}

.hero-content { position: relative; z-index: 1; max-width: 760px; margin: 0 auto; }

.hero-badge {
  display: inline-flex; align-items: center; gap: 8px;
  background: rgba(255,255,255,0.08); backdrop-filter: blur(12px);
  padding: 8px 18px; border-radius: 100px; font-size: 13px;
  font-weight: 600; margin-bottom: 32px; letter-spacing: 0.01em;
  border: 1px solid rgba(255,255,255,0.14);
  box-shadow: inset 0 1px 0 rgba(255,255,255,0.1);
}

.hero h1 {
  font-size: 64px; font-weight: 600; line-height: 1.04; margin-bottom: 24px;
  letter-spacing: -0.035em;
}
.hero h1 em {
  font-style: italic; font-weight: 400;
  background: linear-gradient(120deg, var(--accent-light), #5eead4);
  -webkit-background-clip: text; background-clip: text; -webkit-text-fill-color: transparent;
}
.hero p {
  font-size: 19px; opacity: 0.82; line-height: 1.65; margin-bottom: 40px;
  max-width: 560px; margin-left: auto; margin-right: auto; font-weight: 400;
}

.hero-actions { display: flex; gap: 14px; justify-content: center; flex-wrap: wrap; }

.hero-trust {
  display: flex; gap: 28px; justify-content: center; flex-wrap: wrap;
  margin-top: 36px;
}
.hero-trust span {
  font-size: 14px; font-weight: 600; color: rgba(255,255,255,0.78);
  display: inline-flex; align-items: center; gap: 6px;
}

.hero .btn-lg { padding: 17px 38px; font-size: 16px; }
.hero .btn-white { background: white; color: var(--blue-900); border: none; font-weight: 700; box-shadow: 0 8px 24px -6px rgba(0,0,0,0.3); }
.hero .btn-white:hover { background: #f5f3ff; transform: translateY(-2px); box-shadow: 0 14px 32px -8px rgba(0,0,0,0.4); }
.hero .btn-outline-white { background: rgba(255,255,255,0.06); color: white; border: 1.5px solid rgba(255,255,255,0.3); backdrop-filter: blur(8px); }
.hero .btn-outline-white:hover { background: rgba(255,255,255,0.14); border-color: rgba(255,255,255,0.6); }

.features {
  padding: 100px 40px; max-width: 1140px; margin: 0 auto;
}

.section-eyebrow {
  display: block; text-align: center; font-family: 'Plus Jakarta Sans', sans-serif;
  font-size: 13px; font-weight: 700; letter-spacing: 0.12em; text-transform: uppercase;
  color: var(--accent); margin-bottom: 16px;
}

.features h2 { text-align: center; font-size: 44px; font-weight: 600; margin-bottom: 16px; color: var(--ink); }
.features > p { text-align: center; color: var(--gray-500); font-size: 17px; margin-bottom: 60px; max-width: 520px; margin-left: auto; margin-right: auto; }

.features-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 24px; }

.feature-card {
  background: var(--white); border: 1px solid var(--gray-200);
  border-radius: var(--radius-lg); padding: 38px 32px;
  transition: transform 0.4s cubic-bezier(0.16,1,0.3,1), box-shadow 0.4s, border-color 0.4s;
  position: relative; overflow: hidden;
}
.feature-card::after {
  content: ''; position: absolute; top: 0; left: 0; right: 0; height: 3px;
  background: linear-gradient(90deg, var(--accent), var(--blue-500));
  transform: scaleX(0); transform-origin: left; transition: transform 0.4s ease;
}
.feature-card:hover { border-color: transparent; box-shadow: var(--shadow-lg); transform: translateY(-6px); }
.feature-card:hover::after { transform: scaleX(1); }

.feature-icon {
  width: 56px; height: 56px; border-radius: 16px;
  background: linear-gradient(135deg, var(--blue-50), var(--blue-100));
  display: flex; align-items: center;
  justify-content: center; margin-bottom: 22px; font-size: 26px;
  box-shadow: inset 0 1px 0 rgba(255,255,255,0.6);
}

.feature-card h3 { font-size: 21px; font-weight: 600; margin-bottom: 10px; color: var(--ink); }
.feature-card p { font-size: 15px; color: var(--gray-500); line-height: 1.7; }

.pricing {
  padding: 100px 40px; background: var(--ink); color: white;
  position: relative; overflow: hidden;
}
.pricing::before {
  content: ''; position: absolute; top: -30%; left: 50%; transform: translateX(-50%);
  width: 800px; height: 500px; border-radius: 50%;
  background: radial-gradient(circle, rgba(99,102,241,0.18), transparent 70%);
  pointer-events: none;
}

.pricing .section-eyebrow { color: var(--accent-light); }
.pricing h2 { text-align: center; font-size: 44px; font-weight: 600; margin-bottom: 16px; color: white; position: relative; }
.pricing > p { text-align: center; color: rgba(255,255,255,0.6); margin-bottom: 60px; position: relative; }

.pricing-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 24px; max-width: 960px; margin: 0 auto; position: relative; }

.price-card {
  border: 1px solid rgba(255,255,255,0.1); border-radius: var(--radius-lg);
  padding: 38px 30px; text-align: center;
  transition: transform 0.4s cubic-bezier(0.16,1,0.3,1), box-shadow 0.4s, border-color 0.4s;
  background: rgba(255,255,255,0.04); backdrop-filter: blur(12px);
}
.price-card.featured {
  border-color: var(--accent-light);
  background: linear-gradient(165deg, rgba(20,184,166,0.18), rgba(99,102,241,0.12));
  position: relative; box-shadow: 0 0 40px -8px rgba(20,184,166,0.4);
}
.price-card.featured::before {
  content: '★ Most Popular'; position: absolute; top: -13px; left: 50%; transform: translateX(-50%);
  background: linear-gradient(120deg, var(--accent-light), var(--accent)); color: white; padding: 5px 18px;
  border-radius: 100px; font-size: 11px; font-weight: 700; letter-spacing: 0.04em;
  font-family: 'Plus Jakarta Sans', sans-serif; white-space: nowrap;
  box-shadow: 0 4px 12px -2px rgba(20,184,166,0.5);
}
.price-card:hover { transform: translateY(-6px); box-shadow: var(--shadow-xl); border-color: rgba(255,255,255,0.25); }

.price-card h3 { font-size: 22px; font-weight: 600; margin-bottom: 6px; color: white; }
.price-credits { font-size: 14px; color: rgba(255,255,255,0.55); margin-bottom: 20px; font-family: 'Plus Jakarta Sans', sans-serif; }
.price-amount { font-size: 46px; font-weight: 600; color: white; margin-bottom: 24px; font-family: 'Fraunces', serif; }
.price-amount span { font-size: 15px; font-weight: 400; color: rgba(255,255,255,0.45); font-family: 'Plus Jakarta Sans', sans-serif; }
.price-card .btn-outline { border-color: rgba(255,255,255,0.25); color: white; }
.price-card .btn-outline:hover { background: rgba(255,255,255,0.1); border-color: rgba(255,255,255,0.5); }

.contact-section {
  padding: 100px 40px; max-width: 760px; margin: 0 auto; text-align: center;
}

.contact-section h2 { font-size: 44px; font-weight: 600; margin-bottom: 16px; color: var(--ink); }
.contact-section > p { color: var(--gray-500); margin-bottom: 44px; font-size: 17px; }

.contact-cards { display: flex; gap: 20px; justify-content: center; flex-wrap: wrap; }

.contact-card {
  flex: 1; min-width: 260px; background: var(--white);
  border: 1px solid var(--gray-200); border-radius: var(--radius-lg);
  padding: 36px 28px; text-align: center;
  transition: transform 0.3s, box-shadow 0.3s, border-color 0.3s;
}
.contact-card:hover { border-color: var(--accent); box-shadow: var(--shadow-lg); transform: translateY(-4px); }

.contact-card-icon { font-size: 38px; margin-bottom: 16px; }
.contact-card h4 { font-size: 19px; font-weight: 600; margin-bottom: 8px; color: var(--ink); }
.contact-card .contact-name { color: var(--gray-500); font-size: 14px; margin-bottom: 4px; }
.contact-card .contact-number { color: var(--gray-700); font-size: 15px; font-weight: 700; margin-bottom: 18px; }

.landing-footer {
  background: var(--ink); color: rgba(255,255,255,0.5);
  padding: 40px; text-align: center; font-size: 14px;
  border-top: 1px solid rgba(255,255,255,0.06);
}

/* ==================== PRIVACY BANNER ==================== */
.privacy-banner {
  padding: 80px 40px;
  background: linear-gradient(135deg, var(--accent) 0%, #0f766e 100%);
  position: relative; overflow: hidden;
}
.privacy-banner::before {
  content: ''; position: absolute; top: -40%; right: -10%;
  width: 500px; height: 500px; border-radius: 50%;
  background: rgba(255,255,255,0.06); pointer-events: none;
}
.privacy-content { max-width: 760px; margin: 0 auto; text-align: center; position: relative; color: white; }
.privacy-icon { font-size: 52px; margin-bottom: 18px; }
.privacy-banner h2 { font-size: 38px; font-weight: 600; margin-bottom: 18px; color: white; }
.privacy-banner p { font-size: 17px; line-height: 1.7; opacity: 0.92; margin-bottom: 32px; }
.privacy-points { display: flex; gap: 16px; justify-content: center; flex-wrap: wrap; }
.privacy-point {
  display: flex; align-items: center; gap: 8px;
  background: rgba(255,255,255,0.14); backdrop-filter: blur(8px);
  padding: 12px 22px; border-radius: 100px; font-size: 15px; font-weight: 600;
  border: 1px solid rgba(255,255,255,0.18);
}

/* ==================== FAQ ==================== */
.faq-section {
  padding: 100px 40px; max-width: 800px; margin: 0 auto; text-align: center;
}
.faq-section h2 { font-size: 44px; font-weight: 600; margin-bottom: 16px; color: var(--ink); }
.faq-section > p { color: var(--gray-500); margin-bottom: 48px; font-size: 17px; }
.faq-list { text-align: left; }
.faq-item {
  background: var(--white); border: 1px solid var(--gray-200);
  border-radius: var(--radius); margin-bottom: 12px; cursor: pointer;
  transition: border-color 0.2s, box-shadow 0.2s; overflow: hidden;
}
.faq-item:hover { border-color: var(--blue-300); box-shadow: var(--shadow-sm); }
.faq-item.open { border-color: var(--blue-400); box-shadow: var(--shadow-md); }
.faq-q {
  padding: 20px 24px; font-weight: 600; font-size: 16px; color: var(--ink);
  display: flex; justify-content: space-between; align-items: center; gap: 16px;
  font-family: 'Plus Jakarta Sans', sans-serif;
}
.faq-arrow { transition: transform 0.3s; color: var(--blue-500); font-size: 20px; flex-shrink: 0; }
.faq-item.open .faq-arrow { transform: rotate(180deg); }
.faq-a {
  max-height: 0; overflow: hidden; padding: 0 24px;
  color: var(--gray-600); font-size: 15px; line-height: 1.7;
  transition: max-height 0.3s ease, padding 0.3s ease;
}
.faq-item.open .faq-a { max-height: 200px; padding: 0 24px 20px; }

/* ==================== TERMS ==================== */
.terms-block { margin-bottom: 28px; }
.terms-block h3 { font-size: 20px; color: var(--ink); margin-bottom: 10px; }
.terms-block p { color: var(--gray-600); font-size: 15px; line-height: 1.75; }

/* ==================== AUTH ==================== */
.auth-page {
  min-height: 100vh; display: flex; align-items: center; justify-content: center;
  background:
    radial-gradient(ellipse 60% 50% at 50% 0%, rgba(99,102,241,0.12), transparent 70%),
    radial-gradient(ellipse 50% 40% at 100% 100%, rgba(20,184,166,0.1), transparent 60%),
    var(--gray-50);
  padding: 20px; position: relative;
}
.auth-page::before {
  content: ''; position: absolute; inset: 0;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='40' height='40'%3E%3Cpath d='M0 20h40M20 0v40' stroke='%23000' stroke-width='0.5' opacity='0.025'/%3E%3C/svg%3E");
  pointer-events: none;
}

.auth-card {
  background: var(--white); border-radius: var(--radius-lg);
  box-shadow: var(--shadow-xl); padding: 44px;
  width: 100%; max-width: 430px;
  border: 1px solid var(--gray-200); position: relative; z-index: 1;
}

.auth-card .logo-group { justify-content: center; margin-bottom: 28px; }

.auth-card h2 { text-align: center; font-size: 30px; font-weight: 600; margin-bottom: 8px; color: var(--ink); }
.auth-card .auth-sub { text-align: center; color: var(--gray-500); font-size: 15px; margin-bottom: 32px; }

.form-group { margin-bottom: 18px; }
.form-group label {
  display: block; font-size: 13px; font-weight: 600;
  color: var(--gray-700); margin-bottom: 7px; letter-spacing: 0.01em;
}

.form-input {
  width: 100%; padding: 12px 15px; border: 1.5px solid var(--gray-200);
  border-radius: 10px; font-size: 14px; font-family: 'Plus Jakarta Sans', sans-serif;
  transition: border-color 0.2s, box-shadow 0.2s, background 0.2s; background: var(--gray-50);
  color: var(--gray-800);
}
.form-input:focus { outline: none; border-color: var(--blue-500); background: var(--white); box-shadow: 0 0 0 4px rgba(99,102,241,0.1); }
.form-input::placeholder { color: var(--gray-400); }

select.form-input { cursor: pointer; }

.auth-footer { text-align: center; margin-top: 20px; font-size: 14px; color: var(--gray-500); }
.auth-footer a { color: var(--blue-600); font-weight: 600; cursor: pointer; text-decoration: none; }
.auth-footer a:hover { text-decoration: underline; }

/* ==================== DASHBOARD LAYOUT ==================== */
.app-layout { display: flex; min-height: 100vh; }

.sidebar {
  width: 264px; background: var(--white);
  border-right: 1px solid var(--gray-200);
  display: flex; flex-direction: column;
  position: fixed; top: 0; left: 0; bottom: 0; z-index: 50;
}

.sidebar-header {
  padding: 22px 22px; border-bottom: 1px solid var(--gray-100);
  display: flex; align-items: center; gap: 10px;
}

.sidebar-nav { flex: 1; padding: 16px 12px; }

.nav-item {
  display: flex; align-items: center; gap: 11px;
  padding: 12px 14px; border-radius: 11px; cursor: pointer;
  font-size: 14px; font-weight: 500; color: var(--gray-600);
  transition: background 0.18s, color 0.18s, transform 0.18s; margin-bottom: 3px;
  position: relative;
}
.nav-item:hover { background: var(--blue-50); color: var(--blue-700); }
.nav-item.active {
  background: linear-gradient(135deg, var(--blue-600), var(--blue-700)); color: white;
  box-shadow: 0 4px 12px -2px rgba(79,70,229,0.4);
}
.nav-item .nav-icon { width: 20px; text-align: center; }

.sidebar-footer {
  padding: 16px 18px; border-top: 1px solid var(--gray-100);
}

.user-pill {
  display: flex; align-items: center; gap: 11px;
  padding: 8px 10px; border-radius: 11px;
}

.user-avatar {
  width: 38px; height: 38px; border-radius: 11px;
  background: linear-gradient(135deg, var(--blue-100), var(--blue-200)); color: var(--blue-700);
  display: flex; align-items: center; justify-content: center;
  font-weight: 700; font-size: 15px; flex-shrink: 0;
}

.user-info .user-name { font-size: 13px; font-weight: 700; color: var(--gray-800); }
.user-info .user-role { font-size: 11px; color: var(--gray-400); text-transform: uppercase; font-weight: 600; letter-spacing: 0.5px; }

.main-area {
  flex: 1; margin-left: 264px; display: flex; flex-direction: column;
}

.topbar {
  background: rgba(255,255,255,0.85); backdrop-filter: blur(16px) saturate(180%);
  border-bottom: 1px solid var(--gray-200);
  padding: 16px 32px; display: flex; align-items: center; justify-content: space-between;
  position: sticky; top: 0; z-index: 40;
}

.topbar-left h2 { font-size: 24px; font-weight: 600; color: var(--ink); }
.topbar-left p { font-size: 13px; color: var(--gray-500); }

.topbar-right { display: flex; align-items: center; gap: 12px; }

.notif-btn {
  position: relative; background: var(--gray-100);
  border: 1px solid var(--gray-200); width: 40px; height: 40px;
  border-radius: 11px; display: flex; align-items: center;
  justify-content: center; cursor: pointer; font-size: 16px;
  transition: all 0.2s;
}
.notif-btn:hover { background: var(--blue-50); border-color: var(--blue-300); }

.notif-badge {
  position: absolute; top: -4px; right: -4px;
  background: var(--red-500); color: white;
  width: 18px; height: 18px; border-radius: 50%;
  font-size: 10px; font-weight: 700;
  display: flex; align-items: center; justify-content: center;
  border: 2px solid var(--white);
}

.content { padding: 32px; flex: 1; }

/* ==================== STATS CARDS ==================== */
.stats-grid { display: grid; grid-template-columns: repeat(4, 1fr); gap: 18px; margin-bottom: 28px; }

.stat-card {
  background: var(--white); border: 1px solid var(--gray-200);
  border-radius: var(--radius); padding: 24px;
  transition: transform 0.3s cubic-bezier(0.16,1,0.3,1), box-shadow 0.3s, border-color 0.3s;
  position: relative; overflow: hidden;
}
.stat-card:hover { border-color: var(--blue-200); box-shadow: var(--shadow-md); transform: translateY(-3px); }

.stat-label { font-size: 11px; font-weight: 700; color: var(--gray-500); text-transform: uppercase; letter-spacing: 0.08em; margin-bottom: 10px; }
.stat-value { font-size: 32px; font-weight: 600; color: var(--ink); font-family: 'Fraunces', serif; line-height: 1; }
.stat-sub { font-size: 12px; color: var(--gray-400); margin-top: 6px; }

.stat-card.blue { border-left: 3px solid var(--blue-500); }
.stat-card.green { border-left: 3px solid var(--green-500); }
.stat-card.amber { border-left: 3px solid var(--amber-500); }
.stat-card.red { border-left: 3px solid var(--accent); }

/* ==================== CARDS & PANELS ==================== */
.panel {
  background: var(--white); border: 1px solid var(--gray-200);
  border-radius: var(--radius-lg); overflow: hidden; margin-bottom: 24px;
  box-shadow: var(--shadow-sm);
}

.panel-header {
  padding: 20px 24px; border-bottom: 1px solid var(--gray-100);
  display: flex; align-items: center; justify-content: space-between;
}

.panel-header h3 { font-size: 18px; font-weight: 600; color: var(--ink); }
.panel-body { padding: 24px; }

/* ==================== UPLOAD AREA ==================== */
.upload-zone {
  border: 2px dashed var(--gray-300); border-radius: var(--radius);
  padding: 48px 24px; text-align: center; cursor: pointer;
  transition: border-color 0.25s, background 0.25s, transform 0.25s; background: var(--gray-50);
}
.upload-zone:hover { border-color: var(--blue-400); background: var(--blue-50); }
.upload-zone.dragover { border-color: var(--blue-500); background: var(--blue-100); transform: scale(1.01); }

.upload-icon { font-size: 44px; margin-bottom: 14px; }
.upload-zone h4 { font-size: 17px; font-weight: 600; margin-bottom: 5px; color: var(--ink); font-family: 'Fraunces', serif; }
.upload-zone p { font-size: 13px; color: var(--gray-500); }

.file-selected {
  display: flex; align-items: center; gap: 12px;
  padding: 14px 18px; background: var(--blue-50);
  border: 1px solid var(--blue-200); border-radius: 8px;
  margin-top: 14px;
}
.file-selected .file-name { flex: 1; font-size: 14px; font-weight: 600; color: var(--blue-700); }

/* ==================== TABLE ==================== */
.table-wrap { overflow-x: auto; }

table { width: 100%; border-collapse: collapse; }
th {
  text-align: left; padding: 14px 18px; font-size: 11px;
  font-weight: 700; color: var(--gray-500); text-transform: uppercase;
  letter-spacing: 0.08em; background: var(--gray-50);
  border-bottom: 1px solid var(--gray-200);
}
td {
  padding: 16px 18px; font-size: 14px; border-bottom: 1px solid var(--gray-100);
  color: var(--gray-700);
}
tr:last-child td { border-bottom: none; }
tr:hover td { background: var(--gray-50); }

.badge {
  display: inline-block; padding: 5px 13px; border-radius: 100px;
  font-size: 12px; font-weight: 700; letter-spacing: 0.01em;
}
.badge-processing { background: #fef3c7; color: #92400e; }
.badge-queued { background: #e0e7ff; color: #4338ca; }
.badge-completed { background: #dcfce7; color: #166534; }
.badge-pending { background: var(--blue-100); color: var(--blue-700); }
.badge-rejected { background: #fee2e2; color: #991b1b; }

/* ==================== TIMER ==================== */
.timer-display {
  font-family: 'Fraunces', serif; font-size: 22px; font-weight: 800;
  color: var(--amber-500);
}

/* ==================== NOTIFICATION PANEL ==================== */
.notif-panel {
  position: fixed; top: 0; right: -380px; width: 380px;
  height: 100vh; background: var(--white); z-index: 200;
  box-shadow: -4px 0 24px rgba(0,0,0,0.1);
  transition: right 0.3s cubic-bezier(0.4, 0, 0.2, 1);
  display: flex; flex-direction: column;
  border-left: 1px solid var(--gray-200);
}
.notif-panel.open { right: 0; }

.notif-panel-header {
  padding: 18px 22px; border-bottom: 1px solid var(--gray-200);
  display: flex; align-items: center; justify-content: space-between;
}
.notif-panel-header h3 { font-size: 16px; font-weight: 700; }

.notif-list { flex: 1; overflow-y: auto; padding: 8px; }

.notif-item {
  padding: 14px 16px; border-radius: 8px;
  margin-bottom: 4px; cursor: pointer;
  transition: background 0.15s;
}
.notif-item:hover { background: var(--gray-50); }
.notif-item.unread { background: var(--blue-50); border-left: 3px solid var(--blue-500); }

.notif-item h5 { font-size: 13px; font-weight: 700; margin-bottom: 3px; }
.notif-item p { font-size: 12px; color: var(--gray-500); }
.notif-item .notif-time { font-size: 11px; color: var(--gray-400); margin-top: 4px; }

.overlay {
  position: fixed; inset: 0; background: rgba(0,0,0,0.3);
  z-index: 190; opacity: 0; pointer-events: none;
  transition: opacity 0.3s;
}
.overlay.open { opacity: 1; pointer-events: all; }

/* ==================== CONTACT INLINE ==================== */
.contact-inline {
  display: flex; gap: 14px; flex-wrap: wrap;
}

.contact-chip {
  display: flex; align-items: center; gap: 8px;
  padding: 10px 16px; background: var(--gray-50);
  border: 1px solid var(--gray-200); border-radius: 8px;
  font-size: 13px; color: var(--gray-700); text-decoration: none;
  transition: all 0.2s;
}
.contact-chip:hover { background: var(--blue-50); border-color: var(--blue-300); color: var(--blue-700); }
.contact-chip .chip-icon { font-size: 18px; }

/* ==================== MODAL ==================== */
.modal-overlay {
  position: fixed; inset: 0; background: rgba(0,0,0,0.4);
  display: flex; align-items: center; justify-content: center;
  z-index: 300; opacity: 0; pointer-events: none;
  transition: opacity 0.2s;
}
.modal-overlay.open { opacity: 1; pointer-events: all; }

.modal {
  background: var(--white); border-radius: 16px;
  box-shadow: var(--shadow-xl); padding: 32px;
  width: 100%; max-width: 480px; transform: scale(0.95);
  transition: transform 0.2s;
}
.modal-overlay.open .modal { transform: scale(1); }
.modal h3 { font-size: 18px; font-weight: 700; margin-bottom: 18px; }

/* ==================== RESPONSIVE ==================== */
@media (max-width: 1024px) {
  .stats-grid { grid-template-columns: repeat(2, 1fr); }
  .features-grid { grid-template-columns: repeat(2, 1fr); }
  .pricing-grid { grid-template-columns: 1fr; max-width: 400px; }
}

@media (max-width: 768px) {
  .sidebar { transform: translateX(-100%); transition: transform 0.3s; }
  .sidebar.mobile-open { transform: translateX(0); }
  .main-area { margin-left: 0; }
  .landing-nav { padding: 14px 20px; }
  .hero { padding: 50px 20px; }
  .hero h1 { font-size: 32px; }
  .features, .pricing, .contact-section { padding: 50px 20px; }
  .features-grid { grid-template-columns: 1fr; }
  .stats-grid { grid-template-columns: 1fr 1fr; }
  .content { padding: 20px 16px; }
  .topbar { padding: 12px 16px; }
}

@media (max-width: 480px) {
  .stats-grid { grid-template-columns: 1fr; }
  .hero h1 { font-size: 26px; }
  .hero-actions { flex-direction: column; }
  .contact-cards { flex-direction: column; }
}

/* ==================== ANIMATIONS ==================== */
@keyframes fadeInUp {
  from { opacity: 0; transform: translateY(24px); }
  to { opacity: 1; transform: translateY(0); }
}

@keyframes pulse {
  0%, 100% { opacity: 1; }
  50% { opacity: 0.6; }
}

@keyframes slideIn {
  from { transform: translateX(-20px); opacity: 0; }
  to { transform: translateX(0); opacity: 1; }
}

.anim-in { animation: fadeInUp 0.7s cubic-bezier(0.16,1,0.3,1) both; }
.anim-d1 { animation-delay: 0.09s; }
.anim-d2 { animation-delay: 0.18s; }
.anim-d3 { animation-delay: 0.27s; }
.anim-d4 { animation-delay: 0.36s; }

.pulse { animation: pulse 2s ease-in-out infinite; }

.mobile-menu-btn {
  display: none; background: none; border: none; font-size: 24px;
  cursor: pointer; color: var(--gray-700);
}
@media (max-width: 768px) {
  .mobile-menu-btn { display: block; }
}

/* Admin user list */
.user-row { 
  display: flex; align-items: center; gap: 12px; padding: 12px 0; 
  border-bottom: 1px solid var(--gray-100); 
  transition: background 0.2s;
}
.user-row:hover { background: var(--gray-50); }
.user-row:last-child { border-bottom: none; }

/* Professional enhancements */
.glass {
  background: rgba(255, 255, 255, 0.7);
  backdrop-filter: blur(10px);
  border: 1px solid rgba(255, 255, 255, 0.3);
}

.shine {
  position: relative;
  overflow: hidden;
}
.shine::before {
  content: '';
  position: absolute;
  top: 0;
  left: -100%;
  width: 100%;
  height: 100%;
  background: linear-gradient(90deg, transparent, rgba(255,255,255,0.3), transparent);
  transition: left 0.5s;
}
.shine:hover::before {
  left: 100%;
}

/* Verification badges */
.verify-badge {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  padding: 6px 12px;
  border-radius: 20px;
  font-size: 12px;
  font-weight: 700;
}
.verify-pending { background: #fef3c7; color: #92400e; }
.verify-passed { background: #dcfce7; color: #166534; }
.verify-failed { background: #fee2e2; color: #991b1b; }

/* Dashboard 2-column grid */
.dashboard-grid {
  display: grid;
  grid-template-columns: 1.5fr 1fr;
  gap: 18px;
  margin-bottom: 24px;
}

@media (max-width: 900px) {
  .dashboard-grid { grid-template-columns: 1fr; }
}

/* Online pill */
.online-pill {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  background: var(--green-50, #f0fdf4);
  color: var(--green-600);
  padding: 4px 12px;
  border-radius: 20px;
  font-size: 12px;
  font-weight: 700;
  border: 1px solid #bbf7d0;
}
.online-pill::before {
  content: '';
  width: 8px;
  height: 8px;
  border-radius: 50%;
  background: var(--green-500);
  animation: pulse 2s ease-in-out infinite;
}
.online-pill.empty {
  background: #f1f5f9;
  color: var(--gray-500);
  border-color: var(--gray-200);
}
.online-pill.empty::before {
  background: var(--gray-400);
  animation: none;
}

/* Checker item */
.checker-item {
  display: flex;
  align-items: center;
  gap: 12px;
  padding: 12px 14px;
  border-radius: 10px;
  background: var(--gray-50);
  margin-bottom: 8px;
  transition: all 0.2s;
  border: 1px solid var(--gray-100);
}
.checker-item:hover {
  background: var(--blue-50);
  border-color: var(--blue-200);
}
.checker-item:last-child { margin-bottom: 0; }

.checker-status-dot {
  width: 10px;
  height: 10px;
  border-radius: 50%;
  background: var(--green-500);
  box-shadow: 0 0 0 3px rgba(34, 197, 94, 0.2);
  animation: pulse 2s ease-in-out infinite;
}
.checker-status-dot.busy {
  background: var(--amber-500);
  box-shadow: 0 0 0 3px rgba(245, 158, 11, 0.2);
}

.empty-state {
  text-align: center;
  padding: 32px 16px;
  color: var(--gray-400);
}
.empty-state .empty-icon {
  font-size: 36px;
  margin-bottom: 8px;
  opacity: 0.5;
}

/* Premium panel */
.panel-primary {
  border: 1px solid var(--blue-200);
  box-shadow: 0 4px 20px rgba(37, 99, 235, 0.08);
}
</style>
</head>
<body>

<!-- ==================== SVG LOGO (reusable) ==================== -->
<svg style="display:none">
  <symbol id="logo-icon" viewBox="0 0 40 40">
    <defs>
      <linearGradient id="logoGrad" x1="0" y1="0" x2="40" y2="40" gradientUnits="userSpaceOnUse">
        <stop offset="0" stop-color="#4f46e5"/>
        <stop offset="1" stop-color="#0d9488"/>
      </linearGradient>
    </defs>
    <rect width="40" height="40" rx="11" fill="url(#logoGrad)"/>
    <path d="M20 5 L31 9 V19 C31 26 26 31 20 34 C14 31 9 26 9 19 V9 Z" fill="rgba(255,255,255,0.14)" stroke="rgba(255,255,255,0.5)" stroke-width="1.2"/>
    <path d="M14 20 L18 24 L26 15" stroke="white" stroke-width="2.6" stroke-linecap="round" stroke-linejoin="round" fill="none"/>
  </symbol>
</svg>

<!-- ==================== LANDING PAGE ==================== -->
<div id="page-landing" class="landing-page">
  <nav class="landing-nav">
    <div class="logo-group">
      <svg class="logo-svg"><use href="#logo-icon"/></svg>
      <span class="logo-text">CheckPlag</span>
    </div>
    <div class="nav-actions">
      <button class="lang-toggle" onclick="toggleLang()" id="lang-btn">中文</button>
      <button class="btn btn-outline" onclick="showPage('login')" data-i18n="login">Login</button>
      <button class="btn btn-primary" onclick="showPage('register')" data-i18n="getStarted">Get Started</button>
    </div>
  </nav>

  <section class="hero">
    <div class="hero-content">
      <div class="hero-badge anim-in" data-i18n="heroBadge">⚡ Pure Turnitin Reports — Delivered in 20 Minutes</div>
      <h1 class="anim-in anim-d1" data-i18n="heroTitle">Plagiarism & AI Reports<br>You Can <em>Trust</em></h1>
      <p class="anim-in anim-d2" data-i18n="heroDesc">Get pure Turnitin plagiarism and AI detection reports for your documents. Upload, use a credit, and receive both reports within 20 minutes. Simple, fast, and affordable.</p>
      <div class="hero-actions anim-in anim-d3">
        <button class="btn btn-lg btn-white" onclick="showPage('register')" data-i18n="startNow">Start Now — It's Easy</button>
        <button class="btn btn-lg btn-outline-white" onclick="document.querySelector('.features').scrollIntoView({behavior:'smooth'})" data-i18n="learnMore">Learn More</button>
      </div>
      <div class="hero-trust anim-in anim-d4">
        <span>🔒 100% Confidential</span>
        <span>⚡ 20-Minute Delivery</span>
        <span>🛡️ Your Privacy Protected</span>
      </div>
    </div>
  </section>

  <section class="features">
    <span class="section-eyebrow">How It Works</span>
    <h2 data-i18n="howItWorks">Reports in Three Simple Steps</h2>
    <p data-i18n="howItWorksDesc">From upload to download, the entire process takes under 20 minutes.</p>
    <div class="features-grid">
      <div class="feature-card anim-in anim-d1">
        <div class="feature-icon">📤</div>
        <h3 data-i18n="feat1Title">Upload Document</h3>
        <p data-i18n="feat1Desc">Upload any file type — Word, PDF, or any other format. We accept everything.</p>
      </div>
      <div class="feature-card anim-in anim-d2">
        <div class="feature-icon">⏱️</div>
        <h3 data-i18n="feat2Title">20-Minute Delivery</h3>
        <p data-i18n="feat2Desc">Our team generates pure Turnitin plagiarism and AI detection reports and delivers them within 20 minutes.</p>
      </div>
      <div class="feature-card anim-in anim-d3">
        <div class="feature-icon">📊</div>
        <h3 data-i18n="feat3Title">Download Reports</h3>
        <p data-i18n="feat3Desc">Get your plagiarism report and AI detection report separately. Download both instantly from your dashboard.</p>
      </div>
    </div>
  </section>

  <section class="pricing">
    <span class="section-eyebrow">Pricing</span>
    <h2 data-i18n="pricingTitle">Simple Credit Packages</h2>
    <p data-i18n="pricingDesc">One credit equals one report. Contact us to purchase — no online payment required.</p>
    <div class="pricing-grid">
      <div class="price-card">
        <h3>Starter</h3>
        <div class="price-credits" data-i18n="credit1">1 Credit</div>
        <div class="price-amount">$1</div>
        <button class="btn btn-outline btn-full" onclick="document.querySelector('.contact-section').scrollIntoView({behavior:'smooth'})" data-i18n="contactBuy">Contact to Buy</button>
      </div>
      <div class="price-card featured">
        <h3>Popular</h3>
        <div class="price-credits" data-i18n="credit10">10 Credits</div>
        <div class="price-amount">$9</div>
        <button class="btn btn-primary btn-full" onclick="document.querySelector('.contact-section').scrollIntoView({behavior:'smooth'})" data-i18n="contactBuy">Contact to Buy</button>
      </div>
      <div class="price-card">
        <h3>Pro</h3>
        <div class="price-credits" data-i18n="credit20">20 Credits</div>
        <div class="price-amount">$16</div>
        <button class="btn btn-outline btn-full" onclick="document.querySelector('.contact-section').scrollIntoView({behavior:'smooth'})" data-i18n="contactBuy">Contact to Buy</button>
      </div>
    </div>
  </section>

  <section class="privacy-banner">
    <div class="privacy-content">
      <div class="privacy-icon">🔒</div>
      <h2>Your Privacy Is Our First Priority</h2>
      <p>Your documents are completely confidential. We never share, sell, publish, or store your work beyond what's needed to generate your report. Only the assigned checker accesses your file — and it stays private, always.</p>
      <div class="privacy-points">
        <div class="privacy-point"><span>🛡️</span> 100% Confidential</div>
        <div class="privacy-point"><span>🔐</span> Secure Handling</div>
        <div class="privacy-point"><span>🚫</span> Never Shared or Sold</div>
      </div>
    </div>
  </section>

  <section class="faq-section">
    <span class="section-eyebrow">FAQ</span>
    <h2>Frequently Asked Questions</h2>
    <p>Everything you need to know before getting started.</p>
    <div class="faq-list">
      <div class="faq-item" onclick="this.classList.toggle('open')">
        <div class="faq-q">How long does it take to get my report? <span class="faq-arrow">⌄</span></div>
        <div class="faq-a">Once a checker accepts your order, your plagiarism and AI detection reports are delivered within 20 minutes. Most orders are completed even faster.</div>
      </div>
      <div class="faq-item" onclick="this.classList.toggle('open')">
        <div class="faq-q">How do I pay for credits? <span class="faq-arrow">⌄</span></div>
        <div class="faq-a">Contact us via WhatsApp or Discord to purchase credits. Once payment is confirmed, we add credits to your account instantly. 1 credit = 1 report.</div>
      </div>
      <div class="faq-item" onclick="this.classList.toggle('open')">
        <div class="faq-q">Is my document private and secure? <span class="faq-arrow">⌄</span></div>
        <div class="faq-a">Yes. Your documents are only accessed by the assigned checker to generate your report. We do not share, sell, or publish your work.</div>
      </div>
      <div class="faq-item" onclick="this.classList.toggle('open')">
        <div class="faq-q">What file types can I upload? <span class="faq-arrow">⌄</span></div>
        <div class="faq-a">Any file type is accepted — Word documents, PDFs, text files, and more. Just upload and place your order.</div>
      </div>
      <div class="faq-item" onclick="this.classList.toggle('open')">
        <div class="faq-q">What if I'm not satisfied with my report? <span class="faq-arrow">⌄</span></div>
        <div class="faq-a">You have 24 hours after delivery to report a problem. Our admin reviews every complaint and, if valid, refunds your credit.</div>
      </div>
      <div class="faq-item" onclick="this.classList.toggle('open')">
        <div class="faq-q">Are these genuine Turnitin reports? <span class="faq-arrow">⌄</span></div>
        <div class="faq-a">Yes — we provide pure, authentic Turnitin plagiarism and AI detection reports generated through official institutional access.</div>
      </div>
    </div>
  </section>

  <section class="contact-section">
    <span class="section-eyebrow">Get Started</span>
    <h2 data-i18n="contactTitle">Buy Credits — Contact Us</h2>
    <p data-i18n="contactDesc">Reach out via WhatsApp or Discord to purchase credits. We'll add them to your account instantly.</p>
    <div class="contact-cards">
      <div class="contact-card">
        <div class="contact-card-icon">💬</div>
        <h4>WhatsApp</h4>
        <p class="contact-name">CheckPlag Support</p>
        <p class="contact-number">+92 313 1521781</p>
        <a href="https://wa.me/923131521781" target="_blank" class="btn btn-primary btn-sm btn-full" data-i18n="openWhatsApp">Open WhatsApp</a>
      </div>
      <div class="contact-card">
        <div class="contact-card-icon">🎮</div>
        <h4>Discord</h4>
        <p class="contact-name">humayunsaleem_27113</p>
        <p class="contact-number">discord.gg/Esa7by49</p>
        <a href="https://discord.gg/Esa7by49" target="_blank" class="btn btn-primary btn-sm btn-full" data-i18n="joinDiscord">Join Discord</a>
      </div>
    </div>
  </section>

  <footer class="landing-footer">
    <p style="margin-bottom:10px"><a onclick="showPage('terms')" style="color:rgba(255,255,255,0.7);cursor:pointer;text-decoration:underline;margin:0 10px">Terms of Service</a> · <a onclick="document.querySelector('.faq-section').scrollIntoView({behavior:'smooth'})" style="color:rgba(255,255,255,0.7);cursor:pointer;text-decoration:underline;margin:0 10px">FAQ</a></p>
    <p>© 2026 CheckPlag. All rights reserved.</p>
  </footer>
</div>

<!-- ==================== TERMS OF SERVICE PAGE ==================== -->
<div id="page-terms" class="hidden" style="min-height:100vh;background:var(--gray-50)">
  <nav class="landing-nav">
    <div class="logo-group" onclick="showPage('landing')" style="cursor:pointer">
      <svg class="logo-svg"><use href="#logo-icon"/></svg>
      <span class="logo-text">CheckPlag</span>
    </div>
    <button class="btn btn-outline" onclick="showPage('landing')">← Back to Home</button>
  </nav>
  <div style="max-width:760px;margin:0 auto;padding:60px 40px">
    <h1 style="font-size:40px;color:var(--ink);margin-bottom:8px">Terms of Service</h1>
    <p style="color:var(--gray-500);margin-bottom:40px">Last updated: 2026</p>

    <div class="terms-block">
      <h3>1. Service Description</h3>
      <p>CheckPlag provides plagiarism and AI-detection report generation services. Users purchase credits and submit documents to receive reports, typically delivered within 20 minutes of a checker accepting the order.</p>
    </div>
    <div class="terms-block">
      <h3>2. Credits & Payments</h3>
      <p>Credits are purchased by contacting us via WhatsApp or Discord. One credit equals one report. Credits are added manually after payment confirmation. Credits have no cash value and are non-transferable.</p>
    </div>
    <div class="terms-block">
      <h3>3. Refund Policy</h3>
      <p>If you are unsatisfied with a report, you may report a problem within 24 hours of delivery. Our team reviews each case and, if the complaint is valid, refunds the credit. After 24 hours, orders are automatically considered accepted and no refund is issued. Cancelled pending orders are refunded in full.</p>
    </div>
    <div class="terms-block">
      <h3>4. Document Privacy</h3>
      <p>Documents you upload are used solely to generate your requested reports. We do not sell, share, or publish your documents. Only the assigned checker and admin can access your files.</p>
    </div>
    <div class="terms-block">
      <h3>5. Acceptable Use</h3>
      <p>You agree not to misuse the service or upload unlawful content. CheckPlag reserves the right to refuse service or suspend accounts that violate these terms.</p>
    </div>
    <div class="terms-block">
      <h3>6. Limitation of Liability</h3>
      <p>Reports are provided for informational and reference purposes. CheckPlag is not responsible for academic or institutional decisions made based on our reports.</p>
    </div>
    <div class="terms-block">
      <h3>7. Contact</h3>
      <p>For any questions about these terms, contact us via WhatsApp at +92 313 1521781 or Discord (humayunsaleem_27113).</p>
    </div>
  </div>
  <footer class="landing-footer">
    <p>© 2026 CheckPlag. All rights reserved.</p>
  </footer>
</div>

<!-- ==================== LOGIN PAGE ==================== -->
<div id="page-login" class="auth-page hidden">
  <div class="auth-card">
    <div class="logo-group">
      <svg class="logo-svg"><use href="#logo-icon"/></svg>
      <span class="logo-text">CheckPlag</span>
    </div>
    <h2 data-i18n="loginTitle">Welcome Back</h2>
    <p class="auth-sub" data-i18n="loginSub">Sign in to your account</p>
    <div class="form-group">
      <label data-i18n="usernameLabel">Username</label>
      <input type="text" class="form-input" id="login-email" placeholder="Your username">
    </div>
    <div class="form-group">
      <label data-i18n="passLabel">Password</label>
      <input type="password" class="form-input" id="login-pass" placeholder="••••••••">
    </div>
    <button class="btn btn-primary btn-full" onclick="handleLogin()" data-i18n="loginBtn" style="margin-top:8px">Sign In</button>
    <div id="login-error" style="margin-top:12px;padding:12px 16px;border-radius:8px;font-size:14px;font-weight:600;display:none;border:2px solid"></div>
    <p class="auth-footer" style="margin-top:14px"><a onclick="showForgotPassword()">Forgot password?</a></p>
    <p class="auth-footer" data-i18n="noAccount">Don't have an account? <a onclick="showPage('register')">Sign Up</a></p>
    <p class="auth-footer" style="margin-top:10px"><a onclick="showPage('landing')">← Back to home</a></p>
  </div>
</div>

<!-- ==================== REGISTER PAGE ==================== -->
<div id="page-register" class="auth-page hidden">
  <div class="auth-card">
    <div class="logo-group">
      <svg class="logo-svg"><use href="#logo-icon"/></svg>
      <span class="logo-text">CheckPlag</span>
    </div>
    <h2 data-i18n="regTitle">Create Account</h2>
    <p class="auth-sub" data-i18n="regSub">Join CheckPlag today</p>
    <div class="form-group">
      <label data-i18n="nameLabel">Full Name</label>
      <input type="text" class="form-input" id="reg-name" placeholder="Your name">
    </div>
    <div class="form-group">
      <label data-i18n="usernameLabel">Username</label>
      <input type="text" class="form-input" id="reg-email" placeholder="Choose a username">
    </div>
    <div class="form-group">
      <label data-i18n="passLabel">Password</label>
      <input type="password" class="form-input" id="reg-pass" placeholder="••••••••">
    </div>
    <button class="btn btn-primary btn-full" onclick="handleRegister()" data-i18n="regBtn" style="margin-top:8px">Create Account</button>
    <div id="reg-error" style="margin-top:12px;padding:12px 16px;border-radius:8px;font-size:14px;font-weight:600;display:none;border:2px solid"></div>
    <div style="margin-top:16px;padding:10px 14px;background:var(--green-50);border:1px solid #bbf7d0;border-radius:8px;display:flex;align-items:center;gap:8px">
      <span style="font-size:16px">🔒</span>
      <span style="font-size:12px;color:var(--green-600);font-weight:600">Your information and documents are kept 100% private and secure.</span>
    </div>
    <p class="auth-footer" data-i18n="hasAccount" style="margin-top:16px">Already have an account? <a onclick="showPage('login')">Sign In</a></p>
    <p class="auth-footer" style="margin-top:10px"><a onclick="showPage('landing')">← Back to home</a></p>
  </div>
</div>

<!-- ==================== NOTIFICATION OVERLAY ==================== -->
<div class="overlay" id="notif-overlay" onclick="toggleNotifs()"></div>
<div class="notif-panel" id="notif-panel">
  <div class="notif-panel-header">
    <h3 data-i18n="notifications">🔔 Notifications</h3>
    <button class="btn btn-ghost btn-sm" onclick="toggleNotifs()">✕</button>
  </div>
  <div class="notif-list" id="notif-list"></div>
</div>

<!-- ==================== CLIENT DASHBOARD ==================== -->
<div id="page-client" class="hidden">
  <div class="app-layout">
    <aside class="sidebar" id="sidebar-client">
      <div class="sidebar-header">
        <svg class="logo-svg" style="width:30px;height:30px"><use href="#logo-icon"/></svg>
        <span class="logo-text" style="font-size:18px">CheckPlag</span>
      </div>
      <nav class="sidebar-nav">
        <div class="nav-item active" data-tab="client-dashboard" onclick="switchTab(this,'client')"><span class="nav-icon">📊</span> Dashboard</div>
        <div class="nav-item" data-tab="client-orders" onclick="switchTab(this,'client')"><span class="nav-icon">📋</span> My Orders</div>
        <div class="nav-item" data-tab="client-chat" onclick="switchTab(this,'client')"><span class="nav-icon">💬</span> Talk to Admin <span id="client-chat-badge" style="display:none;background:var(--red-500);color:white;border-radius:50%;width:18px;height:18px;font-size:10px;font-weight:700;align-items:center;justify-content:center;margin-left:auto">0</span></div>
        <div class="nav-item" data-tab="client-credits" onclick="switchTab(this,'client')"><span class="nav-icon">💳</span> Buy Credits</div>
      </nav>
      <div class="sidebar-footer">
        <div class="user-pill">
          <div class="user-avatar" id="client-avatar">U</div>
          <div class="user-info">
            <div class="user-name" id="client-name">User</div>
            <div class="user-role">Client</div>
          </div>
        </div>
        <button class="btn btn-ghost btn-sm btn-full" style="margin-top:8px" onclick="handleLogout()">Logout</button>
      </div>
    </aside>

    <div class="main-area">
      <div class="topbar">
        <div class="topbar-left">
          <button class="mobile-menu-btn" onclick="document.getElementById('sidebar-client').classList.toggle('mobile-open')">☰</button>
          <h2 id="client-topbar-title" data-i18n="dashboard">Dashboard</h2>
        </div>
        <div class="topbar-right">
          <button class="lang-toggle" onclick="toggleLang()" id="lang-btn-client">中文</button>
          <button id="sound-toggle-client" onclick="toggleSound()" title="Mute/Unmute notification sound" style="background:var(--gray-100);border:1px solid var(--gray-200);width:38px;height:38px;border-radius:11px;font-size:16px;cursor:pointer;transition:all 0.2s">🔊</button>
          <button class="notif-btn" onclick="toggleNotifs()">🔔 <span class="notif-badge" id="client-notif-count">0</span></button>
        </div>
      </div>

      <div class="content">
        <!-- Client Dashboard Tab -->
        <div id="client-dashboard" class="tab-content">
          <div class="stats-grid">
            <div class="stat-card blue anim-in anim-d1">
              <div class="stat-label" data-i18n="totalOrders">Total Orders</div>
              <div class="stat-value" id="c-stat-total">0</div>
            </div>
            <div class="stat-card amber anim-in anim-d2">
              <div class="stat-label" data-i18n="processing">Processing</div>
              <div class="stat-value" id="c-stat-proc">0</div>
            </div>
            <div class="stat-card green anim-in anim-d3">
              <div class="stat-label" data-i18n="completed">Completed</div>
              <div class="stat-value" id="c-stat-done">0</div>
            </div>
            <div class="stat-card red anim-in anim-d4">
              <div class="stat-label" data-i18n="credits">Credits</div>
              <div class="stat-value" id="c-stat-credits">0</div>
            </div>
          </div>

          <!-- Two-column section: New Order + Online Checkers -->
          <div class="dashboard-grid">
            <!-- New Order Panel -->
            <div class="panel panel-primary anim-in">
              <div class="panel-header" style="background:linear-gradient(135deg, var(--blue-600), var(--blue-700));color:white;border-bottom:none">
                <h3 style="color:white">📤 Place New Order</h3>
                <span style="font-size:12px;opacity:0.9">Upload & submit instantly</span>
              </div>
              <div class="panel-body">
                <div class="upload-zone" id="upload-zone" onclick="document.getElementById('file-input').click()"
                  ondragover="event.preventDefault();this.classList.add('dragover')"
                  ondragleave="this.classList.remove('dragover')"
                  ondrop="event.preventDefault();this.classList.remove('dragover');handleFileDrop(event)">
                  <div class="upload-icon">📁</div>
                  <h4 data-i18n="dropFile">Click or drag a file here</h4>
                  <p data-i18n="anyFile">Any file type accepted · 1 credit per report</p>
                  <input type="file" id="file-input" style="display:none" onchange="handleFileSelect(event)">
                </div>
                <div id="file-info" class="hidden">
                  <div class="file-selected">
                    <span>📄</span>
                    <span class="file-name" id="selected-file-name"></span>
                    <button class="btn btn-ghost btn-sm" onclick="clearFile()">✕</button>
                  </div>
                </div>
                <div class="form-group" style="margin-top:14px">
                  <label style="font-size:13px;font-weight:600;color:var(--gray-700)">💬 Message to Checker <span style="color:var(--gray-400);font-weight:400">(optional)</span></label>
                  <textarea class="form-input" id="order-message" rows="2" placeholder="Any special instructions for the checker? e.g., 'Please check carefully, this is for my thesis submission'" style="resize:vertical;margin-top:4px"></textarea>
                </div>
                <div style="margin-top:14px;display:flex;justify-content:space-between;align-items:center;gap:10px;flex-wrap:wrap">
                  <span style="font-size:13px;color:var(--gray-500)">⏱️ Reports ready in 20 min</span>
                  <button class="btn btn-primary" id="place-order-btn" onclick="placeOrder()" data-i18n="placeOrder">Place Order (1 Credit)</button>
                </div>
                <div style="margin-top:14px;padding:12px 14px;background:var(--green-50);border:1px solid #bbf7d0;border-radius:10px;display:flex;align-items:center;gap:10px">
                  <span style="font-size:20px">🔒</span>
                  <span style="font-size:12.5px;color:var(--green-600);font-weight:600;line-height:1.5">Your document is 100% confidential. It's only seen by your assigned checker and is never shared, sold, or published.</span>
                </div>
              </div>
            </div>

            <!-- Online Checkers Panel -->
            <div class="panel anim-in anim-d1">
              <div class="panel-header">
                <h3>👥 Available Checkers</h3>
                <span class="online-pill" id="online-count-pill">0 online</span>
              </div>
              <div class="panel-body" id="online-checkers-list">
                <!-- Filled by JS -->
              </div>
            </div>
          </div>

          <div class="panel anim-in anim-d2">
            <div class="panel-header"><h3 data-i18n="recentOrders">Recent Orders</h3></div>
            <div class="table-wrap">
              <table><thead><tr>
                <th>ID</th><th data-i18n="file">File</th><th data-i18n="status">Status</th><th data-i18n="timer">Timer</th><th data-i18n="action">Action</th>
              </tr></thead><tbody id="client-orders-table"></tbody></table>
            </div>
          </div>
        </div>

        <!-- Client Orders Tab -->
        <div id="client-orders" class="tab-content hidden">
          <div class="panel">
            <div class="panel-header"><h3 data-i18n="allOrders">All Orders</h3></div>
            <div class="table-wrap">
              <table><thead><tr>
                <th>ID</th><th data-i18n="file">File</th><th data-i18n="status">Status</th><th data-i18n="timer">Timer</th><th data-i18n="action">Action</th>
              </tr></thead><tbody id="client-all-orders-table"></tbody></table>
            </div>
          </div>
        </div>

        <!-- Client Talk to Admin Tab -->
        <div id="client-chat" class="tab-content hidden">
          <div class="panel">
            <div class="panel-header">
              <h3>💬 Talk to Admin</h3>
              <span style="font-size:12px;color:var(--gray-500)">Send messages directly to admin</span>
            </div>
            <div class="panel-body">
              <p style="font-size:14px;color:var(--gray-600);margin-bottom:18px;line-height:1.6">Have a question, concern, or need help? Send a message and admin will respond as soon as possible. You'll see admin's reply in your notifications.</p>
              
              <div class="form-group">
                <label style="font-weight:700">Subject</label>
                <input type="text" class="form-input" id="chat-subject" placeholder="Brief subject (e.g., Payment Issue, Order Question)">
              </div>
              
              <div class="form-group">
                <label style="font-weight:700">Your Message</label>
                <textarea class="form-input" id="chat-message" rows="5" placeholder="Type your message to admin here..." style="resize:vertical"></textarea>
              </div>
              
              <button class="btn btn-primary" onclick="sendChatToAdmin()">📨 Send Message to Admin</button>
            </div>
          </div>

          <div class="panel">
            <div class="panel-header"><h3>📨 Conversation History</h3></div>
            <div class="panel-body" id="client-chat-history">
              <!-- Filled by JS -->
            </div>
          </div>
        </div>

        <!-- Client Buy Credits Tab -->
        <div id="client-credits" class="tab-content hidden">
          <div class="panel">
            <div class="panel-header"><h3 data-i18n="buyCredits">Buy Credits</h3></div>
            <div class="panel-body">
              <p style="color:var(--gray-600);margin-bottom:20px;line-height:1.7" data-i18n="buyCreditsDesc">To purchase credits, contact us via WhatsApp or Discord. We'll add credits to your account after payment.</p>
              <div class="contact-inline">
                <a href="https://wa.me/923131521781" target="_blank" class="contact-chip">
                  <span class="chip-icon">💬</span>
                  <div><strong>WhatsApp</strong><br><span style="font-size:12px;color:var(--gray-500)">CheckPlag Support · +92 313 1521781</span></div>
                </a>
                <a href="https://discord.gg/Esa7by49" target="_blank" class="contact-chip">
                  <span class="chip-icon">🎮</span>
                  <div><strong>Discord</strong><br><span style="font-size:12px;color:var(--gray-500)">humayunsaleem_27113 · discord.gg/Esa7by49</span></div>
                </a>
              </div>
            </div>
          </div>
          <div class="panel">
            <div class="panel-header"><h3 data-i18n="pricingTitle">Pricing</h3></div>
            <div class="panel-body">
              <div class="pricing-grid" style="max-width:100%">
                <div class="price-card" style="background:white;border:1px solid var(--gray-200);color:var(--ink)"><h3 style="color:var(--ink)">Starter</h3><div class="price-credits" style="color:var(--gray-500)">1 Credit</div><div class="price-amount" style="color:var(--blue-700)">$1</div></div>
                <div class="price-card featured" style="background:linear-gradient(135deg,var(--blue-50),var(--blue-100));border:2px solid var(--blue-400);color:var(--ink)"><h3 style="color:var(--ink)">Popular</h3><div class="price-credits" style="color:var(--gray-500)">10 Credits</div><div class="price-amount" style="color:var(--blue-700)">$9</div></div>
                <div class="price-card" style="background:white;border:1px solid var(--gray-200);color:var(--ink)"><h3 style="color:var(--ink)">Pro</h3><div class="price-credits" style="color:var(--gray-500)">20 Credits</div><div class="price-amount" style="color:var(--blue-700)">$16</div></div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- ==================== CHECKER DASHBOARD ==================== -->
<div id="page-checker" class="hidden">
  <div class="app-layout">
    <aside class="sidebar" id="sidebar-checker">
      <div class="sidebar-header">
        <svg class="logo-svg" style="width:30px;height:30px"><use href="#logo-icon"/></svg>
        <span class="logo-text" style="font-size:18px">CheckPlag</span>
      </div>
      <nav class="sidebar-nav">
        <div class="nav-item active" data-tab="checker-active" onclick="switchTab(this,'checker')"><span class="nav-icon">📥</span> Active Orders</div>
        <div class="nav-item" data-tab="checker-history" onclick="switchTab(this,'checker')"><span class="nav-icon">✅</span> Completed</div>
        <div class="nav-item" data-tab="checker-performance" onclick="switchTab(this,'checker')"><span class="nav-icon">📈</span> Performance</div>
        <div class="nav-item" data-tab="checker-chat" onclick="switchTab(this,'checker')"><span class="nav-icon">💬</span> Talk to Admin <span id="checker-chat-badge" style="display:none;background:var(--red-500);color:white;border-radius:50%;width:18px;height:18px;font-size:10px;font-weight:700;align-items:center;justify-content:center;margin-left:auto">0</span></div>
      </nav>
      <div class="sidebar-footer">
        <div class="user-pill">
          <div class="user-avatar" id="checker-avatar">C</div>
          <div class="user-info">
            <div class="user-name" id="checker-name">Checker</div>
            <div class="user-role">Checker</div>
          </div>
        </div>
        <div style="margin-top:10px;padding:8px 10px;background:var(--blue-50);border-radius:8px;font-size:13px;text-align:center">
          <span style="color:var(--gray-500)" data-i18n="myReports">My Reports:</span>
          <strong id="checker-count" style="color:var(--blue-700);font-size:18px;margin-left:4px">0</strong>
        </div>
        <button class="btn btn-ghost btn-sm btn-full" style="margin-top:8px" onclick="handleLogout()">Logout</button>
      </div>
    </aside>

    <div class="main-area">
      <div class="topbar">
        <div class="topbar-left">
          <button class="mobile-menu-btn" onclick="document.getElementById('sidebar-checker').classList.toggle('mobile-open')">☰</button>
          <h2 data-i18n="checkerDash">Checker Dashboard</h2>
        </div>
        <div class="topbar-right">
          <button id="checker-online-toggle" onclick="toggleCheckerOnline()" style="display:flex;align-items:center;gap:8px;background:var(--green-50);border:1px solid #bbf7d0;color:var(--green-600);padding:8px 14px;border-radius:100px;font-size:13px;font-weight:700;cursor:pointer;font-family:'Plus Jakarta Sans',sans-serif;transition:all 0.2s">
            <span id="online-dot" style="width:9px;height:9px;border-radius:50%;background:var(--green-500)"></span>
            <span id="online-label">Online</span>
          </button>
          <button class="lang-toggle" onclick="toggleLang()">中文</button>
          <button id="sound-toggle-checker" onclick="toggleSound()" title="Mute/Unmute notification sound" style="background:var(--gray-100);border:1px solid var(--gray-200);width:38px;height:38px;border-radius:11px;font-size:16px;cursor:pointer;transition:all 0.2s">🔊</button>
          <button class="notif-btn" onclick="toggleNotifs()">🔔 <span class="notif-badge" id="checker-notif-count">0</span></button>
        </div>
      </div>

      <div class="content">
        <div id="checker-active" class="tab-content">
          <div class="stats-grid" style="grid-template-columns: repeat(3,1fr)">
            <div class="stat-card amber anim-in">
              <div class="stat-label">My Active (Max 5)</div>
              <div class="stat-value" id="ck-stat-active">0</div>
            </div>
            <div class="stat-card green anim-in anim-d1">
              <div class="stat-label" data-i18n="myCompleted">Total Completed</div>
              <div class="stat-value" id="ck-stat-done">0</div>
            </div>
            <div class="stat-card blue anim-in anim-d2" style="background:linear-gradient(135deg,#eff6ff,#dbeafe);border-color:#bfdbfe">
              <div class="stat-label" style="color:var(--blue-600)">✅ Done Today</div>
              <div class="stat-value" id="ck-stat-today" style="color:var(--blue-700)">0</div>
            </div>
          </div>
          <div class="panel">
            <div class="panel-header"><h3>📥 Available & Active Orders</h3><span style="font-size:12px;color:var(--gray-500)">Accept pending orders · Max 5 active</span></div>
            <div class="table-wrap">
              <table><thead><tr>
                <th>ID</th><th data-i18n="client">Client</th><th data-i18n="file">File</th><th data-i18n="timer">Timer</th><th data-i18n="action">Action</th>
              </tr></thead><tbody id="checker-orders-table"></tbody></table>
            </div>
          </div>
        </div>

        <div id="checker-history" class="tab-content hidden">
          <div class="panel">
            <div class="panel-header"><h3 data-i18n="completedOrders">Completed Orders</h3></div>
            <div class="table-wrap">
              <table><thead><tr>
                <th>ID</th><th data-i18n="client">Client</th><th data-i18n="file">File</th><th data-i18n="completedAt">Completed At</th><th>Status</th><th>Action</th>
              </tr></thead><tbody id="checker-history-table"></tbody></table>
            </div>
          </div>
        </div>

        <!-- Checker Performance Tab -->
        <div id="checker-performance" class="tab-content hidden">
          <div class="panel">
            <div class="panel-header"><h3>📈 My Performance</h3></div>
            <div class="panel-body">
              <div class="stats-grid" style="grid-template-columns: repeat(4, 1fr)">
                <div class="stat-card blue"><div class="stat-label">Today</div><div class="stat-value" id="perf-today">0</div></div>
                <div class="stat-card amber"><div class="stat-label">Yesterday</div><div class="stat-value" id="perf-yesterday">0</div></div>
                <div class="stat-card green"><div class="stat-label">This Week</div><div class="stat-value" id="perf-week">0</div></div>
                <div class="stat-card red"><div class="stat-label">All Time</div><div class="stat-value" id="perf-alltime">0</div></div>
              </div>
            </div>
          </div>

          <div class="panel">
            <div class="panel-header"><h3>🏆 Verification Stats</h3></div>
            <div class="panel-body">
              <div class="stats-grid" style="grid-template-columns: repeat(3, 1fr)">
                <div class="stat-card green"><div class="stat-label">✅ Passed</div><div class="stat-value" id="perf-passed">0</div></div>
                <div class="stat-card amber"><div class="stat-label">⏳ Pending</div><div class="stat-value" id="perf-pending">0</div></div>
                <div class="stat-card red"><div class="stat-label">❌ Failed</div><div class="stat-value" id="perf-failed">0</div></div>
              </div>
            </div>
          </div>

          <div class="panel">
            <div class="panel-header"><h3>📅 Daily History (Last 7 Days)</h3></div>
            <div class="panel-body" id="perf-daily-history"></div>
          </div>
        </div>

        <!-- Checker Talk to Admin Tab -->
        <div id="checker-chat" class="tab-content hidden">
          <div class="panel">
            <div class="panel-header">
              <h3>💬 Talk to Admin</h3>
              <span style="font-size:12px;color:var(--gray-500)">Send messages directly to admin</span>
            </div>
            <div class="panel-body">
              <p style="font-size:14px;color:var(--gray-600);margin-bottom:18px;line-height:1.6">Have a question or need help? Send a message to admin. You'll see admin's reply in your notifications and below.</p>
              
              <div class="form-group">
                <label style="font-weight:700">Subject</label>
                <input type="text" class="form-input" id="checker-chat-subject" placeholder="Brief subject (e.g., Account Issue, Payment Question)">
              </div>
              
              <div class="form-group">
                <label style="font-weight:700">Your Message</label>
                <textarea class="form-input" id="checker-chat-message" rows="5" placeholder="Type your message to admin here..." style="resize:vertical"></textarea>
              </div>
              
              <button class="btn btn-primary" onclick="checkerSendChatToAdmin()">📨 Send Message to Admin</button>
            </div>
          </div>

          <div class="panel">
            <div class="panel-header"><h3>📨 Conversation History</h3></div>
            <div class="panel-body" id="checker-chat-history"></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- ==================== ADMIN DASHBOARD ==================== -->
<div id="page-admin" class="hidden">
  <div class="app-layout">
    <aside class="sidebar" id="sidebar-admin">
      <div class="sidebar-header">
        <svg class="logo-svg" style="width:30px;height:30px"><use href="#logo-icon"/></svg>
        <span class="logo-text" style="font-size:18px">CheckPlag</span>
      </div>
      <nav class="sidebar-nav">
        <div class="nav-item active" data-tab="admin-overview" onclick="switchTab(this,'admin')"><span class="nav-icon">📊</span> Overview</div>
        <div class="nav-item" data-tab="admin-orders" onclick="switchTab(this,'admin')"><span class="nav-icon">📋</span> All Orders</div>
        <div class="nav-item" data-tab="admin-problems" onclick="switchTab(this,'admin')"><span class="nav-icon">⚠️</span> Problem Reports</div>
        <div class="nav-item" data-tab="admin-messages" onclick="switchTab(this,'admin')"><span class="nav-icon">💬</span> Messages <span id="admin-chat-badge" style="display:none;background:var(--red-500);color:white;border-radius:50%;width:18px;height:18px;font-size:10px;font-weight:700;align-items:center;justify-content:center;margin-left:auto">0</span></div>
        <div class="nav-item" data-tab="admin-users" onclick="switchTab(this,'admin')"><span class="nav-icon">👥</span> Users</div>
        <div class="nav-item" data-tab="admin-checkers" onclick="switchTab(this,'admin')"><span class="nav-icon">🛡️</span> Checkers</div>
        <div class="nav-item" data-tab="admin-credits" onclick="switchTab(this,'admin')"><span class="nav-icon">💳</span> Manage Credits</div>
      </nav>
      <div class="sidebar-footer">
        <div class="user-pill">
          <div class="user-avatar" style="background:#fee2e2;color:#dc2626">A</div>
          <div class="user-info">
            <div class="user-name">Admin</div>
            <div class="user-role">Administrator</div>
          </div>
        </div>
        <button class="btn btn-ghost btn-sm btn-full" style="margin-top:8px" onclick="handleLogout()">Logout</button>
      </div>
    </aside>

    <div class="main-area">
      <div class="topbar">
        <div class="topbar-left">
          <button class="mobile-menu-btn" onclick="document.getElementById('sidebar-admin').classList.toggle('mobile-open')">☰</button>
          <h2 data-i18n="adminPanel">Admin Panel</h2>
        </div>
        <div class="topbar-right">
          <button class="lang-toggle" onclick="toggleLang()">中文</button>
          <button id="sound-toggle-admin" onclick="toggleSound()" title="Mute/Unmute notification sound" style="background:var(--gray-100);border:1px solid var(--gray-200);width:38px;height:38px;border-radius:11px;font-size:16px;cursor:pointer;transition:all 0.2s">🔊</button>
          <button class="notif-btn" onclick="toggleNotifs()">🔔 <span class="notif-badge" id="admin-notif-count">0</span></button>
        </div>
      </div>

      <div class="content">
        <!-- Admin Overview -->
        <div id="admin-overview" class="tab-content">
          <div class="stats-grid">
            <div class="stat-card blue anim-in"><div class="stat-label">Total Users</div><div class="stat-value" id="a-stat-users">0</div></div>
            <div class="stat-card green anim-in anim-d1"><div class="stat-label">Total Orders</div><div class="stat-value" id="a-stat-orders">0</div></div>
            <div class="stat-card amber anim-in anim-d2"><div class="stat-label">Processing Now</div><div class="stat-value" id="a-stat-proc">0</div></div>
            <div class="stat-card red anim-in anim-d3"><div class="stat-label">Active Checkers</div><div class="stat-value" id="a-stat-checkers">0</div></div>
          </div>

          <!-- Today's Summary -->
          <div class="panel">
            <div class="panel-header">
              <h3>📅 Today's Summary</h3>
              <span style="font-size:13px;color:var(--gray-500)" id="a-today-date"></span>
            </div>
            <div class="panel-body">
              <div class="stats-grid" style="grid-template-columns: repeat(3, 1fr); margin-bottom:18px">
                <div class="stat-card blue"><div class="stat-label">Orders Today</div><div class="stat-value" id="a-today-total">0</div></div>
                <div class="stat-card green"><div class="stat-label">Completed Today</div><div class="stat-value" id="a-today-done">0</div></div>
                <div class="stat-card amber"><div class="stat-label">Processing Today</div><div class="stat-value" id="a-today-proc">0</div></div>
              </div>
            </div>
          </div>

          <!-- Today's Completed Orders (who did what) -->
          <div class="panel">
            <div class="panel-header"><h3>✅ Completed Today — By Checker</h3></div>
            <div class="table-wrap">
              <table><thead><tr>
                <th>ID</th><th>Document</th><th>Client</th><th>Checker</th><th>Completed At</th><th>Reports</th>
              </tr></thead><tbody id="a-today-orders-table"></tbody></table>
            </div>
          </div>

          <!-- Checker Performance Today -->
          <div class="panel">
            <div class="panel-header"><h3>🏆 Checker Performance — Today</h3></div>
            <div class="panel-body" id="a-checker-performance"></div>
          </div>
        </div>

        <!-- Admin All Orders -->
        <div id="admin-orders" class="tab-content hidden">
          <div class="panel">
            <div class="panel-header"><h3>All Orders</h3></div>
            <div class="table-wrap">
              <table><thead><tr>
                <th>ID</th><th>Client</th><th>File</th><th>Status</th><th>Checker</th><th>Timer / Completed</th><th>Reports</th>
              </tr></thead><tbody id="admin-orders-table"></tbody></table>
            </div>
          </div>
        </div>

        <!-- Admin Problem Reports -->
        <div id="admin-problems" class="tab-content hidden">
          <div class="panel">
            <div class="panel-header">
              <h3>⚠️ Orders with Problem Reports</h3>
              <span id="problem-count-badge" class="badge badge-pending" style="margin-left:8px"></span>
            </div>
            <div class="table-wrap">
              <table><thead><tr>
                <th>ID</th><th>Document</th><th>Client</th><th>Checker</th><th>Problem Reported</th><th>Status</th><th>Action</th>
              </tr></thead><tbody id="admin-problems-table"></tbody></table>
            </div>
          </div>
        </div>

        <!-- Admin Messages Tab -->
        <div id="admin-messages" class="tab-content hidden">
          <div class="panel">
            <div class="panel-header">
              <h3>💬 Client Messages</h3>
              <span id="msg-count-badge" class="badge badge-pending" style="margin-left:8px"></span>
            </div>
            <div class="panel-body" id="admin-messages-list">
              <!-- Filled by JS -->
            </div>
          </div>
        </div>

        <!-- Admin Users -->
        <div id="admin-users" class="tab-content hidden">
          <div class="panel">
            <div class="panel-header"><h3>All Users (Clients)</h3></div>
            <div class="panel-body" id="admin-users-list"></div>
          </div>
        </div>

        <!-- Admin Checkers -->
        <div id="admin-checkers" class="tab-content hidden">
          <div class="panel">
            <div class="panel-header"><h3>➕ Create Checker Account</h3></div>
            <div class="panel-body">
              <p style="font-size:13px;color:var(--gray-500);margin-bottom:16px">Create a new checker account. Give the username and password to your checker so they can log in.</p>
              <div class="form-group">
                <label>Checker Name</label>
                <input type="text" class="form-input" id="new-checker-name" placeholder="Checker's full name">
              </div>
              <div class="form-group">
                <label>Username</label>
                <input type="text" class="form-input" id="new-checker-username" placeholder="Choose a username">
              </div>
              <div class="form-group">
                <label>Password</label>
                <input type="text" class="form-input" id="new-checker-pass" placeholder="Set a password">
              </div>
              <button class="btn btn-primary" onclick="adminCreateChecker()">Create Checker Account</button>
              <div id="checker-create-result" style="margin-top:14px;font-size:14px;font-weight:600"></div>
            </div>
          </div>
          <div class="panel">
            <div class="panel-header"><h3>🛡️ All Checkers</h3></div>
            <div class="panel-body" id="admin-checkers-list"></div>
          </div>
          <div class="panel" style="margin-top:20px">
            <div class="panel-header"><h3>📊 Checker Performance Track Record</h3><span style="font-size:12px;color:var(--gray-500)">Full history for all checkers</span></div>
            <div class="table-wrap">
              <table><thead><tr>
                <th>Checker</th>
                <th>Today</th>
                <th>Yesterday</th>
                <th>This Week</th>
                <th>This Month</th>
                <th>All Time</th>
                <th>Status</th>
              </tr></thead><tbody id="admin-checker-track-table"></tbody></table>
            </div>
          </div>
        </div>

        <!-- Admin Manage Credits -->
        <div id="admin-credits" class="tab-content hidden">
          <div class="panel">
            <div class="panel-header"><h3>💳 Manage User Credits</h3></div>
            <div class="panel-body">
              <div class="form-group">
                <label>Select User</label>
                <select class="form-input" id="credit-user-select"></select>
              </div>
              <div class="form-group">
                <label>Credits Amount</label>
                <input type="number" class="form-input" id="credit-amount" value="1" min="1">
              </div>
              <div class="form-group">
                <label>Action</label>
                <div style="display:flex;gap:10px;flex-wrap:wrap">
                  <button class="btn btn-success" onclick="adminAddCredits('add')">➕ Add Credits</button>
                  <button class="btn btn-danger" onclick="adminAddCredits('deduct')">➖ Deduct Credits</button>
                </div>
              </div>
              <div id="credit-result" style="margin-top:14px;font-size:14px;font-weight:600;padding:10px;border-radius:8px;display:none"></div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- ==================== UPLOAD REPORT MODAL (Checker) ==================== -->
<div class="modal-overlay" id="upload-modal">
  <div class="modal">
    <h3>📤 Upload Reports</h3>
    <p style="font-size:13px;color:var(--gray-500);margin-bottom:16px">Upload the plagiarism and AI detection reports separately for this order</p>
    
    <div class="form-group">
      <label>📄 Plagiarism Report <span style="color:var(--red-500)">*</span></label>
      <input type="file" class="form-input" id="report-plag-input" style="padding:8px">
      <span style="font-size:11px;color:var(--gray-400)">Required — Turnitin plagiarism similarity report</span>
    </div>

    <div class="form-group" style="margin-top:18px">
      <label>🤖 AI Detection Report</label>
      <input type="file" class="form-input" id="report-ai-input" style="padding:8px">
      <span style="font-size:11px;color:var(--gray-400)">Optional — Turnitin AI writing detection report</span>
    </div>

    <div class="form-group" style="margin-top:8px">
      <label style="display:flex;align-items:center;gap:8px;cursor:pointer">
        <input type="checkbox" id="ai-not-possible" onchange="document.getElementById('ai-reason-wrap').style.display=this.checked?'block':'none'; document.getElementById('report-ai-input').disabled=this.checked; if(this.checked) document.getElementById('report-ai-input').value='';">
        <span style="font-size:13px;color:var(--gray-600)">AI report is not possible for this document</span>
      </label>
      <div id="ai-reason-wrap" style="display:none;margin-top:10px">
        <label style="font-size:13px;color:var(--red-500);font-weight:600">Reason why AI report is not possible <span style="color:var(--red-500)">*</span></label>
        <textarea class="form-input" id="ai-reason" rows="3" placeholder="e.g. Document contains only images, scanned handwriting, non-English text not supported by AI detection, etc." style="resize:vertical;margin-top:4px"></textarea>
      </div>
    </div>

    <div style="display:flex;gap:10px;justify-content:flex-end;margin-top:18px">
      <button class="btn btn-ghost" onclick="closeModal('upload-modal')">Cancel</button>
      <button class="btn btn-primary" onclick="submitReport()">Upload & Complete</button>
    </div>
  </div>
</div>

<!-- ==================== REPORT PROBLEM MODAL (Client) ==================== -->
<div class="modal-overlay" id="report-problem-modal">
  <div class="modal">
    <h3>⚠️ Report a Problem</h3>
    <p style="font-size:13px;color:var(--gray-500);margin-bottom:16px">Describe the issue with this order. Admin will review and respond.</p>
    
    <div class="form-group">
      <label>Order #<span id="report-order-id"></span> — <span id="report-file-name"></span></label>
    </div>

    <div class="form-group">
      <label>What's the problem? <span style="color:var(--red-500)">*</span></label>
      <textarea class="form-input" id="problem-description" rows="5" placeholder="Describe the issue with the report (e.g., report looks fake, wrong document analyzed, low similarity percentage seems incorrect, etc.)" style="resize:vertical"></textarea>
    </div>

    <div style="display:flex;gap:10px;justify-content:flex-end;margin-top:18px">
      <button class="btn btn-ghost" onclick="closeModal('report-problem-modal')">Cancel</button>
      <button class="btn btn-danger" onclick="submitProblemReport()">Submit Problem Report</button>
    </div>
  </div>
</div>

<!-- ==================== ADMIN REVIEW MODAL ==================== -->
<div class="modal-overlay" id="admin-review-modal">
  <div class="modal" style="max-width:600px">
    <h3>🔍 Review Order Problem</h3>
    <div id="review-order-info" style="padding:14px;background:var(--gray-50);border-radius:8px;margin-bottom:16px"></div>
    
    <div class="form-group">
      <label style="font-weight:700;color:var(--red-600)">Client's Problem Report:</label>
      <div id="review-problem-text" style="padding:12px;background:var(--red-50);border:1px solid var(--red-200);border-radius:8px;margin-top:6px;font-size:14px;line-height:1.6"></div>
    </div>

    <div class="form-group" style="margin-top:18px">
      <label>Response to Client (optional)</label>
      <textarea class="form-input" id="admin-response-text" rows="3" placeholder="Message to send to the client explaining your decision..." style="resize:vertical"></textarea>
    </div>

    <div style="background:var(--blue-50);padding:14px;border-radius:8px;margin-top:18px;border:1px solid var(--blue-200)">
      <p style="font-size:13px;color:var(--blue-800);font-weight:600;margin-bottom:12px">Actions:</p>
      <div style="display:flex;gap:10px;flex-wrap:wrap">
        <button class="btn btn-success" onclick="resolveOrderProblem('refund-pass')">✅ Refund + Mark as Passed</button>
        <button class="btn btn-danger" onclick="resolveOrderProblem('refund-fail')">❌ Refund + Mark as Failed</button>
        <button class="btn btn-outline" onclick="resolveOrderProblem('pass-only')">Pass Without Refund</button>
        <button class="btn btn-ghost" onclick="closeModal('admin-review-modal')">Cancel</button>
      </div>
    </div>
  </div>
</div>

<!-- ==================== FORGOT PASSWORD MODAL ==================== -->
<div class="modal-overlay" id="forgot-modal">
  <div class="modal">
    <h3>🔑 Reset Your Password</h3>
    <p style="font-size:13px;color:var(--gray-500);margin-bottom:16px">Enter your username or email. We'll help you recover your account.</p>
    <div class="form-group">
      <label>Username</label>
      <input type="text" class="form-input" id="forgot-input" placeholder="Your username">
    </div>
    <div id="forgot-result" style="margin-top:8px;padding:10px 14px;border-radius:8px;font-size:13px;font-weight:600;display:none"></div>
    <div style="display:flex;gap:10px;justify-content:flex-end;margin-top:18px">
      <button class="btn btn-ghost" onclick="closeModal('forgot-modal')">Cancel</button>
      <button class="btn btn-primary" onclick="submitForgotPassword()">Recover Account</button>
    </div>
  </div>
</div>

<!-- ==================== ADMIN REPLY MODAL ==================== -->
<div class="modal-overlay" id="reply-modal">
  <div class="modal">
    <h3>↩ Reply to <span id="reply-to-name"></span></h3>
    <div class="form-group" style="margin-top:12px">
      <label>Your Reply</label>
      <textarea class="form-input" id="reply-text" rows="4" placeholder="Type your reply..." style="resize:vertical"></textarea>
    </div>
    <div style="display:flex;gap:10px;justify-content:flex-end;margin-top:14px">
      <button class="btn btn-ghost" onclick="closeModal('reply-modal')">Cancel</button>
      <button class="btn btn-primary" onclick="sendAdminReply()">Send Reply</button>
    </div>
  </div>
</div>

<!-- ==================== USER DETAIL MODAL (Admin) ==================== -->
<div class="modal-overlay" id="user-detail-modal">
  <div class="modal" style="max-width:560px">
    <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:20px">
      <h3 id="ud-title">User Details</h3>
      <button class="btn btn-ghost btn-sm" onclick="closeModal('user-detail-modal')">✕</button>
    </div>

    <!-- User Info -->
    <div style="background:var(--gray-50);border-radius:12px;padding:18px;margin-bottom:16px;border:1px solid var(--gray-200)">
      <div style="display:flex;align-items:center;gap:14px;margin-bottom:16px">
        <div id="ud-avatar" style="width:52px;height:52px;border-radius:14px;background:linear-gradient(135deg,var(--blue-100),var(--blue-200));color:var(--blue-700);display:flex;align-items:center;justify-content:center;font-size:22px;font-weight:700;font-family:Fraunces,serif"></div>
        <div>
          <div id="ud-name" style="font-size:18px;font-weight:700;color:var(--ink)"></div>
          <div id="ud-role" style="font-size:12px;color:var(--gray-500);text-transform:uppercase;font-weight:600;letter-spacing:0.5px"></div>
        </div>
      </div>
      <div style="display:grid;grid-template-columns:1fr 1fr;gap:10px">
        <div style="background:white;padding:10px 14px;border-radius:8px;border:1px solid var(--gray-200)">
          <div style="font-size:11px;font-weight:600;color:var(--gray-500);text-transform:uppercase;letter-spacing:0.5px">Username</div>
          <div id="ud-username" style="font-size:14px;font-weight:600;color:var(--ink);margin-top:2px"></div>
        </div>
        <div style="background:white;padding:10px 14px;border-radius:8px;border:1px solid var(--gray-200)">
          <div style="font-size:11px;font-weight:600;color:var(--gray-500);text-transform:uppercase;letter-spacing:0.5px">Password</div>
          <div id="ud-password" style="font-size:14px;font-weight:600;color:var(--ink);margin-top:2px;font-family:monospace"></div>
        </div>
        <div style="background:white;padding:10px 14px;border-radius:8px;border:1px solid var(--blue-100)">
          <div style="font-size:11px;font-weight:600;color:var(--blue-500);text-transform:uppercase;letter-spacing:0.5px">Current Credits</div>
          <div id="ud-credits" style="font-size:22px;font-weight:700;color:var(--blue-700);font-family:Fraunces,serif;margin-top:2px"></div>
        </div>
        <div style="background:white;padding:10px 14px;border-radius:8px;border:1px solid var(--green-50)">
          <div style="font-size:11px;font-weight:600;color:var(--green-600);text-transform:uppercase;letter-spacing:0.5px">Member Since</div>
          <div id="ud-since" style="font-size:13px;font-weight:600;color:var(--ink);margin-top:2px"></div>
        </div>
      </div>
    </div>

    <!-- Order Stats -->
    <div style="background:var(--gray-50);border-radius:12px;padding:18px;margin-bottom:16px;border:1px solid var(--gray-200)">
      <div style="font-size:13px;font-weight:700;color:var(--ink);margin-bottom:12px">📊 Activity Stats</div>
      <div style="display:grid;grid-template-columns:repeat(4,1fr);gap:8px" id="ud-stats"></div>
    </div>

    <!-- Order History -->
    <div style="background:var(--gray-50);border-radius:12px;padding:18px;margin-bottom:20px;border:1px solid var(--gray-200)">
      <div style="font-size:13px;font-weight:700;color:var(--ink);margin-bottom:12px">📋 Order History</div>
      <div id="ud-orders" style="max-height:180px;overflow-y:auto"></div>
    </div>

    <!-- Actions -->
    <div style="display:flex;gap:10px;justify-content:flex-end;padding-top:14px;border-top:1px solid var(--gray-200)">
      <button class="btn btn-ghost" onclick="closeModal('user-detail-modal')">Close</button>
      <button class="btn btn-danger" id="ud-delete-btn" onclick="deleteUserFromModal()">🗑 Delete Account</button>
    </div>
  </div>
</div>

<script>
// ==================== DATA STORE (in-memory, simulates a database) ====================
// ==================== SUPABASE CONNECTION ====================
const SUPABASE_URL = 'https://ixisjvxvbjktxxjvnvcn.supabase.co';
const SUPABASE_KEY = 'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6Iml4aXNqdnh2YmprdHh4anZudmNuIiwicm9sZSI6ImFub24iLCJpYXQiOjE3Nzk4OTc5MzUsImV4cCI6MjA5NTQ3MzkzNX0.YKFFcpkb_nWjDL910yVmsCuyhdSvonlMY6PYQTJnjek';
const sb = window.supabase ? window.supabase.createClient(SUPABASE_URL, SUPABASE_KEY) : null;
let supabaseReady = true; // Always try to save — Supabase is ready when sb client exists
let isSyncing = false;

const DB = {
  users: [
    { id: 1, name: 'Hamayun Saleem', username: 'Hamayun Saleem', password: 'ascp94322@22', role: 'admin', credits: 0, approved: true },
  ],
  orders: [],
  notifications: [],
  chatMessages: [],
  nextUserId: 2,
  nextOrderId: 1,
  nextNotifId: 1,
  nextChatId: 1
};

// Map a local user object to Supabase row format
function userToRow(u) {
  return { id: u.id, name: u.name, username: u.username, email: u.email || null, password: u.password, role: u.role, credits: u.credits || 0, approved: u.approved !== false, online: u.online !== false };
}
function rowToUser(r) {
  return { id: r.id, name: r.name, username: r.username, email: r.email, password: r.password, role: r.role, credits: r.credits || 0, approved: r.approved !== false, online: r.online !== false };
}

// Load all data from Supabase on startup
async function loadFromSupabase() {
  if (!sb) return;
  try {
    const { data: users } = await sb.from('users').select('*');
    if (users && users.length) {
      DB.users = users.map(rowToUser);
      DB.nextUserId = Math.max(...users.map(u => u.id)) + 1;
    }
    const { data: orders } = await sb.from('orders').select('*');
    if (orders) {
      // Preserve local binary file data that isn't stored in Supabase
      const localFileCache = {};
      DB.orders.forEach(o => {
        localFileCache[o.id] = {
          fileData: o.fileData,
          plagReportData: o.plagReportData || o.plagReportUrl,
          aiReportData: o.aiReportData || o.aiReportUrl
        };
      });

      DB.orders = orders.map(o => {
        const cached = localFileCache[o.id] || {};
        return {
          id: o.id, clientId: o.client_id, clientName: o.client_name,
          fileName: o.file_name,
          fileData: cached.fileData || o.file_url || null,
          fileUrl: o.file_url || cached.fileData || null,
          clientMessage: o.client_message,
          status: o.status, checkerId: o.checker_id, checkerName: o.checker_name,
          placedAt: new Date(o.placed_at).getTime(),
          completedAt: o.completed_at ? new Date(o.completed_at).getTime() : null,
          timerEnd: o.timer_end ? new Date(o.timer_end).getTime() : null,
          reportUploaded: !!o.plag_report,
          plagReport: o.plag_report,
          plagReportData: cached.plagReportData || null,
          plagReportUrl: o.plag_report_url || null,
          aiReport: o.ai_report,
          aiReportData: cached.aiReportData || null,
          aiReportUrl: o.ai_report_url || null,
          aiNotPossible: o.ai_not_possible, aiReason: o.ai_reason,
          verificationDeadline: o.verification_deadline ? new Date(o.verification_deadline).getTime() : null,
          verificationStatus: o.verification_status,
          clientReport: o.client_report, adminResponse: o.admin_response,
          rejectedBy: o.rejected_by || []
        };
      });
      if (orders.length) DB.nextOrderId = Math.max(...orders.map(o => o.id)) + 1;
    }
    const { data: notifs } = await sb.from('notifications').select('*').order('time', { ascending: false }).limit(200);
    if (notifs) {
      DB.notifications = notifs.map(n => ({
        id: n.id, userId: n.user_id, title: n.title, message: n.message,
        time: new Date(n.time).getTime(), read: n.read
      }));
      if (notifs.length) DB.nextNotifId = Math.max(...notifs.map(n => n.id)) + 1;
    }
    const { data: chats } = await sb.from('chat_messages').select('*').order('time', { ascending: true });
    if (chats) {
      DB.chatMessages = chats.map(c => ({
        id: c.id, userId: c.user_id, userName: c.user_name,
        userRole: c.user_role, fromRole: c.from_role,
        subject: c.subject, message: c.message,
        time: new Date(c.time).getTime(), read: c.read
      }));
      if (chats.length) DB.nextChatId = Math.max(...chats.map(c => c.id)) + 1;
    }
    supabaseReady = true;
    console.log('[Supabase] Data loaded successfully');
  } catch (e) {
    console.error('[Supabase] Load error:', e);
  }
}

// Save a user to Supabase
async function saveUser(user) {
  if (!sb || !supabaseReady) return;
  try {
    await sb.from('users').upsert(userToRow(user));
  } catch (e) { console.error('[Supabase] saveUser:', e); }
}

// Save an order to Supabase — file binary data stays local only (too large for DB)
async function saveOrder(order) {
  if (!sb || !supabaseReady) return;
  try {
    const row = {
      id: order.id, client_id: order.clientId, client_name: order.clientName,
      file_name: order.fileName,
      file_url: order.fileUrl || null,
      client_message: order.clientMessage,
      status: order.status, checker_id: order.checkerId, checker_name: order.checkerName,
      placed_at: new Date(order.placedAt).toISOString(),
      completed_at: order.completedAt ? new Date(order.completedAt).toISOString() : null,
      timer_end: order.timerEnd ? new Date(order.timerEnd).toISOString() : null,
      plag_report: order.plagReport,
      plag_report_url: order.plagReportUrl || null,
      ai_report: order.aiReport,
      ai_report_url: order.aiReportUrl || null,
      ai_not_possible: !!order.aiNotPossible, ai_reason: order.aiReason,
      verification_deadline: order.verificationDeadline ? new Date(order.verificationDeadline).toISOString() : null,
      verification_status: order.verificationStatus,
      client_report: order.clientReport, admin_response: order.adminResponse,
      rejected_by: order.rejectedBy || []
    };
    const { error } = await sb.from('orders').upsert(row);
    if (error) console.error('[Supabase] saveOrder error:', error.message);
  } catch (e) { console.error('[Supabase] saveOrder:', e); }
}

async function deleteOrder(orderId) {
  if (!sb || !supabaseReady) return;
  try { await sb.from('orders').delete().eq('id', orderId); } catch (e) { console.error('[Supabase] deleteOrder:', e); }
}

function deleteCompletedOrder(orderId) {
  const order = DB.orders.find(o => o.id === orderId);
  if (!order) return;
  if (order.status !== 'completed') return showToast('You can only delete completed orders.', 'error');
  DB.orders = DB.orders.filter(o => o.id !== orderId);
  deleteOrder(orderId);
  showToast(`Order #${orderId} deleted successfully.`, 'info');
  if (currentUser.role === 'client') refreshClientDash();
  else if (currentUser.role === 'checker') refreshCheckerDash();
  else if (currentUser.role === 'admin') refreshAdminDash();
}

// Lightweight status-only update — used for accept/reject/complete to guarantee it saves
async function saveOrderStatus(order) {
  if (!sb || !supabaseReady) return;
  try {
    const row = {
      id: order.id,
      client_id: order.clientId,
      client_name: order.clientName,
      file_name: order.fileName,
      file_url: order.fileUrl || null,
      client_message: order.clientMessage || null,
      status: order.status,
      checker_id: order.checkerId || null,
      checker_name: order.checkerName || null,
      placed_at: new Date(order.placedAt).toISOString(),
      timer_end: order.timerEnd ? new Date(order.timerEnd).toISOString() : null,
      completed_at: order.completedAt ? new Date(order.completedAt).toISOString() : null,
      plag_report: order.plagReport || null,
      plag_report_url: order.plagReportUrl || null,
      ai_report: order.aiReport || null,
      ai_report_url: order.aiReportUrl || null,
      ai_not_possible: !!order.aiNotPossible,
      ai_reason: order.aiReason || null,
      verification_deadline: order.verificationDeadline ? new Date(order.verificationDeadline).toISOString() : null,
      verification_status: order.verificationStatus || null,
      client_report: order.clientReport || null,
      admin_response: order.adminResponse || null,
      rejected_by: order.rejectedBy || []
    };
    const { error } = await sb.from('orders').upsert(row);
    if (error) console.error('[Supabase] saveOrderStatus error:', error.message);
  } catch (e) { console.error('[Supabase] saveOrderStatus:', e); }
}

async function saveNotification(n) {
  if (!sb || !supabaseReady) return;
  try {
    await sb.from('notifications').upsert({
      id: n.id, user_id: n.userId, title: n.title, message: n.message,
      time: new Date(n.time).toISOString(), read: !!n.read
    });
  } catch (e) { console.error('[Supabase] saveNotification:', e); }
}

async function saveChat(c) {
  if (!sb || !supabaseReady) return;
  try {
    await sb.from('chat_messages').upsert({
      id: c.id, user_id: c.userId, user_name: c.userName,
      user_role: c.userRole, from_role: c.fromRole,
      subject: c.subject, message: c.message,
      time: new Date(c.time).toISOString(), read: !!c.read
    });
  } catch (e) { console.error('[Supabase] saveChat:', e); }
}

// ==================== SUPABASE STORAGE ====================
// Upload a base64 file to Supabase Storage and return its public URL
async function uploadToStorage(base64Data, fileName, folder) {
  // Store base64 directly — simpler and more reliable than Storage buckets
  return base64Data;
}

async function deleteUser(userId) {
  if (!sb || !supabaseReady) return;
  try { await sb.from('users').delete().eq('id', userId); } catch (e) { console.error('[Supabase] deleteUser:', e); }
}


let currentUser = null;
let currentLang = 'en';
let selectedFile = null;
let uploadingOrderId = null;
let timerIntervals = [];

// ==================== i18n ====================
const i18n = {
  en: {
    login: 'Login', getStarted: 'Get Started', heroBadge: '⚡ Pure Turnitin Reports — Plagiarism & AI Detection in 30 Minutes',
    heroTitle: 'Plagiarism & AI Reports<br>You Can Trust', heroDesc: 'Get pure Turnitin plagiarism and AI detection reports for your documents. Upload, use a credit, and receive both reports within 20 minutes. Simple, fast, and affordable.',
    startNow: 'Start Now — It\'s Easy', learnMore: 'Learn More', howItWorks: 'How It Works',
    howItWorksDesc: 'Three simple steps to get your plagiarism & AI detection reports',
    feat1Title: 'Upload Document', feat1Desc: 'Upload any file type — Word, PDF, or any other format. We accept everything.',
    feat2Title: '20-Minute Delivery', feat2Desc: 'Our team generates pure Turnitin plagiarism and AI detection reports and delivers them within 20 minutes.',
    feat3Title: 'Download Reports', feat3Desc: 'Get your plagiarism report and AI detection report separately. Download both instantly from your dashboard.',
    pricingTitle: 'Credit Packages', pricingDesc: 'Buy credits to generate reports. 1 credit = 1 report. Contact us to purchase.',
    credit1: '1 Credit', credit10: '10 Credits', credit20: '20 Credits', contactBuy: 'Contact to Buy',
    contactTitle: 'Buy Credits — Contact Us', contactDesc: 'Reach out via WhatsApp or Discord to purchase credits. We\'ll add them to your account instantly.',
    openWhatsApp: 'Open WhatsApp', joinDiscord: 'Join Discord',
    loginTitle: 'Welcome Back', loginSub: 'Sign in to your account', usernameLabel: 'Username', passLabel: 'Password', loginBtn: 'Sign In',
    noAccount: 'Don\'t have an account? <a onclick="showPage(\'register\')">Sign Up</a>',
    regTitle: 'Create Account', regSub: 'Join CheckPlag today', nameLabel: 'Full Name',
    regBtn: 'Create Account',
    hasAccount: 'Already have an account? <a onclick="showPage(\'login\')">Sign In</a>',
    dashboard: 'Dashboard', totalOrders: 'Total Orders', processing: 'Processing', completed: 'Completed', credits: 'Credits',
    recentOrders: 'Recent Orders', file: 'File', status: 'Status', timer: 'Timer', action: 'Action',
    uploadDoc: 'Upload Document', dropFile: 'Click or drag a file here', anyFile: 'Any file type accepted',
    placeOrder: 'Place Order (1 Credit)', allOrders: 'All Orders', buyCredits: 'Buy Credits',
    buyCreditsDesc: 'To purchase credits, contact us via WhatsApp or Discord. We\'ll add credits to your account after payment.',
    notifications: '🔔 Notifications', checkerDash: 'Checker Dashboard', activeOrders: 'Active Orders',
    myCompleted: 'My Completed', incomingOrders: 'Incoming Orders', completedOrders: 'Completed Orders',
    client: 'Client', completedAt: 'Completed At', myReports: 'My Reports:', adminPanel: 'Admin Panel'
  },
  zh: {
    login: '登录', getStarted: '开始使用', heroBadge: '⚡ 纯Turnitin报告 — 20分钟内完成抄袭和AI检测',
    heroTitle: '值得信赖的<br>抄袭和AI检测报告', heroDesc: '获取纯Turnitin抄袭和AI检测报告。上传文档，使用一个积分，在20分钟内收到两份报告。简单、快速、实惠。',
    startNow: '立即开始', learnMore: '了解更多', howItWorks: '如何运作',
    howItWorksDesc: '三个简单步骤获取您的抄袭和AI检测报告',
    feat1Title: '上传文档', feat1Desc: '上传任何文件类型 — Word、PDF或任何其他格式。我们接受一切。',
    feat2Title: '20分钟交付', feat2Desc: '我们的团队生成纯Turnitin抄袭和AI检测报告，并在20分钟内交付。',
    feat3Title: '下载报告', feat3Desc: '分别获取抄袭报告和AI检测报告。从您的仪表板即时下载两份报告。',
    pricingTitle: '积分套餐', pricingDesc: '购买积分以生成报告。1积分 = 1份报告。联系我们购买。',
    credit1: '1 积分', credit10: '10 积分', credit20: '20 积分', contactBuy: '联系购买',
    contactTitle: '购买积分 — 联系我们', contactDesc: '通过WhatsApp或Discord联系我们购买积分。我们会立即将积分添加到您的账户。',
    openWhatsApp: '打开WhatsApp', joinDiscord: '加入Discord',
    loginTitle: '欢迎回来', loginSub: '登录您的账户', usernameLabel: '用户名', passLabel: '密码', loginBtn: '登录',
    noAccount: '没有账户？<a onclick="showPage(\'register\')">注册</a>',
    regTitle: '创建账户', regSub: '立即加入CheckPlag', nameLabel: '全名',
    regBtn: '创建账户',
    hasAccount: '已有账户？<a onclick="showPage(\'login\')">登录</a>',
    dashboard: '仪表板', totalOrders: '总订单', processing: '处理中', completed: '已完成', credits: '积分',
    recentOrders: '最近订单', file: '文件', status: '状态', timer: '计时器', action: '操作',
    uploadDoc: '上传文档', dropFile: '点击或拖拽文件到此处', anyFile: '接受任何文件类型',
    placeOrder: '下单（1积分）', allOrders: '所有订单', buyCredits: '购买积分',
    buyCreditsDesc: '要购买积分，请通过WhatsApp或Discord联系我们。付款后我们会将积分添加到您的账户。',
    notifications: '🔔 通知', checkerDash: '检查员仪表板', activeOrders: '活跃订单',
    myCompleted: '我已完成', incomingOrders: '收到的订单', completedOrders: '已完成的订单',
    client: '客户', completedAt: '完成时间', myReports: '我的报告：', adminPanel: '管理面板'
  }
};

// ==================== TOAST SYSTEM ====================
function showToast(msg, type) {
  let container = document.getElementById('toast-container');
  if (!container) {
    container = document.createElement('div');
    container.id = 'toast-container';
    container.style.cssText = 'position:fixed;top:20px;right:20px;z-index:9999;display:flex;flex-direction:column;gap:8px;max-width:380px';
    document.body.appendChild(container);
  }
  const toast = document.createElement('div');
  const colors = { error: '#fee2e2;color:#991b1b;border:1px solid #fca5a5', success: '#dcfce7;color:#166534;border:1px solid #86efac', info: '#dbeafe;color:#1e40af;border:1px solid #93c5fd' };
  toast.style.cssText = `background:${colors[type] || colors.info};padding:14px 20px;border-radius:10px;font-size:14px;font-weight:600;font-family:Plus Jakarta Sans,sans-serif;box-shadow:0 4px 12px rgba(0,0,0,0.15);animation:fadeInUp 0.3s ease;cursor:pointer`;
  toast.textContent = msg;
  toast.onclick = () => toast.remove();
  container.appendChild(toast);
  setTimeout(() => { toast.style.opacity = '0'; toast.style.transition = 'opacity 0.3s'; setTimeout(() => toast.remove(), 300); }, 4000);
}

function toggleLang() {
  currentLang = currentLang === 'en' ? 'zh' : 'en';
  document.querySelectorAll('.lang-toggle').forEach(b => b.textContent = currentLang === 'en' ? '中文' : 'EN');
  document.querySelectorAll('[data-i18n]').forEach(el => {
    const key = el.getAttribute('data-i18n');
    if (i18n[currentLang][key]) el.innerHTML = i18n[currentLang][key];
  });
}

// ==================== PAGE NAVIGATION ====================
function showPage(page) {
  document.querySelectorAll('[id^="page-"]').forEach(p => p.classList.add('hidden'));
  document.getElementById('page-' + page).classList.remove('hidden');
  window.scrollTo(0, 0);
  if (page === 'client') refreshClientDash();
  if (page === 'checker') refreshCheckerDash();
  if (page === 'admin') refreshAdminDash();
}

function switchTab(el, role) {
  const sidebar = el.closest('.sidebar-nav');
  sidebar.querySelectorAll('.nav-item').forEach(n => n.classList.remove('active'));
  el.classList.add('active');
  const tabId = el.getAttribute('data-tab');
  const content = el.closest('.app-layout').querySelector('.content');
  content.querySelectorAll('.tab-content').forEach(t => t.classList.add('hidden'));
  document.getElementById(tabId).classList.remove('hidden');
  // Refresh views when switching
  if (tabId === 'client-chat') {
    DB.chatMessages.forEach(c => {
      if (c.userId === currentUser?.id && c.fromRole === 'admin') {
        c.read = true;
        seenChatIds.add(c.id);
        if (sb && supabaseReady) sb.from('chat_messages').update({ read: true }).eq('id', c.id).then(() => {});
      }
    });
    localStorage.setItem('cp_seen_chats', JSON.stringify([...seenChatIds]));
    renderClientChatHistory();
    updateNotifCounts();
  }
  if (tabId === 'checker-chat') {
    DB.chatMessages.forEach(c => {
      if (c.userId === currentUser?.id && c.fromRole === 'admin') {
        c.read = true;
        seenChatIds.add(c.id);
        if (sb && supabaseReady) sb.from('chat_messages').update({ read: true }).eq('id', c.id).then(() => {});
      }
    });
    localStorage.setItem('cp_seen_chats', JSON.stringify([...seenChatIds]));
    renderCheckerChatHistory();
    updateNotifCounts();
  }
  if (tabId === 'checker-performance') renderCheckerPerformance();
  if (tabId === 'admin-messages') renderAdminMessages();
  // Close mobile sidebar
  document.querySelectorAll('.sidebar').forEach(s => s.classList.remove('mobile-open'));
}

// ==================== AUTH ====================
function showMsg(elId, msg, isError) {
  const el = document.getElementById(elId);
  if (!el) return;
  el.style.display = 'block';
  el.style.background = isError ? '#fee2e2' : '#dcfce7';
  el.style.color = isError ? '#991b1b' : '#166534';
  el.style.borderColor = isError ? '#fca5a5' : '#86efac';
  el.textContent = msg;
  if (!isError) setTimeout(() => el.style.display = 'none', 3000);
}

function handleLogin() {
  const username = document.getElementById('login-email').value.trim();
  const pass = document.getElementById('login-pass').value;
  
  if (!username || !pass) {
    showMsg('login-error', '⚠️ Please enter username and password', true);
    showToast('Please enter username and password', 'error');
    return;
  }
  
  const userExists = DB.users.find(u => u.username === username);
  if (!userExists) {
    showMsg('login-error', '❌ Account does not exist. Please register first.', true);
    showToast('Account does not exist! Please register first.', 'error');
    return;
  }
  
  if (userExists.password !== pass) {
    showMsg('login-error', '🔒 Incorrect password. Please try again.', true);
    showToast('Incorrect password!', 'error');
    return;
  }
  
  if (userExists.role === 'checker' && !userExists.approved) {
    showMsg('login-error', '🚫 Your checker account has been disabled by admin.', true);
    showToast('Your account is disabled', 'error');
    return;
  }
  
  document.getElementById('login-error').style.display = 'none';
  currentUser = userExists;
  localStorage.setItem('cp_session', userExists.username);
  if (currentUser.role === 'checker' && currentUser.online === undefined) currentUser.online = true;
  // Pre-seed existing notifications as seen so they don't ring immediately after login
  DB.notifications.filter(n => Number(n.userId) === Number(currentUser.id)).forEach(n => seenNotifIds.add(n.id));
  localStorage.setItem('cp_seen_notifs', JSON.stringify([...seenNotifIds]));
  showPage(userExists.role === 'admin' ? 'admin' : userExists.role === 'checker' ? 'checker' : 'client');
  updateUserUI();
  if (currentUser.role === 'checker') updateCheckerOnlineUI();
  // Delay sound init so login doesn't immediately ring for old notifications
  setTimeout(() => { soundInitialized = true; }, 3000);
}

function handleRegister() {
  const name = document.getElementById('reg-name').value.trim();
  const username = document.getElementById('reg-email').value.trim();
  const pass = document.getElementById('reg-pass').value;
  if (!name || !username || !pass) return showMsg('reg-error', 'Please fill in all fields', true);
  if (DB.users.find(u => u.username === username)) return showMsg('reg-error', 'Username already taken', true);
  const newUser = { id: DB.nextUserId++, name, username, password: pass, role: 'client', credits: 0, approved: true };
  DB.users.push(newUser);
  saveUser(newUser);
  currentUser = newUser;
  localStorage.setItem('cp_session', newUser.username);
  showPage('client');
  updateUserUI();
}

function handleLogout() {
  currentUser = null; selectedFile = null;
  localStorage.removeItem('cp_session');
  timerIntervals.forEach(clearInterval); timerIntervals = [];
  showPage('landing');
}

// ==================== PASSWORD RECOVERY ====================
function showForgotPassword() {
  document.getElementById('forgot-input').value = '';
  document.getElementById('forgot-result').style.display = 'none';
  document.getElementById('forgot-modal').classList.add('open');
}

function submitForgotPassword() {
  const input = document.getElementById('forgot-input').value.trim();
  const resultEl = document.getElementById('forgot-result');
  if (!input) {
    resultEl.style.display = 'block';
    resultEl.style.background = '#fee2e2';
    resultEl.style.color = '#991b1b';
    resultEl.textContent = 'Please enter your username or email.';
    return;
  }
  const user = DB.users.find(u => u.username === input);
  resultEl.style.display = 'block';
  if (!user) {
    resultEl.style.background = '#fee2e2';
    resultEl.style.color = '#991b1b';
    resultEl.textContent = '❌ No account found with that username or email.';
    return;
  }
  // Notify admin of the reset request
  addNotification(1, '🔑 Password Reset Request', `${user.name} (@${user.username}) requested a password reset.`);
  resultEl.style.background = '#dcfce7';
  resultEl.style.color = '#166534';
  resultEl.textContent = '✅ Account found! Contact admin via WhatsApp (+92 313 1521781) to reset your password. (In the live version, a reset link will be emailed automatically.)';
  showToast('Account found! Contact admin to reset your password.', 'success');
}

// ==================== EMAIL NOTIFICATIONS ====================
// Sends an email notification. Works once an email service (e.g. EmailJS) is connected.
// Until then, it logs the email and falls back to in-website notifications.
function sendEmail(toUserId, subject, body) {
  const user = DB.users.find(u => u.id === toUserId);
  if (!user || !user.email) return;
  // PLACEHOLDER: When you connect EmailJS/Resend, the real send goes here.
  // Example with EmailJS:
  //   emailjs.send('service_id', 'template_id', { to_email: user.email, subject, message: body });
  console.log(`[EMAIL → ${user.email}] ${subject}: ${body}`);
}

function updateUserUI() {
  if (!currentUser) return;
  if (currentUser.role === 'client') {
    document.getElementById('client-name').textContent = currentUser.name;
    document.getElementById('client-avatar').textContent = currentUser.name.charAt(0).toUpperCase();
  } else if (currentUser.role === 'checker') {
    document.getElementById('checker-name').textContent = currentUser.name;
    document.getElementById('checker-avatar').textContent = currentUser.name.charAt(0).toUpperCase();
  }
  // Request browser notification permission after login
  requestNotifPermission();
}

// ==================== FILE HANDLING ====================
function handleFileSelect(e) { selectedFile = e.target.files[0]; showFileInfo(); }
function handleFileDrop(e) { selectedFile = e.dataTransfer.files[0]; showFileInfo(); }
function showFileInfo() {
  if (!selectedFile) return;
  document.getElementById('file-info').classList.remove('hidden');
  document.getElementById('selected-file-name').textContent = selectedFile.name;
}
function clearFile() {
  selectedFile = null;
  document.getElementById('file-info').classList.add('hidden');
  document.getElementById('file-input').value = '';
}

// ==================== ORDERS ====================
function placeOrder() {
  if (!currentUser) return;
  if (!selectedFile) return showToast('Please select a file first', 'error');
  if (currentUser.credits < 1) return showToast('Not enough credits! Contact us to buy more.', 'error');
  // Block order if no checkers are online
  const onlineCheckers = DB.users.filter(u => u.role === 'checker' && u.approved && u.online !== false);
  if (onlineCheckers.length === 0) return showToast('⚠ No checkers are available right now. Please try again later or contact us on WhatsApp.', 'error');
  const message = document.getElementById('order-message').value.trim();

  const fileToStore = selectedFile;
  const reader = new FileReader();
  reader.onload = () => {
    currentUser.credits--;
    const order = {
      id: DB.nextOrderId++, clientId: currentUser.id, clientName: currentUser.name,
      fileName: fileToStore.name, fileData: reader.result, clientMessage: message || null,
      status: 'pending', checkerId: null, checkerName: null,
      placedAt: Date.now(), completedAt: null, timerEnd: null, reportUploaded: false,
      rejectedBy: [],
      verificationDeadline: null, verificationStatus: null, clientReport: null, adminResponse: null
    };
    DB.orders.push(order);

    // Save file URL directly
    order.fileUrl = reader.result;
    saveOrderStatus(order);
    saveUser(currentUser);

    addNotification(currentUser.id, 'Order Placed', `Your order #${order.id} for ${order.fileName} is pending. Waiting for a checker to accept.`);
    // Notify all available checkers
    DB.users.filter(u => u.role === 'checker' && u.approved).forEach(ck => {
      addNotification(ck.id, '📥 New Order Available', `Order #${order.id}: ${order.fileName} from ${currentUser.name} — accept or reject it.`);
    });
    showToast('Order placed! Waiting for a checker to accept.', 'success');

    clearFile();
    document.getElementById('order-message').value = '';
    refreshClientDash();
  };
  reader.readAsDataURL(fileToStore);
}

const MAX_ORDERS_PER_CHECKER = 5;

// Client cancels a pending order (only allowed while still pending) — refunds the credit
function cancelOrder(orderId) {
  const order = DB.orders.find(o => o.id === orderId);
  if (!order || !currentUser) return;
  if (order.status !== 'pending') {
    return showToast('This order has already been accepted and cannot be cancelled.', 'error');
  }
  // Refund the credit
  currentUser.credits++;
  // Remove the order
  DB.orders = DB.orders.filter(o => o.id !== orderId);
  deleteOrder(orderId);
  saveUser(currentUser);
  addNotification(currentUser.id, 'Order Cancelled', `Order #${orderId} was cancelled and your credit was refunded.`);
  showToast('Order cancelled. Your credit has been refunded.', 'success');
  refreshClientDash();
}

// ==================== CHECKER ACTIONS ====================
function toggleCheckerOnline() {
  if (!currentUser || currentUser.role !== 'checker') return;
  currentUser.online = !currentUser.online;
  saveUser(currentUser);
  updateCheckerOnlineUI();
  showToast(currentUser.online ? 'You are now Online — visible to clients.' : 'You are now Offline.', currentUser.online ? 'success' : 'info');
  refreshCheckerDash();
}

function updateCheckerOnlineUI() {
  if (!currentUser || currentUser.role !== 'checker') return;
  const btn = document.getElementById('checker-online-toggle');
  const dot = document.getElementById('online-dot');
  const label = document.getElementById('online-label');
  if (!btn) return;
  if (currentUser.online) {
    btn.style.background = 'var(--green-50)';
    btn.style.borderColor = '#bbf7d0';
    btn.style.color = 'var(--green-600)';
    dot.style.background = 'var(--green-500)';
    label.textContent = 'Online';
  } else {
    btn.style.background = '#f1f5f9';
    btn.style.borderColor = 'var(--gray-200)';
    btn.style.color = 'var(--gray-500)';
    dot.style.background = 'var(--gray-400)';
    label.textContent = 'Offline';
  }
}

function acceptOrder(orderId) {
  const order = DB.orders.find(o => o.id === orderId);
  if (!order || !currentUser) return;
  // Check capacity
  const myActive = DB.orders.filter(o => Number(o.checkerId) === Number(currentUser.id) && o.status === 'processing').length;
  if (myActive >= MAX_ORDERS_PER_CHECKER) {
    return showToast(`You already have ${MAX_ORDERS_PER_CHECKER} active orders. Complete one first.`, 'error');
  }
  order.checkerId = currentUser.id;
  order.checkerName = currentUser.name;
  order.status = 'processing';
  order.timerEnd = Date.now() + 20 * 60 * 1000; // 20-min timer starts on accept
  saveOrderStatus(order);
  addNotification(order.clientId, '✅ Order Accepted', `${currentUser.name} accepted your order #${order.id}. Report will be ready within 20 minutes.`);
  sendEmail(order.clientId, 'Your CheckPlag order was accepted', `Good news! Your order #${order.id} (${order.fileName}) has been accepted and your report will be ready within 20 minutes.`);
  showToast(`Order #${orderId} accepted! You have 20 minutes. Download the file and upload the report.`, 'success');
  refreshCheckerDash();
}

function rejectOrder(orderId) {
  const order = DB.orders.find(o => o.id === orderId);
  if (!order || !currentUser) return;
  if (!order.rejectedBy) order.rejectedBy = [];
  order.rejectedBy.push(currentUser.id);
  saveOrderStatus(order);
  addNotification(order.clientId, 'Order Update', `A checker passed on order #${order.id}. It's still pending for other checkers.`);
  showToast(`You rejected order #${orderId}. It remains available for other checkers.`, 'info');
  refreshCheckerDash();
}

// Download the client's original uploaded document (for checkers)
function downloadClientFile(orderId) {
  const order = DB.orders.find(o => o.id === orderId);
  if (!order) return showToast('Order not found.', 'error');
  
  // Use storage URL if available, otherwise local data
  const fileSource = order.fileUrl || order.fileData;
  if (!fileSource) return showToast('File not available. Client needs to re-upload.', 'error');
  
  const a = document.createElement('a');
  a.href = fileSource;
  a.download = order.fileName || `document-${orderId}`;
  a.target = '_blank';
  document.body.appendChild(a);
  a.click();
  document.body.removeChild(a);
  showToast(`Downloading ${order.fileName}...`, 'success');
}

function openUploadModal(orderId) {
  uploadingOrderId = orderId;
  // Reset modal state
  document.getElementById('report-plag-input').value = '';
  document.getElementById('report-ai-input').value = '';
  document.getElementById('report-ai-input').disabled = false;
  document.getElementById('ai-not-possible').checked = false;
  document.getElementById('ai-reason-wrap').style.display = 'none';
  document.getElementById('ai-reason').value = '';
  document.getElementById('upload-modal').classList.add('open');
}

function closeModal(id) { document.getElementById(id).classList.remove('open'); }

function submitReport() {
  const plagInput = document.getElementById('report-plag-input');
  const aiInput = document.getElementById('report-ai-input');
  const aiNotPossible = document.getElementById('ai-not-possible').checked;
  const aiReason = document.getElementById('ai-reason').value.trim();

  if (!plagInput.files.length) return showToast('Please upload the plagiarism report (required)', 'error');
  if (!aiNotPossible && !aiInput.files.length) return showToast('Please upload the AI report or check "AI report is not possible"', 'error');
  if (aiNotPossible && !aiReason) return showToast('Please provide a reason why AI report is not possible', 'error');

  const order = DB.orders.find(o => o.id === uploadingOrderId);
  if (!order) return;

  const plagFile = plagInput.files[0];
  const aiFile = aiNotPossible ? null : aiInput.files[0];

  const readFile = (file) => new Promise((resolve) => {
    if (!file) return resolve(null);
    const reader = new FileReader();
    reader.onload = () => resolve(reader.result);
    reader.onerror = () => resolve(null);
    reader.readAsDataURL(file);
  });

  // Close modal immediately and mark complete — don't wait for anything
  order.status = 'completed';
  order.completedAt = Date.now();
  order.reportUploaded = true;
  order.plagReport = plagFile ? plagFile.name : null;
  order.aiReport = aiFile ? aiFile.name : null;
  order.aiNotPossible = aiNotPossible;
  order.aiReason = aiNotPossible ? aiReason : null;
  order.verificationDeadline = Date.now() + (24 * 60 * 60 * 1000);
  order.verificationStatus = 'pending';

  closeModal('upload-modal');
  showToast('✅ Reports uploaded! Order marked as complete.', 'success');
  refreshCheckerDash();

  let notifMsg = `Your plagiarism report for "${order.fileName}" is ready to download.`;
  if (aiNotPossible) {
    notifMsg += ` AI report not available: ${aiReason}`;
  } else {
    notifMsg += ` AI detection report is also ready.`;
  }
  addNotification(order.clientId, 'Reports Ready! ✅', notifMsg);

  // Read files and save in background
  Promise.all([readFile(plagFile), readFile(aiFile)]).then(([plagData, aiData]) => {
    order.plagReportData = plagData;
    order.plagReportUrl = plagData;
    order.aiReportData = aiData;
    order.aiReportUrl = aiData;
    saveOrderStatus(order);
  }).catch(e => {
    // Even if file read fails, order is already marked complete
    saveOrderStatus(order);
    console.error('File read error:', e);
  });
}

// Real download — triggers actual file download from stored data
function downloadReport(orderId, type) {
  const order = DB.orders.find(o => o.id === orderId);
  if (!order) return;
  
  // Use local data first, fall back to storage URL
  const data = type === 'ai'
    ? (order.aiReportData || order.aiReportUrl)
    : (order.plagReportData || order.plagReportUrl);
  const name = type === 'ai' ? order.aiReport : order.plagReport;
  
  if (!data) {
    showToast('Report not available — checker needs to re-upload.', 'error');
    return;
  }
  const a = document.createElement('a');
  a.href = data;
  a.download = name || `report-${orderId}.pdf`;
  a.target = '_blank';
  document.body.appendChild(a);
  a.click();
  document.body.removeChild(a);
  showToast(`Downloading ${name}...`, 'success');
}

// ==================== NOTIFICATIONS ====================
function addNotification(userId, title, message) {
  const n = { id: DB.nextNotifId++, userId, title, message, time: Date.now(), read: false };
  DB.notifications.unshift(n);
  saveNotification(n);
}

function toggleNotifs() {
  document.getElementById('notif-panel').classList.toggle('open');
  document.getElementById('notif-overlay').classList.toggle('open');
  renderNotifs();
}

function renderNotifs() {
  if (!currentUser) return;
  const notifs = DB.notifications.filter(n => Number(n.userId) === Number(currentUser.id));
  const list = document.getElementById('notif-list');
  if (notifs.length === 0) {
    list.innerHTML = '<div style="padding:40px;text-align:center;color:var(--gray-400)">No notifications yet</div>';
    return;
  }
  list.innerHTML = notifs.map(n => `
    <div class="notif-item ${n.read ? '' : 'unread'}" onclick="this.classList.remove('unread')">
      <h5>${n.title}</h5>
      <p>${n.message}</p>
      <div class="notif-time">${timeAgo(n.time)}</div>
    </div>
  `).join('');
  // Mark as read and seen so they never ring again
  notifs.forEach(n => {
    n.read = true;
    seenNotifIds.add(n.id);
  });
  localStorage.setItem('cp_seen_notifs', JSON.stringify([...seenNotifIds]));
  updateNotifCounts();
}

// ==================== SOUND & NOTIFICATION SYSTEM ====================
// All notification IDs already alerted — loaded from localStorage so refresh doesn't reset
const seenNotifIds = new Set(JSON.parse(localStorage.getItem('cp_seen_notifs') || '[]'));
const seenChatIds = new Set(JSON.parse(localStorage.getItem('cp_seen_chats') || '[]'));
let soundEnabled = localStorage.getItem('cp_sound') !== 'off';
let lastShownNotifId = 0;
let notifPermission = 'default';
let soundInitialized = false; // prevents sound on first load

function toggleSound() {
  soundEnabled = !soundEnabled;
  localStorage.setItem('cp_sound', soundEnabled ? 'on' : 'off');
  ['sound-toggle-client','sound-toggle-checker','sound-toggle-admin'].forEach(id => {
    const el = document.getElementById(id);
    if (el) el.textContent = soundEnabled ? '🔊' : '🔇';
  });
  showToast(soundEnabled ? 'Notification sound ON 🔊' : 'Notification sound OFF 🔇', 'info');
}

function playNotifSound() {
  if (!soundEnabled) return;
  try {
    const ctx = new (window.AudioContext || window.webkitAudioContext)();
    const beeps = [
      { freq: 1500, start: 0.0,  dur: 0.25 },
      { freq: 1800, start: 0.3,  dur: 0.25 },
      { freq: 1500, start: 0.6,  dur: 0.25 },
      { freq: 1800, start: 0.9,  dur: 0.25 },
      { freq: 1500, start: 1.2,  dur: 0.25 },
      { freq: 1800, start: 1.5,  dur: 0.25 },
      { freq: 2000, start: 1.8,  dur: 0.3  },
      { freq: 1500, start: 2.15, dur: 0.3  },
    ];
    beeps.forEach(b => {
      ['square', 'sawtooth', 'triangle'].forEach(type => {
        const osc = ctx.createOscillator();
        const gain = ctx.createGain();
        osc.connect(gain);
        gain.connect(ctx.destination);
        osc.type = type;
        osc.frequency.setValueAtTime(b.freq, ctx.currentTime + b.start);
        gain.gain.setValueAtTime(0, ctx.currentTime + b.start);
        gain.gain.linearRampToValueAtTime(1.0, ctx.currentTime + b.start + 0.01);
        gain.gain.setValueAtTime(1.0, ctx.currentTime + b.start + b.dur - 0.03);
        gain.gain.linearRampToValueAtTime(0, ctx.currentTime + b.start + b.dur);
        osc.start(ctx.currentTime + b.start);
        osc.stop(ctx.currentTime + b.start + b.dur + 0.05);
      });
    });
  } catch(e) {}
}

async function requestNotifPermission() {
  if (!('Notification' in window)) return;
  if (Notification.permission === 'granted') { notifPermission = 'granted'; return; }
  if (Notification.permission !== 'denied') {
    const r = await Notification.requestPermission();
    notifPermission = r;
  }
}

function showBrowserNotif(title, message) {
  if (!soundEnabled) return;
  if (!('Notification' in window) || Notification.permission !== 'granted') return;
  const n = new Notification('CheckPlag — ' + title, { body: message, requireInteraction: false });
  setTimeout(() => n.close(), 5000);
  n.onclick = () => { window.focus(); n.close(); };
}

// Called every 8 seconds by liveSync interval — checks for NEW notifications only
function checkAndAlertNewNotifs() {
  if (!currentUser || !soundInitialized) return;

  // Get notifications that are NEW (not in seenNotifIds)
  const newNotifs = DB.notifications.filter(n =>
    Number(n.userId) === Number(currentUser.id) && !seenNotifIds.has(n.id)
  );

  if (newNotifs.length === 0) return;

  // Play sound once for new notifications
  playNotifSound();

  // Show browser popup for the most recent one
  const latest = newNotifs[0];
  if (latest.id !== lastShownNotifId) {
    showBrowserNotif(latest.title, latest.message);
    lastShownNotifId = latest.id;
  }

  // Add ALL new notifs to seen so they NEVER ring again
  newNotifs.forEach(n => seenNotifIds.add(n.id));
  localStorage.setItem('cp_seen_notifs', JSON.stringify([...seenNotifIds]));

  // Update badge count
  updateNotifCounts();
}

function updateNotifCounts() {
  if (!currentUser) return;

  // Count only notifications not yet seen
  const count = DB.notifications.filter(n =>
    Number(n.userId) === Number(currentUser.id) && !seenNotifIds.has(n.id)
  ).length;

  ['client-notif-count', 'checker-notif-count', 'admin-notif-count'].forEach(id => {
    const el = document.getElementById(id);
    if (el) { el.textContent = count; el.style.display = count > 0 ? 'flex' : 'none'; }
  });

  // Update sound button icons
  ['sound-toggle-client','sound-toggle-checker','sound-toggle-admin'].forEach(id => {
    const el = document.getElementById(id);
    if (el) el.textContent = soundEnabled ? '🔊' : '🔇';
  });

  // Update chat unread badges — use seenChatIds so sync doesn't reset them
  if (currentUser.role === 'client' || currentUser.role === 'checker') {
    const unreadChats = DB.chatMessages.filter(c =>
      Number(c.userId) === Number(currentUser.id) && c.fromRole === 'admin' && !seenChatIds.has(c.id)
    ).length;
    const badgeId = currentUser.role === 'client' ? 'client-chat-badge' : 'checker-chat-badge';
    const badge = document.getElementById(badgeId);
    if (badge) { badge.style.display = unreadChats > 0 ? 'inline-flex' : 'none'; badge.textContent = unreadChats; }
  } else if (currentUser.role === 'admin') {
    const unreadAdminChats = DB.chatMessages.filter(c => c.fromRole !== 'admin' && !seenChatIds.has(c.id)).length;
    const badge = document.getElementById('admin-chat-badge');
    if (badge) { badge.style.display = unreadAdminChats > 0 ? 'inline-flex' : 'none'; badge.textContent = unreadAdminChats; }
  }
}


function timeAgo(ts) {
  const diff = Date.now() - ts;
  const mins = Math.floor(diff / 60000);
  if (mins < 1) return 'Just now';
  if (mins < 60) return mins + 'm ago';
  const hrs = Math.floor(mins / 60);
  if (hrs < 24) return hrs + 'h ago';
  return Math.floor(hrs / 24) + 'd ago';
}

// Returns how long an order took to complete e.g. "14 min 32 sec"
function completionDuration(placedAt, completedAt) {
  if (!placedAt || !completedAt) return '—';
  const diff = completedAt - placedAt;
  const mins = Math.floor(diff / 60000);
  const secs = Math.floor((diff % 60000) / 1000);
  if (mins === 0) return `${secs} sec`;
  if (secs === 0) return `${mins} min`;
  return `${mins} min ${secs} sec`;
}

// ==================== TIMER ====================
function formatTimer(endTime) {
  const diff = endTime - Date.now();
  if (diff <= 0) return '<span style="color:var(--red-500);font-weight:700">Expired</span>';
  const mins = Math.floor(diff / 60000);
  const secs = Math.floor((diff % 60000) / 1000);
  return `<span class="timer-display">${String(mins).padStart(2, '0')}:${String(secs).padStart(2, '0')}</span>`;
}

// ==================== REFRESH DASHBOARDS ====================
function refreshClientDash() {
  if (!currentUser) return;
  const myOrders = DB.orders.filter(o => Number(o.clientId) === Number(currentUser.id)).sort((a, b) => a.placedAt - b.placedAt);
  document.getElementById('c-stat-total').textContent = myOrders.length;
  document.getElementById('c-stat-proc').textContent = myOrders.filter(o => o.status === 'processing').length;
  document.getElementById('c-stat-done').textContent = myOrders.filter(o => o.status === 'completed').length;
  document.getElementById('c-stat-credits').textContent = currentUser.credits;

  // Online Checkers list
  const onlineCheckers = DB.users.filter(u => u.role === 'checker' && u.approved && u.online !== false);
  const onlinePill = document.getElementById('online-count-pill');
  const onlineList = document.getElementById('online-checkers-list');

  // Disable Place Order button if no checkers online
  const placeOrderBtn = document.getElementById('place-order-btn');
  if (placeOrderBtn) {
    if (onlineCheckers.length === 0) {
      placeOrderBtn.disabled = true;
      placeOrderBtn.textContent = '⚠ No Checkers Online';
      placeOrderBtn.style.background = 'var(--gray-300)';
      placeOrderBtn.style.cursor = 'not-allowed';
    } else {
      placeOrderBtn.disabled = false;
      placeOrderBtn.textContent = 'Place Order (1 Credit)';
      placeOrderBtn.style.background = '';
      placeOrderBtn.style.cursor = '';
    }
  }
  if (onlinePill) {
    onlinePill.textContent = `${onlineCheckers.length} online`;
    onlinePill.classList.toggle('empty', onlineCheckers.length === 0);
  }
  if (onlineList) {
    if (onlineCheckers.length === 0) {
      onlineList.innerHTML = `
        <div class="empty-state">
          <div class="empty-icon">😴</div>
          <div style="font-weight:600;font-size:14px;color:var(--gray-500)">0 Online</div>
          <div style="font-size:12px;margin-top:4px">No checkers available right now</div>
          <div style="font-size:11px;margin-top:8px;color:var(--gray-400)">Your order will be processed once a checker comes online</div>
        </div>
      `;
    } else {
      onlineList.innerHTML = onlineCheckers.map(c => {
        const activeCount = DB.orders.filter(o => o.checkerId === c.id && o.status === 'processing').length;
        const isAtMax = activeCount >= MAX_ORDERS_PER_CHECKER;
        const isBusy = activeCount > 0;
        const completedCount = DB.orders.filter(o => o.checkerId === c.id && o.status === 'completed').length;
        let statusText = 'Available';
        let statusColor = 'var(--green-600)';
        let dotClass = '';
        if (isAtMax) { statusText = 'Full'; statusColor = 'var(--red-500)'; dotClass = 'busy'; }
        else if (isBusy) { statusText = `Busy (${activeCount}/5)`; statusColor = 'var(--amber-600)'; dotClass = 'busy'; }
        return `
          <div class="checker-item">
            <div class="user-avatar" style="background:var(--blue-100);color:var(--blue-700)">${c.name.charAt(0).toUpperCase()}</div>
            <div style="flex:1">
              <div style="font-weight:700;font-size:14px;color:var(--gray-800)">${c.name}</div>
              <div style="font-size:11px;color:var(--gray-500)">${completedCount} reports · ${activeCount}/5 active</div>
            </div>
            <div style="display:flex;align-items:center;gap:6px">
              <div class="checker-status-dot ${dotClass}"></div>
              <span style="font-size:11px;font-weight:700;color:${statusColor}">${statusText}</span>
            </div>
          </div>
        `;
      }).join('');
    }
  }

  const renderOrders = (orders, tbodyId) => {
    const tbody = document.getElementById(tbodyId);
    if (orders.length === 0) {
      tbody.innerHTML = '<tr><td colspan="6" style="text-align:center;color:var(--gray-400);padding:32px">No orders yet</td></tr>';
      return;
    }
    tbody.innerHTML = orders.map(o => {
      let statusHtml = `<span class="badge badge-${o.status}">${o.status.charAt(0).toUpperCase() + o.status.slice(1)}</span>`;
      let actionHtml = '<span style="color:var(--gray-400)">Waiting...</span>';

      if (o.status === 'pending') {
        statusHtml += '<br><span style="font-size:11px;color:var(--blue-600);font-weight:600;margin-top:4px;display:inline-block">⏳ Waiting for a checker to accept</span>';
        actionHtml = `<button class="btn btn-danger btn-sm" onclick="cancelOrder(${o.id})">✕ Cancel Order</button>`;
      }

      if (o.status === 'completed') {
        // Add verification status badge
        if (o.verificationStatus === 'passed') {
          statusHtml += '<br><span class="verify-badge verify-passed" style="margin-top:4px">✓ Verified</span>';
        } else if (o.verificationStatus === 'failed') {
          statusHtml += '<br><span class="verify-badge verify-failed" style="margin-top:4px">✗ Failed</span>';
        } else if (o.verificationStatus === 'pending') {
          const timeLeft = o.verificationDeadline - Date.now();
          if (timeLeft > 0) {
            const hrs = Math.floor(timeLeft / 3600000);
            statusHtml += `<br><span class="verify-badge verify-pending pulse" style="margin-top:4px">⏳ ${hrs}h to verify</span>`;
          } else {
            statusHtml += '<br><span class="verify-badge verify-passed" style="margin-top:4px">✓ Auto-verified</span>';
          }
        }

        actionHtml = '<div style="display:flex;flex-direction:column;gap:6px">';
        // Plagiarism report button
        if (o.plagReportData || o.plagReportUrl) {
          actionHtml += `<button class="btn btn-primary btn-sm" onclick="downloadReport(${o.id}, 'plag')">⬇ Plagiarism Report</button>`;
        } else {
          actionHtml += `<span style="font-size:12px;color:var(--gray-400)">📄 Plag report (session ended — ask checker to re-upload)</span>`;
        }
        // AI report or reason
        if (o.aiNotPossible) {
          actionHtml += `<div style="padding:8px 10px;background:#fee2e2;border-radius:8px;border-left:3px solid var(--red-500)">`;
          actionHtml += `<span style="font-size:12px;font-weight:700;color:var(--red-600)">⚠ AI Report Not Available</span>`;
          if (o.aiReason) {
            actionHtml += `<br><span style="font-size:11px;color:var(--red-700)">Reason: ${o.aiReason}</span>`;
          }
          actionHtml += `</div>`;
        } else if (o.aiReportData || o.aiReportUrl) {
          actionHtml += `<button class="btn btn-outline btn-sm" onclick="downloadReport(${o.id}, 'ai')">⬇ AI Report</button>`;
        } else if (o.aiReport) {
          actionHtml += `<span style="font-size:12px;color:var(--gray-400)">🤖 AI report (session ended — ask checker to re-upload)</span>`;
        }
        
        // Show Report Problem button only if pending and no report submitted yet
        if (o.verificationStatus === 'pending' && !o.clientReport) {
          actionHtml += `<button class="btn btn-danger btn-sm" onclick="openReportProblem(${o.id})">⚠ Report Problem</button>`;
        } else if (o.clientReport && o.verificationStatus === 'pending') {
          actionHtml += `<span style="font-size:11px;color:var(--amber-600);font-weight:600">⏳ Under review</span>`;
        } else if (o.adminResponse) {
          actionHtml += `<button class="btn btn-ghost btn-sm" onclick="showAdminResponse(${o.id})" style="font-size:11px">💬 Admin Response</button>`;
        }

        // Delete button for verified or failed orders
        if (o.verificationStatus === 'passed' || o.verificationStatus === 'failed') {
          actionHtml += `<button class="btn btn-ghost btn-sm" onclick="deleteCompletedOrder(${o.id})" style="color:var(--red-400);font-size:11px;margin-top:2px">🗑 Delete</button>`;
        }
        
        actionHtml += '</div>';
      }
      return `<tr>
        <td><strong>#${o.id}</strong></td>
        <td>📄 ${o.fileName}</td>
        <td>${statusHtml}</td>
        <td>${o.status === 'processing' ? formatTimer(o.timerEnd) : o.status === 'completed' ? `<span style="font-size:12px;color:var(--green-600);font-weight:600">⏱ ${completionDuration(o.placedAt, o.completedAt)}</span>` : '—'}</td>
        <td>${actionHtml}</td>
      </tr>`;
    }).join('');
  };

  renderOrders(myOrders.slice(-10).reverse(), 'client-orders-table');
  renderOrders(myOrders.reverse(), 'client-all-orders-table');
  updateNotifCounts();
}

function refreshCheckerDash() {
  if (!currentUser) return;
  // Pending orders available to accept — only if checker is online
  const isOnline = currentUser.online !== false;
  const pendingOrders = isOnline
    ? DB.orders.filter(o => o.status === 'pending' && (!o.rejectedBy || !o.rejectedBy.includes(currentUser.id)))
    : [];
  // My active (accepted) orders
  const myActiveOrders = DB.orders.filter(o => o.status === 'processing' && Number(o.checkerId) === Number(currentUser.id));
  const myCompleted = DB.orders.filter(o => o.status === 'completed' && Number(o.checkerId) === Number(currentUser.id));

  document.getElementById('ck-stat-active').textContent = `${myActiveOrders.length} / ${MAX_ORDERS_PER_CHECKER}`;
  document.getElementById('ck-stat-done').textContent = myCompleted.length;
  // Today's completed count
  const todayStart = new Date(); todayStart.setHours(0,0,0,0);
  const todayCount = myCompleted.filter(o => o.completedAt && o.completedAt >= todayStart.getTime()).length;
  document.getElementById('ck-stat-today').textContent = todayCount;
  document.getElementById('checker-count').textContent = myCompleted.length;

  const tbody = document.getElementById('checker-orders-table');
  let rows = '';

  // Pending orders section (available to pick)
  if (pendingOrders.length > 0) {
    rows += pendingOrders.map(o => {
      let messageHtml = '';
      if (o.clientMessage) {
        messageHtml = `<div style="margin-top:6px;padding:8px 10px;background:#fef3c7;border-left:3px solid var(--amber-500);border-radius:4px;font-size:12px;color:#92400e"><strong>💬 Client message:</strong> ${o.clientMessage}</div>`;
      }
      return `<tr style="background:#eef2ff">
        <td><strong>#${o.id}</strong></td>
        <td>${o.clientName}</td>
        <td>📄 ${o.fileName}<br><button class="btn btn-primary btn-sm" onclick="downloadClientFile(${o.id})" style="margin-top:6px">⬇ Download Document</button>${messageHtml}</td>
        <td><span class="badge badge-pending">⏳ Pending</span></td>
        <td><div style="display:flex;gap:6px"><button class="btn btn-success btn-sm" onclick="acceptOrder(${o.id})">✓ Accept</button><button class="btn btn-danger btn-sm" onclick="rejectOrder(${o.id})">✕ Reject</button></div></td>
      </tr>`;
    }).join('');
  }

  // My active orders section
  if (myActiveOrders.length > 0) {
    rows += myActiveOrders.map(o => {
      let messageHtml = '';
      if (o.clientMessage) {
        messageHtml = `<div style="margin-top:6px;padding:8px 10px;background:#fef3c7;border-left:3px solid var(--amber-500);border-radius:4px;font-size:12px;color:#92400e"><strong>💬 Client message:</strong> ${o.clientMessage}</div>`;
      }
      return `<tr>
        <td><strong>#${o.id}</strong></td>
        <td>${o.clientName}</td>
        <td>📄 ${o.fileName}<br><button class="btn btn-primary btn-sm" onclick="downloadClientFile(${o.id})" style="margin-top:6px">⬇ Download Document</button>${messageHtml}</td>
        <td>${formatTimer(o.timerEnd)}</td>
        <td><button class="btn btn-success btn-sm" onclick="openUploadModal(${o.id})">Upload Report</button></td>
      </tr>`;
    }).join('');
  }

  if (rows === '') {
    const offlineMsg = !isOnline ? '<br><span style="font-size:12px;color:var(--gray-500);font-weight:600">You are Offline — go Online to receive orders</span>' : '';
    tbody.innerHTML = `<tr><td colspan="5" style="text-align:center;color:var(--gray-400);padding:32px">No orders available right now${offlineMsg}</td></tr>`;
  } else {
    tbody.innerHTML = rows;
  }

  const histTbody = document.getElementById('checker-history-table');
  if (myCompleted.length === 0) {
    histTbody.innerHTML = '<tr><td colspan="5" style="text-align:center;color:var(--gray-400);padding:32px">No completed orders</td></tr>';
  } else {
    histTbody.innerHTML = myCompleted.map(o => {
      let verifyBadge = '';
      if (o.verificationStatus === 'passed') verifyBadge = '<span class="verify-badge verify-passed">✓ Passed</span>';
      else if (o.verificationStatus === 'failed') verifyBadge = '<span class="verify-badge verify-failed">✗ Failed</span>';
      else if (o.verificationStatus === 'pending') verifyBadge = '<span class="verify-badge verify-pending">⏳ Pending</span>';
      
      return `<tr>
        <td><strong>#${o.id}</strong></td><td>${o.clientName}</td><td>📄 ${o.fileName}</td>
        <td>${new Date(o.completedAt).toLocaleString()}<br><span style="font-size:11px;color:var(--green-600);font-weight:600">⏱ Completed in ${completionDuration(o.placedAt, o.completedAt)}</span></td>
        <td>${verifyBadge}</td>
        <td><button class="btn btn-ghost btn-sm" onclick="deleteCompletedOrder(${o.id})" style="color:var(--red-400)">🗑 Delete</button></td>
      </tr>`;
    }).join('');
  }
  updateNotifCounts();
}

function refreshAdminDash() {
  const clients = DB.users.filter(u => u.role === 'client');
  const checkers = DB.users.filter(u => u.role === 'checker');
  const allOrders = DB.orders;

  // Helper: check if timestamp is today
  const isToday = (ts) => {
    if (!ts) return false;
    const d = new Date(ts); const now = new Date();
    return d.getFullYear() === now.getFullYear() && d.getMonth() === now.getMonth() && d.getDate() === now.getDate();
  };

  const todayOrders = allOrders.filter(o => isToday(o.placedAt));
  const todayCompleted = allOrders.filter(o => o.status === 'completed' && isToday(o.completedAt));
  const todayProcessing = allOrders.filter(o => o.status === 'processing' && isToday(o.placedAt));

  // Top stats
  document.getElementById('a-stat-users').textContent = clients.length;
  document.getElementById('a-stat-orders').textContent = allOrders.length;
  document.getElementById('a-stat-proc').textContent = allOrders.filter(o => o.status === 'processing').length;
  document.getElementById('a-stat-checkers').textContent = checkers.filter(c => c.approved).length;

  // Today's date
  document.getElementById('a-today-date').textContent = new Date().toLocaleDateString('en-US', { weekday: 'long', year: 'numeric', month: 'long', day: 'numeric' });

  // Today's summary stats
  document.getElementById('a-today-total').textContent = todayOrders.length;
  document.getElementById('a-today-done').textContent = todayCompleted.length;
  document.getElementById('a-today-proc').textContent = todayProcessing.length;

  // Today's completed orders table
  const todayTbody = document.getElementById('a-today-orders-table');
  if (todayCompleted.length === 0) {
    todayTbody.innerHTML = '<tr><td colspan="6" style="text-align:center;color:var(--gray-400);padding:32px">No orders completed today yet</td></tr>';
  } else {
    todayTbody.innerHTML = todayCompleted.map(o => {
      let reportBtns = o.plagReportData || o.plagReportUrl
        ? `<button class="btn btn-primary btn-sm" onclick="downloadReport(${o.id}, 'plag')">⬇ Plag</button>`
        : `<span style="font-size:11px;color:var(--gray-400)">Plag file not in session</span>`;
      if (o.aiNotPossible) {
        reportBtns += ` <div style="margin-top:4px;padding:6px 8px;background:#fee2e2;border-radius:6px;font-size:11px;color:var(--red-600)"><strong>⚠ No AI Report</strong>${o.aiReason ? '<br>'+o.aiReason : ''}</div>`;
      } else if (o.aiReportData || o.aiReportUrl) {
        reportBtns += ` <button class="btn btn-outline btn-sm" onclick="downloadReport(${o.id}, 'ai')">⬇ AI</button>`;
      } else if (o.aiReport) {
        reportBtns += ` <span style="font-size:11px;color:var(--gray-400)">AI file not in session</span>`;
      }
      return `<tr>
        <td><strong>#${o.id}</strong></td>
        <td>📄 ${o.fileName}</td>
        <td>${o.clientName}</td>
        <td><strong style="color:var(--blue-700)">${o.checkerName || '—'}</strong></td>
        <td>${new Date(o.completedAt).toLocaleTimeString()}<br><span style="font-size:11px;color:var(--green-600);font-weight:600">⏱ ${completionDuration(o.placedAt, o.completedAt)}</span></td>
        <td>${reportBtns}</td>
      </tr>`;
    }).join('');
  }

  // Checker Performance Today
  const perfDiv = document.getElementById('a-checker-performance');
  const checkerStats = checkers.map(c => ({
    ...c,
    todayCount: todayCompleted.filter(o => o.checkerId === c.id).length,
    totalCount: allOrders.filter(o => o.checkerId === c.id && o.status === 'completed').length
  })).filter(c => c.todayCount > 0 || c.approved).sort((a, b) => b.todayCount - a.todayCount);

  if (checkerStats.length === 0) {
    perfDiv.innerHTML = '<p style="color:var(--gray-400)">No checker activity</p>';
  } else {
    perfDiv.innerHTML = checkerStats.map(c => `
      <div class="user-row" style="align-items:center">
        <div class="user-avatar" style="background:${c.todayCount > 0 ? '#dcfce7' : '#f1f5f9'};color:${c.todayCount > 0 ? '#166534' : '#94a3b8'}">${c.name.charAt(0)}</div>
        <div style="flex:1">
          <div style="font-weight:700;font-size:14px">${c.name}</div>
          <div style="font-size:12px;color:var(--gray-500)">@${c.username}</div>
        </div>
        <div style="text-align:center;padding:0 16px">
          <div style="font-size:22px;font-weight:800;color:${c.todayCount > 0 ? 'var(--green-600)' : 'var(--gray-400)'};font-family:Fraunces,serif">${c.todayCount}</div>
          <div style="font-size:10px;color:var(--gray-400);text-transform:uppercase;font-weight:600">Today</div>
        </div>
        <div style="text-align:center;padding:0 16px">
          <div style="font-size:22px;font-weight:800;color:var(--blue-700);font-family:Fraunces,serif">${c.totalCount}</div>
          <div style="font-size:10px;color:var(--gray-400);text-transform:uppercase;font-weight:600">All Time</div>
        </div>
      </div>
    `).join('');
  }

  // Admin ALL orders table (with view report buttons)
  const adminTbody = document.getElementById('admin-orders-table');
  adminTbody.innerHTML = allOrders.length === 0
    ? '<tr><td colspan="7" style="text-align:center;color:var(--gray-400);padding:32px">No orders</td></tr>'
    : [...allOrders].reverse().map(o => {
      let timeCol = o.status === 'processing' ? formatTimer(o.timerEnd) : (o.completedAt ? `${new Date(o.completedAt).toLocaleString()}<br><span style="font-size:11px;color:var(--green-600);font-weight:600">⏱ ${completionDuration(o.placedAt, o.completedAt)}</span>` : '—');
      let reportCol = '—';
      if (o.status === 'completed') {
        reportCol = '<div style="display:flex;flex-direction:column;gap:4px">';
        // Plag report
        if (o.plagReportData || o.plagReportUrl) {
          reportCol += `<button class="btn btn-primary btn-sm" onclick="downloadReport(${o.id}, 'plag')">⬇ Plag Report</button>`;
        } else {
          reportCol += `<span style="font-size:11px;color:var(--gray-400)">Plag file not in session</span>`;
        }
        // AI report
        if (o.aiNotPossible) {
          reportCol += `<div style="padding:6px 8px;background:#fee2e2;border-radius:6px;margin-top:2px">`;
          reportCol += `<span style="font-size:11px;font-weight:700;color:var(--red-600)">⚠ AI Not Available</span>`;
          if (o.aiReason) reportCol += `<br><span style="font-size:10px;color:var(--red-700)">${o.aiReason}</span>`;
          reportCol += `</div>`;
        } else if (o.aiReportData || o.aiReportUrl) {
          reportCol += `<button class="btn btn-outline btn-sm" onclick="downloadReport(${o.id}, 'ai')">⬇ AI Report</button>`;
        } else if (o.aiReport) {
          reportCol += `<span style="font-size:11px;color:var(--gray-400)">AI file not in session</span>`;
        }
        reportCol += '</div>';
      }
      return `<tr>
        <td><strong>#${o.id}</strong></td><td>${o.clientName}</td><td>📄 ${o.fileName}</td>
        <td><span class="badge badge-${o.status}">${o.status.charAt(0).toUpperCase() + o.status.slice(1)}</span></td>
        <td>${o.checkerName || '—'}</td>
        <td>${timeCol}</td>
        <td>${reportCol}</td>
        <td>${o.status === 'completed' ? `<button class="btn btn-ghost btn-sm" onclick="deleteCompletedOrder(${o.id})" style="color:var(--red-400)">🗑</button>` : '—'}</td>
      </tr>`;
    }).join('');

  // Users list
  const usersDiv = document.getElementById('admin-users-list');
  usersDiv.innerHTML = clients.length === 0 ? '<p style="color:var(--gray-400)">No clients</p>' : clients.map(u => {
    const orderCount = DB.orders.filter(o => Number(o.clientId) === Number(u.id)).length;
    const creditsUsed = DB.orders.filter(o => Number(o.clientId) === Number(u.id) && o.status !== 'pending').length;
    return `
    <div class="user-row">
      <div class="user-avatar">${u.name.charAt(0)}</div>
      <div style="flex:1">
        <div style="font-weight:700;font-size:14px">${u.name}</div>
        <div style="font-size:12px;color:var(--gray-500)">@${u.username} · ${orderCount} orders · ${creditsUsed} credits used</div>
      </div>
      <div style="display:flex;align-items:center;gap:8px">
        <div style="font-size:13px;font-weight:700;color:var(--blue-700)">${u.credits} credits</div>
        <button class="btn btn-primary btn-sm" onclick="openUserDetail(${u.id})">View</button>
      </div>
    </div>`;
  }).join('');

  // Checkers list
  const checkersDiv = document.getElementById('admin-checkers-list');
  checkersDiv.innerHTML = checkers.length === 0 ? '<p style="color:var(--gray-400)">No checkers yet. Create one above.</p>' : checkers.map(c => {
    const completedCount = DB.orders.filter(o => Number(o.checkerId) === Number(c.id) && o.status === 'completed').length;
    return `<div class="user-row">
      <div class="user-avatar" style="background:${c.approved ? '#dcfce7' : '#fee2e2'};color:${c.approved ? '#166534' : '#991b1b'}">${c.name.charAt(0)}</div>
      <div style="flex:1">
        <div style="font-weight:700;font-size:14px">${c.name} <span class="badge ${c.approved ? 'badge-completed' : 'badge-rejected'}" style="margin-left:6px">${c.approved ? 'Active' : 'Disabled'}</span></div>
        <div style="font-size:12px;color:var(--gray-500)">@${c.username} · ${completedCount} reports completed</div>
      </div>
      <div style="display:flex;gap:6px">
        <button class="btn btn-white btn-sm" onclick="openUserDetail(${c.id})">View</button>
        ${c.approved
          ? `<button class="btn btn-danger btn-sm" onclick="toggleCheckerStatus(${c.id}, false)">Disable</button>`
          : `<button class="btn btn-success btn-sm" onclick="toggleCheckerStatus(${c.id}, true)">Enable</button>`
        }
        <button class="btn btn-ghost btn-sm" onclick="deleteChecker(${c.id})" style="color:var(--red-500)">🗑</button>
      </div>
    </div>`;
  }).join('');

  // Credit user select — only rebuild if the option list changed, preserve current selection
  const sel = document.getElementById('credit-user-select');
  const newOptionsHtml = clients.map(u => `<option value="${u.id}">${u.name} (@${u.username}) — ${u.credits} credits</option>`).join('');
  const newSignature = clients.map(u => `${u.id}:${u.credits}`).join('|');
  if (sel.dataset.signature !== newSignature) {
    const prevValue = sel.value;
    sel.innerHTML = newOptionsHtml;
    if (prevValue && clients.some(u => String(u.id) === prevValue)) {
      sel.value = prevValue;
    }
    sel.dataset.signature = newSignature;
  }

  // Problem Reports table — show all orders where client reported a problem
  const problemOrders = allOrders.filter(o => o.clientReport && o.clientReport.trim() !== '' && !o.adminResponse);
  const problemBadge = document.getElementById('problem-count-badge');
  if (problemBadge) {
    problemBadge.textContent = problemOrders.length + ' pending';
    problemBadge.style.display = problemOrders.length > 0 ? 'inline-block' : 'none';
  }
  
  const problemTbody = document.getElementById('admin-problems-table');
  if (!problemTbody) return;
  if (problemOrders.length === 0) {
    problemTbody.innerHTML = '<tr><td colspan="7" style="text-align:center;color:var(--gray-400);padding:32px">No problem reports</td></tr>';
  } else {
    problemTbody.innerHTML = problemOrders.map(o => `<tr style="background:var(--red-50)">
      <td><strong>#${o.id}</strong></td>
      <td>📄 ${o.fileName}</td>
      <td>${o.clientName}</td>
      <td>${o.checkerName || '—'}</td>
      <td style="max-width:300px"><span style="font-size:13px;color:var(--red-700)">"${(o.clientReport||'').substring(0, 80)}${(o.clientReport||'').length > 80 ? '...' : ''}"</span></td>
      <td><span class="verify-badge verify-pending">Needs Review</span></td>
      <td><button class="btn btn-primary btn-sm" onclick="openAdminReview(${o.id})">Review</button></td>
    </tr>`).join('');
  }

  // Auto-refresh messages list and count
  renderAdminMessages();

  // Checker track record table
  const trackTbody = document.getElementById('admin-checker-track-table');
  if (trackTbody) {
    const now = Date.now();
    const todayStart = new Date(); todayStart.setHours(0,0,0,0);
    const yesterdayStart = new Date(todayStart); yesterdayStart.setDate(yesterdayStart.getDate()-1);
    const weekStart = new Date(todayStart); weekStart.setDate(weekStart.getDate()-7);
    const monthStart = new Date(todayStart); monthStart.setDate(1);

    if (checkers.length === 0) {
      trackTbody.innerHTML = '<tr><td colspan="7" style="text-align:center;color:var(--gray-400);padding:24px">No checkers yet</td></tr>';
    } else {
      trackTbody.innerHTML = checkers.map(c => {
        const cOrders = allOrders.filter(o => Number(o.checkerId) === Number(c.id) && o.status === 'completed' && o.completedAt);
        const today = cOrders.filter(o => o.completedAt >= todayStart.getTime()).length;
        const yesterday = cOrders.filter(o => o.completedAt >= yesterdayStart.getTime() && o.completedAt < todayStart.getTime()).length;
        const week = cOrders.filter(o => o.completedAt >= weekStart.getTime()).length;
        const month = cOrders.filter(o => o.completedAt >= monthStart.getTime()).length;
        const allTime = cOrders.length;
        const statusBadge = c.approved
          ? `<span style="color:var(--green-600);font-weight:700">● Active</span>`
          : `<span style="color:var(--red-500);font-weight:700">● Disabled</span>`;
        return `<tr>
          <td><strong>${c.name}</strong><br><span style="font-size:11px;color:var(--gray-400)">@${c.username}</span></td>
          <td><span style="font-size:18px;font-weight:700;color:var(--blue-700)">${today}</span></td>
          <td><span style="font-size:18px;font-weight:700;color:var(--gray-600)">${yesterday}</span></td>
          <td><span style="font-size:18px;font-weight:700;color:var(--blue-600)">${week}</span></td>
          <td><span style="font-size:18px;font-weight:700;color:var(--green-600)">${month}</span></td>
          <td><span style="font-size:18px;font-weight:700;color:var(--ink)">${allTime}</span></td>
          <td>${statusBadge}</td>
        </tr>`;
      }).join('');
    }
  }

  updateNotifCounts();
}

// ==================== USER DETAIL MODAL ====================
let viewingUserId = null;

function openUserDetail(userId) {
  const user = DB.users.find(u => Number(u.id) === Number(userId));
  if (!user) return;
  viewingUserId = userId;

  // Populate header
  document.getElementById('ud-title').textContent = user.role === 'checker' ? '🔍 Checker Details' : '👤 Client Details';
  document.getElementById('ud-avatar').textContent = user.name.charAt(0).toUpperCase();
  document.getElementById('ud-name').textContent = user.name;
  document.getElementById('ud-role').textContent = user.role.toUpperCase();
  document.getElementById('ud-username').textContent = user.username;
  document.getElementById('ud-password').textContent = user.password;
  document.getElementById('ud-credits').textContent = user.credits + ' credits';
  document.getElementById('ud-since').textContent = 'Active user';

  // Stats
  const userOrders = user.role === 'client'
    ? DB.orders.filter(o => Number(o.clientId) === Number(userId))
    : DB.orders.filter(o => Number(o.checkerId) === Number(userId) && o.status === 'completed');

  const totalOrders = userOrders.length;
  const completedOrders = userOrders.filter(o => o.status === 'completed').length;
  const pendingOrders = userOrders.filter(o => o.status === 'pending' || o.status === 'processing').length;
  const creditsUsed = user.role === 'client' ? userOrders.filter(o => o.status !== 'pending' || o.status === 'completed').length : 0;

  const statsEl = document.getElementById('ud-stats');
  if (user.role === 'client') {
    statsEl.innerHTML = `
      <div style="background:white;padding:10px;border-radius:8px;border:1px solid var(--gray-200);text-align:center">
        <div style="font-size:22px;font-weight:700;color:var(--blue-700);font-family:Fraunces,serif">${totalOrders}</div>
        <div style="font-size:10px;color:var(--gray-500);font-weight:600;text-transform:uppercase">Total Orders</div>
      </div>
      <div style="background:white;padding:10px;border-radius:8px;border:1px solid var(--gray-200);text-align:center">
        <div style="font-size:22px;font-weight:700;color:var(--green-600);font-family:Fraunces,serif">${completedOrders}</div>
        <div style="font-size:10px;color:var(--gray-500);font-weight:600;text-transform:uppercase">Completed</div>
      </div>
      <div style="background:white;padding:10px;border-radius:8px;border:1px solid var(--gray-200);text-align:center">
        <div style="font-size:22px;font-weight:700;color:var(--amber-500);font-family:Fraunces,serif">${pendingOrders}</div>
        <div style="font-size:10px;color:var(--gray-500);font-weight:600;text-transform:uppercase">Active</div>
      </div>
      <div style="background:white;padding:10px;border-radius:8px;border:1px solid var(--gray-200);text-align:center">
        <div style="font-size:22px;font-weight:700;color:var(--blue-600);font-family:Fraunces,serif">${user.credits}</div>
        <div style="font-size:10px;color:var(--gray-500);font-weight:600;text-transform:uppercase">Credits Left</div>
      </div>
    `;
  } else {
    const passedOrders = userOrders.filter(o => o.verificationStatus === 'passed').length;
    const failedOrders = userOrders.filter(o => o.verificationStatus === 'failed').length;
    statsEl.innerHTML = `
      <div style="background:white;padding:10px;border-radius:8px;border:1px solid var(--gray-200);text-align:center">
        <div style="font-size:22px;font-weight:700;color:var(--blue-700);font-family:Fraunces,serif">${totalOrders}</div>
        <div style="font-size:10px;color:var(--gray-500);font-weight:600;text-transform:uppercase">Reports Done</div>
      </div>
      <div style="background:white;padding:10px;border-radius:8px;border:1px solid var(--gray-200);text-align:center">
        <div style="font-size:22px;font-weight:700;color:var(--green-600);font-family:Fraunces,serif">${passedOrders}</div>
        <div style="font-size:10px;color:var(--gray-500);font-weight:600;text-transform:uppercase">Passed</div>
      </div>
      <div style="background:white;padding:10px;border-radius:8px;border:1px solid var(--gray-200);text-align:center">
        <div style="font-size:22px;font-weight:700;color:var(--red-500);font-family:Fraunces,serif">${failedOrders}</div>
        <div style="font-size:10px;color:var(--gray-500);font-weight:600;text-transform:uppercase">Failed</div>
      </div>
      <div style="background:white;padding:10px;border-radius:8px;border:1px solid var(--gray-200);text-align:center">
        <div style="font-size:22px;font-weight:700;color:var(--amber-500);font-family:Fraunces,serif">${user.approved ? '✓' : '✗'}</div>
        <div style="font-size:10px;color:var(--gray-500);font-weight:600;text-transform:uppercase">Status</div>
      </div>
    `;
  }

  // Order history
  const ordersEl = document.getElementById('ud-orders');
  if (userOrders.length === 0) {
    ordersEl.innerHTML = '<p style="color:var(--gray-400);font-size:13px;text-align:center;padding:16px">No orders yet</p>';
  } else {
    ordersEl.innerHTML = [...userOrders].reverse().map(o => `
      <div style="display:flex;justify-content:space-between;align-items:center;padding:8px 10px;background:white;border-radius:8px;margin-bottom:6px;border:1px solid var(--gray-200)">
        <div>
          <span style="font-weight:700;font-size:13px;color:var(--ink)">#${o.id}</span>
          <span style="font-size:12px;color:var(--gray-500);margin-left:8px">📄 ${o.fileName}</span>
        </div>
        <div style="display:flex;align-items:center;gap:8px">
          ${o.completedAt ? `<span style="font-size:11px;color:var(--green-600)">⏱ ${completionDuration(o.placedAt, o.completedAt)}</span>` : ''}
          <span class="badge badge-${o.status}" style="font-size:11px">${o.status.charAt(0).toUpperCase() + o.status.slice(1)}</span>
        </div>
      </div>
    `).join('');
  }

  document.getElementById('user-detail-modal').classList.add('open');
}

function deleteUserFromModal() {
  const user = DB.users.find(u => Number(u.id) === Number(viewingUserId));
  if (!user) return;
  if (user.role === 'admin') return showToast('Cannot delete admin account', 'error');

  DB.users = DB.users.filter(u => Number(u.id) !== Number(viewingUserId));
  deleteUser(viewingUserId);
  closeModal('user-detail-modal');
  showToast(`Account "${user.name}" deleted.`, 'info');
  refreshAdminDash();
}

function toggleCheckerStatus(id, enable) {
  const user = DB.users.find(u => u.id === id);
  if (user) {
    user.approved = enable;
    saveUser(user);
    showToast(enable ? `${user.name} has been enabled.` : `${user.name} has been disabled.`, enable ? 'success' : 'info');
  }
  refreshAdminDash();
}

function deleteChecker(id) {
  const user = DB.users.find(u => u.id === id);
  if (user) {
    DB.users = DB.users.filter(u => u.id !== id);
    deleteUser(id);
    showToast(`Checker "${user.name}" has been deleted.`, 'info');
  }
  refreshAdminDash();
}

function adminCreateChecker() {
  const name = document.getElementById('new-checker-name').value.trim();
  const username = document.getElementById('new-checker-username').value.trim();
  const pass = document.getElementById('new-checker-pass').value;
  if (!name || !username || !pass) return showToast('Please fill in all fields', 'error');
  if (DB.users.find(u => u.username === username)) return showToast('Username already taken', 'error');
  const newChecker = { id: DB.nextUserId++, name, username, password: pass, role: 'checker', credits: 0, approved: true, online: true };
  DB.users.push(newChecker);
  saveUser(newChecker);
  document.getElementById('new-checker-name').value = '';
  document.getElementById('new-checker-username').value = '';
  document.getElementById('new-checker-pass').value = '';
  const resultEl = document.getElementById('checker-create-result');
  resultEl.style.color = 'var(--green-600)';
  resultEl.textContent = `✅ Checker "${name}" created! Username: ${username}`;
  showToast(`Checker account "${name}" created successfully!`, 'success');
  refreshAdminDash();
}

function adminAddCredits(action) {
  const userId = parseInt(document.getElementById('credit-user-select').value);
  const amount = parseInt(document.getElementById('credit-amount').value);
  const resultEl = document.getElementById('credit-result');
  
  if (!amount || amount < 1) return showToast('Enter a valid amount', 'error');
  const user = DB.users.find(u => u.id === userId);
  if (!user) return showToast('Please select a user', 'error');
  
  resultEl.style.display = 'block';
  
  if (action === 'add') {
    user.credits += amount;
    saveUser(user);
    addNotification(userId, 'Credits Added! 💳', `${amount} credit(s) have been added to your account by admin.`);
    resultEl.style.background = '#dcfce7';
    resultEl.style.color = '#166534';
    resultEl.textContent = `✅ Added ${amount} credits to ${user.name}. New balance: ${user.credits}`;
    showToast(`Added ${amount} credits to ${user.name}`, 'success');
  } else if (action === 'deduct') {
    if (user.credits < amount) {
      resultEl.style.background = '#fee2e2';
      resultEl.style.color = '#991b1b';
      resultEl.textContent = `❌ Cannot deduct ${amount} credits. ${user.name} only has ${user.credits} credits.`;
      showToast(`Not enough credits to deduct`, 'error');
      return;
    }
    user.credits -= amount;
    saveUser(user);
    addNotification(userId, 'Credits Deducted', `${amount} credit(s) have been deducted from your account by admin.`);
    resultEl.style.background = '#fee2e2';
    resultEl.style.color = '#991b1b';
    resultEl.textContent = `➖ Deducted ${amount} credits from ${user.name}. New balance: ${user.credits}`;
    showToast(`Deducted ${amount} credits from ${user.name}`, 'info');
  }
  
  refreshAdminDash();
}

// ==================== PROBLEM REPORT & VERIFICATION SYSTEM ====================
let currentReportOrderId = null;
let currentReviewOrderId = null;

function openReportProblem(orderId) {
  const order = DB.orders.find(o => o.id === orderId);
  if (!order) return;
  currentReportOrderId = orderId;
  document.getElementById('report-order-id').textContent = orderId;
  document.getElementById('report-file-name').textContent = order.fileName;
  document.getElementById('problem-description').value = '';
  document.getElementById('report-problem-modal').classList.add('open');
}

function submitProblemReport() {
  const problem = document.getElementById('problem-description').value.trim();
  if (!problem) return showToast('Please describe the problem', 'error');
  const order = DB.orders.find(o => o.id === currentReportOrderId);
  if (!order) return;
  
  order.clientReport = problem;
  saveOrderStatus(order);
  addNotification(1, 'Problem Reported', `Client reported a problem with order #${order.id}: ${order.fileName}`);
  showToast('Problem reported. Admin will review and respond soon.', 'success');
  closeModal('report-problem-modal');
  refreshClientDash();
}

function showAdminResponse(orderId) {
  const order = DB.orders.find(o => o.id === orderId);
  if (!order || !order.adminResponse) return;
  showToast(`Admin: ${order.adminResponse}`, 'info');
}

function openAdminReview(orderId) {
  const order = DB.orders.find(o => o.id === orderId);
  if (!order) return;
  currentReviewOrderId = orderId;
  
  document.getElementById('review-order-info').innerHTML = `
    <div style="display:flex;justify-content:space-between;align-items:center">
      <div>
        <strong style="font-size:16px">Order #${order.id}</strong><br>
        <span style="font-size:13px;color:var(--gray-500)">Client: ${order.clientName} | File: ${order.fileName}</span><br>
        <span style="font-size:13px;color:var(--gray-500)">Checker: ${order.checkerName}</span>
      </div>
      <div style="text-align:right">
        <span class="badge badge-${order.status}">${order.status}</span>
      </div>
    </div>
  `;
  document.getElementById('review-problem-text').textContent = order.clientReport || 'No problem reported';
  document.getElementById('admin-response-text').value = '';
  document.getElementById('admin-review-modal').classList.add('open');
}

function resolveOrderProblem(action) {
  const order = DB.orders.find(o => o.id === currentReviewOrderId);
  if (!order) return;
  const client = DB.users.find(u => u.id === order.clientId);
  const adminResponse = document.getElementById('admin-response-text').value.trim();
  
  if (action === 'refund-pass') {
    client.credits += 1;
    order.verificationStatus = 'passed';
    order.adminResponse = adminResponse || 'Your credit has been refunded. Order marked as passed.';
    saveUser(client); saveOrderStatus(order);
    addNotification(order.clientId, 'Problem Resolved ✅', `Order #${order.id}: Credit refunded. ${order.adminResponse}`);
    showToast('Order passed, credit refunded to client.', 'success');
  } else if (action === 'refund-fail') {
    client.credits += 1;
    order.verificationStatus = 'failed';
    order.adminResponse = adminResponse || 'Report was invalid. Credit refunded, order marked as failed.';
    saveUser(client); saveOrderStatus(order);
    addNotification(order.clientId, 'Order Failed ❌', `Order #${order.id}: ${order.adminResponse}`);
    addNotification(order.checkerId, 'Order Failed ❌', `Your report for order #${order.id} was marked as failed by admin.`);
    showToast('Order failed, credit refunded to client.', 'info');
  } else if (action === 'pass-only') {
    order.verificationStatus = 'passed';
    order.adminResponse = adminResponse || 'Order reviewed and approved. No refund issued.';
    saveOrderStatus(order);
    addNotification(order.clientId, 'Order Verified ✅', `Order #${order.id}: ${order.adminResponse}`);
    showToast('Order marked as passed, no refund.', 'success');
  }
  
  closeModal('admin-review-modal');
  refreshAdminDash();
}

// Auto-verify orders after 24 hours
function checkAutoVerification() {
  DB.orders.forEach(order => {
    if (order.status === 'completed' && order.verificationStatus === 'pending') {
      if (Date.now() > order.verificationDeadline && !order.clientReport) {
        order.verificationStatus = 'passed';
        saveOrderStatus(order);
        addNotification(order.checkerId, 'Order Verified ✅', `Order #${order.id} has been automatically verified (24h passed).`);
      }
    }
  });
}

// Run verification check every minute
setInterval(checkAutoVerification, 60000);

// ==================== CLIENT-ADMIN CHAT ====================
function sendChatToAdmin() {
  const subject = document.getElementById('chat-subject').value.trim();
  const message = document.getElementById('chat-message').value.trim();
  if (!subject || !message) return showToast('Please fill in subject and message', 'error');
  if (!currentUser) return;
  
  const newChat = {
    id: DB.nextChatId++,
    userId: currentUser.id,
    userName: currentUser.name,
    userRole: 'client',
    fromRole: 'client',
    subject: subject,
    message: message,
    time: Date.now(),
    read: false
  };
  DB.chatMessages.push(newChat);
  saveChat(newChat);
  
  addNotification(1, '💬 New Message from Client', `${currentUser.name}: "${subject}"`);
  
  document.getElementById('chat-subject').value = '';
  document.getElementById('chat-message').value = '';
  showToast('Message sent to admin! You\'ll be notified when they reply.', 'success');
  renderClientChatHistory();
}

function checkerSendChatToAdmin() {
  const subject = document.getElementById('checker-chat-subject').value.trim();
  const message = document.getElementById('checker-chat-message').value.trim();
  if (!subject || !message) return showToast('Please fill in subject and message', 'error');
  if (!currentUser) return;
  
  const newChat = {
    id: DB.nextChatId++,
    userId: currentUser.id,
    userName: currentUser.name,
    userRole: 'checker',
    fromRole: 'checker',
    subject: subject,
    message: message,
    time: Date.now(),
    read: false
  };
  DB.chatMessages.push(newChat);
  saveChat(newChat);
  
  addNotification(1, '💬 New Message from Checker', `${currentUser.name}: "${subject}"`);
  
  document.getElementById('checker-chat-subject').value = '';
  document.getElementById('checker-chat-message').value = '';
  showToast('Message sent to admin! You\'ll be notified when they reply.', 'success');
  renderCheckerChatHistory();
}

function renderCheckerChatHistory() {
  if (!currentUser) return;
  const myChats = DB.chatMessages
    .filter(c => Number(c.userId) === Number(currentUser.id))
    .sort((a, b) => b.time - a.time);
  
  const container = document.getElementById('checker-chat-history');
  if (!container) return;
  
  if (myChats.length === 0) {
    container.innerHTML = '<div class="empty-state"><div class="empty-icon">💭</div><div style="font-weight:600;color:var(--gray-500)">No messages yet</div><div style="font-size:12px;margin-top:4px">Send your first message above</div></div>';
    return;
  }
  
  container.innerHTML = myChats.map(c => {
    const isFromAdmin = c.fromRole === 'admin';
    return `
      <div style="padding:14px;border-radius:10px;margin-bottom:10px;border-left:4px solid ${isFromAdmin ? 'var(--green-500)' : 'var(--blue-500)'};background:${isFromAdmin ? '#f0fdf4' : '#eff6ff'}">
        <div style="display:flex;justify-content:space-between;align-items:start;margin-bottom:6px">
          <strong style="color:${isFromAdmin ? 'var(--green-700)' : 'var(--blue-700)'};font-size:14px">${isFromAdmin ? '👨‍💼 Admin' : '🔍 You'} ${c.subject ? `· ${c.subject}` : ''}</strong>
          <span style="font-size:11px;color:var(--gray-400)">${timeAgo(c.time)}</span>
        </div>
        <div style="font-size:14px;color:var(--gray-700);line-height:1.5;white-space:pre-wrap">${c.message}</div>
      </div>
    `;
  }).join('');
}

function renderClientChatHistory() {
  if (!currentUser) return;
  const myChats = DB.chatMessages
    .filter(c => Number(c.userId) === Number(currentUser.id))
    .sort((a, b) => b.time - a.time);
  
  const container = document.getElementById('client-chat-history');
  if (!container) return;
  
  if (myChats.length === 0) {
    container.innerHTML = '<div class="empty-state"><div class="empty-icon">💭</div><div style="font-weight:600;color:var(--gray-500)">No messages yet</div><div style="font-size:12px;margin-top:4px">Send your first message above</div></div>';
    return;
  }
  
  container.innerHTML = myChats.map(c => {
    const isFromAdmin = c.fromRole === 'admin';
    return `
      <div style="padding:14px;border-radius:10px;margin-bottom:10px;border-left:4px solid ${isFromAdmin ? 'var(--green-500)' : 'var(--blue-500)'};background:${isFromAdmin ? '#f0fdf4' : '#eff6ff'}">
        <div style="display:flex;justify-content:space-between;align-items:start;margin-bottom:6px">
          <strong style="color:${isFromAdmin ? 'var(--green-700)' : 'var(--blue-700)'};font-size:14px">${isFromAdmin ? '👨‍💼 Admin' : '👤 You'} ${c.subject ? `· ${c.subject}` : ''}</strong>
          <span style="font-size:11px;color:var(--gray-400)">${timeAgo(c.time)}</span>
        </div>
        <div style="font-size:14px;color:var(--gray-700);line-height:1.5;white-space:pre-wrap">${c.message}</div>
      </div>
    `;
  }).join('');
}

function renderAdminMessages() {
  const container = document.getElementById('admin-messages-list');
  const badge = document.getElementById('msg-count-badge');
  if (!container) return;
  
  // Group messages by user
  const grouped = {};
  DB.chatMessages.forEach(c => {
    if (!grouped[c.userId]) grouped[c.userId] = { userName: c.userName, userRole: c.userRole, messages: [] };
    grouped[c.userId].messages.push(c);
  });
  
  // Count unread from users (not admin)
  const unreadCount = DB.chatMessages.filter(c => c.fromRole !== 'admin' && !c.read).length;
  if (badge) {
    badge.textContent = unreadCount + ' unread';
    badge.style.display = unreadCount > 0 ? 'inline-block' : 'none';
  }
  
  const userIds = Object.keys(grouped);
  if (userIds.length === 0) {
    container.innerHTML = '<div class="empty-state"><div class="empty-icon">💬</div><div style="font-weight:600;color:var(--gray-500)">No messages yet</div></div>';
    return;
  }
  
  container.innerHTML = userIds.map(uid => {
    const group = grouped[uid];
    const sortedMsgs = group.messages.sort((a, b) => a.time - b.time);
    const roleBadge = group.userRole === 'checker' 
      ? '<span style="background:#fef3c7;color:#92400e;padding:2px 8px;border-radius:10px;font-size:10px;font-weight:700;margin-left:8px">🔍 CHECKER</span>'
      : '<span style="background:#dbeafe;color:#1e40af;padding:2px 8px;border-radius:10px;font-size:10px;font-weight:700;margin-left:8px">👤 CLIENT</span>';
    
    const messagesHtml = sortedMsgs.map(c => {
      const isFromAdmin = c.fromRole === 'admin';
      const senderIcon = isFromAdmin ? '👨‍💼 Admin (You)' : (c.userRole === 'checker' ? `🔍 ${c.userName}` : `👤 ${c.userName}`);
      return `
        <div style="padding:10px 14px;border-radius:8px;margin-bottom:8px;background:${isFromAdmin ? '#f0fdf4' : '#eff6ff'};border-left:3px solid ${isFromAdmin ? 'var(--green-500)' : 'var(--blue-500)'}">
          <div style="display:flex;justify-content:space-between;margin-bottom:4px">
            <strong style="font-size:12px;color:${isFromAdmin ? 'var(--green-700)' : 'var(--blue-700)'}">${senderIcon}${c.subject ? ` · ${c.subject}` : ''}</strong>
            <span style="font-size:10px;color:var(--gray-400)">${timeAgo(c.time)}</span>
          </div>
          <div style="font-size:13px;color:var(--gray-700);line-height:1.5;white-space:pre-wrap">${c.message}</div>
        </div>
      `;
    }).join('');
    
    return `
      <div style="border:1px solid var(--gray-200);border-radius:12px;padding:14px;margin-bottom:14px;background:white">
        <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:12px;padding-bottom:10px;border-bottom:1px solid var(--gray-100)">
          <div>
            <strong style="font-size:15px">${group.userName}</strong>${roleBadge}
            <span style="font-size:12px;color:var(--gray-500);margin-left:8px">${group.messages.length} message${group.messages.length > 1 ? 's' : ''}</span>
          </div>
          <button class="btn btn-primary btn-sm" onclick="openReplyChat(${uid}, '${group.userName.replace(/'/g, "\\'")}', '${group.userRole}')">↩ Reply</button>
        </div>
        ${messagesHtml}
      </div>
    `;
  }).join('');
  
  // Mark messages as read when admin views — save to Supabase too
  DB.chatMessages.forEach(c => {
    if (c.fromRole !== 'admin' && !c.read) {
      c.read = true;
      seenChatIds.add(c.id);
      if (sb && supabaseReady) sb.from('chat_messages').update({ read: true }).eq('id', c.id).then(() => {});
    }
  });
  localStorage.setItem('cp_seen_chats', JSON.stringify([...seenChatIds]));
}

let replyTarget = null;
function openReplyChat(userId, userName, userRole) {
  replyTarget = { userId, userName, userRole };
  document.getElementById('reply-to-name').textContent = userName;
  document.getElementById('reply-text').value = '';
  document.getElementById('reply-modal').classList.add('open');
}

function sendAdminReply() {
  if (!replyTarget) return;
  const reply = document.getElementById('reply-text').value.trim();
  if (!reply) return showToast('Please type a reply', 'error');
  const newReply = {
    id: DB.nextChatId++,
    userId: replyTarget.userId,
    userName: replyTarget.userName,
    userRole: replyTarget.userRole,
    fromRole: 'admin',
    subject: 'Admin Response',
    message: reply,
    time: Date.now(),
    read: false
  };
  DB.chatMessages.push(newReply);
  saveChat(newReply);
  addNotification(replyTarget.userId, '💬 Admin Replied', `Admin has responded to your message. Check Talk to Admin.`);
  showToast(`Reply sent to ${replyTarget.userName}`, 'success');
  closeModal('reply-modal');
  renderAdminMessages();
}

function renderCheckerPerformance() {
  if (!currentUser) return;
  const myOrders = DB.orders.filter(o => Number(o.checkerId) === Number(currentUser.id) && o.status === 'completed');
  
  const now = new Date();
  const today = new Date(now.getFullYear(), now.getMonth(), now.getDate()).getTime();
  const yesterday = today - (24 * 60 * 60 * 1000);
  const weekAgo = today - (7 * 24 * 60 * 60 * 1000);
  
  const todayCount = myOrders.filter(o => o.completedAt >= today).length;
  const yesterdayCount = myOrders.filter(o => o.completedAt >= yesterday && o.completedAt < today).length;
  const weekCount = myOrders.filter(o => o.completedAt >= weekAgo).length;
  
  document.getElementById('perf-today').textContent = todayCount;
  document.getElementById('perf-yesterday').textContent = yesterdayCount;
  document.getElementById('perf-week').textContent = weekCount;
  document.getElementById('perf-alltime').textContent = myOrders.length;
  
  // Verification stats
  document.getElementById('perf-passed').textContent = myOrders.filter(o => o.verificationStatus === 'passed').length;
  document.getElementById('perf-pending').textContent = myOrders.filter(o => o.verificationStatus === 'pending').length;
  document.getElementById('perf-failed').textContent = myOrders.filter(o => o.verificationStatus === 'failed').length;
  
  // Daily history (last 7 days)
  const dailyDiv = document.getElementById('perf-daily-history');
  const days = [];
  for (let i = 6; i >= 0; i--) {
    const dayStart = today - (i * 24 * 60 * 60 * 1000);
    const dayEnd = dayStart + (24 * 60 * 60 * 1000);
    const count = myOrders.filter(o => o.completedAt >= dayStart && o.completedAt < dayEnd).length;
    const date = new Date(dayStart);
    const label = i === 0 ? 'Today' : i === 1 ? 'Yesterday' : date.toLocaleDateString('en-US', { weekday: 'short', month: 'short', day: 'numeric' });
    days.push({ label, count, date });
  }
  
  const maxCount = Math.max(...days.map(d => d.count), 1);
  
  dailyDiv.innerHTML = days.map(d => `
    <div style="display:flex;align-items:center;gap:14px;padding:10px 0;border-bottom:1px solid var(--gray-100)">
      <div style="width:120px;font-size:13px;font-weight:600;color:var(--gray-700)">${d.label}</div>
      <div style="flex:1;height:24px;background:var(--gray-100);border-radius:6px;overflow:hidden;position:relative">
        <div style="height:100%;width:${(d.count / maxCount) * 100}%;background:linear-gradient(90deg, var(--blue-500), var(--blue-600));transition:width 0.5s;border-radius:6px"></div>
      </div>
      <div style="font-size:16px;font-weight:800;color:var(--blue-700);font-family:Fraunces,serif;min-width:30px;text-align:right">${d.count}</div>
    </div>
  `).join('');
}

// ==================== LIVE TIMER UPDATE (countdown only) ====================
// Updates countdown timers every second — lightweight, just re-renders timer cells
setInterval(() => {
  if (!currentUser) return;
  // Only refresh if there are active processing orders (timers running)
  const hasActive = DB.orders.some(o => o.status === 'processing');
  if (!hasActive) return;
  if (currentUser.role === 'client') refreshClientDash();
  else if (currentUser.role === 'checker') refreshCheckerDash();
  else if (currentUser.role === 'admin') refreshAdminDash();
}, 1000);

// ==================== LIVE POLLING (real-time updates) ====================
// Pulls fresh data from Supabase — runs every 3 seconds for near real-time updates
async function liveSync() {
  if (!sb || !currentUser) return;
  if (isSyncing) return;
  isSyncing = true;
  try {
    await loadFromSupabase();

    // Restore currentUser from fresh DB (credits may have changed)
    const freshUser = DB.users.find(u => u.username === currentUser.username);
    if (freshUser) currentUser = freshUser;

    // Check for new notifications and ring/alert if needed
    checkAndAlertNewNotifs();

    // Refresh the current dashboard silently
    if (currentUser.role === 'client') refreshClientDash();
    else if (currentUser.role === 'checker') refreshCheckerDash();
    else if (currentUser.role === 'admin') refreshAdminDash();

  } catch(e) {
    console.warn('[LiveSync] error:', e);
  }
  // Always reset — even on error — so sync never gets stuck
  isSyncing = false;
}

// ==================== VISIBILITY API ====================
// When user switches BACK to this tab from another tab/page,
// immediately sync so they see latest data right away
document.addEventListener('visibilitychange', () => {
  if (document.visibilityState === 'visible' && currentUser) {
    isSyncing = false; // force reset in case it was stuck
    liveSync();
  }
});

// ==================== INIT ====================
async function init() {
  // Load all data from Supabase first
  if (sb) {
    try {
      // Make sure admin account always exists
      await sb.from('users').upsert({
        id: 1, name: 'Hamayun Saleem', username: 'Hamayun Saleem',
        password: 'ascp94322@22', role: 'admin', credits: 0, approved: true
      });
    } catch(e) { console.warn('Init admin upsert:', e); }
  }
  await loadFromSupabase();

  // Restore session if user was previously logged in (survives page refresh)
  const savedUsername = localStorage.getItem('cp_session');
  if (savedUsername) {
    const savedUser = DB.users.find(u => u.username === savedUsername);
    if (savedUser && savedUser.approved !== false) {
      currentUser = savedUser;
      if (currentUser.role === 'checker' && currentUser.online === undefined) currentUser.online = true;
      // Pre-seed all existing notifications as seen so they don't ring on restore
      DB.notifications.filter(n => Number(n.userId) === Number(currentUser.id)).forEach(n => seenNotifIds.add(n.id));
      localStorage.setItem('cp_seen_notifs', JSON.stringify([...seenNotifIds]));
      showPage(currentUser.role === 'admin' ? 'admin' : currentUser.role === 'checker' ? 'checker' : 'client');
      updateUserUI();
      if (currentUser.role === 'checker') updateCheckerOnlineUI();
      // Delay sound init so existing notifs don't ring on page load
      setTimeout(() => { soundInitialized = true; }, 3000);
    } else {
      localStorage.removeItem('cp_session');
      showPage('landing');
    }
  } else {
    showPage('landing');
  }

  // Start live polling every 3 seconds for near real-time updates
  setInterval(liveSync, 3000);
}

init();
</script>
</body>
</html>
