---
permalink: /conference/
title: ""
---

<link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css">
<style>
:root { --ink:#1c2733; --acc:#1f5c5a; --acc-soft:rgba(31,92,90,0.07); --red:#8c2f39; --rule:rgba(28,39,51,0.2); --mut:#5b6672; }
@media (prefers-color-scheme: dark) { :root { --ink:#e6eaee; --acc:#79c2ba; --acc-soft:rgba(121,194,186,0.09); --red:#e48c96; --rule:rgba(255,255,255,0.2); --mut:#9aa5b1; } }
h1[id] { position:relative; margin:0.5em 0 0.6em; padding-bottom:0.5em; font-family:Georgia,"Iowan Old Style","Palatino Linotype",serif; font-size:1.05em; font-weight:700; letter-spacing:0.16em; text-transform:uppercase; color:var(--ink); border-bottom:1px solid var(--rule); }
h1[id]::after { content:""; position:absolute; left:0; bottom:-1px; width:3.2rem; height:3px; background:var(--acc); }
h2[id] { display:flex; align-items:center; gap:0.8em; margin:2.2em 0 0.4em; font-family:ui-monospace,SFMono-Regular,Menlo,Consolas,monospace; font-size:1.05em; font-weight:700; letter-spacing:0.1em; color:var(--acc); }
h2[id]::after { content:""; flex:1; height:1px; background:var(--rule); }
.mapwrap { position:relative; }
#confmap { height:440px; border:1px solid var(--rule); border-radius:2px; background:var(--acc-soft); z-index:0; }
.mapctl { position:absolute; right:10px; top:10px; z-index:500; display:flex; flex-direction:column; gap:6px; }
.mapctl button { font:inherit; font-size:0.74em; font-weight:700; letter-spacing:0.08em; text-transform:uppercase; cursor:pointer; padding:0.5em 0.9em; color:var(--acc); background:rgba(255,255,255,0.92); border:1px solid var(--acc); border-radius:2px; transition:background 0.2s,color 0.2s; }
.mapctl button:hover, .mapctl button.on { background:var(--acc); color:#fff; }
.mapnote { margin:0.5em 0 0; font-size:0.78em; font-style:italic; color:var(--mut); }
.pin { position:relative; width:30px; height:30px; border-radius:50%; background:var(--acc); border:2px solid #fff; box-shadow:0 2px 6px rgba(0,0,0,0.35); color:#fff; display:flex; align-items:center; justify-content:center; font:700 12px ui-monospace,Menlo,monospace; transition:transform 0.2s ease,background 0.2s ease; }
.pin::before { content:""; position:absolute; inset:-2px; border-radius:50%; border:2px solid var(--acc); opacity:0; }
.pin.on { background:var(--red); transform:scale(1.25); }
.pin.on::before { border-color:var(--red); animation:pinPulse 1.2s ease-out infinite; }
@keyframes pinPulse { from { transform:scale(1); opacity:0.8; } to { transform:scale(2.2); opacity:0; } }
#confmap .leaflet-tile-pane { filter:grayscale(0.85) contrast(0.95) brightness(1.03); }
@media (prefers-color-scheme: dark) { #confmap .leaflet-tile-pane { filter:invert(1) hue-rotate(180deg) grayscale(0.7) brightness(0.9); } }
.leaflet-popup-content { font-family:Georgia,"Iowan Old Style",serif; font-size:0.9em; line-height:1.45; margin:10px 14px; }
.leaflet-popup-content .pc-city { font:700 0.72em ui-monospace,Menlo,monospace; letter-spacing:0.12em; text-transform:uppercase; color:#8c2f39; margin-bottom:0.3em; }
.leaflet-popup-content .pc-ev { margin:0.35em 0 0; }
.leaflet-popup-content .pc-ev i { display:block; font-style:normal; font:0.78em ui-monospace,Menlo,monospace; color:#5b6672; }
ul.events { list-style:none; margin:0; padding:0; }
li.ev { display:grid; grid-template-columns:8.5em 1fr; gap:0 1.2em; padding:0.95em 0.6em 0.9em; border-bottom:1px solid var(--rule); cursor:pointer; transition:background 0.25s ease,padding-left 0.25s ease; animation:evRise 0.5s ease both; }
li.ev:hover, li.ev.hl { background:var(--acc-soft); padding-left:1em; }
li.ev.hl .when { color:var(--red); }
@keyframes evRise { from { opacity:0; transform:translateY(8px); } to { opacity:1; transform:none; } }
.when { font-family:ui-monospace,SFMono-Regular,Menlo,Consolas,monospace; font-size:0.8em; color:var(--acc); padding-top:0.2em; }
.when.tba { color:var(--mut); font-style:italic; }
.what b { font-family:Georgia,"Iowan Old Style","Palatino Linotype",serif; font-size:1.02em; line-height:1.4; color:var(--ink); }
.where { display:block; margin-top:0.2em; font-family:ui-monospace,SFMono-Regular,Menlo,Consolas,monospace; font-size:0.68em; letter-spacing:0.12em; text-transform:uppercase; color:var(--mut); }
@media (max-width:600px) { li.ev { grid-template-columns:1fr; } .when { padding-bottom:0.2em; } #confmap { height:340px; } }
@media (prefers-reduced-motion: reduce) { li.ev, .pin::before { animation:none !important; } }
</style>

# Conferences & Invited Talks

## 2026

<ul class="events">
<li class="ev" data-city="Bengaluru" data-year="2026" data-start="2026-09-02">
<span class="when">Sep 2–4</span>
<span class="what"><b>XXI International Conference on Public Policy and Management, Centre for Public Policy (CPP), IIM Bangalore</b><span class="where">Bengaluru, Karnataka</span></span>
</li>
<li class="ev" data-city="Sri City" data-year="2026" data-start="2026-06-17">
<span class="when">Jun 17–19</span>
<span class="what"><b>Research Symposium on Finance and Economics (RSFE), Krea University</b><span class="where">Virtual · hosted at IFMR GSB, Krea University, Sri City</span></span>
</li>
<li class="ev" data-city="Mohali" data-year="2026" data-start="2026-03-20">
<span class="when">Mar 20–21</span>
<span class="what"><b>Peace and Conflict (PAC) Workshop, Plaksha University</b><span class="where">Mohali, Punjab</span></span>
</li>
<li class="ev" data-city="Kolkata" data-year="2026" data-start="2026-03-13">
<span class="when">Mar 13–14</span>
<span class="what"><b>IIM Calcutta Economics Research Conference</b><span class="where">Kolkata, West Bengal</span></span>
</li>
<li class="ev" data-city="Kanpur" data-year="2026" data-start="2026-02-13">
<span class="when">Feb 13–14</span>
<span class="what"><b>Research Scholars’ Day, IIT Kanpur</b><span class="where">Kanpur, Uttar Pradesh</span></span>
</li>
<li class="ev" data-city="Thiruvananthapuram" data-year="2026" data-start="2026-02-05">
<span class="when">Feb 5–7</span>
<span class="what"><b>Second CDS PhD Colloquium — <i>Crossroads</i></b><span class="where">Thiruvananthapuram, Kerala</span></span>
</li>
<li class="ev" data-city="Hyderabad" data-year="2026" data-start="2026-01-29">
<span class="when">Jan 29–31</span>
<span class="what"><b>7th Annual Conference of Economics &amp; Finance (ACEF), BITS Pilani, Hyderabad Campus</b><span class="where">Hyderabad, Telangana</span></span>
</li>
<li class="ev" data-city="Ahmedabad" data-year="2026" data-start="2026-01-09">
<span class="when">Jan 9–10</span>
<span class="what"><b>7th Annual Economics Conference, Ahmedabad University</b><span class="where">Ahmedabad, Gujarat</span></span>
</li>
<li class="ev" data-city="Kolkata" data-year="2026" data-start="2026-01-06">
<span class="when">Jan 6–8</span>
<span class="what"><b>XXXVth Annual Conference on Contemporary Issues in Development Economics, Jadavpur University</b><span class="where">Kolkata, West Bengal</span></span>
</li>
</ul>

## 2025

<ul class="events">
<li class="ev" data-city="Thiruvananthapuram" data-year="2025" data-start="2025-12-17">
<span class="when">Dec 17–19</span>
<span class="what"><b>XXX IIPS National Seminar</b><span class="where">Thiruvananthapuram, Kerala</span></span>
</li>
</ul>

## Map

<div class="mapwrap"><div id="confmap" role="img" aria-label="Map of conference locations"></div><div class="mapctl"><button type="button" id="btn-play">Play journey</button><button type="button" id="btn-view">Show world</button></div></div>

<script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"></script>
<script>
(function () {
  var COORDS = { 'Bengaluru':[12.9716,77.5946], 'Sri City':[13.5260,79.9950], 'Mohali':[30.7046,76.7179], 'Kolkata':[22.5726,88.3639], 'Kanpur':[26.4499,80.3319], 'Thiruvananthapuram':[8.5241,76.9366], 'Hyderabad':[17.3850,78.4867], 'Ahmedabad':[23.0225,72.5714] };
  var items = Array.prototype.slice.call(document.querySelectorAll('li.ev'));
  var groups = {};
  items.forEach(function (li) { var c = li.getAttribute('data-city'); (groups[c] = groups[c] || []).push(li); });
  var dated = items.filter(function (li) { return li.getAttribute('data-start'); }).sort(function (a, b) { return a.getAttribute('data-start') < b.getAttribute('data-start') ? -1 : 1; });
  var seq = [];
  dated.forEach(function (li) { var c = li.getAttribute('data-city'); if (seq[seq.length - 1] !== c) { seq.push(c); } });
  if (!window.L) { document.getElementById('confmap').outerHTML = '<p class="mapnote">The map could not be loaded.</p>'; return; }
  var map = L.map('confmap', { scrollWheelZoom: false, worldCopyJump: true, zoomSnap: 0.25 });
  var dark = window.matchMedia && window.matchMedia('(prefers-color-scheme: dark)').matches;
  var base = L.tileLayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', { attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors', maxZoom: 18, minZoom: 2, referrerPolicy: 'origin' }).addTo(map);
  var fails = 0;
  base.on('tileerror', function () {
    fails++;
    if (fails === 4) {
      map.removeLayer(base);
      L.tileLayer('https://server.arcgisonline.com/ArcGIS/rest/services/Canvas/World_Light_Gray_Base/MapServer/tile/{z}/{y}/{x}', { attribution: 'Tiles &copy; Esri', maxZoom: 16, minZoom: 2 }).addTo(map);
    }
  });
  map.on('click', function () { map.scrollWheelZoom.enable(); });
  var pins = {}, all = [];
  Object.keys(groups).forEach(function (c) {
    var ll = COORDS[c];
    if (!ll) { return; }
    var list = groups[c];
    var icon = L.divIcon({ className: '', html: '<div class="pin"><b>' + list.length + '</b></div>', iconSize: [30, 30], iconAnchor: [15, 15], popupAnchor: [0, -16] });
    var html = '<div class="pc-city">' + c + '</div>';
    list.forEach(function (li) {
      var w = li.querySelector('.when').textContent;
      html += '<div class="pc-ev">' + li.querySelector('.what b').innerHTML + '<i>' + w + ' ' + li.getAttribute('data-year') + '</i></div>';
    });
    var m = L.marker(ll, { icon: icon, title: c }).addTo(map).bindPopup(html, { maxWidth: 280 });
    m.on('mouseover', function () { setOn(c, true); });
    m.on('mouseout', function () { setOn(c, false); });
    m.on('popupopen', function () { setOn(c, true); });
    m.on('popupclose', function () { setOn(c, false); });
    pins[c] = m;
    all.push(ll);
  });
  function setOn(c, on) {
    var m = pins[c];
    if (m && m._icon) { var p = m._icon.firstChild; if (p) { p.classList.toggle('on', on); } }
    (groups[c] || []).forEach(function (li) { li.classList.toggle('hl', on); });
  }
  function fitIndia() { map.fitBounds(all, { padding: [40, 40], maxZoom: 6 }); }
  fitIndia();
  var world = false;
  var vbtn = document.getElementById('btn-view');
  vbtn.addEventListener('click', function () {
    world = !world;
    if (world) { map.flyTo([22, 40], 2.5, { duration: 1.4 }); } else { fitIndia(); }
    vbtn.textContent = world ? 'Fit venues' : 'Show world';
  });
  items.forEach(function (li) {
    var c = li.getAttribute('data-city');
    li.addEventListener('mouseenter', function () { setOn(c, true); });
    li.addEventListener('mouseleave', function () { if (!pins[c] || !pins[c].isPopupOpen()) { setOn(c, false); } });
    li.addEventListener('click', function () { if (pins[c]) { map.flyTo(COORDS[c], 6, { duration: 1 }); pins[c].openPopup(); document.getElementById('confmap').scrollIntoView({ behavior: 'smooth', block: 'center' }); } });
  });
  var pbtn = document.getElementById('btn-play');
  var timer = null, step = 0;
  function stop() { clearInterval(timer); timer = null; pbtn.classList.remove('on'); pbtn.textContent = 'Play journey'; map.closePopup(); }
  pbtn.addEventListener('click', function () {
    if (timer) { stop(); return; }
    if (!seq.length) { return; }
    pbtn.classList.add('on'); pbtn.textContent = 'Stop';
    step = 0;
    var go = function () {
      if (step >= seq.length) { stop(); fitIndia(); return; }
      var c = seq[step++];
      map.flyTo(COORDS[c], 6, { duration: 1.3 });
      setTimeout(function () { if (timer) { pins[c].openPopup(); } }, 1300);
    };
    go();
    timer = setInterval(go, 3200);
  });
})();
</script>
