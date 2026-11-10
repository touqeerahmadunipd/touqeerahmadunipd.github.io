---
layout: archive
title: "Teaching"
permalink: /teaching/
author_profile: true
---

{% include base_path %}

<style>
  .te{--accent:#0f86a8;--accent-soft:rgba(15,134,168,.10);--warm:#d0683d;--warm-soft:rgba(208,104,61,.12);--card:var(--global-bg-color);--line:var(--global-border-color);--muted:color-mix(in srgb,var(--global-text-color) 75%,transparent)}
  html[data-theme="dark"] .te{--accent:#20a0c4;--accent-soft:rgba(32,160,196,.16);--warm:#d9744a;--warm-soft:rgba(217,116,74,.18)}
  .te *{box-sizing:border-box}
  .te a{text-decoration:none}
  .te p{margin:0 0 1em}

  .te-hero{position:relative;border-radius:16px;overflow:hidden;margin:0 0 1.6em;background:#145a6c}
  .te-hero img{display:block;width:100%;height:250px;object-fit:cover;opacity:.6;margin:0}
  .te-hero .ov{position:absolute;inset:0;background:linear-gradient(90deg,rgba(10,50,62,.92),rgba(10,50,62,.3));display:flex;flex-direction:column;justify-content:flex-end;padding:1.3em 1.5em;color:#fff}
  .te-hero h2{color:#fff;margin:0 0 .25em;font-size:1.5em;border:0}
  .te-hero p{margin:0;font-size:.85em;color:rgba(255,255,255,.88);max-width:34em}
  .te-hero small{position:absolute;right:1em;bottom:.7em;font-size:.65em;color:rgba(255,255,255,.75)}

  .te-stats{display:grid;grid-template-columns:repeat(4,1fr);gap:.8em;margin:0 0 1.6em}
  .te-stat{border:1px solid var(--line);border-radius:12px;padding:.9em 1em;background:var(--card);position:relative;overflow:hidden}
  .te-stat::before{content:"";position:absolute;left:0;top:0;bottom:0;width:4px;background:var(--accent)}
  .te-stat:nth-child(even)::before{background:var(--warm)}
  .te-stat b{display:block;font-size:1.45em;line-height:1.1}
  .te-stat span{font-size:.7em;color:var(--muted)}
  @media (max-width:700px){.te-stats{grid-template-columns:1fr 1fr}}

  .te-chart{border:1px solid var(--line);border-radius:14px;padding:1em 1.1em .7em;margin:0 0 1.8em;background:var(--card)}
  .te-chart h3{font-size:.9em;margin:0 0 .4em}
  .te-chart h3 i{color:var(--accent)}
  .te-legend{display:flex;flex-wrap:wrap;gap:1.1em;font-size:.72em;color:var(--muted);margin:0 0 .4em}
  .te-legend span{display:inline-flex;align-items:center;gap:.45em}
  .te-legend i{width:.9em;height:.9em;border-radius:3px;display:inline-block}
  .te-chart svg{display:block;width:100%;height:auto}
  .te svg text{fill:var(--global-text-color);fill-opacity:.8;font-size:11px;font-family:inherit}
  .te svg .val{fill-opacity:1;font-weight:700}
  .te svg .pg{fill:var(--accent)}
  .te svg .ug{fill:var(--warm)}

  .te h2.te-h{display:flex;align-items:center;gap:.5em;font-size:1.25em;margin:1.8em 0 .8em;padding-bottom:.4em;border-bottom:1px solid var(--line)}
  .te h2.te-h i{color:var(--accent);font-size:.85em}

  .te-inst{border:1px solid var(--line);border-radius:16px;background:var(--card);overflow:hidden;margin:0 0 1.4em}
  .te-inst .head{display:grid;grid-template-columns:3.2em 1fr auto;gap:1em;align-items:center;padding:1.1em 1.2em;border-bottom:1px solid var(--line);background:linear-gradient(90deg,var(--cs),transparent)}
  .te-inst .ic{width:3.2em;height:3.2em;border-radius:12px;display:grid;place-items:center;background:var(--c);color:#fff;font-size:1em}
  .te-inst h3{font-size:1em;margin:0 0 .15em;line-height:1.3}
  .te-inst .sub{font-size:.74em;color:var(--muted);margin:0!important;line-height:1.45}
  .te-inst .lvl{font-size:.66em;font-weight:700;letter-spacing:.04em;text-transform:uppercase;padding:.3em .7em;border-radius:6px;background:var(--c);color:#fff;white-space:nowrap}
  .te-inst.pg{--c:var(--accent);--cs:var(--accent-soft)}
  .te-inst.ug{--c:var(--warm);--cs:var(--warm-soft)}
  .te-inst .summary{font-size:.8em;padding:.9em 1.2em 0;margin:0!important}
  .te-courses{display:grid;grid-template-columns:1fr 1fr;gap:.7em;align-items:start;padding:.9em 1.2em 1.1em}
  @media (max-width:760px){.te-courses{grid-template-columns:1fr}.te-inst .head{grid-template-columns:3.2em 1fr}.te-inst .lvl{grid-column:2;justify-self:start}}
  .te-course{border:1px solid var(--line);border-radius:12px;padding:.8em .9em;border-top:3px solid var(--c);transition:transform .2s ease, box-shadow .2s ease}
  .te-course:hover{transform:translateY(-2px);box-shadow:0 10px 22px -16px rgba(0,0,0,.4)}
  .te-course h4{font-size:.86em;margin:0 0 .3em;display:flex;justify-content:space-between;gap:.6em;align-items:baseline}
  .te-course h4 span{font-size:.8em;font-weight:700;color:var(--c);white-space:nowrap}
  .te-course .when{font-size:.7em;color:var(--muted);margin:0 0 .5em!important}
  .te-course details{font-size:.74em}
  .te-course summary{cursor:pointer;font-weight:600;color:var(--c);list-style:none}
  .te-course summary::-webkit-details-marker{display:none}
  .te-course summary::before{content:"+ ";font-weight:700}
  .te-course details[open] summary::before{content:"\2212  "}
  .te-course ul{margin:.45em 0 .2em 1.1em;padding:0}
  .te-course li{margin:0 0 .15em;line-height:1.4}
  .te-course .r{display:inline-flex;align-items:center;gap:.35em;font-size:.68em;margin-top:.5em;padding:.2em .6em;border-radius:999px;background:var(--cs);color:var(--c);font-weight:600}
  .te-more{display:inline-flex;align-items:center;gap:.4em;font-size:.76em;font-weight:600;color:var(--c)!important;margin:0 1.2em 1.1em}
  .te-more:hover{text-decoration:underline}

  .te-approach{display:grid;grid-template-columns:repeat(3,1fr);gap:.8em}
  @media (max-width:760px){.te-approach{grid-template-columns:1fr}}
  .te-ap{border:1px solid var(--line);border-radius:12px;padding:1em;background:var(--card)}
  .te-ap .ic{width:2.3em;height:2.3em;border-radius:10px;display:grid;place-items:center;background:var(--accent-soft);color:var(--accent);margin-bottom:.6em}
  .te-ap:nth-child(2) .ic{background:var(--warm-soft);color:var(--warm)}
  .te-ap h4{font-size:.86em;margin:0 0 .3em}
  .te-ap p{font-size:.76em;color:var(--muted);margin:0!important;line-height:1.5}
</style>

<div class="te" id="te-root">

<div class="te-hero">
  <img src="/images/chattue.jpg" alt="Château de Vincennes, Paris">
  <div class="ov">
    <h2><i class="fas fa-chalkboard-user"></i> Teaching</h2>
    <p>Undergraduate and postgraduate statistics courses, from probability and inference to regression, econometrics and research methods, always with hands-on R workshops.</p>
  </div>
  <small>Château de Vincennes, Paris</small>
</div>

<div class="te-stats">
  <div class="te-stat"><b>427.5</b><span>Teaching hours</span></div>
  <div class="te-stat"><b>9</b><span>Courses taught</span></div>
  <div class="te-stat"><b>2</b><span>Institutions, 2016–2019</span></div>
  <div class="te-stat"><b>R</b><span>Practical workshops in every course</span></div>
</div>

<div class="te-chart">
  <h3><i class="fas fa-chart-bar"></i> Teaching hours by course</h3>
  <div class="te-legend">
    <span><i style="background:var(--accent)"></i>Postgraduate · AIOU</span>
    <span><i style="background:var(--warm)"></i>Undergraduate · Govt. Hashmat Ali Islamia College</span>
  </div>
  <svg id="te-hours" viewBox="0 0 600 270" role="img" aria-label="Horizontal bar chart of teaching hours for each of the nine courses"></svg>
</div>

<h2 class="te-h"><i class="fas fa-building-columns"></i> Teaching experience</h2>

<div class="te-inst ug">
  <div class="head">
    <div class="ic"><i class="fas fa-school"></i></div>
    <div>
      <h3>Lecturer in Statistics · Govt. Hashmat Ali Islamia College</h3>
      <p class="sub">Department of Statistics · Higher Education Department, Govt. of Punjab · Rawalpindi, Pakistan · Feb 2018 – Nov 2019 · 202.5 hours</p>
    </div>
    <span class="lvl">Undergraduate</span>
  </div>
  <p class="summary">Delivered lectures, tutorials and workshops for bachelor's students, with a focus on applying statistical concepts in R.</p>
  <div class="te-courses">
    <div class="te-course"><h4>Statistical Theory I &amp; II <span>90 h</span></h4><p class="when">Feb 2018 – Dec 2018</p>
      <details><summary>Topics</summary><ul><li>Point and interval estimation</li><li>Unbiased estimators and their variance</li><li>Central Limit Theorem</li><li>Likelihood estimation and method of moments</li><li>Hypothesis testing, likelihood ratio tests and ANOVA</li></ul></details>
      <span class="r"><i class="fab fa-r-project"></i> Inference on real datasets in R</span></div>
    <div class="te-course"><h4>Introductory Statistics <span>45 h</span></h4><p class="when">Feb 2018 – Jun 2018</p>
      <details><summary>Topics</summary><ul><li>Definition and branches of statistics</li><li>Charts and graphical representation of data</li><li>Types of variables and data</li><li>Measures of central tendency and dispersion</li><li>Index numbers</li></ul></details>
      <span class="r"><i class="fab fa-r-project"></i> Reading statistical output in R</span></div>
    <div class="te-course"><h4>Statistics and Probability <span>45 h</span></h4><p class="when">Jan 2019 – Jun 2019</p>
      <details><summary>Topics</summary><ul><li>Definitions and laws of probability</li><li>Discrete and continuous random variables</li><li>Joint and marginal distributions</li><li>Moment generating functions</li><li>Expectation, variance, covariance and correlation</li><li>Central Limit Theorem and Law of Large Numbers</li></ul></details>
      <span class="r"><i class="fab fa-r-project"></i> Simulation and visualisation in R</span></div>
    <div class="te-course"><h4>Business Statistics <span>22.5 h</span></h4><p class="when">Sep 2019 – Nov 2019</p>
      <details><summary>Topics</summary><ul><li>Descriptive statistics for commerce students</li><li>Data visualisation</li><li>Basic inferential methods</li></ul></details>
      <span class="r"><i class="fab fa-r-project"></i> Business data analysis in R</span></div>
  </div>
  <a class="te-more" href="/teaching/2018-spring-teaching-1">Full course details <i class="fas fa-arrow-right"></i></a>
</div>

<div class="te-inst pg">
  <div class="head">
    <div class="ic"><i class="fas fa-graduation-cap"></i></div>
    <div>
      <h3>Teaching Assistant Lecturer · Allama Iqbal Open University (AIOU)</h3>
      <p class="sub">Department of Statistics · Islamabad, Pakistan · Jul 2016 – Jan 2018 · 225 hours</p>
    </div>
    <span class="lvl">Postgraduate</span>
  </div>
  <p class="summary">Taught master's-level courses through lectures, tutorials and workshops, emphasising the application of statistical methods in R.</p>
  <div class="te-courses">
    <div class="te-course"><h4>Statistical Methods <span>45 h</span></h4><p class="when">Autumn semester 2016</p>
      <details><summary>Topics</summary><ul><li>Statistical methods and branches of statistics</li><li>Types of variables and data</li><li>Measures of central tendency and dispersion</li><li>Statistical inference and hypothesis testing</li><li>Nonparametric statistics</li></ul></details>
      <span class="r"><i class="fab fa-r-project"></i> Applied sessions in R</span></div>
    <div class="te-course"><h4>Regression Analysis <span>45 h</span></h4><p class="when">Autumn semester 2016</p>
      <details><summary>Topics</summary><ul><li>Simple and multiple linear regression</li><li>Model assumptions and residual analysis</li><li>Least squares, R² and adjusted R²</li><li>t-tests, F-tests and multicollinearity</li><li>Logistic and nonlinear regression</li></ul></details>
      <span class="r"><i class="fab fa-r-project"></i> Model fitting and diagnostics in R</span></div>
    <div class="te-course"><h4>Nonparametric Statistics <span>45 h</span></h4><p class="when">Spring semester 2017</p>
      <details><summary>Topics</summary><ul><li>Distribution-free and rank-based methods</li><li>Wilcoxon, Mann–Whitney and Kruskal–Wallis tests</li><li>Kolmogorov–Smirnov and Anderson–Darling tests</li><li>Robust alternatives to parametric methods</li></ul></details>
      <span class="r"><i class="fab fa-r-project"></i> Real-data analysis in R</span></div>
    <div class="te-course"><h4>Econometrics <span>45 h</span></h4><p class="when">Spring semester 2017</p>
      <details><summary>Topics</summary><ul><li>Simple, multiple and dummy-variable regression</li><li>Multicollinearity, heteroscedasticity, autocorrelation</li><li>Model specification and diagnostic testing</li><li>Simultaneous equations and time series econometrics</li><li>Panel data and qualitative response models</li></ul></details>
      <span class="r"><i class="fab fa-r-project"></i> Applied econometrics in R</span></div>
    <div class="te-course"><h4>Research Methods <span>45 h</span></h4><p class="when">Autumn semester 2018</p>
      <details><summary>Topics</summary><ul><li>Research framework and problem formulation</li><li>Sampling design, measurement and scaling</li><li>Data collection and processing</li><li>Parametric and nonparametric testing</li><li>Report writing, presentation, Word and LaTeX</li></ul></details>
      <span class="r"><i class="fas fa-clipboard-list"></i> Student surveys and research reports</span></div>
  </div>
  <a class="te-more" href="/teaching/2016-spring-teaching-1">Full course details <i class="fas fa-arrow-right"></i></a>
</div>

<h2 class="te-h"><i class="fas fa-lightbulb"></i> How I teach</h2>
<div class="te-approach">
  <div class="te-ap"><div class="ic"><i class="fab fa-r-project"></i></div><h4>Learning by doing</h4><p>Every course pairs theory with R workshops, so students fit models and interpret output on real data.</p></div>
  <div class="te-ap"><div class="ic"><i class="fas fa-magnifying-glass-chart"></i></div><h4>Real-world problems</h4><p>Methods are motivated by applied questions in economics, business and environmental data.</p></div>
  <div class="te-ap"><div class="ic"><i class="fas fa-pen-nib"></i></div><h4>From analysis to report</h4><p>Students practise the full workflow: designing a study, analysing it and writing it up, including in LaTeX.</p></div>
</div>

</div>

<script>
(function(){
  var NS='http://www.w3.org/2000/svg',svg=document.getElementById('te-hours'); if(!svg) return;
  var data=[['Statistical Theory I & II',90,'ug'],['Statistical Methods',45,'pg'],['Regression Analysis',45,'pg'],['Nonparametric Statistics',45,'pg'],['Econometrics',45,'pg'],['Research Methods',45,'pg'],['Introductory Statistics',45,'ug'],['Statistics and Probability',45,'ug'],['Business Statistics',22.5,'ug']];
  function el(tag,a,txt){var e=document.createElementNS(NS,tag);for(var k in a)e.setAttribute(k,a[k]);if(txt!=null)e.textContent=txt;svg.appendChild(e);return e;}
  var L=160,R=560,T=6,row=28,bh=18,max=90;
  data.forEach(function(d,i){
    var y=T+i*row,w=d[1]/max*(R-L),r=Math.min(4,bh/2);
    el('text',{x:L-10,y:y+bh/2+4,'text-anchor':'end'},d[0]);
    el('path',{d:'M'+L+','+y+'H'+(L+w-r)+'Q'+(L+w)+','+y+' '+(L+w)+','+(y+r)+'V'+(y+bh-r)+'Q'+(L+w)+','+(y+bh)+' '+(L+w-r)+','+(y+bh)+'H'+L+'Z','class':d[2]});
    el('text',{x:L+w+6,y:y+bh/2+4,'class':'val'},d[1]+' h');
  });
  el('line',{x1:L,x2:L,y1:T-4,y2:T+data.length*row-6,stroke:'currentColor','stroke-opacity':.3});
})();
</script>
