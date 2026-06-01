<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Marketing — PocketKnife Projects</title>
  <style>
    :root {
      --bg: #0e0f11;
      --surface: #1a1b1e;
      --border: #2a2b2f;
      --accent: #c9a84c;
      --text: #f0f0f0;
      --text-mid: #9a9a9a;
      --radius: 14px;
    }

    * { box-sizing: border-box; margin: 0; padding: 0; }

    body {
      background: var(--bg);
      color: var(--text);
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif;
      line-height: 1.6;
    }

    /* ── NAV ── */
    nav {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 20px 32px;
      border-bottom: 1px solid var(--border);
      position: sticky;
      top: 0;
      background: rgba(14, 15, 17, 0.92);
      backdrop-filter: blur(12px);
      z-index: 100;
    }

    .nav-logo {
      font-size: 15px;
      font-weight: 800;
      letter-spacing: 1px;
      color: var(--accent);
      text-decoration: none;
    }

    .nav-links {
      display: flex;
      gap: 28px;
      list-style: none;
    }

    .nav-links a {
      color: var(--text-mid);
      text-decoration: none;
      font-size: 14px;
      font-weight: 500;
      transition: color 0.2s;
    }

    .nav-links a:hover { color: var(--text); }

    /* ── HERO ── */
    .hero {
      text-align: center;
      padding: 100px 24px 80px;
      max-width: 760px;
      margin: 0 auto;
    }

    .hero-eyebrow {
      font-size: 11px;
      font-weight: 800;
      letter-spacing: 3px;
      color: var(--accent);
      text-transform: uppercase;
      margin-bottom: 20px;
    }

    .hero h1 {
      font-size: 56px;
      font-weight: 900;
      line-height: 1.1;
      letter-spacing: -1.5px;
      margin-bottom: 24px;
    }

    .hero h1 span { color: var(--accent); }

    .hero p {
      font-size: 18px;
      color: var(--text-mid);
      max-width: 500px;
      margin: 0 auto 40px;
      line-height: 1.7;
    }

    .hero-btns {
      display: flex;
      gap: 14px;
      justify-content: center;
      flex-wrap: wrap;
    }

    .btn-primary {
      display: inline-block;
      background: var(--accent);
      color: #0e0f11;
      font-size: 15px;
      font-weight: 700;
      padding: 16px 32px;
      border-radius: var(--radius);
      text-decoration: none;
      transition: opacity 0.2s;
    }

    .btn-primary:hover { opacity: 0.85; }

    .btn-secondary {
      display: inline-block;
      background: transparent;
      color: var(--text);
      font-size: 15px;
      font-weight: 600;
      padding: 16px 32px;
      border-radius: var(--radius);
      border: 1px solid var(--border);
      text-decoration: none;
      transition: border-color 0.2s;
    }

    .btn-secondary:hover { border-color: var(--accent); }

    .hero-accent-line {
      width: 64px;
      height: 3px;
      background: var(--accent);
      border-radius: 2px;
      margin: 60px auto 0;
    }

    /* ── TAGLINE STRIP ── */
    .tagline-strip {
      border-top: 1px solid var(--border);
      border-bottom: 1px solid var(--border);
      padding: 20px 32px;
      display: flex;
      justify-content: center;
      gap: 48px;
      flex-wrap: wrap;
    }

    .tagline-item {
      font-size: 12px;
      font-weight: 700;
      letter-spacing: 2px;
      color: var(--text-mid);
      text-transform: uppercase;
    }

    .tagline-item span { color: var(--accent); margin-right: 8px; }

    /* ── SECTIONS ── */
    section {
      max-width: 900px;
      margin: 0 auto;
      padding: 80px 24px;
    }

    .section-label {
      font-size: 11px;
      font-weight: 800;
      letter-spacing: 2.5px;
      text-transform: uppercase;
      color: var(--accent);
      margin-bottom: 16px;
    }

    .section-title {
      font-size: 36px;
      font-weight: 800;
      letter-spacing: -0.5px;
      line-height: 1.2;
      margin-bottom: 14px;
    }

    .section-body {
      font-size: 16px;
      color: var(--text-mid);
      max-width: 540px;
      line-height: 1.7;
      margin-bottom: 40px;
    }

    /* ── FEATURE GRID ── */
    .feature-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
      gap: 14px;
    }

    .feature-card {
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: var(--radius);
      padding: 24px;
      transition: border-color 0.2s;
    }

    .feature-card:hover { border-color: var(--accent); }

    .feature-icon {
      font-size: 28px;
      margin-bottom: 12px;
    }

    .feature-card h3 {
      font-size: 15px;
      font-weight: 700;
      color: var(--text);
      margin-bottom: 6px;
    }

    .feature-card p {
      font-size: 13px;
      color: var(--text-mid);
      line-height: 1.6;
    }

    /* ── HOW IT WORKS ── */
    .steps {
      display: flex;
      flex-direction: column;
      gap: 0;
    }

    .step {
      display: flex;
      gap: 24px;
      align-items: flex-start;
      padding: 28px 0;
      border-bottom: 1px solid var(--border);
    }

    .step:last-child { border-bottom: none; }

    .step-number {
      font-size: 11px;
      font-weight: 800;
      letter-spacing: 2px;
      color: var(--accent);
      min-width: 32px;
      padding-top: 2px;
    }

    .step h3 {
      font-size: 17px;
      font-weight: 700;
      margin-bottom: 6px;
    }

    .step p {
      font-size: 14px;
      color: var(--text-mid);
      line-height: 1.65;
    }

    /* ── NO NONSENSE STRIP ── */
    .no-nonsense {
      background: var(--surface);
      border-top: 1px solid var(--border);
      border-bottom: 1px solid var(--border);
      padding: 60px 24px;
      text-align: center;
    }

    .no-nonsense h2 {
      font-size: 30px;
      font-weight: 800;
      margin-bottom: 14px;
    }

    .no-nonsense p {
      color: var(--text-mid);
      font-size: 16px;
      max-width: 480px;
      margin: 0 auto 32px;
      line-height: 1.7;
    }

    .pills {
      display: flex;
      justify-content: center;
      gap: 12px;
      flex-wrap: wrap;
    }

    .pill {
      background: rgba(201, 168, 76, 0.1);
      color: var(--accent);
      border: 1px solid rgba(201, 168, 76, 0.3);
      font-size: 13px;
      font-weight: 700;
      padding: 8px 18px;
      border-radius: 40px;
    }

    /* ── CTA ── */
    .cta {
      text-align: center;
      padding: 100px 24px;
    }

    .cta h2 {
      font-size: 42px;
      font-weight: 900;
      letter-spacing: -1px;
      margin-bottom: 16px;
    }

    .cta h2 span { color: var(--accent); }

    .cta p {
      color: var(--text-mid);
      font-size: 16px;
      margin-bottom: 40px;
    }

    /* ── FOOTER ── */
    footer {
      text-align: center;
      padding: 32px 24px;
      border-top: 1px solid var(--border);
      color: var(--text-mid);
      font-size: 13px;
      display: flex;
      justify-content: center;
      gap: 24px;
      flex-wrap: wrap;
    }

    footer a {
      color: var(--text-mid);
      text-decoration: none;
      transition: color 0.2s;
    }

    footer a:hover { color: var(--accent); }

    /* ── RESPONSIVE ── */
    @media (max-width: 600px) {
      .hero h1 { font-size: 38px; }
      .section-title { font-size: 28px; }
      .cta h2 { font-size: 30px; }
      .tagline-strip { gap: 20px; }
      nav { padding: 16px 20px; }
      .nav-links { display: none; }
    }
  </style>
