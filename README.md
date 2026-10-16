<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="description" content="Saif Zeid's cybersecurity portfolio. Explore hands-on projects in security operations, Splunk investigations, and Python phishing detection.">
  <meta name="theme-color" content="#f8f9f5">
  <title>Saif Zeid | Cybersecurity Portfolio</title>
  <style>
    :root{--bg:#f8f9f5;--ink:#20352d;--muted:#58665e;--accent:#28644a;--line:#d9dfd6;--soft:#eaf0e7}
    *{box-sizing:border-box}
    html{scroll-behavior:smooth;scroll-padding-top:28px}
    body{margin:0;background:var(--bg);color:var(--ink);font-family:system-ui,-apple-system,BlinkMacSystemFont,"Segoe UI",sans-serif;font-size:16px;line-height:1.7}
    a{color:inherit;text-underline-offset:5px}
    a:focus-visible{outline:3px solid var(--accent);outline-offset:6px;border-radius:3px}
    .skip{position:absolute;left:16px;top:-80px;background:var(--ink);color:white;padding:10px 18px;z-index:10}
    .skip:focus{top:12px}
    .wrap{max-width:1040px;margin:auto;padding:0 32px}
    header{display:flex;align-items:center;justify-content:space-between;padding:27px 0;border-bottom:1px solid var(--line);gap:20px}
    .brand{text-decoration:none;font-size:19px;font-weight:750;letter-spacing:-.6px}
    .brand span{color:var(--accent)}
    nav{display:flex;gap:26px;font-size:14px}
    nav a{text-decoration:none;color:var(--muted)}
    nav a:hover{color:var(--accent);text-decoration:underline}
    .hero{padding:85px 0 72px;max-width:820px}
    .eyebrow{font-size:12px;font-weight:700;letter-spacing:2px;text-transform:uppercase;color:var(--accent);margin:0 0 22px}
    h1{font-size:clamp(48px,8vw,80px);line-height:1.08;letter-spacing:-4px;margin:0 0 24px;font-weight:650}
    .intro{font-size:clamp(20px,3vw,26px);line-height:1.55;max-width:710px;letter-spacing:-.4px;margin:0 0 18px}
    .description{max-width:650px;color:var(--muted);margin:0 0 28px}
    .actions{display:flex;gap:14px;flex-wrap:wrap;align-items:center}
    .button{display:inline-flex;align-items:center;justify-content:center;gap:16px;padding:11px 20px;border:1px solid var(--ink);border-radius:6px;text-decoration:none;font-size:14px;font-weight:600;transition:background .2s}
    .button.primary{background:var(--ink);color:white}
    .button.primary:hover{background:var(--accent)}
    .button.secondary:hover{background:var(--soft)}
    .availability{margin-top:32px;display:flex;align-items:flex-start;gap:10px;font-size:13px;color:var(--muted)}
    .dot{width:7px;height:7px;flex-shrink:0;background:var(--accent);border-radius:50%;margin-top:8px}
    section{padding:45px 0;border-top:1px solid var(--line)}
    .section-head{display:flex;align-items:baseline;justify-content:space-between;gap:20px;margin-bottom:25px}
    h2{font-size:26px;letter-spacing:-.8px;font-weight:650;margin:0}
    .section-note{font-size:13px;color:var(--muted);margin:0}
    .projects{display:grid;grid-template-columns:1fr 1fr;gap:22px}
    .project{background:white;border:1px solid var(--line);border-radius:10px;padding:28px;display:flex;flex-direction:column}
    .project-label{font-size:11px;letter-spacing:1.6px;font-weight:650;text-transform:uppercase;color:var(--accent);margin:0 0 20px}
    h3{font-size:22px;line-height:1.3;letter-spacing:-.5px;margin:0 0 14px;font-weight:650}
    .project p:not(.project-label){font-size:15px;color:var(--muted);margin:0 0 16px}
    .project ul{margin:0 0 24px;padding-left:19px;font-size:14px;color:var(--muted)}
    .project li{margin-bottom:7px}
    .tags{display:flex;flex-wrap:wrap;gap:7px;margin-top:auto;margin-bottom:23px}
    .tag{font-size:11px;background:var(--soft);color:var(--accent);padding:4px 9px;border-radius:4px}
    .project-link{font-size:14px;font-weight:650;text-decoration:none;align-self:flex-start}
    .project-link:hover{text-decoration:underline}
    .skills{display:grid;grid-template-columns:repeat(3,1fr);gap:28px}
    .skill h3{font-size:15px;margin-bottom:10px}
    .skill p{color:var(--muted);font-size:14px;margin:0}
    .about{display:grid;grid-template-columns:1fr 2fr;gap:50px}
    .about p{color:var(--muted);margin:0 0 16px;font-size:15px}
    .about strong{color:var(--ink);font-weight:600}
    footer{border-top:1px solid var(--line);padding:25px 0 32px;display:flex;justify-content:space-between;gap:15px;font-size:12px;color:var(--muted)}
    footer a{text-decoration:none}
    footer a:hover{text-decoration:underline}
    @media(max-width:650px){
      .wrap{padding:0 22px}header{padding:22px 0}nav{gap:15px;font-size:13px}
      .hero{padding:55px 0 48px}h1{letter-spacing:-2px}.intro{font-size:21px}
      .projects,.skills,.about{grid-template-columns:1fr}.project{padding:24px}
      .section-head{display:block}.section-note{margin-top:5px}.skills{gap:23px}.about{gap:20px}
      section{padding:34px 0}footer{flex-wrap:wrap}
    }
    @media(prefers-reduced-motion:reduce){html{scroll-behavior:auto}*{transition:none!important}}
  </style>
</head>
<body>
<a class="skip" href="#main">Skip to content</a>
<div class="wrap">
  <header>
    <a class="brand" href="#" aria-label="Saif Zeid home">Saif Zeid<span>.</span></a>
    <nav aria-label="Main navigation">
      <a href="#projects">Projects</a>
      <a href="#skills">Skills</a>
      <a href="#about">About</a>
    </nav>
  </header>
  <main id="main">
    <div class="hero">
      <p class="eyebrow">Cybersecurity portfolio · Winnipeg, Canada</p>
      <h1>Hi, I'm Saif.</h1>
      <p class="intro">Learning how to detect threats,<br>investigate incidents, and protect systems.</p>
      <p class="description">I'm a Cybersecurity student at Red River College Polytechnic. Through hands-on labs and personal projects, I turn what I learn into practical security skills.</p>
      <div class="actions">
        <a class="button primary" href="#projects">Explore my projects <span aria-hidden="true">↓</span></a>
        <a class="button secondary" href="https://github.com/Saif-Zeid">View GitHub <span aria-hidden="true">↗</span></a>
      </div>
      <p class="availability"><span class="dot" aria-hidden="true"></span>Seeking a four-month co-op · January–April 2027 · Open to relocating to Toronto</p>
    </div>
    <section id="projects" aria-labelledby="projects-title">
      <div class="section-head">
        <h2 id="projects-title">Selected projects</h2>
        <p class="section-note">Built, tested, and documented.</p>
      </div>
      <div class="projects">
        <article class="project">
          <p class="project-label">01 / Security operations</p>
          <h3>Enterprise SOC Analyst Lab</h3>
          <p>A virtual lab for practicing centralized logging, threat detection, and incident investigation with Splunk.</p>
          <ul>
            <li>Investigated repeated failed logins and correlated them with a Windows account lockout.</li>
            <li>Built an SPL detection rule to alert on repeated authentication failures.</li>
            <li>Documented findings and mapped the detection to MITRE ATT&amp;CK.</li>
          </ul>
          <div class="tags" aria-label="Technologies"><span class="tag">Splunk</span><span class="tag">Windows</span><span class="tag">Ubuntu</span><span class="tag">VMware</span></div>
          <a class="project-link" href="https://github.com/Saif-Zeid/enterprise-soc-analyst-lab">Explore SOC lab <span aria-hidden="true">↗</span></a>
        </article>
        <article class="project">
          <p class="project-label">02 / Email security</p>
          <h3>Email Phishing Detection Analyzer</h3>
          <p>A Python tool that examines email files for phishing indicators and explains the evidence behind each risk score.</p>
          <ul>
            <li>Analyzes email content, sender information, and embedded URLs.</li>
            <li>Flags suspicious links and sender/Reply-To domain mismatches.</li>
            <li>Uses rule-based scoring to classify messages as low, medium, or high risk.</li>
          </ul>
          <div class="tags" aria-label="Technologies"><span class="tag">Python</span><span class="tag">Email analysis</span><span class="tag">Linux</span><span class="tag">Git</span></div>
          <a class="project-link" href="https://github.com/Saif-Zeid/ai-security-project">Explore phishing analyzer <span aria-hidden="true">↗</span></a>
        </article>
      </div>
    </section>
    <section id="skills" aria-labelledby="skills-title">
      <div class="section-head"><h2 id="skills-title">What I work with</h2></div>
      <div class="skills">
        <div class="skill"><h3>Security &amp; investigation</h3><p>Log analysis, phishing analysis, threat detection, incident investigation, and network security.</p></div>
        <div class="skill"><h3>Tools &amp; environments</h3><p>Splunk, Wireshark, Wazuh, VMware, Windows, and Linux.</p></div>
        <div class="skill"><h3>Code &amp; documentation</h3><p>Python, SQL, Git, SPL searches, investigation reports, and technical documentation.</p></div>
      </div>
    </section>
    <section id="about" aria-labelledby="about-title" class="about">
      <h2 id="about-title">A little about me</h2>
      <div>
        <p>I'm based in <strong>Winnipeg, Manitoba</strong>, and studying Cybersecurity at <strong>Red River College Polytechnic</strong>. I'm particularly interested in security operations and phishing prevention.</p>
        <p>I enjoy building lab environments, investigating what the logs reveal, and explaining my findings clearly. This portfolio follows that work as I keep learning.</p>
        <a class="project-link" href="https://github.com/Saif-Zeid">Find me on GitHub <span aria-hidden="true">↗</span></a>
      </div>
    </section>
  </main>
  <footer><span>Saif Zeid · Cybersecurity portfolio</span><a href="#main">Back to top ↑</a></footer>
</div>
</body>
</html>
