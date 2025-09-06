<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>First Last — CV</title>
  <meta name="description" content="Single-page CV for First Last — Full‑Stack Java Developer." />
  <meta property="og:title" content="First Last — CV" />
  <meta property="og:description" content="Single-page CV for First Last — Full‑Stack Java Developer." />
  <meta name="theme-color" content="#0ea5e9" />
  <style>
    :root{
      --bg:#ffffff; --fg:#0b1220; --muted:#5b6579; --accent:#0ea5e9; --chip:#eef6ff; --line:#e9eef5; --card:#f8fafc;
      --mono: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;
      --sans: Inter, ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Ubuntu, Cantarell, Noto Sans, Arial, "Apple Color Emoji", "Segoe UI Emoji";
    }
    @media (prefers-color-scheme: dark){
      :root{ --bg:#0b1220; --fg:#e6eaf2; --muted:#a7b0c2; --accent:#38bdf8; --chip:#0f2138; --line:#1b2538; --card:#0f1a2b; }
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{margin:0; background:var(--bg); color:var(--fg); font-family:var(--sans); line-height:1.5}
    a{color:var(--accent); text-decoration:none}
    a:hover{ text-decoration:underline }
    .page{max-width:960px; margin:40px auto; padding:0 24px}
    header{display:grid; grid-template-columns:1fr auto; gap:16px; align-items:center; padding:24px; border:1px solid var(--line); border-radius:16px; background:var(--card)}
    h1{margin:0; font-size:clamp(28px, 3vw, 40px)}
    .role{margin-top:4px; color:var(--muted); font-weight:500}
    .contact{display:flex; flex-wrap:wrap; gap:8px}
    .chip{border:1px solid var(--line); background:var(--chip); color:inherit; padding:6px 10px; border-radius:999px; font-size:14px}
    .chip code{font-family:var(--mono)}
    .columns{display:grid; grid-template-columns:2fr 1fr; gap:24px; margin-top:24px}
    section{border:1px solid var(--line); border-radius:16px; padding:20px; background:var(--card)}
    section h2{margin:0 0 12px; font-size:18px; letter-spacing:.3px; text-transform:uppercase}
    .summary{color:var(--fg)}
    .tags{display:flex; flex-wrap:wrap; gap:8px; margin-top:8px}
    .tag{font-size:12px; padding:6px 10px; border-radius:999px; background:var(--chip); border:1px solid var(--line)}
    .item{margin-bottom:16px}
    .item:last-child{margin-bottom:0}
    .item header{display:flex; justify-content:space-between; align-items:baseline; padding:0; border:none; background:transparent}
    .item h3{margin:0; font-size:16px}
    .item .meta{color:var(--muted); font-size:13px}
    ul.tight{margin:8px 0 0 18px}
    ul.tight li{margin:4px 0}
    aside{display:grid; gap:24px}
    .download{position:fixed; right:16px; bottom:16px; padding:10px 14px; border-radius:999px; background:var(--accent); color:#001018; font-weight:700; border:none; cursor:pointer; box-shadow:0 6px 20px rgba(14,165,233,.35)}
    .sr-only{position:absolute;width:1px;height:1px;padding:0;margin:-1px;overflow:hidden;clip:rect(0,0,0,0);white-space:nowrap;border:0}
    @media (max-width: 800px){ .columns{grid-template-columns:1fr} header{grid-template-columns:1fr} }
    @page { size: A4; margin: 14mm }
    @media print{
      .download{ display:none }
      .page{ margin:0; padding:0 }
      header,section{ background:#fff; border-color:#ddd; box-shadow:none }
      a{ color:inherit; text-decoration:none }
      .chip,.tag{ background:#f4f4f4; border-color:#e5e5e5 }
    }
  </style>
</head>
<body>
  <a class="sr-only" href="#main">Skip to content</a>
  <div class="page">
    <header aria-label="Heading">
      <div>
        <h1>First Last</h1>
        <div class="role">Full‑Stack Java Developer</div>
      </div>
      <nav class="contact" aria-label="Contact">
        <span class="chip">📍 City, Country</span>
        <a class="chip" href="mailto:you@example.com">✉️ you@example.com</a>
        <a class="chip" href="tel:+10000000000">☎️ +1‑000‑000‑0000</a>
        <a class="chip" href="https://github.com/yourhandle" target="_blank" rel="noopener">🐙 github.com/yourhandle</a>
        <a class="chip" href="https://www.linkedin.com/in/yourhandle" target="_blank" rel="noopener">🔗 linkedin.com/in/yourhandle</a>
        <span class="chip"><code>Portfolio: yourdomain.dev</code></span>
      </nav>
    </header>

    <main id="main" class="columns">
      <div>
        <section aria-labelledby="summary">
          <h2 id="summary">Profile</h2>
          <p class="summary">Full‑stack engineer specializing in Java/Spring Boot backends and modern front‑ends (React/Angular). Experienced with AWS (EC2, ECS/Fargate, RDS, S3, CloudFront) and CI/CD (GitHub Actions). Passionate about building reliable services and clean UX.</p>
          <div class="tags" aria-label="Key skills">
            <span class="tag">Java • Spring Boot</span>
            <span class="tag">REST • GraphQL</span>
            <span class="tag">AWS • Docker</span>
            <span class="tag">RDBMS • NoSQL</span>
            <span class="tag">React • TypeScript</span>
            <span class="tag">CI/CD • Testing</span>
          </div>
        </section>

        <section aria-labelledby="experience">
          <h2 id="experience">Experience</h2>

          <article class="item">
            <header>
              <h3>Senior Full‑Stack Engineer — Company Name</h3>
              <div class="meta">Jan 2023 – Present · Remote</div>
            </header>
            <ul class="tight">
              <li>Led design & development of a multi‑tenant Spring Boot API (Java 17) serving 50k+ MAU, deployed on AWS ECS Fargate behind ALB; cut p95 latency by 35%.</li>
              <li>Built CI/CD pipelines with GitHub Actions, Docker, and AWS CDK; automated blue/green deployments.</li>
              <li>Implemented React/TypeScript front‑end with component library and accessibility checks.</li>
            </ul>
          </article>

          <article class="item">