</head>
<body>

  <!-- NAV -->
  <nav>
    <a class="nav-logo" href="#">⚒ POCKETKNIFE PROJECTS</a>
    <ul class="nav-links">
      <li><a href="#features">Features</a></li>
      <li><a href="#how-it-works">How It Works</a></li>
      <li><a href="https://cjaurum7690.github.io/pocketknifetools-support/support_projects.html">Support</a></li>
    </ul>
  </nav>

  <!-- HERO -->
  <div class="hero">
    <p class="hero-eyebrow">Available on the App Store</p>
    <h1>Run your projects.<br /><span>Not your subscriptions.</span></h1>
    <p>A full project management toolkit that lives entirely on your iPhone or iPad. 
      No account, no cloud, no monthly fee — just your work, organized.</p>
    <div class="hero-btns">
      <a class="btn-primary" href="#">Download on the App Store</a>
      <a class="btn-secondary" href="#features">See what's inside</a>
    </div>
    <div class="hero-accent-line"></div>
  </div>

  <!-- TAGLINE STRIP -->
  <div class="tagline-strip">
    <span class="tagline-item"><span>✓</span> No account required</span>
    <span class="tagline-item"><span>✓</span> Fully offline</span>
    <span class="tagline-item"><span>✓</span> No subscription</span>
    <span class="tagline-item"><span>✓</span> Dark mode</span>
  </div>

  <!-- FEATURES -->
  <section id="features">
    <p class="section-label">Features</p>
    <h2 class="section-title">Everything a project needs.<br />Nothing it doesn't.</h2>
    <p class="section-body">PocketKnife Projects packs a full PM toolkit into a clean, fast mobile app. Every section of a project is one tap away.</p>

    <div class="feature-grid">
      <div class="feature-card">
        <div class="feature-icon">🏁</div>
        <h3>Milestones</h3>
        <p>Define key deliverables, set due dates, assign owners, and chain dependencies so nothing falls out of order.</p>
      </div>
      <div class="feature-card">
        <div class="feature-icon">💰</div>
        <h3>Budget</h3>
        <p>Log expenses by category and track spending against your total project budget in real time.</p>
      </div>
      <div class="feature-card">
        <div class="feature-icon">📋</div>
        <h3>Meetings</h3>
        <p>Record agendas, attendees, and notes — so every meeting produces something you can act on.</p>
      </div>
      <div class="feature-card">
        <div class="feature-icon">✅</div>
        <h3>Action Items</h3>
        <p>Capture tasks from meetings with owners and due dates. Track them open until closed.</p>
      </div>
      <div class="feature-card">
        <div class="feature-icon">⚠️</div>
        <h3>Risks</h3>
        <p>Score risks by probability and impact, document mitigation plans, and assign owners before problems become surprises.</p>
      </div>
      <div class="feature-card">
        <div class="feature-icon">🔥</div>
        <h3>Issues</h3>
        <p>Track active problems by priority and link them directly to milestones or risks for full context.</p>
      </div>
      <div class="feature-card">
        <div class="feature-icon">🧭</div>
        <h3>Decisions</h3>
        <p>Log every key decision, who made it, and why. The record you'll be glad you kept six months from now.</p>
      </div>
      <div class="feature-card">
        <div class="feature-icon">🌙</div>
        <h3>Dark Mode</h3>
        <p>A sharp, minimal design in light or dark — toggle it from the home screen at any time.</p>
      </div>
    </div>
  </section>

  <!-- HOW IT WORKS -->
  <section id="how-it-works" style="border-top: 1px solid var(--border); padding-top: 80px;">
    <p class="section-label">How It Works</p>
    <h2 class="section-title">Up and running in seconds.</h2>
    <p class="section-body">No setup, no onboarding screens, no tutorial you have to skip. Just open the app and go.</p>

    <div class="steps">
      <div class="step">
        <span class="step-number">01</span>
        <div>
          <h3>Create a project</h3>
          <p>Tap <strong>+ New Project</strong>, give it a name, start date, and end date. Set a status, priority, and optional budget. Done in under a minute.</p>
        </div>
      </div>
      <div class="step">
        <span class="step-number">02</span>
        <div>
          <h3>Build it out</h3>
          <p>Tap into your project to access all eight sections. Add milestones first to map the path, then fill in budget, risks, and meetings as the project evolves.</p>
        </div>
      </div>
      <div class="step">
        <span class="step-number">03</span>
        <div>
          <h3>Stay on top of it</h3>
          <p>Your home screen groups every project by status so you always know what's active, what's stalled, and what's done. Long press any project to delete it.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- NO NONSENSE -->
  <div class="no-nonsense">
    <h2>No cloud. No account. No bill.</h2>
    <p>Your project data lives on your device — encrypted with iOS and backed up with your phone. PocketKnife Projects is a one-time download with nothing to log into and nothing to cancel.</p>
    <div class="pills">
      <span class="pill">100% Offline</span>
      <span class="pill">No Account</span>
      <span class="pill">No Subscription</span>
      <span class="pill">No Ads</span>
      <span class="pill">Private by Design</span>
    </div>
  </div>

  <!-- CTA -->
  <div class="cta">
    <h2>Your next project<br /><span>starts here.</span></h2>
    <p>Download PocketKnife Projects free from the App Store.</p>
    <a class="btn-primary" href="#">Download on the App Store</a>
  </div>

  <!-- FOOTER -->
  <footer>
    <span>&copy; 2025 PocketKnife Projects</span>
    <a href="support.html">Support</a>
    <a href="mailto:scottkotowicz@gmail.com">Contact</a>
  </footer>

</body>
</html>
