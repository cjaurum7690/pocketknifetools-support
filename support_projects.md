<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Support — PocketKnife Projects</title>
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

    header {
      padding: 60px 24px 40px;
      text-align: center;
      border-bottom: 1px solid var(--border);
    }

    header .eyebrow {
      font-size: 12px;
      font-weight: 700;
      letter-spacing: 3px;
      color: var(--accent);
      text-transform: uppercase;
      margin-bottom: 10px;
    }

    header h1 {
      font-size: 36px;
      font-weight: 800;
      color: var(--text);
      letter-spacing: -0.5px;
    }

    header p {
      margin-top: 10px;
      color: var(--text-mid);
      font-size: 16px;
      max-width: 480px;
      margin-left: auto;
      margin-right: auto;
    }

    .accent-line {
      width: 48px;
      height: 3px;
      background: var(--accent);
      border-radius: 2px;
      margin: 20px auto 0;
    }

    main {
      max-width: 720px;
      margin: 0 auto;
      padding: 48px 24px 80px;
    }

    section {
      margin-bottom: 48px;
    }

    h2 {
      font-size: 11px;
      font-weight: 800;
      letter-spacing: 2.5px;
      text-transform: uppercase;
      color: var(--accent);
      margin-bottom: 20px;
    }

    .card {
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: var(--radius);
      padding: 20px 24px;
      margin-bottom: 12px;
    }

    .card h3 {
      font-size: 16px;
      font-weight: 700;
      color: var(--text);
      margin-bottom: 6px;
    }

    .card p, .card li {
      font-size: 14px;
      color: var(--text-mid);
      line-height: 1.65;
    }

    .card ul {
      padding-left: 18px;
      margin-top: 6px;
    }

    .card li {
      margin-bottom: 4px;
    }

    .feature-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 12px;
    }

    @media (max-width: 540px) {
      .feature-grid { grid-template-columns: 1fr; }
      header h1 { font-size: 28px; }
    }

    .tag {
      display: inline-block;
      background: rgba(201, 168, 76, 0.12);
      color: var(--accent);
      font-size: 11px;
      font-weight: 700;
      letter-spacing: 1px;
      padding: 3px 10px;
      border-radius: 20px;
      margin-bottom: 10px;
    }

    .contact-btn {
      display: inline-block;
      margin-top: 16px;
      background: var(--accent);
      color: #0e0f11;
      font-size: 15px;
      font-weight: 700;
      padding: 14px 28px;
      border-radius: var(--radius);
      text-decoration: none;
      transition: opacity 0.2s;
    }

    .contact-btn:hover { opacity: 0.85; }

    footer {
      text-align: center;
      padding: 32px 24px;
      border-top: 1px solid var(--border);
      color: var(--text-mid);
      font-size: 13px;
    }
  </style>
</head>
<body>

  <header>
    <p class="eyebrow">Support</p>
    <h1>PocketKnife Projects</h1>
    <p>Everything you need to get the most out of the app — and get help when you need it.</p>
    <div class="accent-line"></div>
  </header>

  <main>

    <!-- Getting Started -->
    <section>
      <h2>Getting Started</h2>
      <div class="card">
        <h3>Creating your first project</h3>
        <p>Tap <strong>+ New Project</strong> on the home screen. Give your project a name, start date, and end date — those three fields are required. You can also add a description, set a status, assign a priority level, and enter a total budget. Tap <strong>Create Project</strong> when you're ready.</p>
      </div>
      <div class="card">
        <h3>Project statuses</h3>
        <p>Projects are organized on the home screen by status. The available statuses are:</p>
        <ul>
          <li><strong>Pending</strong> — not yet started</li>
          <li><strong>Planning</strong> — in the planning phase</li>
          <li><strong>Active</strong> — currently in progress</li>
          <li><strong>On Hold</strong> — paused</li>
          <li><strong>Complete</strong> — finished</li>
        </ul>
        <p style="margin-top:10px;">Tap a project card to open it, then tap the status field in the edit screen to update it at any time.</p>
      </div>
      <div class="card">
        <h3>Priority levels</h3>
        <p>Priorities run from <strong>P1 (Critical)</strong> to <strong>P5 (Low)</strong>. Each project card shows its priority with a color-coded bar and badge so you can triage at a glance.</p>
      </div>
    </section>

    <!-- Features -->
    <section>
      <h2>Features</h2>
      <div class="feature-grid">
        <div class="card">
          <span class="tag">Milestones</span>
          <p>Track key deliverables with due dates, owners, and dependencies between milestones.</p>
        </div>
        <div class="card">
          <span class="tag">Budget</span>
          <p>Log expenses by category and monitor spending against your total project budget.</p>
        </div>
        <div class="card">
          <span class="tag">Meetings</span>
          <p>Record meeting notes, attendees, agendas, and outcomes in one place.</p>
        </div>
        <div class="card">
          <span class="tag">Action Items</span>
          <p>Capture tasks from meetings with owners, due dates, and open/closed tracking.</p>
        </div>
        <div class="card">
          <span class="tag">Risks</span>
          <p>Log risks with probability and impact scores, mitigation plans, and owners.</p>
        </div>
        <div class="card">
          <span class="tag">Issues</span>
          <p>Track active problems by priority and link them to milestones or risks.</p>
        </div>
        <div class="card">
          <span class="tag">Decisions</span>
          <p>Document key decisions, who made them, and the context behind them.</p>
        </div>
        <div class="card">
          <span class="tag">Dark Mode</span>
          <p>Tap the moon/sun icon on the home screen to toggle between light and dark mode.</p>
        </div>
      </div>
    </section>

    <!-- FAQ -->
    <section>
      <h2>FAQ</h2>
      <div class="card">
        <h3>Does the app require an account or internet connection?</h3>
        <p>No. PocketKnife Projects is fully offline. All your data is stored locally on your device — no account, no sign-in, no network connection required.</p>
      </div>
      <div class="card">
        <h3>How do I delete a project?</h3>
        <p>Long press any project card on the home screen. A confirmation dialog will appear before anything is deleted. Deleting a project removes all of its associated data — milestones, budget entries, meetings, action items, risks, issues, and decisions.</p>
      </div>
      <div class="card">
        <h3>Can I back up my data?</h3>
        <p>Your data is stored in your device's local app storage. It will be included in your iCloud or iTunes device backup if you have device backups enabled. There is no separate in-app export feature at this time.</p>
      </div>
      <div class="card">
        <h3>Is there a subscription or in-app purchase?</h3>
        <p>No. PocketKnife Projects is a one-time download with no subscriptions, no in-app purchases, and no premium tiers.</p>
      </div>
    </section>

    <!-- Contact -->
    <section>
      <h2>Contact</h2>
      <div class="card">
        <h3>Still need help?</h3>
        <p>If you've run into a bug or have a feature request, we'd love to hear from you. Reach out via email and we'll get back to you as soon as we can.</p>
        <a class="contact-btn" href="mailto:scottkotowicz@gmail.com">Email Support</a>
      </div>
    </section>

  </main>

  <footer>
    &copy; 2026 PocketKnife Projects &nbsp;·&nbsp; All rights reserved
  </footer>

</body>
</html>
