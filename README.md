
<style>
  * { box-sizing: border-box; margin: 0; padding: 0; }
  body { background: transparent; }
  .wrap { font-family: 'Courier New', monospace; padding: 16px 0; }
  .screen { background: #0d0d0d; border-radius: 12px; border: 1px solid #1a1a1a; overflow: hidden; max-width: 660px; margin: 0 auto; }
  .bar { background: #1a1a1a; padding: 10px 14px; display: flex; align-items: center; gap: 8px; border-bottom: 1px solid #222; }
  .dot { width: 11px; height: 11px; border-radius: 50%; }
  .bar-title { color: #555; font-size: 12px; margin-left: auto; margin-right: auto; letter-spacing: 2px; }
  .body { padding: 20px 24px 24px; }
  .header { text-align: center; margin-bottom: 22px; }
  .name { color: #00FF41; font-size: 22px; font-weight: bold; letter-spacing: 4px; line-height: 1; }
  .sub { color: #555; font-size: 11px; letter-spacing: 3px; margin-top: 6px; }
  .blink { animation: blink 1s step-end infinite; }
  @keyframes blink { 0%,100%{opacity:1} 50%{opacity:0} }
  .divider { border: none; border-top: 1px solid #1e1e1e; margin: 14px 0; }
  .terminal-lines { margin-bottom: 18px; }
  .line { display: flex; gap: 8px; margin-bottom: 6px; font-size: 13px; line-height: 1.5; opacity: 0; }
  .line.show { opacity: 1; }
  .prompt { color: #00FF41; flex-shrink: 0; }
  .cmd { color: #888; }
  .val { color: #fff; }
  .pink { color: #FF0080; }
  .gold { color: #FFD700; }
  .blue { color: #00BFFF; }
  .skills-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 10px; margin-bottom: 18px; }
  .skill-group { }
  .skill-label { color: #444; font-size: 10px; letter-spacing: 2px; margin-bottom: 6px; }
  .skill-bar-row { display: flex; align-items: center; gap: 7px; margin-bottom: 4px; }
  .skill-name { color: #888; font-size: 11px; width: 68px; flex-shrink: 0; }
  .bar-track { flex: 1; height: 5px; background: #1a1a1a; border-radius: 3px; overflow: hidden; }
  .bar-fill { height: 100%; border-radius: 3px; width: 0; transition: width 1.2s cubic-bezier(.4,0,.2,1); }
  .links { display: flex; gap: 10px; justify-content: center; }
  .link-btn { background: #111; border: 1px solid #222; color: #666; font-family: 'Courier New', monospace; font-size: 11px; padding: 6px 14px; border-radius: 6px; cursor: pointer; letter-spacing: 1px; transition: all .2s; text-decoration: none; }
  .link-btn:hover { border-color: #00FF41; color: #00FF41; }
  .stats-row { display: flex; gap: 10px; margin-bottom: 18px; }
  .stat { flex: 1; background: #111; border: 1px solid #1a1a1a; border-radius: 8px; padding: 10px 12px; text-align: center; }
  .stat-val { font-size: 18px; font-weight: bold; }
  .stat-lbl { color: #444; font-size: 10px; letter-spacing: 1px; margin-top: 3px; }
</style>
<div class="wrap">
  <div class="screen">
    <div class="bar">
      <div class="dot" style="background:#ff5f56"></div>
      <div class="dot" style="background:#ffbd2e"></div>
      <div class="dot" style="background:#27c93f"></div>
      <span class="bar-title">alb3rt05 — bash</span>
    </div>
    <div class="body">
      <div class="header">
        <div class="name">ALBERTO<span class="blink">_</span></div>
        <div class="sub">FULLSTACK DEVELOPER</div>
      </div>
      <hr class="divider"/>
      <div class="terminal-lines" id="lines">
        <div class="line" data-delay="100"><span class="prompt">$</span><span class="cmd">whoami</span></div>
        <div class="line" data-delay="400"><span class="prompt">→</span><span class="val">Fullstack dev · Angular · Vue · Next.js · Java · Python</span></div>
        <div class="line" data-delay="900"><span class="prompt">$</span><span class="cmd">cat status.txt</span></div>
        <div class="line" data-delay="1200"><span class="prompt">→</span><span class="pink">ONLINE</span><span class="val"> · Building things that matter</span></div>
        <div class="line" data-delay="1700"><span class="prompt">$</span><span class="cmd">git log --oneline -1</span></div>
        <div class="line" data-delay="2000"><span class="prompt">→</span><span class="gold">627 commits</span><span class="val"> · still going strong</span></div>
        <div class="line" data-delay="2500"><span class="prompt">$</span><span class="cmd">open portfolio</span></div>
        <div class="line" data-delay="2800"><span class="prompt">→</span><span class="blue">albertocostanzo.netlify.app</span><span class="blink" style="color:#00FF41"> ▌</span></div>
      </div>
      <hr class="divider"/>
      <div class="skills-grid" id="skills-grid">
        <div class="skill-group">
          <div class="skill-label">FRONTEND</div>
          <div class="skill-bar-row"><span class="skill-name">Angular</span><div class="bar-track"><div class="bar-fill" data-w="90" style="background:#DD0031"></div></div></div>
          <div class="skill-bar-row"><span class="skill-name">Vue</span><div class="bar-track"><div class="bar-fill" data-w="85" style="background:#4FC08D"></div></div></div>
          <div class="skill-bar-row"><span class="skill-name">Next.js</span><div class="bar-track"><div class="bar-fill" data-w="80" style="background:#aaa"></div></div></div>
          <div class="skill-bar-row"><span class="skill-name">TypeScript</span><div class="bar-track"><div class="bar-fill" data-w="88" style="background:#007ACC"></div></div></div>
        </div>
        <div class="skill-group">
          <div class="skill-label">BACKEND & DATA</div>
          <div class="skill-bar-row"><span class="skill-name">Java</span><div class="bar-track"><div class="bar-fill" data-w="82" style="background:#ED8B00"></div></div></div>
          <div class="skill-bar-row"><span class="skill-name">Python</span><div class="bar-track"><div class="bar-fill" data-w="75" style="background:#3776AB"></div></div></div>
          <div class="skill-bar-row"><span class="skill-name">MongoDB</span><div class="bar-track"><div class="bar-fill" data-w="78" style="background:#47A248"></div></div></div>
          <div class="skill-bar-row"><span class="skill-name">SQL</span><div class="bar-track"><div class="bar-fill" data-w="80" style="background:#4479A1"></div></div></div>
        </div>
      </div>
      <hr class="divider"/>
      <div class="stats-row">
        <div class="stat"><div class="stat-val" style="color:#00FF41">627</div><div class="stat-lbl">COMMITS</div></div>
        <div class="stat"><div class="stat-val" style="color:#FF0080">3+</div><div class="stat-lbl">YEARS XP</div></div>
        <div class="stat"><div class="stat-val" style="color:#FFD700">99</div><div class="stat-lbl">LVL</div></div>
        <div class="stat"><div class="stat-val" style="color:#00BFFF">∞</div><div class="stat-lbl">COFFEE</div></div>
      </div>
      <div class="links">
        <a class="link-btn" href="https://albertocostanzo.netlify.app">▶ PORTFOLIO</a>
        <a class="link-btn" href="mailto:alberto.cosyanzo05@gmail.com">✉ EMAIL</a>
        <a class="link-btn" href="https://instagram.com/0__albert__5">◈ INSTAGRAM</a>
      </div>
    </div>
  </div>
</div>
<script>
  document.querySelectorAll('#lines .line').forEach(el => {
    setTimeout(() => el.classList.add('show'), parseInt(el.dataset.delay));
  });
  setTimeout(() => {
    document.querySelectorAll('.bar-fill').forEach(el => {
      el.style.width = el.dataset.w + '%';
    });
  }, 3200);
</script>
