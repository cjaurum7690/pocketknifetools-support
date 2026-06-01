<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Privacy Policy — PocketKnife Projects</title>
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
    }

    header .meta {
      margin-top: 12px;
      color: var(--text-mid);
      font-size: 14px;
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
      margin-bottom: 44px;
    }

    h2 {
      font-size: 11px;
      font-weight: 800;
      letter-spacing: 2.5px;
      text-transform: uppercase;
      color: var(--accent);
      margin-bottom: 16px;
    }

    .card {
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: var(--radius);
      padding: 24px;
      margin-bottom: 12px;
    }

    .card h3 {
      font-size: 16px;
      font-weight: 700;
      color: var(--text);
      margin-bottom: 10px;
    }

    .card p {
      font-size: 14px;
      color: var(--text-mid);
      line-height: 1.7;
      margin-bottom: 10px;
    }

    .card p:last-child { margin-bottom: 0; }

    .card ul {
      padding-left: 18px;
      margin-top: 6px;
    }

    .card li {
      font-size: 14px;
      color: var(--text-mid);
      line-height: 1.65;
      margin-bottom: 4px;
    }

    .highlight {
      background: rgba(201, 168, 76, 0.08);
      border: 1px solid rgba(201, 168, 76, 0.25);
      border-radius: var(--radius);
      padding: 20px 24px;
      margin-bottom: 40px;
    }

    .highlight p {
      font-size: 15px;
      color: var(--text);
      line-height: 1.7;
    }

    .highlight strong { color: var(--accent); }

    a {
      color: var(--accent);
      text-decoration: none;
    }

    a:hover { text-decoration: underline; }

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

    footer a { color: var(--text-mid); }
    footer a:hover { color: var(--accent); }

    @media (max-width: 600px) {
      header h1 { font-size: 28px; }
    }
  </style>
</head>
<body>

  <header>
    <p class="eyebrow">Legal</p>
    <h1>Privacy Policy</h1>
    <p class="meta">PocketKnife Projects &nbsp;·&nbsp; Effective Date: June 1, 2026</p>
    <div class="accent-line"></div>
  </header>

  <main>

    <div class="highlight">
      <p><strong>The short version:</strong> PocketKnife Projects does not collect, transmit, or share any of your data. Everything you enter stays on your device. We have no servers, no accounts, and no way to see your information.</p>
    </div>

    <!-- Overview -->
    <section>
      <h2>Overview</h2>
      <div class="card">
        <h3>Who we are</h3>
        <p>PocketKnife Projects is an independent iOS application developed by CJ Aurum Creative. This Privacy Policy describes how the app handles your information.</p>
      </div>
      <div class="card">
        <h3>Scope</h3>
        <p>This policy applies to the PocketKnife Projects mobile application available on the Apple App Store. It does not apply to any third-party services, websites, or applications you may access independently.</p>
      </div>
    </section>

    <!-- Data Collection -->
    <section>
      <h2>Data Collection</h2>
      <div class="card">
        <h3>What we collect</h3>
        <p>Nothing. PocketKnife Projects does not collect any personal information, usage data, analytics, crash reports, or any other data from your device.</p>
      </div>
      <div class="card">
        <h3>What you enter in the app</h3>
        <p>All content you create in PocketKnife Projects — project names, descriptions, milestones, budget entries, meeting notes, action items, risks, issues, and decisions — is stored exclusively in a local database on your device using SQLite.</p>
        <p>This data never leaves your device. It is not transmitted to any server, not synced to any cloud service operated by us, and not accessible to the developer in any form.</p>
      </div>
    </section>

    <!-- Data Storage -->
    <section>
      <h2>Data Storage &amp; Security</h2>
      <div class="card">
        <h3>On-device storage</h3>
        <p>Your data is stored in the app's private local storage on your iPhone or iPad. It is protected by iOS app sandboxing, which prevents other apps from accessing it.</p>
      </div>
      <div class="card">
        <h3>iCloud &amp; device backups</h3>
        <p>If you have iCloud Backup or iTunes/Finder device backups enabled, your device backup may include the app's local database as part of your overall device backup. This is controlled entirely by your device settings and Apple — not by PocketKnife Projects.</p>
        <p>We recommend reviewing Apple's privacy policy at <a href="https://www.apple.com/legal/privacy/" target="_blank" rel="noopener">apple.com/legal/privacy</a> for details on how your device backups are handled.</p>
      </div>
      <div class="card">
        <h3>No external servers</h3>
        <p>PocketKnife Projects operates no servers and maintains no databases outside of your device. There is no backend infrastructure of any kind associated with this app.</p>
      </div>
    </section>

    <!-- Third Parties -->
    <section>
      <h2>Third-Party Services</h2>
      <div class="card">
        <h3>No third-party SDKs or analytics</h3>
        <p>PocketKnife Projects does not integrate any third-party analytics platforms, advertising networks, crash reporting tools, or tracking SDKs. No third-party code in this app has access to your data.</p>
      </div>
      <div class="card">
        <h3>Apple App Store</h3>
        <p>Downloading the app through the Apple App Store is subject to Apple's own privacy practices. Apple may collect certain information as part of the App Store purchase and download process, which is governed by Apple's Privacy Policy and is outside our control.</p>
      </div>
    </section>

    <!-- Children -->
    <section>
      <h2>Children's Privacy</h2>
      <div class="card">
        <h3>Not directed at children</h3>
        <p>PocketKnife Projects is a general-purpose productivity application. It is not directed at children under the age of 13, and we do not knowingly collect any information from children. Because no data is collected from any user, there is no special risk to children's data.</p>
      </div>
    </section>

    <!-- Your Rights -->
    <section>
      <h2>Your Rights &amp; Control</h2>
      <div class="card">
        <h3>Your data, your control</h3>
        <p>Because all data is stored locally on your device, you have complete control over it at all times. You can:</p>
        <ul>
          <li>Delete individual projects, entries, or items within the app at any time</li>
          <li>Delete all app data by uninstalling PocketKnife Projects from your device</li>
          <li>Manage device backup settings through your iPhone's Settings app</li>
        </ul>
      </div>
      <div class="card">
        <h3>No account to delete</h3>
        <p>Because PocketKnife Projects requires no account and stores no data on external servers, there is no account to request deletion of. Uninstalling the app from your device permanently removes all associated data.</p>
      </div>
    </section>

    <!-- Changes -->
    <section>
      <h2>Changes to This Policy</h2>
      <div class="card">
        <h3>Updates</h3>
        <p>If this Privacy Policy is updated, the revised version will be posted at this URL with an updated effective date. Continued use of the app after any changes constitutes acceptance of the updated policy.</p>
        <p>Given the nature of this app — no data collection, no servers, no accounts — we do not anticipate material changes to this policy.</p>
      </div>
    </section>

    <!-- Contact -->
    <section>
      <h2>Contact</h2>
      <div class="card">
        <h3>Questions?</h3>
        <p>If you have any questions about this Privacy Policy, you can reach us at:</p>
        <p style="margin-top: 12px;"><a href="mailto:scottkotowicz@gmail.com">scottkotowicz@gmail.com</a></p>
      </div>
    </section>

  </main>

  <footer>
    <span>&copy; 2026 PocketKnife Projects</span>
    <a href="https://cjaurum7690.github.io/pocketknifetools-support/index_projects.html">Home</a>
    <a href="https://cjaurum7690.github.io/pocketknifetools-support/support_projects.html">Support</a>
    <a href="mailto:scottkotowicz@gmail.com">Contact</a>
  </footer>

</body>
</html>
