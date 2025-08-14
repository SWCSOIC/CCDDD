
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Hello Buggu Ji — Call Me</title>
  <style>
    :root{
      --bg:#f5f7fb;
      --card:#ffffff;
      --accent1:#1fa65a; /* main green */
      --accent2:#14a04d; /* darker green */
      --shadow: 0 10px 30px rgba(17,24,39,0.08);
      --glass: rgba(255,255,255,0.6);
      --text:#0f1720;
      --muted:#566270;
    }
    * { box-sizing: border-box; }
    html,body {
      height:100%;
      margin:0;
      font-family: Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
      background: linear-gradient(180deg, #eef3f8 0%, var(--bg) 100%);
      color:var(--text);
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
    }

    .wrap {
      min-height:100%;
      display:flex;
      align-items:center;
      justify-content:center;
      padding:48px 20px;
    }

    .card {
      background:var(--card);
      width:100%;
      max-width:520px;
      border-radius:18px;
      box-shadow: var(--shadow);
      padding:40px;
      text-align:center;
      border: 1px solid rgba(15,23,36,0.04);
    }

    h1 {
      margin:0 0 26px 0;
      font-size:28px;
      letter-spacing: -0.2px;
    }

    p.lead {
      margin:0 0 30px 0;
      color:var(--muted);
      font-size:15px;
    }

    /* Dial button */
    .dial {
      display:inline-flex;
      align-items:center;
      gap:14px;
      text-decoration:none;
      background: linear-gradient(180deg, var(--accent1), var(--accent2));
      border-radius:999px;
      padding:18px 22px;
      box-shadow: 0 8px 24px rgba(31, 122, 73, 0.18), inset 0 -6px 18px rgba(0,0,0,0.06);
      color: #fff;
      font-weight:600;
      font-size:16px;
      transition: transform .12s ease, box-shadow .12s ease;
      -webkit-tap-highlight-color: transparent;
    }

    .dial:active { transform: translateY(2px) scale(.997); }
    .dial:hover { transform: translateY(-3px); box-shadow: 0 18px 36px rgba(31,122,73,0.18); }

    /* circle with icon */
    .dial .circle {
      width:56px;
      height:56px;
      min-width:56px;
      border-radius:50%;
      background: radial-gradient(circle at 35% 25%, rgba(255,255,255,0.18), rgba(255,255,255,0) 40%), rgba(255,255,255,0.06);
      display:flex;
      align-items:center;
      justify-content:center;
      box-shadow: 0 6px 14px rgba(4,16,10,0.12), inset 0 -6px 10px rgba(0,0,0,0.08);
    }

    /* phone icon (white) */
    .phone-svg { width:28px; height:28px; display:block; }

    /* small note under button */
    .note {
      margin-top:18px;
      color:var(--muted);
      font-size:13px;
    }

    /* accessibility focus */
    .dial:focus {
      outline: 3px solid rgba(34,197,94,0.18);
      outline-offset: 6px;
      border-radius:999px;
    }

    @media (max-width:420px){
      .card { padding:28px; }
      .dial { padding:14px 16px; gap:12px; }
      .dial .circle { width:48px; height:48px; min-width:48px; }
    }
  </style>
</head>
<body>
  <div class="wrap">
    <main class="card" role="main">
      <h1>Hello Buggu Ji</h1>
      <p class="lead">Tap the green dial below to open your phone's dialer with the number filled in.</p>

      <!--
        Replace the phone number in href below with your actual number.
        Example formats that work:
          tel:+911234567890   (recommended: include country code)
          tel:0123456789      (local number)
      -->
      <a
        class="dial"
        href="tel:+918779627537"
        aria-label="Call Buggu Ji at +91 8779627537"
        title="Call me"
      >
        <span class="circle" aria-hidden="true">
          <!-- phone icon (SVG) -->
          <svg class="phone-svg" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" aria-hidden="true" focusable="false">
            <path d="M21 16.5v3a1.5 1.5 0 0 1-1.67 1.49c-1.87-.18-3.75-.78-5.5-1.9a1.5 1.5 0 0 1-.64-2.05l1-1.8a17.5 17.5 0 0 1-6.1-6.1l-1.8 1a1.5 1.5 0 0 1-2.05-.64A18.02 18.02 0 0 1 3.01 4.67 1.5 1.5 0 0 1 4.5 3h3A1.5 1.5 0 0 1 9 4.33c.07 1.1.42 2.18 1 3.14.6 1 1.39 1.87 2.37 2.46.99.6 2.07.94 3.16 1a1.5 1.5 0 0 1 1.33 1.5v3z" fill="#ffffff"/>
          </svg>
        </span>
        <span>Call me</span>
      </a>

      <div class="note" aria-hidden="true">Works on phones and devices that support `tel:` links.</div>
    </main>
  </div>
</body>
</html>
