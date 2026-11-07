---
permalink: /
title: ""
excerpt: "Home"
author_profile: true
redirect_from: 
  - /home/
  - /home.html
---

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&family=Lora:ital,wght@0,400;0,600;1,400&family=Merriweather:wght@400;700;900&display=swap" rel="stylesheet">
<style>
:root { --head:"Merriweather",Georgia,serif; --text:"Lora",Georgia,serif; --ui:"Inter","Open Sans",system-ui,sans-serif;
  --ink:#1b2430; --acc:#0f6b66; --acc-soft:rgba(15,107,102,0.09); --red:#a02a3a; --rule:rgba(20,30,45,0.28); --mut:#4f5d6b; --on-acc:#fff; --glow:160,42,58; }
@media (prefers-color-scheme: dark) { :root { --ink:#eef2f6; --acc:#6fd6c9; --acc-soft:rgba(111,214,201,0.10); --red:#f4a3b0; --rule:rgba(255,255,255,0.24); --mut:#aab6c3; --on-acc:#0b1318; --glow:244,163,176; } }
:root[data-hp="light"] { --ink:#1b2430; --acc:#0f6b66; --acc-soft:rgba(15,107,102,0.09); --red:#a02a3a; --rule:rgba(20,30,45,0.28); --mut:#4f5d6b; --on-acc:#fff; --glow:160,42,58; }
:root[data-hp="dark"] { --ink:#eef2f6; --acc:#6fd6c9; --acc-soft:rgba(111,214,201,0.10); --red:#f4a3b0; --rule:rgba(255,255,255,0.24); --mut:#aab6c3; --on-acc:#0b1318; --glow:244,163,176; }
.chip, .copy { font-family:var(--ui); }
.bio { font-family:var(--text); line-height:1.7; color:var(--ink); }
.bio strong { font-family:var(--head); font-weight:700; }
.kicker { font-family:var(--ui); font-size:0.72em; letter-spacing:0.14em; text-transform:uppercase; color:var(--red); font-weight:700; margin:0 0 0.4em; }
h2[id] { position:relative; display:flex; align-items:center; gap:0.8em; margin:2.4em 0 0.9em; padding-bottom:0.45em; font-family:var(--head); font-size:1em; font-weight:700; letter-spacing:0.16em; text-transform:uppercase; color:var(--ink); border-bottom:1px solid var(--rule); }
h2[id]::after { content:""; position:absolute; left:0; bottom:-1px; width:3.2rem; height:3px; background:var(--acc); }
.hint { font-size:0.82em; font-style:italic; color:var(--mut); margin:-0.4em 0 0.9em; }
.timeline { list-style:none; margin:0; padding:0 0 0 1.6em; position:relative; }
.timeline::before { content:""; position:absolute; left:0.45em; top:0.4em; bottom:0.4em; width:2px; background:var(--rule); }
.timeline::after { content:""; position:absolute; left:0.45em; top:0.4em; width:2px; height:var(--fill,0%); max-height:calc(100% - 0.8em); background:var(--acc); transition:height 1.4s ease; }
.timeline li { position:relative; margin:0 0 1.3em; padding:0.5em 0.9em; border-radius:2px; transition:background 0.25s ease; }
.timeline li::before { content:""; position:absolute; left:-1.55em; top:0.95em; width:0.8em; height:0.8em; border-radius:50%; background:var(--bgc,#fff); border:2px solid var(--acc); transition:background 0.25s ease,transform 0.25s ease; }
.timeline li:hover { background:var(--acc-soft); }
.timeline li:hover::before { background:var(--acc); transform:scale(1.25); }
.timeline li.now::before { background:var(--red); border-color:var(--red); animation:tlPulse 1.8s ease-out infinite; }
@keyframes tlPulse { 0% { box-shadow:0 0 0 0 rgba(var(--glow),0.45); } 100% { box-shadow:0 0 0 10px rgba(var(--glow),0); } }
.tl-year { font-family:var(--ui); font-size:0.74em; letter-spacing:0.1em; color:var(--acc); }
.tl-what { display:block; font-family:var(--head); font-weight:700; color:var(--ink); }
.tl-where { display:block; font-family:var(--text); font-size:0.9em; color:var(--mut); }
.chips { display:flex; flex-wrap:wrap; gap:0.5em; margin:0 0 0.6em; }
.chip { font:inherit; font-size:0.88em; cursor:pointer; padding:0.4em 0.9em; color:var(--ink); background:transparent; border:1px solid var(--rule); border-radius:2px; transition:all 0.2s ease; }
.chip:hover { border-color:var(--acc); color:var(--acc); transform:translateY(-2px); }
.chip[aria-pressed="true"] { background:var(--acc); border-color:var(--acc); color:var(--on-acc); }
.chip:focus-visible { outline:2px solid var(--acc); outline-offset:2px; }
.related { min-height:3.2em; margin:0.4em 0 0; padding:0.8em 1.1em; border-left:3px solid var(--acc); background:var(--acc-soft); font-family:var(--text); font-size:0.93em; line-height:1.6; }
.related.empty { color:var(--mut); font-style:italic; }
.related .rl-h { font-family:var(--ui); font-size:0.72em; letter-spacing:0.12em; text-transform:uppercase; color:var(--red); margin-bottom:0.4em; }
.related ul { margin:0; padding-left:1.1em; }
.related a { color:var(--acc); text-decoration:none; border-bottom:1px dotted var(--acc); }
.related a:hover { color:var(--ink); }
.related.fade { animation:abRise 0.3s ease; }
@keyframes abRise { from { opacity:0; transform:translateY(6px); } to { opacity:1; transform:none; } }
.stats { display:grid; grid-template-columns:repeat(auto-fit,minmax(170px,1fr)); gap:0.9em; }
.stat { padding:0.9em 1em 0.8em; border:1px solid var(--rule); border-top:3px solid var(--acc); border-radius:2px; transition:transform 0.25s ease,border-color 0.25s ease,background 0.25s ease; }
.stat:hover { transform:translateY(-4px); border-color:var(--acc); background:var(--acc-soft); }
.stat .num { font-family:var(--head); font-size:2.1em; font-weight:700; line-height:1; color:var(--ink); }
.stat .num small { font-size:0.42em; margin-left:0.25em; letter-spacing:0.08em; color:var(--acc); }
.stat .txt { font-family:var(--text); margin:0.5em 0 0.3em; font-size:0.84em; line-height:1.4; }
.stat .src { font-family:var(--ui); font-size:0.66em; letter-spacing:0.06em; text-transform:uppercase; color:var(--mut); }
.contact { display:flex; flex-direction:column; gap:0.6em; }
.mail { display:flex; align-items:center; flex-wrap:wrap; gap:0.7em; }
.mail a { font-family:var(--ui); font-size:0.9em; color:var(--acc); text-decoration:none; border-bottom:1px solid var(--acc); }
.mail a:hover { color:var(--ink); border-bottom-color:var(--ink); }
.copy { font:inherit; font-size:0.72em; font-weight:700; letter-spacing:0.08em; text-transform:uppercase; cursor:pointer; padding:0.3em 0.8em; color:var(--acc); background:transparent; border:1px solid var(--acc); border-radius:2px; transition:all 0.2s; }
.copy:hover, .copy.ok { background:var(--acc); color:var(--on-acc); }
@media (prefers-reduced-motion: reduce) { .timeline::after, .related.fade, .timeline li.now::before { animation:none !important; transition:none !important; } .stat, .chip { transition:none; } }
</style>

<p class="kicker">Welcome to my website</p>

<p class="bio">I am a <strong>Ph.D. scholar in Development Studies</strong> in the Department of Liberal Arts at the <strong>Indian Institute of Technology Hyderabad (IITH)</strong>, India. My current research focuses on the <strong>causal impact of internet access on women's attitudes and behaviour</strong>. My doctoral thesis studies these aspects in the context of India.</p>

## Education

<ul class="timeline" id="timeline">
<li class="now"><span class="tl-year">Present</span><span class="tl-what">Ph.D., Development Studies</span><span class="tl-where">Department of Liberal Arts, Indian Institute of Technology Hyderabad</span></li>
<li><span class="tl-year">2023</span><span class="tl-what">Master’s, Population Studies and Health Economics</span><span class="tl-where">Gokhale Institute of Politics and Economics, Pune</span></li>
<li><span class="tl-year">2021</span><span class="tl-what">Bachelor’s, Economics</span><span class="tl-where">University of Calcutta</span></li>
</ul>

## Research Interests

<p class="hint">Select an interest to see the related work.</p>
<div class="chips" id="chips">
<button type="button" class="chip" data-k="micro" aria-pressed="false">Applied Microeconometrics</button>
<button type="button" class="chip" data-k="dev" aria-pressed="false">Empirical Development Economics</button>
<button type="button" class="chip" data-k="gender" aria-pressed="false">Gender Economics</button>
<button type="button" class="chip" data-k="health" aria-pressed="false">Health Economics</button>
<button type="button" class="chip" data-k="political" aria-pressed="false">Political Economy</button>
</div>
<div class="related empty" id="related" aria-live="polite">Nothing selected yet.</div>

## Findings at a Glance

<p class="hint">Headline estimates from my papers, in percentage points.</p>
<div class="stats" id="stats">
<div class="stat"><div class="num"><span class="n" data-v="21" data-d="0">21</span><small>pp</small></div><p class="txt">Lower likelihood of a woman justifying intimate partner violence when exposed to the internet</p><div class="src">Rewiring Gender Norms</div></div>
<div class="stat"><div class="num"><span class="n" data-v="17" data-d="0">17</span><small>pp</small></div><p class="txt">Lower risk of experiencing intimate partner violence among women with internet access</p><div class="src">The Protective Power of Connectivity</div></div>
<div class="stat"><div class="num"><span class="n" data-v="10" data-d="0">10</span><small>pp</small></div><p class="txt">Higher overall financial autonomy among women with internet exposure</p><div class="src">Banking on Connectivity</div></div>
<div class="stat"><div class="num"><span class="n" data-v="12.8" data-d="1">12.8</span><small>pp</small></div><p class="txt">Rise in primary LPG adoption after Bihar’s alcohol prohibition</p><div class="src">From Liquor to LPG</div></div>
<div class="stat"><div class="num"><span class="n" data-v="7" data-d="0">7</span><small>pp</small></div><p class="txt">Higher chance of hygienic period product use for each extra year of age at marriage</p><div class="src">Knot Too Early</div></div>
<div class="stat"><div class="num"><span class="n" data-v="2.5" data-d="1">2.5</span><small>pp</small></div><p class="txt">Higher chance of major depression in later life for women exposed to a riot in childhood</p><div class="src">The Long Shadow of Communal Violence</div></div>
</div>

## Contact

<div class="contact">
<div class="mail"><a href="mailto:la24resch11001@iith.ac.in">la24resch11001@iith.ac.in</a><button type="button" class="copy" data-m="la24resch11001@iith.ac.in">Copy</button></div>
<div class="mail"><a href="mailto:sagnikkumargupta00@gmail.com">sagnikkumargupta00@gmail.com</a><button type="button" class="copy" data-m="sagnikkumargupta00@gmail.com">Copy</button></div>
</div>

<script>
(function () {
  var RELATED = {
    micro: ['Applied Microeconometrics', ['Rewiring Gender Norms (Instrumental variables)', 'The Protective Power of Connectivity (Instrumental variables)', 'Banking on Connectivity (Instrumental variables)', 'Knot Too Early (Instrumental variables)', 'From Liquor to LPG (Matched difference-in-differences)', 'The Long Shadow of Communal Violence (Variation across districts and birth cohorts)']],
    dev: ['Empirical Development Economics', ['Rewiring Gender Norms', 'The Protective Power of Connectivity', 'Banking on Connectivity', 'Knot Too Early', 'From Liquor to LPG', 'The Long Shadow of Communal Violence']],
    gender: ['Gender Economics', ['Rewiring Gender Norms', 'The Protective Power of Connectivity', 'Banking on Connectivity', 'Knot Too Early', 'The Long Shadow of Communal Violence']],
    health: ['Health Economics', ['The Protective Power of Connectivity (Intimate partner violence)', 'Knot Too Early (Menstrual hygiene)', 'The Long Shadow of Communal Violence (Mental health)']],
    political: ['Political Economy', ['The Long Shadow of Communal Violence', 'From Liquor to LPG (Alcohol prohibition policy)']]
  };
  var chips = Array.prototype.slice.call(document.querySelectorAll('.chip'));
  var panel = document.getElementById('related');
  chips.forEach(function (b) {
    b.addEventListener('click', function () {
      var already = b.getAttribute('aria-pressed') === 'true';
      chips.forEach(function (x) { x.setAttribute('aria-pressed', 'false'); });
      panel.classList.remove('fade');
      void panel.offsetWidth;
      if (already) { panel.className = 'related empty'; panel.textContent = 'Nothing selected yet.'; return; }
      b.setAttribute('aria-pressed', 'true');
      var d = RELATED[b.getAttribute('data-k')];
      var html = '<div class="rl-h">Related work · ' + d[0] + '</div><ul>';
      d[1].forEach(function (t) { html += '<li><a href="/research/">' + t + '</a></li>'; });
      panel.className = 'related fade';
      panel.innerHTML = html + '</ul>';
    });
  });
  var reduce = window.matchMedia && window.matchMedia('(prefers-reduced-motion: reduce)').matches;
  var tl = document.getElementById('timeline');
  function lum(c){var m=c.match(/[\d.]+/g);if(!m||(m.length>3&&+m[3]===0))return null;return (0.299*m[0]+0.587*m[1]+0.114*m[2])/255;}
  function sync(){
    var el=document.body,c=null;
    while(el){c=getComputedStyle(el).backgroundColor;if(lum(c)!==null)break;el=el.parentElement;}
    var l=lum(c||'');
    if(l!==null)document.documentElement.setAttribute('data-hp',l<0.5?'dark':'light');
    if(tl)tl.style.setProperty('--bgc',(l!==null)?c:'#fff');
  }
  sync();
  try{new MutationObserver(sync).observe(document.documentElement,{attributes:true,attributeFilter:['class','data-theme']});}catch(e){}
  document.addEventListener('click',function(){setTimeout(sync,60);});
  if(window.matchMedia)window.matchMedia('(prefers-color-scheme: dark)').addEventListener('change',function(){setTimeout(sync,60);});
  if (tl) {
    if ('IntersectionObserver' in window && !reduce) {
      var o1 = new IntersectionObserver(function (e) { if (e[0].isIntersecting) { tl.style.setProperty('--fill', '100%'); o1.disconnect(); } }, { threshold: 0.3 });
      o1.observe(tl);
    } else { tl.style.setProperty('--fill', '100%'); }
  }
  var nums = Array.prototype.slice.call(document.querySelectorAll('.n'));
  function run(el) {
    var v = parseFloat(el.getAttribute('data-v')), d = parseInt(el.getAttribute('data-d'), 10), t0 = null;
    function f(t) {
      if (t0 === null) { t0 = t; }
      var p = Math.min((t - t0) / 1100, 1), e = 1 - Math.pow(1 - p, 3);
      el.textContent = (v * e).toFixed(d);
      if (p < 1) { requestAnimationFrame(f); }
    }
    requestAnimationFrame(f);
  }
  if ('IntersectionObserver' in window && !reduce) {
    nums.forEach(function (n) { n.textContent = (0).toFixed(parseInt(n.getAttribute('data-d'), 10)); });
    var o2 = new IntersectionObserver(function (es) { es.forEach(function (x) { if (x.isIntersecting) { run(x.target); o2.unobserve(x.target); } }); }, { threshold: 0.6 });
    nums.forEach(function (n) { o2.observe(n); });
  }
  Array.prototype.forEach.call(document.querySelectorAll('.copy'), function (b) {
    b.addEventListener('click', function () {
      var m = b.getAttribute('data-m');
      var done = function () { b.classList.add('ok'); b.textContent = 'Copied'; setTimeout(function () { b.classList.remove('ok'); b.textContent = 'Copy'; }, 1600); };
      if (navigator.clipboard && navigator.clipboard.writeText) { navigator.clipboard.writeText(m).then(done); }
      else { var t = document.createElement('textarea'); t.value = m; document.body.appendChild(t); t.select(); try { document.execCommand('copy'); done(); } catch (x) {} document.body.removeChild(t); }
    });
  });
})();
</script>
