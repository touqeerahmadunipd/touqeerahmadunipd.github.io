---
layout: archive
title: "Talks and presentations"
permalink: /talks/
author_profile: true
---

{% include base_path %}

<style>
  .tk{--accent:#0f86a8;--accent-soft:rgba(15,134,168,.10);--warm:#d0683d;--warm-soft:rgba(208,104,61,.12);--violet:#7c5cc4;--violet-soft:rgba(124,92,196,.13);--green:#3f9a3f;--green-soft:rgba(63,154,63,.14);--card:var(--global-bg-color);--line:var(--global-border-color);--muted:color-mix(in srgb,var(--global-text-color) 75%,transparent)}
  html[data-theme="dark"] .tk{--accent:#20a0c4;--accent-soft:rgba(32,160,196,.16);--warm:#d9744a;--warm-soft:rgba(217,116,74,.18);--violet:#a58ae6;--violet-soft:rgba(165,138,230,.18);--green:#6cc46c;--green-soft:rgba(108,196,108,.16)}
  .tk *{box-sizing:border-box}
  .tk a{text-decoration:none}
  .tk p{margin:0 0 1em}

  .tk-hero{position:relative;border-radius:16px;overflow:hidden;margin:0 0 1.6em;background:#145a6c}
  .tk-hero img{display:block;width:100%;height:250px;object-fit:cover;object-position:center 40%;opacity:.6;margin:0}
  .tk-hero .ov{position:absolute;inset:0;background:linear-gradient(90deg,rgba(10,50,62,.92),rgba(10,50,62,.3));display:flex;flex-direction:column;justify-content:flex-end;padding:1.3em 1.5em;color:#fff}
  .tk-hero h2{color:#fff;margin:0 0 .25em;font-size:1.5em;border:0}
  .tk-hero p{margin:0;font-size:.85em;color:rgba(255,255,255,.88);max-width:34em}
  .tk-hero small{position:absolute;right:1em;bottom:.7em;font-size:.65em;color:rgba(255,255,255,.75)}

  .tk-stats{display:grid;grid-template-columns:repeat(5,1fr);gap:.7em;margin:0 0 1.4em}
  .tk-stat{border:1px solid var(--line);border-radius:12px;padding:.85em .9em;background:var(--card);position:relative;overflow:hidden}
  .tk-stat::before{content:"";position:absolute;left:0;top:0;bottom:0;width:4px;background:var(--c,var(--accent))}
  .tk-stat b{display:block;font-size:1.45em;line-height:1.1}
  .tk-stat span{font-size:.7em;color:var(--muted)}
  @media (max-width:760px){.tk-stats{grid-template-columns:1fr 1fr}}

  .tk-places{border:1px solid var(--line);border-radius:14px;padding:.9em 1.1em;margin:0 0 1.8em;background:var(--card)}
  .tk-places h3{font-size:.88em;margin:0 0 .6em}
  .tk-places h3 i{color:var(--accent)}
  .tk-place{display:inline-flex;align-items:center;gap:.4em;font-size:.76em;padding:.35em .75em;margin:0 .35em .4em 0;border-radius:999px;background:var(--accent-soft);color:var(--global-text-color)}
  .tk-place em{font-style:normal;font-weight:700;color:var(--accent)}

  .tk-tools{display:flex;flex-wrap:wrap;gap:.5em;margin:0 0 1.2em}
  .tk-chip{font:inherit;font-size:.74em;font-weight:600;padding:.45em .9em;border-radius:999px;border:1.5px solid var(--line);background:var(--card);color:var(--global-text-color);cursor:pointer;transition:all .15s;display:inline-flex;align-items:center;gap:.45em}
  .tk-chip i.d{width:.6em;height:.6em;border-radius:50%;background:var(--c,var(--accent));display:inline-block}
  .tk-chip:hover{border-color:var(--accent)}
  .tk-chip[aria-pressed="true"]{background:var(--global-text-color);border-color:var(--global-text-color);color:var(--global-bg-color)}

  .tk-year{display:flex;align-items:center;gap:.6em;font-size:.82em;font-weight:700;color:var(--accent);margin:1.4em 0 .7em;letter-spacing:.04em}
  .tk-year::after{content:"";flex:1;height:1px;background:var(--line)}
  .tk-list{list-style:none;margin:0;padding:0;display:grid;gap:.75em}
  .tk-item{margin:0;display:grid;grid-template-columns:4.4em 1fr;gap:1em;align-items:start;border:1px solid var(--line);border-radius:12px;padding:.95em 1.1em;background:var(--card);transition:transform .2s ease, box-shadow .2s ease, border-color .2s ease}
  .tk-item:hover{transform:translateY(-2px);box-shadow:0 10px 22px -16px rgba(0,0,0,.4);border-color:var(--c)}
  .tk-date{text-align:center;border-radius:10px;background:var(--c);color:#fff;padding:.45em .2em;line-height:1.15}
  .tk-date b{display:block;font-size:1.25em}
  .tk-date span{font-size:.64em;text-transform:uppercase;letter-spacing:.05em}
  .tk-item h3{font-size:.93em;line-height:1.38;margin:0 0 .3em}
  .tk-au{font-size:.7em;color:var(--muted);margin:0 0 .35em!important}
  .tk-au b{color:var(--global-text-color)}
  .tk-ev{font-size:.72em;margin:0 0 .5em!important;line-height:1.45}
  .tk-ev i{color:var(--muted);margin-right:.3em}
  .tk-meta{display:flex;flex-wrap:wrap;gap:.4em;align-items:center}
  .tk-type{font-size:.66em;font-weight:700;letter-spacing:.04em;text-transform:uppercase;padding:.25em .65em;border-radius:6px;background:var(--cs);color:var(--c)}
  .tk-loc{font-size:.72em;color:var(--muted)}
  .tk-btn{margin-left:auto;font-size:.72em;font-weight:600;padding:.32em .85em;border-radius:999px;border:1.5px solid var(--c);color:var(--c)!important;display:inline-flex;align-items:center;gap:.4em;transition:all .15s}
  .tk-btn:hover{background:var(--c);color:#fff!important}
  .t-inv{--c:var(--warm);--cs:var(--warm-soft)}
  .t-con{--c:var(--accent);--cs:var(--accent-soft)}
  .t-pos{--c:var(--violet);--cs:var(--violet-soft)}
  .t-sem{--c:var(--green);--cs:var(--green-soft)}
  [hidden]{display:none!important}
</style>

<div class="tk" id="tk-root">

<div class="tk-hero">
  <img src="/images/msaintmich1.png" alt="Mont Saint-Michel, Brittany, France">
  <div class="ov">
    <h2><i class="fas fa-person-chalkboard"></i> Talks &amp; presentations</h2>
    <p>Invited and contributed talks, posters and seminars on extreme value theory, discrete extremes and statistical learning.</p>
  </div>
  <small>Mont Saint-Michel, Brittany, France</small>
</div>

<div class="tk-stats">
  <div class="tk-stat t-inv"><b>4</b><span>Invited talks</span></div>
  <div class="tk-stat t-con"><b>3</b><span>Contributed talks</span></div>
  <div class="tk-stat t-pos"><b>3</b><span>Posters</span></div>
  <div class="tk-stat t-sem"><b>3</b><span>Seminars</span></div>
  <div class="tk-stat"><b>8</b><span>Countries</span></div>
</div>

<div class="tk-places">
  <h3><i class="fas fa-earth-europe"></i> Where I have presented</h3>
  <span class="tk-place">🇳🇴 Norway <em>2</em></span>
  <span class="tk-place">🇵🇰 Pakistan <em>3</em></span>
  <span class="tk-place">🇬🇧 United Kingdom <em>2</em></span>
  <span class="tk-place">🇮🇹 Italy <em>2</em></span>
  <span class="tk-place">🇫🇷 France <em>1</em></span>
  <span class="tk-place">🇳🇱 Netherlands <em>1</em></span>
  <span class="tk-place">🇵🇹 Portugal <em>1</em></span>
  <span class="tk-place">🇨🇭 Switzerland <em>1</em></span>
</div>

<div class="tk-tools" role="toolbar" aria-label="Filter talks by type">
  <button class="tk-chip" aria-pressed="true" data-f="all">All</button>
  <button class="tk-chip t-inv" aria-pressed="false" data-f="t-inv"><i class="d"></i>Invited talks</button>
  <button class="tk-chip t-con" aria-pressed="false" data-f="t-con"><i class="d"></i>Contributed talks</button>
  <button class="tk-chip t-pos" aria-pressed="false" data-f="t-pos"><i class="d"></i>Posters</button>
  <button class="tk-chip t-sem" aria-pressed="false" data-f="t-sem"><i class="d"></i>Seminars</button>
</div>

<div id="tk-all">

<div class="tk-year">2026</div>
<ul class="tk-list">
  <li class="tk-item t-pos"><div class="tk-date"><b>21</b><span>Jul</span></div><div>
    <h3>A flexible model for spatio-temporal modeling of low-threshold exceedances</h3>
    <p class="tk-au"><b>Ahmad, T.</b>, &amp; Thorarinsdottir, T. L.</p>
    <p class="tk-ev"><i class="fas fa-location-dot"></i>7th International Conference on Advances in Extreme Value Analysis and Application to Natural Hazards (EVAN 2026), Delft University of Technology · 21–24 July 2026</p>
    <div class="tk-meta"><span class="tk-type">Poster</span><span class="tk-loc">🇳🇱 Delft, Netherlands</span><a class="tk-btn" href="{{ '/files/Poster_EVAN.pdf' | relative_url }}" target="_blank" rel="noopener noreferrer"><i class="fas fa-image"></i> Poster</a></div>
  </div></li>

  <li class="tk-item t-con"><div class="tk-date"><b>28</b><span>Jun</span></div><div>
    <h3>A new extension of the generalized Pareto distribution for modeling low threshold exceedances</h3>
    <p class="tk-au"><b>Ahmad, T.</b>, &amp; Thorarinsdottir, T. L.</p>
    <p class="tk-ev"><i class="fas fa-location-dot"></i>40th International Workshop on Statistical Modelling (IWSM 2026), University of Oslo · 28 June – 3 July 2026</p>
    <div class="tk-meta"><span class="tk-type">Contributed talk</span><span class="tk-loc">🇳🇴 Oslo, Norway</span><a class="tk-btn" href="{{ '/files/IWSM2026_slide_Touqeer.pdf' | relative_url }}" target="_blank" rel="noopener noreferrer"><i class="fas fa-file-pdf"></i> Slides</a></div>
  </div></li>

  <li class="tk-item t-inv"><div class="tk-date"><b>21</b><span>May</span></div><div>
    <h3>Nearest-neighbor LASSO logistic regression for gradient estimation</h3>
    <p class="tk-au"><b>Ahmad, T.</b>, Portier, F., &amp; Stupfler, G.</p>
    <p class="tk-ev"><i class="fas fa-location-dot"></i>Workshop on High-Dimensional Statistical Learning, Oslo Centre for Biostatistics and Epidemiology (OCBE) · 21 May 2026</p>
    <div class="tk-meta"><span class="tk-type">Invited talk</span><span class="tk-loc">🇳🇴 Oslo, Norway</span><a class="tk-btn" href="{{ '/files/SLIDE_OCBE.pdf' | relative_url }}" target="_blank" rel="noopener noreferrer"><i class="fas fa-file-pdf"></i> Slides</a></div>
  </div></li>
</ul>

<div class="tk-year">2024</div>
<ul class="tk-list">
  <li class="tk-item t-inv"><div class="tk-date"><b>14</b><span>Dec</span></div><div>
    <h3>An extended generalized Pareto regression model for count data</h3>
    <p class="tk-au"><b>Ahmad, T.</b>, Gaetan, C., &amp; Naveau, P.</p>
    <p class="tk-ev"><i class="fas fa-location-dot"></i>17th International Conference of the ERCIM Working Group on Computational and Methodological Statistics (CMStatistics 2024), King’s College London · 14–16 December 2024</p>
    <div class="tk-meta"><span class="tk-type">Invited talk</span><span class="tk-loc">🇬🇧 London, UK</span><a class="tk-btn" href="{{ '/files/CMstatistics2024.pdf' | relative_url }}" target="_blank" rel="noopener noreferrer"><i class="fas fa-file-pdf"></i> Slides</a></div>
  </div></li>

  <li class="tk-item t-pos"><div class="tk-date"><b>25</b><span>Jun</span></div><div>
    <h3>Local logistic regression for dimension reduction in classification</h3>
    <p class="tk-au"><b>Ahmad, T.</b>, Portier, F., &amp; Stupfler, G.</p>
    <p class="tk-ev"><i class="fas fa-location-dot"></i>International Symposium on Nonparametric Statistics (ISNPS 2024) · 25–29 June 2024</p>
    <div class="tk-meta"><span class="tk-type">Poster</span><span class="tk-loc">🇵🇹 Braga, Portugal</span><a class="tk-btn" href="{{ '/files/Poster_Braga.pdf' | relative_url }}" target="_blank" rel="noopener noreferrer"><i class="fas fa-image"></i> Poster</a></div>
  </div></li>

  <li class="tk-item t-pos"><div class="tk-date"><b>14</b><span>Feb</span></div><div>
    <h3>Dimension reduction for binary classification problems</h3>
    <p class="tk-au"><b>Ahmad, T.</b>, Portier, F., &amp; Stupfler, G.</p>
    <p class="tk-ev"><i class="fas fa-location-dot"></i>Causality in Extremes Workshop and Mini-Courses, University of Geneva · 14–16 February 2024</p>
    <div class="tk-meta"><span class="tk-type">Poster</span><span class="tk-loc">🇨🇭 Geneva, Switzerland</span><a class="tk-btn" href="{{ '/files/Poster_Geneva.pdf' | relative_url }}" target="_blank" rel="noopener noreferrer"><i class="fas fa-image"></i> Poster</a></div>
  </div></li>
</ul>

<div class="tk-year">2023</div>
<ul class="tk-list">
  <li class="tk-item t-inv"><div class="tk-date"><b>14</b><span>Dec</span></div><div>
    <h3>A flexible novel extension of the discrete generalized Pareto distribution</h3>
    <p class="tk-au"><b>Ahmad, T.</b>, &amp; Arshad, I. A.</p>
    <p class="tk-ev"><i class="fas fa-location-dot"></i>2nd International Conference on Recent Trends in Statistics &amp; Data Analytics, National University of Sciences and Technology (NUST) · 14–15 December 2023</p>
    <div class="tk-meta"><span class="tk-type">Invited talk</span><span class="tk-loc">🇵🇰 Islamabad, Pakistan</span><a class="tk-btn" href="{{ '/files/NUST_conference_2023.pdf' | relative_url }}" target="_blank" rel="noopener noreferrer"><i class="fas fa-file-pdf"></i> Slides</a></div>
  </div></li>

  <li class="tk-item t-con"><div class="tk-date"><b>26</b><span>Jun</span></div><div>
    <h3>A latent process model for discrete extremes</h3>
    <p class="tk-au"><b>Ahmad, T.</b>, &amp; Gaetan, C.</p>
    <p class="tk-ev"><i class="fas fa-location-dot"></i>13th International Conference on Extreme Value Analysis (EVA 2023), Bocconi University · 26–30 June 2023</p>
    <div class="tk-meta"><span class="tk-type">Contributed talk</span><span class="tk-loc">🇮🇹 Milan, Italy</span><a class="tk-btn" href="{{ '/files/EVA_2023.pdf' | relative_url }}" target="_blank" rel="noopener noreferrer"><i class="fas fa-file-pdf"></i> Slides</a></div>
  </div></li>
</ul>

<div class="tk-year">2022</div>
<ul class="tk-list">
  <li class="tk-item t-con"><div class="tk-date"><b>17</b><span>Dec</span></div><div>
    <h3>Modelling of discrete extremes through extended versions of discrete generalized Pareto distribution</h3>
    <p class="tk-au"><b>Ahmad, T.</b>, Gaetan, C., &amp; Naveau, P.</p>
    <p class="tk-ev"><i class="fas fa-location-dot"></i>15th International Conference of the ERCIM Working Group on Computational and Methodological Statistics (CMStatistics 2022), King’s College London · 17–19 December 2022</p>
    <div class="tk-meta"><span class="tk-type">Contributed talk</span><span class="tk-loc">🇬🇧 London, UK</span></div>
  </div></li>

  <li class="tk-item t-inv"><div class="tk-date"><b>23</b><span>Sep</span></div><div>
    <h3>Modelling the entire range of discrete extreme data</h3>
    <p class="tk-au"><b>Ahmad, T.</b></p>
    <p class="tk-ev"><i class="fas fa-location-dot"></i>International Conference on Recent Trends in Statistics &amp; Data Analytics, National University of Sciences and Technology (NUST) · 23 September 2022</p>
    <div class="tk-meta"><span class="tk-type">Invited talk</span><span class="tk-loc">🇵🇰 Islamabad, Pakistan</span></div>
  </div></li>

  <li class="tk-item t-sem"><div class="tk-date"><b>19</b><span>Apr</span></div><div>
    <h3>Some new versions of discrete extreme models</h3>
    <p class="tk-au"><b>Ahmad, T.</b></p>
    <p class="tk-ev"><i class="fas fa-location-dot"></i>Laboratoire de Mathématiques de Versailles · 19 April 2022</p>
    <div class="tk-meta"><span class="tk-type">Seminar</span><span class="tk-loc">🇫🇷 Versailles, France</span></div>
  </div></li>

  <li class="tk-item t-sem"><div class="tk-date"><b>17</b><span>Feb</span></div><div>
    <h3>Some new versions of discrete extreme models</h3>
    <p class="tk-au"><b>Ahmad, T.</b></p>
    <p class="tk-ev"><i class="fas fa-location-dot"></i>Department of Statistical Sciences, University of Padova · 17 February 2022</p>
    <div class="tk-meta"><span class="tk-type">Seminar</span><span class="tk-loc">🇮🇹 Padova, Italy</span></div>
  </div></li>

  <li class="tk-item t-sem"><div class="tk-date"><b>28</b><span>Jan</span></div><div>
    <h3>Extreme value theory and its role in the modeling of rare events</h3>
    <p class="tk-au"><b>Ahmad, T.</b></p>
    <p class="tk-ev"><i class="fas fa-location-dot"></i>Department of Statistics, Allama Iqbal Open University · 28 January 2022</p>
    <div class="tk-meta"><span class="tk-type">Seminar</span><span class="tk-loc">🇵🇰 Islamabad, Pakistan</span></div>
  </div></li>
</ul>

</div>
</div>

<script>
(function(){
  var root=document.getElementById('tk-root'); if(!root) return;
  var chips=root.querySelectorAll('.tk-chip'),items=root.querySelectorAll('#tk-all .tk-item');
  chips.forEach(function(c){c.addEventListener('click',function(){
    var f=c.getAttribute('data-f');
    chips.forEach(function(x){x.setAttribute('aria-pressed',x===c?'true':'false');});
    items.forEach(function(it){it.hidden=!(f==='all'||it.classList.contains(f));});
    root.querySelectorAll('#tk-all .tk-year').forEach(function(h){var ul=h.nextElementSibling;var any=ul&&ul.querySelector('.tk-item:not([hidden])');h.hidden=!any;ul.hidden=!any;});
  });});
})();
</script>
