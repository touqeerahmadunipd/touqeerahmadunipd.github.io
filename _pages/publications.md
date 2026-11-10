---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<style>
  .pb{--accent:#0f86a8;--accent-soft:rgba(15,134,168,.10);--warm:#d0683d;--warm-soft:rgba(208,104,61,.12);--card:var(--global-bg-color);--line:var(--global-border-color);--muted:color-mix(in srgb,var(--global-text-color) 75%,transparent)}
  html[data-theme="dark"] .pb{--accent:#20a0c4;--accent-soft:rgba(32,160,196,.16);--warm:#d9744a;--warm-soft:rgba(217,116,74,.18)}
  .pb *{box-sizing:border-box}
  .pb a{text-decoration:none}
  .pb p{margin:0 0 1em}

  .pb-hero{position:relative;border-radius:16px;overflow:hidden;margin:0 0 1.6em;min-height:190px;background:#145a6c}
  .pb-hero img{display:block;width:100%;height:230px;object-fit:cover;opacity:.55;margin:0}
  .pb-hero .ov{position:absolute;inset:0;background:linear-gradient(90deg,rgba(10,50,62,.92),rgba(10,50,62,.35));display:flex;flex-direction:column;justify-content:flex-end;padding:1.3em 1.5em;color:#fff}
  .pb-hero h2{color:#fff;margin:0 0 .25em;font-size:1.5em;border:0}
  .pb-hero p{margin:0;font-size:.85em;color:rgba(255,255,255,.88);max-width:34em}
  .pb-hero small{position:absolute;right:1em;bottom:.7em;font-size:.65em;color:rgba(255,255,255,.7)}

  .pb-stats{display:grid;grid-template-columns:repeat(4,1fr);gap:.8em;margin:0 0 1.6em}
  .pb-stat{border:1px solid var(--line);border-radius:12px;padding:.9em 1em;background:var(--card);position:relative;overflow:hidden}
  .pb-stat::before{content:"";position:absolute;left:0;top:0;bottom:0;width:4px;background:var(--accent)}
  .pb-stat:nth-child(even)::before{background:var(--warm)}
  .pb-stat b{display:block;font-size:1.5em;line-height:1.1}
  .pb-stat span{font-size:.72em;color:var(--muted)}
  @media (max-width:700px){.pb-stats{grid-template-columns:1fr 1fr}}

  .pb-chart{border:1px solid var(--line);border-radius:14px;padding:1em 1em .6em;margin:0 0 1.8em;background:var(--card)}
  .pb-chart h3{font-size:.9em;margin:0 0 .5em}
  .pb-chart svg{display:block;width:100%;height:auto}
  .pb svg text{fill:var(--global-text-color);fill-opacity:.75;font-size:11px;font-family:inherit}
  .pb svg .lab{fill-opacity:.95;font-weight:700}
  .pb svg .bar{fill:var(--accent);transition:opacity .2s}
  .pb svg .bar.now{fill:var(--warm)}
  .pb svg .bar.dim{opacity:.25}

  .pb-tools{display:flex;flex-wrap:wrap;gap:.5em;align-items:center;margin:0 0 1.2em}
  .pb-chip{font:inherit;font-size:.74em;font-weight:600;padding:.45em .9em;border-radius:999px;border:1.5px solid var(--line);background:var(--card);color:var(--global-text-color);cursor:pointer;transition:all .15s}
  .pb-chip:hover{border-color:var(--accent);color:var(--accent)}
  .pb-chip[aria-pressed="true"]{background:var(--accent);border-color:var(--accent);color:#fff}
  .pb-search{flex:1 1 180px;min-width:160px;font:inherit;font-size:.8em;padding:.5em .9em;border-radius:999px;border:1.5px solid var(--line);background:var(--card);color:var(--global-text-color)}
  .pb-search:focus{outline:none;border-color:var(--accent)}
  .pb-count{font-size:.74em;color:var(--muted);margin:-.4em 0 1em}

  .pb h2.pb-h{display:flex;align-items:center;gap:.5em;font-size:1.25em;margin:1.6em 0 .8em;padding-bottom:.4em;border-bottom:1px solid var(--line)}
  .pb h2.pb-h i{color:var(--accent);font-size:.85em}
  .pb-year{display:flex;align-items:center;gap:.6em;font-size:.82em;font-weight:700;color:var(--accent);margin:1.3em 0 .6em;letter-spacing:.04em}
  .pb-year::after{content:"";flex:1;height:1px;background:var(--line)}

  .pb-list{list-style:none;margin:0;padding:0;display:grid;gap:.75em}
  .pb-item{margin:0;border:1px solid var(--line);border-radius:12px;padding:.95em 1.1em .85em;background:var(--card);border-left:4px solid var(--accent);transition:transform .2s ease, box-shadow .2s ease, border-color .2s ease}
  .pb-item:hover{transform:translateY(-2px);box-shadow:0 10px 22px -16px rgba(0,0,0,.4);border-color:var(--accent)}
  .pb-item.top{border-left-color:var(--warm)}
  .pb-item h3{font-size:.95em;line-height:1.38;margin:0 0 .3em}
  .pb-item h3 a{color:var(--global-text-color)}
  .pb-item h3 a:hover{color:var(--accent)}
  .pb-au{font-size:.78em;color:var(--muted);margin:0 0 .45em}
  .pb-au b{color:var(--global-text-color)}
  .pb-meta{display:flex;flex-wrap:wrap;gap:.4em;align-items:center}
  .pb-venue{font-size:.7em;font-weight:700;padding:.25em .65em;border-radius:6px;background:var(--accent-soft);color:var(--accent)}
  .pb-venue.top{background:var(--warm);color:#fff}
  .pb-tag{font-size:.66em;padding:.2em .6em;border-radius:999px;border:1px solid var(--line);color:var(--muted)}
  .pb-act{margin-left:auto;display:flex;gap:.4em}
  .pb-btn{font:inherit;font-size:.7em;font-weight:600;padding:.3em .75em;border-radius:999px;border:1.5px solid var(--accent);color:var(--accent)!important;background:transparent;cursor:pointer;transition:all .15s}
  .pb-btn:hover{background:var(--accent);color:#fff!important}
  .pb-empty{display:none;font-size:.85em;color:var(--muted);padding:1em 0}

  .pb-scholar{margin-top:2em;border-radius:14px;padding:1.2em 1.4em;background:linear-gradient(135deg,#0f86a8,#145a6c);color:#fff;display:flex;flex-wrap:wrap;gap:1em;align-items:center;justify-content:space-between}
  .pb-scholar p{margin:0;color:rgba(255,255,255,.9);font-size:.88em}
  .pb-scholar a{display:inline-flex;align-items:center;gap:.5em;background:#fff;color:#145a6c!important;font-weight:700;font-size:.8em;padding:.55em 1em;border-radius:999px}
  [hidden]{display:none!important}
</style>

<div class="pb" id="pb-root">

<div class="pb-hero">
  <img src="/images/capri1.jpg" alt="Capri, Italy">
  <div class="ov">
    <h2><i class="fas fa-book-open"></i> Research output</h2>
    <p>Papers on extreme value theory, risk assessment, uncertainty quantification and statistical learning, with applications to climate, hydrology, energy and finance.</p>
  </div>
  <small>Capri, Italy</small>
</div>

<div class="pb-stats">
  <div class="pb-stat"><b>19</b><span>Journal &amp; conference papers</span></div>
  <div class="pb-stat"><b>3</b><span>Preprints</span></div>
  <div class="pb-stat"><b>5</b><span>Papers in 2026 so far</span></div>
  <div class="pb-stat"><b>NeurIPS</b><span>2025, imbalanced classification</span></div>
</div>

<!--
<div class="pb-chart">
  <h3><i class="fas fa-chart-column" style="color:var(--accent)"></i> Publications per year</h3>
  <svg id="pb-years" viewBox="0 0 600 150" role="img" aria-label="Bar chart of the number of published papers per year from 2019 to 2026"></svg>
</div>
-->

<h2 class="pb-h"><i class="fas fa-file-lines"></i> Published articles</h2>

<div class="pb-tools" role="toolbar" aria-label="Filter publications">
  <button class="pb-chip" aria-pressed="true" data-f="all">All</button>
  <button class="pb-chip" aria-pressed="false" data-f="evt">Extreme value theory</button>
  <button class="pb-chip" aria-pressed="false" data-f="climate">Climate &amp; environment</button>
  <button class="pb-chip" aria-pressed="false" data-f="risk">Risk assessment</button>
  <button class="pb-chip" aria-pressed="false" data-f="learning">Statistical learning</button>
  <button class="pb-chip" aria-pressed="false" data-f="design">Design of experiments</button>
  <button class="pb-chip" aria-pressed="false" data-f="other">Other</button>
  <input class="pb-search" id="pb-q" type="search" placeholder="Search title, journal or co-author" aria-label="Search publications">
</div>
<p class="pb-count" id="pb-count">Showing all 19 published articles</p>

<div id="pb-pubs">

<div class="pb-year" data-y="2026">2026</div>
<ul class="pb-list">
  <li class="pb-item" data-t="climate risk"><h3><a href="https://doi.org/10.1007/s11356-026-38256-z" target="_blank" rel="noopener noreferrer">A novel multivariate vine-copula–based drought index with application to high-elevation catchments</a></h3>
    <p class="pb-au">Badar, Z., Ahmad, I., <b>Ahmad, T.</b>, &amp; Almanjahie, I. M.</p>
    <div class="pb-meta"><span class="pb-venue">Environmental Science and Pollution Research · 33(32), 16359–16379</span><span class="pb-tag">Drought</span><span class="pb-tag">Copulas</span>
    <span class="pb-act"><button class="pb-btn" data-cite>Cite</button><a class="pb-btn" href="https://doi.org/10.1007/s11356-026-38256-z" target="_blank" rel="noopener noreferrer">DOI</a></span></div></li>

  <li class="pb-item" data-t="design"><h3><a href="https://doi.org/10.1080/10543406.2026.2680927" target="_blank" rel="noopener noreferrer">Order-of-addition in mixture and component-amount designs in orthogonal blocks</a></h3>
    <p class="pb-au">Hasan, T., &amp; <b>Ahmad, T.</b></p>
    <div class="pb-meta"><span class="pb-venue">Journal of Biopharmaceutical Statistics</span><span class="pb-tag">Optimal designs</span>
    <span class="pb-act"><button class="pb-btn" data-cite>Cite</button><a class="pb-btn" href="https://doi.org/10.1080/10543406.2026.2680927" target="_blank" rel="noopener noreferrer">DOI</a></span></div></li>

  <li class="pb-item" data-t="other"><h3><a href="https://doi.org/10.1080/00949655.2026.2660176" target="_blank" rel="noopener noreferrer">A new composite Mann–Whitney test for two-sample survival comparisons with right-censored data</a></h3>
    <p class="pb-au">Hussain, A., &amp; <b>Ahmad, T.</b></p>
    <div class="pb-meta"><span class="pb-venue">Journal of Statistical Computation and Simulation · 96(13), 3252–3272</span><span class="pb-tag">Survival analysis</span>
    <span class="pb-act"><button class="pb-btn" data-cite>Cite</button><a class="pb-btn" href="https://doi.org/10.1080/00949655.2026.2660176" target="_blank" rel="noopener noreferrer">DOI</a></span></div></li>

  <li class="pb-item" data-t="evt climate"><h3><a href="https://doi.org/10.1016/j.ejrh.2026.103330" target="_blank" rel="noopener noreferrer">Regional modeling of zero-inflated precipitation in Pakistan by classical and Bayesian approaches</a></h3>
    <p class="pb-au">Abbas, A., <b>Ahmad, T.</b>, &amp; Ahmad, I.</p>
    <div class="pb-meta"><span class="pb-venue">Journal of Hydrology: Regional Studies · 65, 103330</span><span class="pb-tag">Precipitation</span><span class="pb-tag">Bayesian</span>
    <span class="pb-act"><button class="pb-btn" data-cite>Cite</button><a class="pb-btn" href="https://doi.org/10.1016/j.ejrh.2026.103330" target="_blank" rel="noopener noreferrer">DOI</a></span></div></li>

  <li class="pb-item" data-t="evt"><h3><a href="https://doi.org/10.1080/02664763.2026.2634785" target="_blank" rel="noopener noreferrer">New flexible versions of the extended generalized Pareto distribution for count data</a></h3>
    <p class="pb-au"><b>Ahmad, T.</b>, &amp; Arshad, I. A.</p>
    <div class="pb-meta"><span class="pb-venue">Journal of Applied Statistics</span><span class="pb-tag">Discrete extremes</span>
    <span class="pb-act"><button class="pb-btn" data-cite>Cite</button><a class="pb-btn" href="https://doi.org/10.1080/02664763.2026.2634785" target="_blank" rel="noopener noreferrer">DOI</a></span></div></li>
</ul>

<div class="pb-year" data-y="2025">2025</div>
<ul class="pb-list">
  <li class="pb-item top" data-t="learning"><h3><a href="https://proceedings.neurips.cc/paper_files/paper/2025/file/e715ad3d527e246af3ab286c3f3d367c-Paper-Conference.pdf" target="_blank" rel="noopener noreferrer">Concentration and excess risk bounds for imbalanced classification with synthetic oversampling</a></h3>
    <p class="pb-au"><b>Ahmad, T.</b>, Kalan, M. M., Portier, F., &amp; Stupfler, G.</p>
    <div class="pb-meta"><span class="pb-venue top">NeurIPS 2025</span><span class="pb-tag">Imbalanced data</span><span class="pb-tag">Learning theory</span>
    <span class="pb-act"><button class="pb-btn" data-cite>Cite</button><a class="pb-btn" href="https://proceedings.neurips.cc/paper_files/paper/2025/file/e715ad3d527e246af3ab286c3f3d367c-Paper-Conference.pdf" target="_blank" rel="noopener noreferrer">PDF</a></span></div></li>

  <li class="pb-item" data-t="evt climate risk"><h3><a href="https://doi.org/10.1002/joc.8705" target="_blank" rel="noopener noreferrer">Estimating extreme drought risk through classical and Bayesian paradigms</a></h3>
    <p class="pb-au"><b>Ahmad, T.</b>, Sabir, S., Arshad, I. A., Hasan, T., &amp; Albalawi, O.</p>
    <div class="pb-meta"><span class="pb-venue">International Journal of Climatology · 45(2), e8705</span><span class="pb-tag">Drought</span><span class="pb-tag">Bayesian MCMC</span>
    <span class="pb-act"><button class="pb-btn" data-cite>Cite</button><a class="pb-btn" href="https://doi.org/10.1002/joc.8705" target="_blank" rel="noopener noreferrer">DOI</a></span></div></li>

  <li class="pb-item" data-t="evt climate"><h3><a href="https://doi.org/10.1080/03610918.2025.2585398" target="_blank" rel="noopener noreferrer">Modeling zero-inflated precipitation extremes</a></h3>
    <p class="pb-au">Abbas, A., <b>Ahmad, T.</b>, &amp; Ahmad, I.</p>
    <div class="pb-meta"><span class="pb-venue">Communications in Statistics – Simulation and Computation</span><span class="pb-tag">Precipitation</span>
    <span class="pb-act"><button class="pb-btn" data-cite>Cite</button><a class="pb-btn" href="https://doi.org/10.1080/03610918.2025.2585398" target="_blank" rel="noopener noreferrer">DOI</a></span></div></li>

  <li class="pb-item" data-t="design"><h3><a href="https://doi.org/10.1002/pst.70047" target="_blank" rel="noopener noreferrer">Order of addition in mixture-amount experiments</a></h3>
    <p class="pb-au">Hasan, T., &amp; <b>Ahmad, T.</b></p>
    <div class="pb-meta"><span class="pb-venue">Pharmaceutical Statistics · 24(6), e70047</span><span class="pb-tag">Mixture experiments</span>
    <span class="pb-act"><button class="pb-btn" data-cite>Cite</button><a class="pb-btn" href="https://doi.org/10.1002/pst.70047" target="_blank" rel="noopener noreferrer">DOI</a></span></div></li>

  <li class="pb-item" data-t="evt risk"><h3><a href="https://doi.org/10.1007/s00181-025-02784-3" target="_blank" rel="noopener noreferrer">Novel modeling for assessment of extreme values risk in cryptocurrencies portfolio</a></h3>
    <p class="pb-au">Rehman, S. U., <b>Ahmad, T.</b>, &amp; Wu, D.</p>
    <div class="pb-meta"><span class="pb-venue">Empirical Economics · 69(4), 2065–2092</span><span class="pb-tag">VaR &amp; ES</span><span class="pb-tag">Copulas</span>
    <span class="pb-act"><button class="pb-btn" data-cite>Cite</button><a class="pb-btn" href="https://doi.org/10.1007/s00181-025-02784-3" target="_blank" rel="noopener noreferrer">DOI</a></span></div></li>

  <li class="pb-item" data-t="evt"><h3><a href="https://doi.org/10.1177/1471082X241266729" target="_blank" rel="noopener noreferrer">An extended generalized Pareto regression model for count data</a></h3>
    <p class="pb-au"><b>Ahmad, T.</b>, Gaetan, C., &amp; Naveau, P.</p>
    <div class="pb-meta"><span class="pb-venue">Statistical Modelling · 25(5), 416–431</span><span class="pb-tag">Discrete extremes</span><span class="pb-tag">GAMs</span>
    <span class="pb-act"><button class="pb-btn" data-cite>Cite</button><a class="pb-btn" href="https://doi.org/10.1177/1471082X241266729" target="_blank" rel="noopener noreferrer">DOI</a></span></div></li>
</ul>

<div class="pb-year" data-y="2024">2024</div>
<ul class="pb-list">
  <li class="pb-item" data-t="climate risk"><h3><a href="https://doi.org/10.1016/j.heliyon.2024.e25422" target="_blank" rel="noopener noreferrer">A detailed study on quantification and modeling of drought characteristics using different copula families</a></h3>
    <p class="pb-au">Ahmad, I., <b>Ahmad, T.</b>, Rehman, S. U., Almanjahie, I. M., &amp; Alshahrani, F.</p>
    <div class="pb-meta"><span class="pb-venue">Heliyon · 10(3), e25422</span><span class="pb-tag">Drought</span><span class="pb-tag">Copulas</span>
    <span class="pb-act"><button class="pb-btn" data-cite>Cite</button><a class="pb-btn" href="https://doi.org/10.1016/j.heliyon.2024.e25422" target="_blank" rel="noopener noreferrer">DOI</a></span></div></li>

  <li class="pb-item" data-t="evt climate"><h3><a href="https://doi.org/10.1016/j.heliyon.2023.e23388" target="_blank" rel="noopener noreferrer">Estimation of regional and at-site quantiles of extreme winds under flood index procedure</a></h3>
    <p class="pb-au">Ahmad, I., <b>Ahmad, T.</b>, Shahzad, U., Ameer, M. A., Emam, W., Tashkandy, Y., &amp; Badar, Z.</p>
    <div class="pb-meta"><span class="pb-venue">Heliyon · 10(1), e23388</span><span class="pb-tag">Extreme winds</span>
    <span class="pb-act"><button class="pb-btn" data-cite>Cite</button><a class="pb-btn" href="https://doi.org/10.1016/j.heliyon.2023.e23388" target="_blank" rel="noopener noreferrer">DOI</a></span></div></li>
</ul>

<div class="pb-year" data-y="2023">2023</div>
<ul class="pb-list">
  <li class="pb-item" data-t="evt climate"><h3><a href="https://doi.org/10.1016/j.egyr.2023.01.093" target="_blank" rel="noopener noreferrer">An efficient Bayesian modelling of extreme winds in the favour of energy generation in Pakistan</a></h3>
    <p class="pb-au"><b>Ahmad, T.</b>, Ahmad, I., Arshad, I. A., &amp; Almanjahie, I. M.</p>
    <div class="pb-meta"><span class="pb-venue">Energy Reports · 9, 2980–2992</span><span class="pb-tag">Extreme winds</span><span class="pb-tag">Bayesian</span>
    <span class="pb-act"><button class="pb-btn" data-cite>Cite</button><a class="pb-btn" href="https://doi.org/10.1016/j.egyr.2023.01.093" target="_blank" rel="noopener noreferrer">DOI</a></span></div></li>
</ul>

<div class="pb-year" data-y="2022">2022</div>
<ul class="pb-list">
  <li class="pb-item" data-t="evt climate"><h3><a href="https://doi.org/10.1002/joc.7240" target="_blank" rel="noopener noreferrer">A comprehensive study on the Bayesian modelling of extreme rainfall: A case study from Pakistan</a></h3>
    <p class="pb-au"><b>Ahmad, T.</b>, Ahmad, I., Arshad, I. A., &amp; Bianco, N.</p>
    <div class="pb-meta"><span class="pb-venue">International Journal of Climatology · 42(1), 208–224</span><span class="pb-tag">Extreme rainfall</span><span class="pb-tag">Bayesian</span>
    <span class="pb-act"><button class="pb-btn" data-cite>Cite</button><a class="pb-btn" href="https://doi.org/10.1002/joc.7240" target="_blank" rel="noopener noreferrer">DOI</a></span></div></li>
</ul>

<div class="pb-year" data-y="2021">2021</div>
<ul class="pb-list">
  <li class="pb-item" data-t="other"><h3><a href="https://doi.org/10.1155/2021/6289337" target="_blank" rel="noopener noreferrer">Bayesian analysis of cancer data using a 4-component exponential mixture model</a></h3>
    <p class="pb-au">Noor, F., Masood, S., Sabar, Y., Shah, S., <b>Ahmad, T.</b>, Abdollahi, A., &amp; Sajid, A.</p>
    <div class="pb-meta"><span class="pb-venue">Computational and Mathematical Methods in Medicine · 2021, 6289337</span><span class="pb-tag">Bayesian</span>
    <span class="pb-act"><button class="pb-btn" data-cite>Cite</button><a class="pb-btn" href="https://doi.org/10.1155/2021/6289337" target="_blank" rel="noopener noreferrer">DOI</a></span></div></li>

  <li class="pb-item" data-t="other"><h3>Estimating the determinants of female labor force participation in Pakistan</h3>
    <p class="pb-au">Cheema, A. R., Firdous, S., &amp; <b>Ahmad, T.</b></p>
    <div class="pb-meta"><span class="pb-venue">International Journal of Disaster Recovery and Business Continuity · 12(1), 413–424</span><span class="pb-tag">Applied statistics</span>
    <span class="pb-act"><button class="pb-btn" data-cite>Cite</button></span></div></li>

  <li class="pb-item" data-t="other"><h3>Family planning and fertility reduction in Pakistan</h3>
    <p class="pb-au">Cheema, A. R., Firdous, S., <b>Ahmad, T.</b>, &amp; Imran, M.</p>
    <div class="pb-meta"><span class="pb-venue">Ilkogretim Online · 20(5)</span><span class="pb-tag">Applied statistics</span>
    <span class="pb-act"><button class="pb-btn" data-cite>Cite</button></span></div></li>
</ul>

<div class="pb-year" data-y="2019">2019</div>
<ul class="pb-list">
  <li class="pb-item" data-t="evt climate"><h3><a href="https://doi.org/10.15666/aeer/1706_1372913748" target="_blank" rel="noopener noreferrer">Modelling of extreme rainfall in Punjab, Pakistan using Bayesian and frequentist approach</a></h3>
    <p class="pb-au">Ahmad, I., <b>Ahmad, T.</b>, &amp; Almanjahie, I. M.</p>
    <div class="pb-meta"><span class="pb-venue">Applied Ecology and Environmental Research · 17(6), 13729–13748</span><span class="pb-tag">Extreme rainfall</span>
    <span class="pb-act"><button class="pb-btn" data-cite>Cite</button><a class="pb-btn" href="https://doi.org/10.15666/aeer/1706_1372913748" target="_blank" rel="noopener noreferrer">DOI</a></span></div></li>
</ul>

</div>
<p class="pb-empty" id="pb-empty">No articles match this filter.</p>

<h2 class="pb-h"><i class="fas fa-flask"></i> Preprints</h2>
<ul class="pb-list">
  <li class="pb-item" data-t="evt"><h3><a href="https://arxiv.org/abs/2510.27365" target="_blank" rel="noopener noreferrer">Flexible model for varying levels of zeros and outliers in count data</a></h3>
    <p class="pb-au"><b>Ahmad, T.</b>, et al. (2025)</p>
    <div class="pb-meta"><span class="pb-venue">arXiv:2510.27365</span><span class="pb-tag">Discrete extremes</span>
    <span class="pb-act"><a class="pb-btn" href="https://arxiv.org/abs/2510.27365" target="_blank" rel="noopener noreferrer">arXiv</a></span></div></li>
  <li class="pb-item" data-t="evt climate"><h3><a href="https://doi.org/10.48550/arXiv.2507.15099" target="_blank" rel="noopener noreferrer">Space–time modeling for drought classification and prediction</a></h3>
    <p class="pb-au"><b>Ahmad, T.</b>, &amp; Hasan, T. (2025)</p>
    <div class="pb-meta"><span class="pb-venue">arXiv:2507.15099</span><span class="pb-tag">Drought</span><span class="pb-tag">EGPD</span>
    <span class="pb-act"><a class="pb-btn" href="https://doi.org/10.48550/arXiv.2507.15099" target="_blank" rel="noopener noreferrer">arXiv</a></span></div></li>
  <li class="pb-item" data-t="learning"><h3><a href="https://doi.org/10.48550/arXiv.2407.08485" target="_blank" rel="noopener noreferrer">Logistic lasso regression with nearest neighbors for gradient-based dimension reduction</a></h3>
    <p class="pb-au"><b>Ahmad, T.</b>, Portier, F., &amp; Stupfler, G. (2024)</p>
    <div class="pb-meta"><span class="pb-venue">arXiv:2407.08485</span><span class="pb-tag">Dimension reduction</span>
    <span class="pb-act"><a class="pb-btn" href="https://doi.org/10.48550/arXiv.2407.08485" target="_blank" rel="noopener noreferrer">arXiv</a></span></div></li>
</ul>

<div class="pb-scholar">
  <p><b>Always up to date:</b> my complete list with citation counts is on Google Scholar.</p>
  <a href="https://scholar.google.com/citations?user=0Unv8IAAAAAJ&hl=en" target="_blank" rel="noopener noreferrer"><i class="fas fa-graduation-cap"></i> Google Scholar profile</a>
</div>

</div>

<script>
(function(){
  var NS='http://www.w3.org/2000/svg';
  var root=document.getElementById('pb-root'); if(!root) return;
  function el(svg,tag,a,txt){var e=document.createElementNS(NS,tag);for(var k in a)e.setAttribute(k,a[k]);if(txt!=null)e.textContent=txt;svg.appendChild(e);return e;}

  /* ---- per-year bar chart, counted from the list itself ---- */
  var counts={};
  root.querySelectorAll('#pb-pubs .pb-year').forEach(function(h){var ul=h.nextElementSibling;counts[h.getAttribute('data-y')]=ul?ul.querySelectorAll('.pb-item').length:0;});
  var years=[];for(var y=2019;y<=2026;y++)years.push(String(y));
  var svg=document.getElementById('pb-years');
  if(svg){
    var L=20,R=590,T=18,B=124,max=1;years.forEach(function(y){max=Math.max(max,counts[y]||0);});
    var bw=(R-L)/years.length;
    el(svg,'line',{x1:L,x2:R,y1:B,y2:B,stroke:'currentColor','stroke-opacity':.25});
    years.forEach(function(y,i){
      var v=counts[y]||0,h=v/max*(B-T-10),x=L+i*bw+bw*.22,w=bw*.56,top=B-h,r=Math.min(5,w/2,h);
      var d=v?('M'+x+','+B+'V'+(top+r)+'Q'+x+','+top+' '+(x+r)+','+top+'H'+(x+w-r)+'Q'+(x+w)+','+top+' '+(x+w)+','+(top+r)+'V'+B+'Z'):'';
      if(v){var b=el(svg,'path',{d:d,'class':'bar'+(y==='2026'?' now':''),'data-y':y});b.style.cursor='pointer';b.addEventListener('click',function(){var t=root.querySelector('.pb-year[data-y="'+y+'"]');if(t)t.scrollIntoView({behavior:'smooth',block:'start'});});}
      el(svg,'text',{x:x+w/2,y:B+16,'text-anchor':'middle'},y);
      if(v)el(svg,'text',{x:x+w/2,y:top-6,'text-anchor':'middle','class':'lab'},v);
    });
  }

  /* ---- filters and search ---- */
  var chips=root.querySelectorAll('.pb-chip'),q=document.getElementById('pb-q'),cnt=document.getElementById('pb-count'),empty=document.getElementById('pb-empty');
  var items=root.querySelectorAll('#pb-pubs .pb-item'),total=items.length,f='all';
  var labels={all:'',evt:'extreme value theory',climate:'climate &amp; environment',risk:'risk assessment',learning:'statistical learning',design:'design of experiments',other:'other topics'};
  function apply(){
    var s=(q.value||'').toLowerCase().trim(),shown=0;
    items.forEach(function(it){var ok=(f==='all'||(' '+it.getAttribute('data-t')+' ').indexOf(' '+f+' ')>-1)&&(!s||it.textContent.toLowerCase().indexOf(s)>-1);it.hidden=!ok;if(ok)shown++;});
    root.querySelectorAll('#pb-pubs .pb-year').forEach(function(h){var ul=h.nextElementSibling,any=ul&&ul.querySelector('.pb-item:not([hidden])');h.hidden=!any;ul.hidden=!any;});
    empty.style.display=shown?'none':'block';
    cnt.innerHTML=(shown===total&&!s)?'Showing all '+total+' published articles':'Showing '+shown+' of '+total+' published articles'+(f!=='all'?' in '+labels[f]:'')+(s?' matching “'+q.value.replace(/</g,'')+'”':'');
  }
  chips.forEach(function(c){c.addEventListener('click',function(){chips.forEach(function(x){x.setAttribute('aria-pressed',x===c?'true':'false');});f=c.getAttribute('data-f');apply();});});
  q.addEventListener('input',apply);

  /* ---- copy citation ---- */
  root.querySelectorAll('[data-cite]').forEach(function(btn){
    btn.addEventListener('click',function(){
      var it=btn.closest('.pb-item'),yr=it.parentNode.previousElementSibling.getAttribute('data-y');
      var au=it.querySelector('.pb-au').textContent.trim(),ti=it.querySelector('h3').textContent.trim(),ve=it.querySelector('.pb-venue').textContent.replace(' · ',', ').trim();
      var link=it.querySelector('h3 a'),txt=au+' ('+yr+'). '+ti+'. '+ve+'.'+(link?' '+link.href:'');
      var done=function(){var o=btn.textContent;btn.textContent='Copied!';setTimeout(function(){btn.textContent=o;},1500);};
      if(navigator.clipboard&&navigator.clipboard.writeText){navigator.clipboard.writeText(txt).then(done,function(){window.prompt('Copy citation:',txt);});}else{window.prompt('Copy citation:',txt);}
    });
  });
})();
</script>
