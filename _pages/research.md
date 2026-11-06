---
permalink: /research/
title: ""
---

<style>
:root { --ink:#1c2733; --acc:#1f5c5a; --acc-soft:rgba(31,92,90,0.07); --red:#8c2f39; --rule:rgba(28,39,51,0.2); --mut:#5b6672; }
@media (prefers-color-scheme: dark) { :root { --ink:#e6eaee; --acc:#79c2ba; --acc-soft:rgba(121,194,186,0.09); --red:#e48c96; --rule:rgba(255,255,255,0.2); --mut:#9aa5b1; } }
.toolbar { display:flex; flex-wrap:wrap; align-items:center; justify-content:space-between; gap:0.8em 1.5em; margin:0.5em 0 1.8em; padding:0.8em 0; border-top:2px solid var(--ink); border-bottom:1px solid var(--rule); }
.ledger { font-family:ui-monospace,SFMono-Regular,Menlo,Consolas,monospace; font-size:0.78em; letter-spacing:0.02em; color:var(--mut); }
.ledger b { color:var(--ink); font-size:1.25em; margin-right:0.25em; }
.ledger span + span::before { content:"/"; margin:0 0.9em; opacity:0.45; }
.tools { display:flex; gap:0.6em; align-items:center; }
#rp-search { font:inherit; font-size:0.85em; padding:0.4em 0.7em; width:15em; max-width:100%; color:var(--ink); background:transparent; border:1px solid var(--rule); border-radius:2px; }
#rp-search:focus { outline:2px solid var(--acc); outline-offset:1px; }
#abs-toggle { font:inherit; font-size:0.8em; cursor:pointer; padding:0.45em 0.9em; color:var(--acc); background:transparent; border:1px solid var(--acc); border-radius:2px; transition:background 0.2s,color 0.2s; }
#abs-toggle:hover { background:var(--acc); color:#fff; }
#rp-empty { font-style:italic; color:var(--mut); }
h1[id] { position:relative; display:flex; align-items:baseline; justify-content:space-between; margin:2.6em 0 1em; padding-bottom:0.5em; font-family:Georgia,"Iowan Old Style","Palatino Linotype",serif; font-size:1.05em; font-weight:700; letter-spacing:0.16em; text-transform:uppercase; color:var(--ink); border-bottom:1px solid var(--rule); }
h1[id]::after { content:""; position:absolute; left:0; bottom:-1px; width:3.2rem; height:3px; background:var(--acc); }
h1[id] .count { font-family:ui-monospace,SFMono-Regular,Menlo,Consolas,monospace; font-size:0.8em; font-weight:400; letter-spacing:0; color:var(--mut); }
ul.papers { list-style:none; margin:0; padding:0; counter-reset:paper; }
li.entry { position:relative; list-style:none; counter-increment:paper; margin:0; padding:1.3em 0 1.2em 3.4em; border-bottom:1px solid var(--rule); transition:background 0.25s ease; animation:rpRise 0.55s ease both; }
li.entry::before { content:counter(paper,decimal-leading-zero); position:absolute; left:0; top:1.55em; font-family:ui-monospace,SFMono-Regular,Menlo,Consolas,monospace; font-size:0.85em; color:var(--mut); transition:color 0.25s; }
li.entry::after { content:""; position:absolute; left:-1.1em; top:1.1em; bottom:1em; width:2px; background:var(--acc); transform:scaleY(0); transform-origin:top; transition:transform 0.3s ease; }
li.entry:hover { background:var(--acc-soft); }
li.entry:hover::before { color:var(--acc); }
li.entry:hover::after { transform:scaleY(1); }
@keyframes rpRise { from { opacity:0; transform:translateY(10px); } to { opacity:1; transform:none; } }
.kicker { display:block; margin-bottom:0.3em; font-family:ui-monospace,SFMono-Regular,Menlo,Consolas,monospace; font-size:0.68em; letter-spacing:0.12em; text-transform:uppercase; color:var(--mut); }
.kicker.pub { color:var(--red); font-weight:700; }
.paper-title { font-family:Georgia,"Iowan Old Style","Palatino Linotype",serif; font-size:1.12em; font-weight:700; line-height:1.38; color:var(--ink); text-decoration:none !important; }
a.paper-title:hover { color:var(--acc); text-decoration:underline !important; text-decoration-thickness:1px; text-underline-offset:4px; }
.journal, .outlet { display:block; margin:0.25em 0 0.1em; font-family:Georgia,"Iowan Old Style",serif; font-size:0.95em; color:var(--acc); }
.glo-link { display:inline-block; margin:0.45em 0.8em 0.1em 0; font-size:0.78em; font-weight:700; letter-spacing:0.06em; text-transform:uppercase; text-decoration:none !important; color:var(--acc); border-bottom:1px solid var(--acc); }
a.glo-link::after { content:" ↗"; }
a.glo-link:hover { color:var(--ink); border-bottom-color:var(--ink); }
span.glo-link { color:var(--mut); border-bottom:1px dashed var(--mut); }
.authors { display:block; margin-top:0.35em; font-family:Georgia,"Iowan Old Style",serif; font-size:0.92em; font-style:italic; color:var(--mut); }
.authors a { color:inherit; border-bottom:1px dotted currentColor; text-decoration:none; }
.authors a:hover { color:var(--acc); }
details.abstract { margin:0.7em 0 0; }
details.abstract > summary { display:inline-flex; align-items:center; gap:0.55em; cursor:pointer; list-style:none; user-select:none; font-size:0.74em; font-weight:700; letter-spacing:0.14em; text-transform:uppercase; color:var(--acc); }
details.abstract > summary::-webkit-details-marker { display:none; }
details.abstract > summary::marker { content:""; }
details.abstract > summary::before { content:""; width:0.45em; height:0.45em; border-right:2px solid currentColor; border-bottom:2px solid currentColor; transform:rotate(-45deg); transition:transform 0.25s ease; }
details.abstract[open] > summary::before { transform:rotate(45deg); }
details.abstract > summary:hover { color:var(--ink); }
details.abstract > summary:focus-visible { outline:2px solid var(--acc); outline-offset:3px; }
details.abstract .abstract-text { margin:0.7em 0 0.2em; padding:0.9em 1.2em; border-left:3px solid var(--acc); background:var(--acc-soft); font-family:Georgia,"Iowan Old Style",serif; font-size:0.93em; line-height:1.7; text-align:justify; hyphens:auto; }
details.abstract[open] .abstract-text { animation:rpRise 0.3s ease; }
li.entry mark { background:rgba(228,180,60,0.35); color:inherit; padding:0 0.1em; }
@media (max-width:600px) { li.entry { padding-left:2.4em; } .tools { width:100%; } #rp-search { flex:1; width:auto; } }
@media (prefers-reduced-motion: reduce) { li.entry, details.abstract .abstract-text { animation:none !important; } li.entry::after, li.entry { transition:none; } }
</style>

<div class="toolbar"><div class="ledger" id="ledger"></div><div class="tools"><input id="rp-search" type="search" placeholder="Search titles and abstracts  ( / )" aria-label="Search papers"><button id="abs-toggle" type="button">Expand all abstracts</button></div></div>
<p id="rp-empty" hidden>No papers match your search.</p>

# Peer-reviewed Publications

<ul class="papers">
<li class="entry">
<span class="kicker pub">Journal Article · 2026</span>
<a href="https://link.springer.com/article/10.1007/s11150-026-09887-5" class="paper-title">Rewiring Gender Norms: Causal Evidence on Internet Exposure and Justification of Intimate Partner Violence</a>
<span class="journal">Review of Economics of the Household</span>
<a href="https://www.econstor.eu/handle/10419/333329" class="glo-link">GLO Discussion Paper</a>
<span class="authors">with <a href="https://maniniojha.wordpress.com/">Dr. Manini Ojha</a> and <a href="https://gauravdhamija5.weebly.com/">Dr. Gaurav Dhamija</a></span>
<details class="abstract">
<summary>Abstract</summary>
<div class="abstract-text">This paper evaluates the causal impact of women’s exposure to the internet on their attitudes towards intimate partner violence using data from the most recent round of the National Family Health Survey. To address potential endogeneity, we exploit exogenous variation in district-level mobile tower density in India as an instrument for women’s internet exposure. The instrumental variables estimation provides evidence that a woman’s exposure to internet reduces her likelihood of justifying intimate partner violence by 21 percentage points. The results are robust to an extensive set of individual, household, and district-level controls, alternative definitions of both the exposure and outcome variables, and a range of falsification tests. Sub-sample analyses reveal that the effect holds across social group, wealth, education, and geography, with particularly strong effects among women in non-poor households, with lower education, and in urban areas. We further provide suggestive evidence that internet exposure increases women’s employment, awareness, relaxes mobility constraints, and reduces husbands’ justification of intimate partner violence. It suggests that changes in both women’s opportunities and intra-household gender norms constitute potential pathways through which internet exposure reduces women’s justification of intimate partner violence. Overall, the findings highlight the transformative potential of digital connectivity in challenging regressive gender norms.</div>
</details>
</li>
</ul>

# Working Papers

<ul class="papers">
<li class="entry">
<span class="kicker">Working Paper · GLO DP 1690</span>
<a href="https://www.econstor.eu/handle/10419/331320" class="paper-title">The Protective Power of Connectivity: Internet Exposure and Intimate Partner Violence</a>
<a href="/files/pdf/GLO-DP-1690.pdf" class="glo-link">GLO Discussion Paper</a>
<span class="authors">with <a href="https://gauravdhamija5.weebly.com/">Dr. Gaurav Dhamija</a> and <a href="https://maniniojha.wordpress.com/">Dr. Manini Ojha</a></span>
<details class="abstract">
<summary>Abstract</summary>
<div class="abstract-text">We study the effect of women’s exposure to the internet on the incidence of intimate partner violence (IPV) utilizing data from a large-scale nationally representative data for India. Utilizing an instrumental variable approach, we exploit the exogenous variation arising from cellular tower density at the district level as an instrument for internet exposure. We find women who have access to the internet are at a significantly lower risk of exposure to physical, sexual, emotional and any IPV by 17, 5, 9 and 18 percentage points. We provide further indicative evidence that women’s attitudes justifying violence works as a channel of our estimated causal impacts. Our results are robust to a host of sensitivity checks, additional controls, alternative definitions and falsification analysis. We document important heterogeneity in the effects across social groups, wealth index, area of residence, and women’s education levels. The effects appear to be particularly important for women from wealthier households and those who are more educated.</div>
</details>
</li>
<li class="entry">
<span class="kicker">Working Paper · GLO DP 1697</span>
<a href="https://www.econstor.eu/handle/10419/333697" class="paper-title">Banking on Connectivity: Internet Exposure and Women’s Financial Autonomy</a>
<a href="/files/pdf/GLO-DP-1697.pdf" class="glo-link">GLO Discussion Paper</a>
<span class="authors">with <a href="https://gauravdhamija5.weebly.com/">Dr. Gaurav Dhamija</a> and <a href="https://maniniojha.wordpress.com/">Dr. Manini Ojha</a></span>
<details class="abstract">
<summary>Abstract</summary>
<div class="abstract-text">We examine whether women's exposure to the internet enhances their economic agency in India. Using nationally representative data and an instrumental variables strategy that exploits plausibly exogenous variation in district-level mobile tower density, we identify the causal effect of internet access on women's financial control and use of formal banks. We find that internet exposure increases women's overall financial autonomy by 10 percentage points. We document improvements in independent mobility, employment, and financial awareness which we consider potential mechanisms of our estimated effects. Disaggregated outcomes show higher likelihood that women have money of their own over which they full control, as well as increased ownership and active use of a bank account. Our results are robust to additional controls and a battery of sensitivity analyses. Heterogeneity analyses indicate that effects are concentrated among women with at least secondary education, and among those from historically disadvantaged social groups. Overall, our findings highlight the importance of digital connectivity in enhancing the usage of financial resources, with important implications for women's autonomy and participation in the formal economy.</div>
</details>
</li>
<li class="entry">
<span class="kicker">Working Paper · SSRN</span>
<a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6257379" class="paper-title">Knot Too Early: The Causal Impact of Women's Age at Marriage on Period Product Use</a>
<a href="/files/pdf/ssrn-6257379.pdf" class="glo-link">Working Paper</a>
<span class="authors">with <a href="https://sites.google.com/iima.ac.in/karan-babbar/home">Dr. Karan Babbar</a> and <a href="https://gauravdhamija5.weebly.com/">Dr. Gaurav Dhamija</a></span>
<details class="abstract">
<summary>Abstract</summary>
<div class="abstract-text">This paper evaluates the causal impact of women’s age at marriage on their likelihood of using hygienic period products, using the most recent round of the National Family Health Survey (NFHS-5) in India. To address potential endogeneity, we exploit exogenous variation in a woman's age at menarche as an instrument for her age at marriage. The instrumental variable (IV) estimation provides robust evidence that a one-year increase in a woman's age at marriage increases, on an average, the likelihood of hygienic product use by 7 percentage points. We also provide suggestive evidence that higher education and increased household decision-making power are potential mechanisms driving this effect. These findings signify the importance of enforcing laws regulating the legal age of marriage, and highlight the broader need for societal shifts that promote later marriage, better menstrual hygiene, and the empowerment of young women.</div>
</details>
</li>
<li class="entry">
<span class="kicker">Working Paper · Policy Edge 2026-0001</span>
<a href="https://www.policyedge.in/working-paper/wp-from-liquor-to-lpg-spillover-effects-of-alcohol-prohibition-on-clean-fuel-adoption" class="paper-title">From Liquor to LPG: Spillover effects of alcohol prohibition on clean fuel adoption</a>
<a href="/files/pdf/TPE_WP_2026-0001.pdf" class="glo-link">Policy Edge Working Paper</a>
<span class="authors">with <a href="https://gauravdhamija5.weebly.com/">Dr. Gaurav Dhamija</a> and <a href="https://maniniojha.wordpress.com/">Dr. Manini Ojha</a></span>
<details class="abstract">
<summary>Abstract</summary>
<div class="abstract-text">This paper examines whether Bihar’s 2016 alcohol prohibition generated spillover effects on household adoption of LPG as a primary cooking fuel. Although clean cooking lies well outside the policy’s intended scope, prohibition may affect fuel choice by altering household expenditure patterns and intra-household dynamics. Using repeated cross-sectional data from the Household Consumption Expenditure Surveys of 2011–12 and 2023–24, we implement a PSM-DID design, comparing Bihar with Jharkhand. We estimate that the prohibition increased primary LPG adoption by 12.8 percentage points. The effect is concentrated in rural areas and is robust to alternative estimators, sample restrictions, and falsification tests. We further discuss that this spillover operates through reduced alcohol spending that relaxes the budget constraint for recurring LPG use and improved women’s intra-household agency following prohibition. The results highlight that policies aimed at curbing socially costly consumption can generate broader welfare gains in unexpected domains, including clean energy adoption.</div>
</details>
</li>
<li class="entry">
<span class="kicker">Working Paper</span>
<a href="https://www.dropbox.com/scl/fo/oxivc59t7de1zea2rultr/AAiGN7QtmEX-5grNwKnrwrg?dl=0&amp;e=1&amp;preview=The+Long+Shadow+of+Communal+Violence.pdf&amp;rlkey=u8q14ur09l983r2v9dc9dj2sc" class="paper-title">The Long Shadow of Communal Violence: Childhood Exposure and Later-Life Mental Health</a>
<a href="/files/pdf/Childhood_Riot_Exposure_and_Mental_Health.pdf" class="glo-link">Working Paper</a>
<span class="authors">with <a href="https://www.reetikasindhi.com">Reetika Sindhi</a> and <a href="https://gauravdhamija5.weebly.com/">Dr. Gaurav Dhamija</a></span>
<details class="abstract">
<summary>Abstract</summary>
<div class="abstract-text">Violent conflict affects millions of children worldwide. It often occurs in short and localized episodes rather than full-scale wars. However, the long-run costs of short and local violence between communities are rarely measured. We examine the long-run effect of childhood exposure to Hindu-Muslim riots on women’s mental health in India. We link historical riot records from 1950-1990 to respondents’ childhood districts in the Longitudinal Ageing Study in India. Our empirical strategy exploits variation in riot exposure across childhood districts and birth cohorts. Women exposed to at least one riot between birth and age 14 are 2.5 percentage points more likely to have major depressive disorder in later life. This represents 30 percent of the sample mean. The estimate is stable across a range of identification and robustness checks. A back-of-the-envelope calculation suggests that about one in nine cases of depression among Indian women aged 45 and older in 2018 can be traced to a riot in their childhood district, a loss we value at $0.9 to $2.7 billion a year. A single day of rioting is enough to produce this effect. We further provide suggestive evidence that parents’ decisions after a riot play a role. Among unmarried girls aged 5 to 17, exposure to a riot raises the probability of marriage in a given year by 8 percent, pointing to child marriage as one channel through which the effect persists.</div>
</details>
</li>
</ul>

# Work in Progress

<ul class="papers">
<li class="entry">
<span class="kicker">Work in Progress</span>
<span class="paper-title">Causal Impact of Internet Exposure on Period Products Usage in India</span>
<span class="authors">with <a href="https://gauravdhamija5.weebly.com/">Dr. Gaurav Dhamija</a> and <a href="https://maniniojha.wordpress.com/">Dr. Manini Ojha</a></span>
</li>
</ul>

# Other Publications

<ul class="papers">
<li class="entry">
<span class="kicker">Opinion · 19 September 2026</span>
<a href="https://www.policyedge.in/p/how-digital-access-can-change-domestic-violence" class="paper-title">How Digital Access Can Change Domestic Violence</a>
<span class="outlet">The Policy Edge</span>
<span class="authors">with <a href="https://gauravdhamija5.weebly.com/">Dr. Gaurav Dhamija</a> and <a href="https://maniniojha.wordpress.com/">Dr. Manini Ojha</a></span>
</li>
</ul>

<script>
(function () {
  var entries = Array.prototype.slice.call(document.querySelectorAll('li.entry'));
  var heads = Array.prototype.slice.call(document.querySelectorAll('h1[id]'));
  var ledger = document.getElementById('ledger');
  var labels = { 'peer-reviewed-publications': 'published', 'working-papers': 'working papers', 'work-in-progress': 'in progress', 'other-publications': 'other' };
  heads.forEach(function (h) {
    var ul = h.nextElementSibling;
    if (!ul || ul.tagName !== 'UL') { return; }
    var n = ul.querySelectorAll(':scope > li').length;
    var c = document.createElement('span');
    c.className = 'count';
    c.textContent = '(' + (n < 10 ? '0' : '') + n + ')';
    h.appendChild(c);
    h.__ul = ul;
    if (ledger) {
      var s = document.createElement('span');
      s.innerHTML = '<b>' + n + '</b>' + (labels[h.id] || h.textContent.toLowerCase());
      ledger.appendChild(s);
    }
  });
  var btn = document.getElementById('abs-toggle');
  var open = false;
  if (btn) {
    btn.addEventListener('click', function () {
      open = !open;
      document.querySelectorAll('details.abstract').forEach(function (d) { d.open = open; });
      btn.textContent = open ? 'Collapse all abstracts' : 'Expand all abstracts';
    });
  }
  var box = document.getElementById('rp-search');
  var empty = document.getElementById('rp-empty');
  if (box) {
    box.addEventListener('input', function () {
      var q = box.value.trim().toLowerCase();
      var shown = 0;
      entries.forEach(function (li) {
        var d = li.querySelector('details.abstract');
        var head = li.textContent.toLowerCase();
        var abs = d ? d.textContent.toLowerCase() : '';
        var hit = !q || head.indexOf(q) > -1;
        li.style.display = hit ? '' : 'none';
        if (hit) { shown++; }
        if (d) { d.open = !!q && hit && abs.indexOf(q) > -1; }
      });
      heads.forEach(function (h) {
        if (!h.__ul) { return; }
        var any = Array.prototype.some.call(h.__ul.children, function (li) { return li.style.display !== 'none'; });
        h.style.display = any ? '' : 'none';
        h.__ul.style.display = any ? '' : 'none';
      });
      if (empty) { empty.hidden = shown > 0; }
    });
    document.addEventListener('keydown', function (e) {
      var t = (e.target && e.target.tagName) || '';
      if (e.key === '/' && t !== 'INPUT' && t !== 'TEXTAREA') { e.preventDefault(); box.focus(); }
    });
  }
})();
</script>
