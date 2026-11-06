---
permalink: /research/
title: ""
---

<style>
:root { --acc:#52adc8; --acc2:#7c5cff; --gold:#d4a017; --card:rgba(255,255,255,0.72); --bd:rgba(82,173,200,0.28); --mut:#6b7280; --shadow:rgba(40,70,110,0.14); }
@media (prefers-color-scheme: dark) { :root { --card:rgba(30,41,59,0.6); --mut:#9aa4b2; --shadow:rgba(0,0,0,0.45); } }
#rp-bar { position:fixed; top:0; left:0; height:3px; width:0; z-index:9999; background:linear-gradient(90deg,var(--acc),var(--acc2),#ff6fb5); transition:width 0.1s linear; }
h1[id] { display:flex; align-items:center; gap:0.6em; font-weight:800; letter-spacing:0.01em; margin:1.6em 0 0.8em; background:linear-gradient(100deg,var(--acc),var(--acc2) 55%,#ff6fb5); background-size:200% 100%; -webkit-background-clip:text; background-clip:text; -webkit-text-fill-color:transparent; animation:rpShift 8s ease-in-out infinite alternate; }
h1[id]::after { content:""; flex:1; height:2px; border-radius:2px; background:linear-gradient(90deg,var(--acc),transparent); }
h1[id] .count { order:2; -webkit-text-fill-color:#fff; background:linear-gradient(135deg,var(--acc),var(--acc2)); font-size:0.42em; font-weight:700; padding:0.25em 0.8em; border-radius:999px; box-shadow:0 2px 8px var(--shadow); }
@keyframes rpShift { from { background-position:0% 50%; } to { background-position:100% 50%; } }
hr { border:0; height:1px; background:linear-gradient(90deg,transparent,var(--bd),transparent); margin:2.2em 0 0.5em; }
.abs-bar { display:flex; justify-content:flex-end; margin:0.5em 0 -0.5em; }
.abs-toggle { cursor:pointer; border:1px solid var(--bd); background:var(--card); color:var(--acc); font-weight:700; font-size:0.8em; padding:0.45em 1.1em; border-radius:999px; backdrop-filter:blur(6px); transition:all 0.25s ease; }
.abs-toggle:hover { background:linear-gradient(135deg,var(--acc),var(--acc2)); color:#fff; transform:translateY(-2px); box-shadow:0 6px 16px var(--shadow); }
ul:has(> li.entry) { list-style:none; padding-left:0; margin-left:0; }
li.entry { --mx:50%; --my:50%; position:relative; list-style:none; margin:0 0 1.3em; padding:1.2em 1.4em 0.9em 1.7em; border-radius:16px; border:1px solid var(--bd); background:radial-gradient(420px circle at var(--mx) var(--my),rgba(124,92,255,0.13),transparent 45%),var(--card); backdrop-filter:blur(8px); box-shadow:0 4px 18px var(--shadow); transition:transform 0.3s ease,box-shadow 0.3s ease,border-color 0.3s ease; }
li.entry::before { content:""; position:absolute; left:0; top:14px; bottom:14px; width:4px; border-radius:4px; background:linear-gradient(180deg,var(--acc),var(--acc2)); transition:top 0.3s,bottom 0.3s,box-shadow 0.3s; }
li.entry:hover { transform:translateY(-4px); box-shadow:0 14px 32px var(--shadow); border-color:var(--acc); }
li.entry:hover::before { top:6px; bottom:6px; box-shadow:0 0 14px var(--acc); }
li.entry:has(.journal) { border-color:rgba(212,160,23,0.55); }
li.entry:has(.journal)::before { background:linear-gradient(180deg,#ffd76a,var(--gold)); }
li.entry:has(.journal)::after { content:"★ PUBLISHED"; position:absolute; top:-0.7em; right:1.1em; font-size:0.66em; font-weight:800; letter-spacing:0.08em; color:#4a3500; background:linear-gradient(135deg,#ffe58a,#f0b429); padding:0.3em 0.9em; border-radius:999px; box-shadow:0 3px 10px rgba(212,160,23,0.4); }
li.entry:has(> span.paper-title) { border-style:dashed; }
li.entry:has(> span.paper-title)::after { content:"⏳ IN PROGRESS"; position:absolute; top:-0.7em; right:1.1em; font-size:0.66em; font-weight:800; letter-spacing:0.08em; color:#fff; background:linear-gradient(135deg,var(--acc2),#ff6fb5); padding:0.3em 0.9em; border-radius:999px; }
.rv li.entry { opacity:0; transform:translateY(24px); }
.rv li.entry.in { opacity:1; transform:none; transition:opacity 0.7s ease,transform 0.7s ease,box-shadow 0.3s ease,border-color 0.3s ease; }
.rv li.entry.in:hover { transform:translateY(-4px); transition:transform 0.3s ease,box-shadow 0.3s ease,border-color 0.3s ease; }
.paper-title { font-weight:700; font-size:1.07em; line-height:1.4; text-decoration:none !important; background:linear-gradient(90deg,var(--acc),var(--acc2)) 0 100% / 0% 2px no-repeat; transition:background-size 0.4s ease; }
a.paper-title:hover { background-size:100% 2px; }
.journal { display:inline-block; margin:0.3em 0; font-size:0.92em; font-weight:600; color:var(--gold); }
.outlet { display:inline-block; margin:0.3em 0; font-size:0.92em; font-weight:600; color:var(--acc2); }
.glo-link { display:inline-block; margin:0.35em 0.2em 0.2em 0; padding:0.1em 0.85em; font-size:0.78em; font-weight:700; letter-spacing:0.02em; border:1px solid var(--bd); border-radius:999px; text-decoration:none !important; transition:all 0.25s ease; }
a.glo-link:hover { color:#fff !important; background:linear-gradient(135deg,var(--acc),var(--acc2)); border-color:transparent; transform:translateY(-2px); box-shadow:0 5px 14px var(--shadow); }
.authors { display:block; margin-top:0.2em; font-size:0.9em; font-style:italic; color:var(--mut); }
details.abstract { margin:0.6em 0 0.3em; }
details.abstract > summary { display:inline-flex; align-items:center; gap:0.5em; cursor:pointer; list-style:none; user-select:none; font-size:0.84em; font-weight:700; letter-spacing:0.04em; color:var(--acc); padding:0.2em 0; transition:color 0.2s ease; }
details.abstract > summary::-webkit-details-marker { display:none; }
details.abstract > summary::marker { content:""; }
details.abstract > summary::before { content:""; width:0.5em; height:0.5em; border-right:2px solid currentColor; border-bottom:2px solid currentColor; transform:rotate(-45deg); transition:transform 0.3s ease; margin-right:0.15em; }
details.abstract[open] > summary::before { transform:rotate(45deg); }
details.abstract > summary:hover { color:var(--acc2); }
details.abstract > summary:focus-visible { outline:2px solid var(--acc); outline-offset:3px; border-radius:3px; }
details.abstract .abstract-text { margin:0.5em 0 0.4em; padding:0.9em 1.2em; border-left:3px solid var(--acc2); border-radius:0 10px 10px 0; background:linear-gradient(135deg,rgba(82,173,200,0.1),rgba(124,92,255,0.08)); font-size:0.92em; line-height:1.7; text-align:justify; }
details.abstract[open] .abstract-text { animation:rpFade 0.35s ease; }
@keyframes rpFade { from { opacity:0; transform:translateY(-8px); } to { opacity:1; transform:none; } }
@media (prefers-reduced-motion: reduce) { h1[id], li.entry, details.abstract .abstract-text { animation:none !important; transition:none !important; } .rv li.entry { opacity:1; transform:none; } }
</style>

<div id="rp-bar"></div>
<div class="abs-bar"><button class="abs-toggle" id="abs-toggle" type="button">▾ Expand all abstracts</button></div>

# Peer-reviewed Publications

* <a href="https://link.springer.com/article/10.1007/s11150-026-09887-5" class="paper-title">
Rewiring Gender Norms: Causal Evidence on Internet Exposure and Justification of Intimate Partner Violence
</a>  
<span class="journal"><em>Review of Economics of the Household</em>, 2026</span>  
<a href="https://www.econstor.eu/handle/10419/333329" class="glo-link">GLO Discussion Paper</a>  
<span class="authors">
with <a href="https://maniniojha.wordpress.com/">Dr. Manini Ojha</a>,
Sagnik Kumar Gupta and
<a href="https://gauravdhamija5.weebly.com/">Dr. Gaurav Dhamija</a>
</span>
<details class="abstract">
<summary>Abstract</summary>
<div class="abstract-text">
This paper evaluates the causal impact of women’s exposure to the internet on their attitudes towards intimate partner violence using data from the most recent round of the National Family Health Survey. To address potential endogeneity, we exploit exogenous variation in district-level mobile tower density in India as an instrument for women’s internet exposure. The instrumental variables estimation provides evidence that a woman’s exposure to internet reduces her likelihood of justifying intimate partner violence by 21 percentage points. The results are robust to an extensive set of individual, household, and district-level controls, alternative definitions of both the exposure and outcome variables, and a range of falsification tests. Sub-sample analyses reveal that the effect holds across social group, wealth, education, and geography, with particularly strong effects among women in non-poor households, with lower education, and in urban areas. We further provide suggestive evidence that internet exposure increases women’s employment, awareness, relaxes mobility constraints, and reduces husbands’ justification of intimate partner violence. It suggests that changes in both women’s opportunities and intra-household gender norms constitute potential pathways through which internet exposure reduces women’s justification of intimate partner violence. Overall, the findings highlight the transformative potential of digital connectivity in challenging regressive gender norms.
</div>
</details>

---

# Working Papers

* <a href="https://www.econstor.eu/handle/10419/331320" class="paper-title">
The Protective Power of Connectivity: Internet Exposure and Intimate Partner Violence
</a>  
<a href="/files/pdf/GLO-DP-1690.pdf" class="glo-link">GLO Discussion Paper</a>  
<span class="authors">
with <a href="https://gauravdhamija5.weebly.com/">Dr. Gaurav Dhamija</a> and
<a href="https://maniniojha.wordpress.com/">Dr. Manini Ojha</a>
</span>
<details class="abstract">
<summary>Abstract</summary>
<div class="abstract-text">
We study the effect of women’s exposure to the internet on the incidence of intimate partner violence (IPV) utilizing data from a large-scale nationally representative data for India. Utilizing an instrumental variable approach, we exploit the exogenous variation arising from cellular tower density at the district level as an instrument for internet exposure. We find women who have access to the internet are at a significantly lower risk of exposure to physical, sexual, emotional and any IPV by 17, 5, 9 and 18 percentage points. We provide further indicative evidence that women’s attitudes justifying violence works as a channel of our estimated causal impacts. Our results are robust to a host of sensitivity checks, additional controls, alternative definitions and falsification analysis. We document important heterogeneity in the effects across social groups, wealth index, area of residence, and women’s education levels. The effects appear to be particularly important for women from wealthier households and those who are more educated.
</div>
</details>

* <a href="https://www.econstor.eu/handle/10419/333697" class="paper-title">
Banking on Connectivity: Internet Exposure and Women’s Financial Autonomy
</a>  
<a href="/files/pdf/GLO-DP-1697.pdf" class="glo-link">GLO Discussion Paper</a>  
<span class="authors">
with <a href="https://gauravdhamija5.weebly.com/">Dr. Gaurav Dhamija</a> and
<a href="https://maniniojha.wordpress.com/">Dr. Manini Ojha</a>
</span>
<details class="abstract">
<summary>Abstract</summary>
<div class="abstract-text">
We examine whether women's exposure to the internet enhances their economic agency in India. Using nationally representative data and an instrumental variables strategy that exploits plausibly exogenous variation in district-level mobile tower density, we identify the causal effect of internet access on women's financial control and use of formal banks. We find that internet exposure increases women's overall financial autonomy by 10 percentage points. We document improvements in independent mobility, employment, and financial awareness which we consider potential mechanisms of our estimated effects. Disaggregated outcomes show higher likelihood that women have money of their own over which they full control, as well as increased ownership and active use of a bank account. Our results are robust to additional controls and a battery of sensitivity analyses. Heterogeneity analyses indicate that effects are concentrated among women with at least secondary education, and among those from historically disadvantaged social groups. Overall, our findings highlight the importance of digital connectivity in enhancing the usage of financial resources, with important implications for women's autonomy and participation in the formal economy.
</div>
</details>

* <a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6257379" class="paper-title">
Knot Too Early: The Causal Impact of Women's Age at Marriage on Period Product Use
</a>  
<a href="/files/pdf/ssrn-6257379.pdf" class="glo-link">Working Paper</a>  
<span class="authors">
with <a href="https://sites.google.com/iima.ac.in/karan-babbar/home">Dr. Karan Babbar</a> and
<a href="https://gauravdhamija5.weebly.com/">Dr. Gaurav Dhamija</a>
</span>
<details class="abstract">
<summary>Abstract</summary>
<div class="abstract-text">
This paper evaluates the causal impact of women’s age at marriage on their likelihood of using hygienic period products, using the most recent round of the National Family Health Survey (NFHS-5) in India. To address potential endogeneity, we exploit exogenous variation in a woman's age at menarche as an instrument for her age at marriage. The instrumental variable (IV) estimation provides robust evidence that a one-year increase in a woman's age at marriage increases, on an average, the likelihood of hygienic product use by 7 percentage points. We also provide suggestive evidence that higher education and increased household decision-making power are potential mechanisms driving this effect. These findings signify the importance of enforcing laws regulating the legal age of marriage, and highlight the broader need for societal shifts that promote later marriage, better menstrual hygiene, and the empowerment of young women.
</div>
</details>

* <a href="https://www.policyedge.in/working-paper/wp-from-liquor-to-lpg-spillover-effects-of-alcohol-prohibition-on-clean-fuel-adoption" class="paper-title">
From Liquor to LPG: Spillover effects of alcohol prohibition on clean fuel adoption
</a>  
<a href="/files/pdf/TPE_WP_2026-0001.pdf" class="glo-link"> Policy Edge Working Paper</a>  
<span class="authors">
with <a href="https://gauravdhamija5.weebly.com/">Dr. Gaurav Dhamija</a> and
<a href="https://maniniojha.wordpress.com/">Dr. Manini Ojha</a>
</span>
<details class="abstract">
<summary>Abstract</summary>
<div class="abstract-text">
This paper examines whether Bihar’s 2016 alcohol prohibition generated spillover effects on household adoption of LPG as a primary cooking fuel. Although clean cooking lies well outside the policy’s intended scope, prohibition may affect fuel choice by altering household expenditure patterns and intra-household dynamics. Using repeated cross-sectional data from the Household Consumption Expenditure Surveys of 2011–12 and 2023–24, we implement a PSM-DID design, comparing Bihar with Jharkhand. We estimate that the prohibition increased primary LPG adoption by 12.8 percentage points. The effect is concentrated in rural areas and is robust to alternative estimators, sample restrictions, and falsification tests. We further discuss that this spillover operates through reduced alcohol spending that relaxes the budget constraint for recurring LPG use and improved women’s intra-household agency following prohibition. The results highlight that policies aimed at curbing socially costly consumption can generate broader welfare gains in unexpected domains, including clean energy adoption.
</div>
</details>

* <a href="https://www.dropbox.com/scl/fo/oxivc59t7de1zea2rultr/AAiGN7QtmEX-5grNwKnrwrg?dl=0&e=1&preview=The+Long+Shadow+of+Communal+Violence.pdf&rlkey=u8q14ur09l983r2v9dc9dj2sc" class="paper-title">
The Long Shadow of Communal Violence: Childhood Exposure and Later-Life Mental Health 
</a>  
<a href="/files/pdf/Childhood_Riot_Exposure_and_Mental_Health.pdf" class="glo-link">Working Paper</a>  
<span class="authors">
with <a href="https://www.reetikasindhi.com">Reetika Sindhi</a> and
<a href="https://gauravdhamija5.weebly.com/">Dr. Gaurav Dhamija</a>
</span>
<details class="abstract">
<summary>Abstract</summary>
<div class="abstract-text">
Violent conflict affects millions of children worldwide. It often occurs in short and localized episodes rather than full-scale wars. However, the long-run costs of short and local violence between communities are rarely measured. We examine the long-run effect of childhood exposure to Hindu-Muslim riots on women’s mental health in India. We link historical riot records from 1950-1990 to respondents’ childhood districts in the Longitudinal Ageing Study in India. Our empirical strategy exploits variation in riot exposure across childhood districts and birth cohorts. Women exposed to at least one riot between birth and age 14 are 2.5 percentage points more likely to have major depressive disorder in later life. This represents 30 percent of the sample mean. The estimate is stable across a range of identification and robustness checks. A back-of-the-envelope calculation suggests that about one in nine cases of depression among Indian women aged 45 and older in 2018 can be traced to a riot in their childhood district, a loss we value at $0.9 to $2.7 billion a year. A single day of rioting is enough to produce this effect. We further provide suggestive evidence that parents’ decisions after a riot play a role. Among unmarried girls aged 5 to 17, exposure to a riot raises the probability of marriage in a given year by 8 percent, pointing to child marriage as one channel through which the effect persists.
</div>
</details>

---

# Work in Progress

* <span class="paper-title">
Causal Impact of Internet Exposure on Period Products Usage in India
</span>  
<span class="glo-link">Work in Progress</span>  
<span class="authors">
with <a href="https://gauravdhamija5.weebly.com/">Dr. Gaurav Dhamija</a> and
<a href="https://maniniojha.wordpress.com/">Dr. Manini Ojha</a>
</span>

---

# Other Publications

* <a href="https://www.policyedge.in/p/how-digital-access-can-change-domestic-violence" class="paper-title">
How Digital Access Can Change Domestic Violence
</a>  
<span class="outlet"><em>The Policy Edge</em> · Opinion · 19 September 2026</span>  
<span class="authors">
with <a href="https://gauravdhamija5.weebly.com/">Dr. Gaurav Dhamija</a> and
<a href="https://maniniojha.wordpress.com/">Dr. Manini Ojha</a>
</span>

<script>
(function () {
  var root = document.documentElement;
  var reduce = window.matchMedia && window.matchMedia('(prefers-reduced-motion: reduce)').matches;
  var entries = Array.prototype.filter.call(document.querySelectorAll('li'), function (li) { return li.querySelector(':scope > .paper-title'); });
  entries.forEach(function (li) {
    li.classList.add('entry');
    li.addEventListener('mousemove', function (e) {
      var r = li.getBoundingClientRect();
      li.style.setProperty('--mx', (e.clientX - r.left) + 'px');
      li.style.setProperty('--my', (e.clientY - r.top) + 'px');
    });
  });
  if (!reduce && 'IntersectionObserver' in window) {
    root.classList.add('rv');
    var io = new IntersectionObserver(function (items) {
      items.forEach(function (it) { if (it.isIntersecting) { it.target.classList.add('in'); io.unobserve(it.target); } });
    }, { threshold: 0.12 });
    entries.forEach(function (li, i) { li.style.transitionDelay = (i % 3) * 80 + 'ms'; io.observe(li); });
  }
  document.querySelectorAll('h1[id]').forEach(function (h) {
    var el = h.nextElementSibling;
    while (el && el.tagName !== 'UL' && el.tagName !== 'H1') { el = el.nextElementSibling; }
    if (el && el.tagName === 'UL') {
      var n = el.querySelectorAll(':scope > li').length;
      var b = document.createElement('span');
      b.className = 'count';
      b.textContent = n;
      h.appendChild(b);
    }
  });
  var btn = document.getElementById('abs-toggle');
  var bar = document.getElementById('rp-bar');
  var open = false;
  if (btn) {
    btn.addEventListener('click', function () {
      open = !open;
      document.querySelectorAll('details.abstract').forEach(function (d) { d.open = open; });
      btn.textContent = open ? '▴ Collapse all abstracts' : '▾ Expand all abstracts';
    });
  }
  window.addEventListener('scroll', function () {
    var h = document.documentElement.scrollHeight - window.innerHeight;
    if (bar && h > 0) { bar.style.width = (window.scrollY / h * 100) + '%'; }
  }, { passive: true });
})();
</script>
