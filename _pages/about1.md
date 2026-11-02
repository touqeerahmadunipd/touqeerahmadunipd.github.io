---
permalink: /
title: "Hello! I'm Touqeer Ahmad 👋"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<style>
  /* ---------- Home page styles (scoped to .hp) ---------- */
  .hp{--accent:#0f86a8;--accent-soft:rgba(15,134,168,.10);--warm:#d0683d;--warm-soft:rgba(208,104,61,.12);
      --c1:#0f86a8;--c2:#d0683d;--fig-bg:#fbfcfc;--fig-ink:var(--global-text-color);
      --card:var(--global-bg-color);--line:var(--global-border-color);--muted:color-mix(in srgb,var(--global-text-color) 78%,transparent)}
  html[data-theme="dark"] .hp{--c1:#20a0c4;--c2:#d9744a;--fig-bg:#2b2f33;--accent:#20a0c4;--accent-soft:rgba(32,160,196,.16);--warm:#d9744a;--warm-soft:rgba(217,116,74,.18)}
  .hp *{box-sizing:border-box}
  .hp p{margin:0 0 1em}
  .hp a{text-decoration:none}
  .hp-role{display:inline-flex;align-items:center;gap:.5em;font-size:.72em;font-weight:600;letter-spacing:.04em;text-transform:uppercase;color:var(--accent);background:var(--accent-soft);padding:.45em .9em;border-radius:999px;margin-bottom:1.1em}
  .hp-role .dot{width:.55em;height:.55em;border-radius:50%;background:var(--warm);box-shadow:0 0 0 .25em var(--warm-soft);animation:hp-pulse 2.4s infinite}
  @keyframes hp-pulse{50%{box-shadow:0 0 0 .45em transparent}}
  .hp-lead{font-size:1.12em;line-height:1.6}
  .hp-lead strong{color:var(--accent)}

  .hp-btns{display:flex;flex-wrap:wrap;gap:.6em;margin:1.4em 0 2em}
  .hp-btn{display:inline-flex;align-items:center;gap:.5em;font-size:.78em;font-weight:600;padding:.6em 1.1em;border-radius:999px;border:1.5px solid var(--accent);color:var(--accent)!important;transition:all .2s ease}
  .hp-btn:hover{background:var(--accent);color:#fff!important;transform:translateY(-2px);box-shadow:0 6px 16px -8px var(--accent)}
  .hp-btn.solid{background:var(--accent);color:#fff!important}

  .hp h2.hp-h{display:flex;align-items:center;gap:.55em;font-size:1.3em;margin:2.2em 0 .9em;padding-bottom:.45em;border-bottom:1px solid var(--line)}
  .hp h2.hp-h i{color:var(--accent);font-size:.85em}

  /* figures */
  .hp-fig{margin:0;border:1px solid var(--line);border-radius:14px;background:var(--fig-bg);padding:1em 1em .8em;overflow:hidden}
  .hp-fig svg{display:block;width:100%;height:auto;overflow:visible}
  .hp-fig figcaption{font-family:inherit;font-size:.74em;color:var(--muted);line-height:1.5;margin-top:.6em}
  .hp-fig figcaption b{color:var(--global-text-color)}
  .hp-legend{display:flex;flex-wrap:wrap;gap:1.1em;font-size:.72em;color:var(--muted);margin:0 0 .5em}
  .hp-legend span{display:inline-flex;align-items:center;gap:.45em}
  .hp-legend i{display:inline-block;width:.9em;height:.9em;border-radius:3px}
  .hp-legend i.ln{height:2px;border-radius:2px;width:1.4em}
  .hp-legend i.dt{border-radius:50%;width:.7em;height:.7em}
  .hp-legend i.ho{border-radius:50%;width:.7em;height:.7em;background:none!important;border:2px solid var(--c2)}
  .hp svg .ax{stroke:var(--fig-ink);stroke-opacity:.35;stroke-width:1}
  .hp svg .grid{stroke:var(--fig-ink);stroke-opacity:.08;stroke-width:1}
  .hp svg text{fill:var(--fig-ink);fill-opacity:.7;font-size:10px;font-family:inherit}
  .hp svg text.lab{fill-opacity:.9;font-weight:600}
  .hp svg .c1{fill:var(--c1)} .hp svg .c2{fill:var(--c2)}
  .hp svg .s1{stroke:var(--c1)} .hp svg .s2{stroke:var(--c2)}
  .hp svg .hit{fill:transparent}
  .hp svg .hit:hover + .mk, .hp svg .mk:hover{filter:brightness(1.15)}

  .hp-grid{display:grid;grid-template-columns:1fr 1fr;gap:1em}
  @media (max-width:760px){.hp-grid{grid-template-columns:1fr}}
  .hp-grid .hp-fig{transition:transform .2s ease, box-shadow .2s ease, border-color .2s ease}
  .hp-grid .hp-fig:hover{transform:translateY(-3px);border-color:var(--accent);box-shadow:0 10px 24px -14px rgba(0,0,0,.35)}
  .hp-fig h3{font-size:.92em;margin:0 0 .25em;display:flex;align-items:center;gap:.5em}
  .hp-fig h3 i{color:var(--accent);font-size:.9em}
  .hp-fig .sub{font-size:.76em;color:var(--muted);margin:0 0 .6em;line-height:1.45}

  #hp-tip{position:fixed;pointer-events:none;z-index:9999;background:#1d2327;color:#fff;font-size:12px;line-height:1.35;padding:.4em .65em;border-radius:6px;opacity:0;transition:opacity .12s;white-space:nowrap}

  .hp-news{list-style:none;margin:0;padding:0;position:relative}
  .hp-news::before{content:"";position:absolute;left:.42em;top:.6em;bottom:.6em;width:2px;background:var(--line)}
  .hp-news li{position:relative;padding:0 0 1.05em 2em;font-size:.88em;line-height:1.55;margin:0}
  .hp-news li::before{content:"";position:absolute;left:0;top:.42em;width:.95em;height:.95em;border-radius:50%;background:var(--global-bg-color);border:2.5px solid var(--accent)}
  .hp-news li:first-child::before{background:var(--warm);border-color:var(--warm)}
  .hp-tag{display:inline-block;font-size:.72em;font-weight:700;letter-spacing:.04em;text-transform:uppercase;padding:.2em .6em;border-radius:6px;margin-right:.5em;vertical-align:.1em}
  .t-pub{background:var(--accent-soft);color:var(--accent)}
  .t-acc{background:rgba(63,154,63,.14);color:#3f9a3f}
  .t-sw{background:rgba(124,92,196,.14);color:#7c5cc4}
  .hp-news a.go{font-weight:600;color:var(--accent);white-space:nowrap}
  .hp-news a.go:hover{text-decoration:underline}
  .hp-all{display:inline-flex;align-items:center;gap:.4em;font-size:.8em;font-weight:600;color:var(--accent)!important;margin-top:.2em}
  .hp-all:hover{text-decoration:underline}

  .hp-events{display:grid;gap:.8em}
  .hp-event{display:grid;grid-template-columns:4.6em 1fr;gap:1em;align-items:center;border:1px solid var(--line);border-radius:12px;padding:.9em 1em;background:var(--card);transition:border-color .2s ease}
  .hp-event:hover{border-color:var(--accent)}
  .hp-date{text-align:center;border-radius:10px;background:var(--accent);color:#fff;padding:.45em .2em;line-height:1.15}
  .hp-date b{display:block;font-size:1.25em}
  .hp-date span{font-size:.66em;text-transform:uppercase;letter-spacing:.05em}
  .hp-event:nth-child(even) .hp-date{background:var(--warm)}
  .hp-event h3{font-size:.88em;margin:0 0 .2em;line-height:1.35}
  .hp-event p{font-size:.76em;color:var(--muted);margin:0}
  .hp-event a{font-weight:600;color:var(--accent)}

  .hp-contact{margin-top:2.4em;border-radius:16px;padding:1.6em 1.6em 1.3em;background:linear-gradient(135deg,#0f86a8,#145a6c);color:#fff}
  .hp-contact h2{color:#fff;border:0;margin:0 0 .4em;font-size:1.3em}
  .hp-contact p{color:rgba(255,255,255,.88);font-size:.88em}
  .hp-mails{display:flex;flex-wrap:wrap;gap:.6em;margin:.4em 0 1em}
  .hp-mail{display:inline-flex;align-items:center;gap:.5em;background:rgba(255,255,255,.14);border:1px solid rgba(255,255,255,.25);color:#fff!important;padding:.5em .9em;border-radius:999px;font-size:.8em;font-weight:600;transition:background .2s}
  .hp-mail:hover{background:rgba(255,255,255,.26)}
  .hp-contact details{font-size:.74em;color:rgba(255,255,255,.78)}
  .hp-contact summary{cursor:pointer}
  .hp-contact details p{margin:.4em 0 0;font-size:1em;color:rgba(255,255,255,.72)}

  .hp-reveal{opacity:0;transform:translateY(12px);transition:opacity .6s ease, transform .6s ease}
  .hp-reveal.in{opacity:1;transform:none}
  .hp-draw{stroke-dasharray:2000;stroke-dashoffset:2000}
  .in .hp-draw, .hp-draw.in{transition:stroke-dashoffset 2.2s ease-out;stroke-dashoffset:0}
  @media (prefers-reduced-motion:reduce){.hp-reveal{opacity:1;transform:none}.hp-role .dot{animation:none}.hp-draw{stroke-dashoffset:0}}
</style>

<div class="hp">

<div class="hp-role"><span class="dot"></span>DSTrain – MSCA Research Fellow · University of Oslo</div>

<p class="hp-lead">I am a Marie Skłodowska-Curie Research Fellow in the Department of Mathematics at the <strong>University of Oslo</strong>, Norway. I develop statistical models for <strong>rare and extreme events</strong>, and my current research focuses on the stochastic modelling of natural processes.</p>

<p>Previously, I was a Postdoctoral Research Fellow at the Institut Denis Poisson, University of Orléans, France (May–October 2025), where I worked on missing data in high-dimensional environmental datasets. Before that, I held a postdoctoral position at ENSAI, France, focusing on dimension reduction and imbalanced data classification. I earned my PhD in Statistical Sciences, with a Doctor Europaeus title, from the University of Padova, Italy, with a thesis <em>On the modeling of discrete extreme values</em>.</p>

<div class="hp-btns">
  <a class="hp-btn solid" href="/files/Touqeer_CV.pdf"><i class="fas fa-file-arrow-down"></i> Download CV</a>
  <a class="hp-btn" href="https://scholar.google.com/citations?user=0Unv8IAAAAAJ&hl=en" target="_blank" rel="noopener noreferrer"><i class="fas fa-graduation-cap"></i> Google Scholar</a>
  <a class="hp-btn" href="https://github.com/touqeerahmadunipd" target="_blank" rel="noopener noreferrer"><i class="fab fa-github"></i> GitHub</a>
</div>

<figure class="hp-fig hp-reveal">
  <h3><i class="fas fa-chart-column"></i> Modelling the whole distribution, tail included</h3>
  <div class="hp-legend">
    <span><i style="background:var(--c1)"></i>Observed counts</span>
    <span><i style="background:var(--c2)"></i>Above threshold <em>u</em></span>
    <span><i class="ln" style="background:var(--global-text-color)"></i>Fitted discrete extended GPD</span>
  </div>
  <svg id="hp-fig-main" viewBox="0 0 640 230" role="img" aria-label="Histogram of zero-inflated count data with a heavy right tail and a fitted discrete extended generalized Pareto curve"></svg>
  <figcaption><b>Illustration.</b> Count data with many zeros and a heavy tail, such as avalanche or precipitation counts. The discrete extended generalized Pareto model fits the bulk and the extremes together, with no need to pick a threshold.</figcaption>
</figure>

<h2 class="hp-h hp-reveal"><i class="fas fa-compass"></i> Research interests</h2>

<p class="hp-reveal">My work lies at the intersection of stochastic processes, statistical modelling and machine learning. I am particularly interested in:</p>

<div class="hp-grid hp-reveal">
  <figure class="hp-fig">
    <h3><i class="fas fa-wave-square"></i> Spatio-temporal extremes</h3>
    <p class="sub">Modelling and analysis of spatiotemporal dependence in extreme events.</p>
    <svg id="hp-fig-ts" viewBox="0 0 300 160" role="img" aria-label="Daily time series with a high threshold and the exceedances highlighted"></svg>
    <figcaption>Peaks over a high threshold <em>u</em> in a daily series.</figcaption>
  </figure>
  <figure class="hp-fig">
    <h3><i class="fas fa-mountain-sun"></i> Natural &amp; environmental systems</h3>
    <p class="sub">Stochastic modelling of complex natural and environmental systems.</p>
    <svg id="hp-fig-rl" viewBox="0 0 300 160" role="img" aria-label="Return level plot with fitted curve, confidence band and empirical points"></svg>
    <figcaption>Return levels with a 95% band: how big is the 100-year event?</figcaption>
  </figure>
  <figure class="hp-fig">
    <h3><i class="fas fa-diagram-project"></i> Statistical learning</h3>
    <p class="sub">Methods for high-dimensional, imbalanced or incomplete datasets.</p>
    <div class="hp-legend">
      <span><i class="dt" style="background:var(--c1)"></i>Majority</span>
      <span><i class="dt" style="background:var(--c2)"></i>Minority</span>
      <span><i class="ho"></i>Synthetic</span>
    </div>
    <svg id="hp-fig-cl" viewBox="0 0 300 150" role="img" aria-label="Imbalanced two-class scatter plot with synthetic minority points and a decision boundary"></svg>
    <figcaption>Imbalanced classification with synthetic oversampling.</figcaption>
  </figure>
  <figure class="hp-fig">
    <h3><i class="fas fa-earth-europe"></i> Climate applications</h3>
    <p class="sub">Dimension reduction and data-driven approaches in environmental and climate research.</p>
    <svg id="hp-fig-map" viewBox="0 0 300 166" role="img" aria-label="Gridded map of estimated 100-year return levels on a single-hue colour scale"></svg>
    <figcaption>Gridded map of estimated 100-year return levels.</figcaption>
  </figure>
</div>

<h2 class="hp-h hp-reveal"><i class="fas fa-bullhorn"></i> Latest news</h2>

<ul class="hp-news hp-reveal">
  <li><span class="hp-tag t-pub">Published</span>Order-of-addition in mixture and component-amount designs in orthogonal blocks, in <strong>Journal of Biopharmaceutical Statistics</strong>. <a class="go" href="https://doi.org/10.1080/10543406.2026.2680927" target="_blank" rel="noopener noreferrer">Read →</a></li>
  <li><span class="hp-tag t-pub">Published</span>Regional modeling of zero-inflated precipitation in Pakistan by classical and Bayesian approaches, in <strong>Journal of Hydrology: Regional Studies</strong>. <a class="go" href="https://doi.org/10.1016/j.ejrh.2026.103330" target="_blank" rel="noopener noreferrer">Read →</a></li>
  <li><span class="hp-tag t-sw">Software</span>Released the new R package <strong>egpd</strong>, jointly with <a href="https://www.lshtm.ac.uk/aboutus/people/frost.simon" target="_blank" rel="noopener noreferrer">Simon Frost</a>. <a class="go" href="https://github.com/sdwfrost/egpd" target="_blank" rel="noopener noreferrer">View →</a></li>
  <li><span class="hp-tag t-acc">Accepted</span>New flexible versions of the extended generalized Pareto distribution for count data, in <strong>Journal of Applied Statistics</strong>.</li>
</ul>

<a class="hp-all hp-reveal" href="/publications/">See all publications <i class="fas fa-arrow-right"></i></a>

<h2 class="hp-h hp-reveal"><i class="fas fa-calendar-days"></i> Conferences 2026</h2>

<div class="hp-events hp-reveal">
  <div class="hp-event">
    <div class="hp-date"><b>28</b><span>Jun 2026</span></div>
    <div><h3>40th International Workshop on Statistical Modelling (IWSM)</h3><p>28 June – 2 July 2026 · University of Oslo, Norway · <a href="https://www.mn.uio.no/math/english/research/groups/statistics-data-science/events/conferences/iwsm2026/" target="_blank" rel="noopener noreferrer">More info</a></p></div>
  </div>
  <div class="hp-event">
    <div class="hp-date"><b>21</b><span>Jul 2026</span></div>
    <div><h3>7th Int. Conference on Advances in Extreme Value Analysis and Application to Natural Hazards (EVAN)</h3><p>21 – 23 July 2026 · Delft University of Technology, Netherlands · <a href="https://evan2026.weebly.com/" target="_blank" rel="noopener noreferrer">More info</a></p></div>
  </div>
</div>

<div class="hp-contact hp-reveal">
  <h2><i class="fas fa-envelope-open-text"></i> Get in touch</h2>
  <p>Interested in extremes, environmental data or a collaboration? Feel free to email me.</p>
  <div class="hp-mails">
    <a class="hp-mail" href="mailto:touqeera@math.uio.no"><i class="fas fa-building-columns"></i> touqeera [at] math.uio.no</a>
    <a class="hp-mail" href="mailto:touqeer.ahmad8960@gmail.com"><i class="fas fa-envelope"></i> touqeer.ahmad8960 [at] gmail.com</a>
  </div>
  <details>
    <summary>Old addresses (no longer in use)</summary>
    <p>touqeer.ahmad [at] univ-orleans.fr · touqeer.ahmad [at] ensai.fr · touqeer.ahmad [at] phd.unipd.it</p>
  </details>
</div>

</div>

<div id="hp-tip"></div>

<script>
(function(){
  var NS='http://www.w3.org/2000/svg';
  function rng(seed){return function(){seed|=0;seed=seed+0x6D2B79F5|0;var t=Math.imul(seed^seed>>>15,1|seed);t=t+Math.imul(t^t>>>7,61|t)^t;return((t^t>>>14)>>>0)/4294967296;};}
  function gauss(r){var u=1-r(),v=r();return Math.sqrt(-2*Math.log(u))*Math.cos(2*Math.PI*v);}
  function el(svg,tag,a,txt){var e=document.createElementNS(NS,tag);for(var k in a)e.setAttribute(k,a[k]);if(txt!=null)e.textContent=txt;svg.appendChild(e);return e;}
  var tip=document.getElementById('hp-tip');
  function hover(node,text){
    node.style.cursor='default';
    node.addEventListener('mousemove',function(ev){tip.textContent=text;tip.style.opacity=1;tip.style.left=(ev.clientX+12)+'px';tip.style.top=(ev.clientY-30)+'px';});
    node.addEventListener('mouseleave',function(){tip.style.opacity=0;});
  }
  function fmt(x,d){return x.toFixed(d==null?1:d);}

  /* ---------- Main: zero-inflated discrete EGPD ---------- */
  (function(){
    var svg=document.getElementById('hp-fig-main'); if(!svg) return;
    var W=640,H=230,L=44,R=628,T=10,B=196, n=31, u=12;
    var xi=.32,sigma=2.6,kappa=1.5,pi0=.18;
    function F(x){return x<=0?0:Math.pow(1-Math.pow(1+xi*x/sigma,-1/xi),kappa);}
    var r=rng(7), model=[], obs=[];
    for(var k=0;k<n;k++){var p=(1-pi0)*(F(k+1)-F(k))+(k===0?pi0:0);model.push(p);obs.push(Math.max(0,p*(1+.16*gauss(r))));}
    var lo=Math.log10(.0004),hi=Math.log10(.4), bw=(R-L)/n, y=function(v){var l=Math.log10(Math.max(v,.0004));return B-(Math.min(l,hi)-lo)/(hi-lo)*(B-T);};
    [[.001,'0.001'],[.01,'0.01'],[.1,'0.1']].forEach(function(t){el(svg,'line',{x1:L,x2:R,y1:y(t[0]),y2:y(t[0]),class:'grid'});el(svg,'text',{x:L-8,y:y(t[0])+3,'text-anchor':'end'},t[1]);});
    el(svg,'line',{x1:L,x2:R,y1:B,y2:B,class:'ax'});
    obs.forEach(function(v,k){
      var x=L+k*bw+1, w=bw-2, h=Math.max(B-y(v),1.5), top=B-h, rr=Math.min(4,w/2,h);
      var d='M'+x+','+B+'V'+(top+rr)+'Q'+x+','+top+' '+(x+rr)+','+top+'H'+(x+w-rr)+'Q'+(x+w)+','+top+' '+(x+w)+','+(top+rr)+'V'+B+'Z';
      var bar=el(svg,'path',{d:d,class:'mk '+(k>=u?'c2':'c1')});
      var hit=el(svg,'rect',{x:L+k*bw,y:T,width:bw,height:B-T,class:'hit'});
      hover(hit,'count '+k+' · observed '+fmt(obs[k]*100)+'% · model '+fmt(model[k]*100)+'%');
      if(k%5===0) el(svg,'text',{x:L+k*bw+bw/2,y:B+14,'text-anchor':'middle'},k);
    });
    var d=''; model.forEach(function(v,k){d+=(k?'L':'M')+(L+k*bw+bw/2).toFixed(1)+','+y(v).toFixed(1);});
    el(svg,'path',{d:d,fill:'none',stroke:'currentColor',style:'color:var(--global-text-color)','stroke-width':2,'stroke-linejoin':'round',class:'hp-draw'});
    var ux=L+u*bw; el(svg,'line',{x1:ux,x2:ux,y1:T+4,y2:B,class:'s2','stroke-width':1.5,'stroke-dasharray':'4 4'});
    el(svg,'text',{x:ux+6,y:T+12,class:'lab'},'threshold u');
    el(svg,'text',{x:L+bw+6,y:y(model[0])+4,class:'lab'},'← excess zeros');el(svg,'text',{x:R-4,y:y(model[24])-14,'text-anchor':'end',class:'lab'},'heavy tail: rare, large counts');
    el(svg,'text',{x:(L+R)/2,y:H-4,'text-anchor':'middle'},'count');
    el(svg,'text',{x:12,y:(T+B)/2,'text-anchor':'middle',transform:'rotate(-90 12 '+(T+B)/2+')'},'proportion (log scale)');
  })();

  /* ---------- Time series with exceedances ---------- */
  (function(){
    var svg=document.getElementById('hp-fig-ts'); if(!svg) return;
    var L=30,R=294,T=8,B=134,n=150,r=rng(11),v=[],prev=0;
    for(var i=0;i<n;i++){var s=1+.5*Math.sin(i/n*2*Math.PI*1.5);var z=Math.pow(1-r(),-.28)-1;prev=.45*prev+z*s;v.push(prev);}
    var srt=v.slice().sort(function(a,b){return a-b}),u=srt[Math.floor(.92*n)],vmax=srt[n-1]*1.08;
    var x=function(i){return L+i/(n-1)*(R-L)},y=function(t){return B-t/vmax*(B-T)};
    el(svg,'line',{x1:L,x2:R,y1:B,y2:B,class:'ax'});
    var d='';v.forEach(function(t,i){d+=(i?'L':'M')+x(i).toFixed(1)+','+y(t).toFixed(1);});
    el(svg,'path',{d:d,fill:'none',class:'s1 hp-draw','stroke-width':1.5,'stroke-linejoin':'round'});
    el(svg,'line',{x1:L,x2:R,y1:y(u),y2:y(u),class:'s2','stroke-width':1.5,'stroke-dasharray':'4 4'});
    el(svg,'text',{x:L+2,y:y(u)-5,class:'lab'},'u');
    v.forEach(function(t,i){if(t>u){var c=el(svg,'circle',{cx:x(i),cy:y(t),r:4,class:'c2 mk',stroke:'var(--fig-bg)','stroke-width':2});hover(c,'day '+(i+1)+' · value '+fmt(t)+' · excess '+fmt(t-u));}});
    el(svg,'text',{x:(L+R)/2,y:152,'text-anchor':'middle'},'time (days)');
    el(svg,'text',{x:R,y:T+4,'text-anchor':'end',class:'lab'},'exceedances');
  })();

  /* ---------- Return level plot ---------- */
  (function(){
    var svg=document.getElementById('hp-fig-rl'); if(!svg) return;
    var L=34,R=294,T=8,B=134, mu=30,sg=8,xi=.12;
    function z(Tp){var yp=-Math.log(1-1/Tp);return mu+sg/xi*(Math.pow(yp,-xi)-1);}
    var lx=function(Tp){return L+(Math.log10(Tp)-Math.log10(1.2))/(3-Math.log10(1.2))*(R-L)};
    var ymin=20,ymax=z(1000)*1.18, y=function(t){return B-(t-ymin)/(ymax-ymin)*(B-T)};
    [1,10,100,1000].forEach(function(t){var xx=lx(Math.max(t,1.2));el(svg,'line',{x1:xx,x2:xx,y1:T,y2:B,class:'grid'});el(svg,'text',{x:xx,y:B+13,'text-anchor':'middle'},t);});
    el(svg,'line',{x1:L,x2:R,y1:B,y2:B,class:'ax'});
    [40,60,80,100].forEach(function(t){if(t<ymax){el(svg,'text',{x:L-6,y:y(t)+3,'text-anchor':'end'},t);}});
    var up='',lo='',mid='',pts=[];
    for(var i=0;i<=60;i++){var Tp=Math.pow(10,Math.log10(1.2)+i/60*(3-Math.log10(1.2))),w=1.2+.0045*Math.pow(Math.log10(Tp)+.2,2.6)*40;pts.push([Tp,z(Tp),w]);}
    pts.forEach(function(p,i){up+=(i?'L':'M')+lx(p[0]).toFixed(1)+','+y(p[1]+p[2]).toFixed(1);mid+=(i?'L':'M')+lx(p[0]).toFixed(1)+','+y(p[1]).toFixed(1);});
    pts.slice().reverse().forEach(function(p){lo+='L'+lx(p[0]).toFixed(1)+','+y(p[1]-p[2]).toFixed(1);});
    el(svg,'path',{d:up+lo+'Z',class:'c1','fill-opacity':.16});
    el(svg,'path',{d:mid,fill:'none',class:'s1 hp-draw','stroke-width':2});
    var r=rng(3),m=40;
    for(var k=0;k<m;k++){var Tp=1/(1-(k+1-.44)/(m+.12)),g=z(Tp)+(1.5+.06*z(Tp))*gauss(r)*.6;if(Tp>=1.2){var c=el(svg,'circle',{cx:lx(Tp),cy:y(g),r:3.5,class:'c2 mk',stroke:'var(--fig-bg)','stroke-width':1.5});hover(c,'observed annual maximum · T ≈ '+fmt(Tp,0)+' yr · '+fmt(g));}}
    var z100=z(100), c=el(svg,'circle',{cx:lx(100),cy:y(z100),r:4.5,fill:'var(--fig-bg)',class:'s1','stroke-width':2.5});
    hover(c,'100-year return level ≈ '+fmt(z100));
    el(svg,'text',{x:lx(100)-6,y:y(z100)-9,'text-anchor':'end',class:'lab'},'100-yr level');
    el(svg,'text',{x:(L+R)/2,y:157,'text-anchor':'middle'},'return period (years, log scale)');
  })();

  /* ---------- Imbalanced classification ---------- */
  (function(){
    var svg=document.getElementById('hp-fig-cl'); if(!svg) return;
    var L=8,R=292,T=6,B=144,r=rng(21);
    var x=function(a){return L+a*(R-L)},y=function(b){return B-b*(B-T)};
    el(svg,'path',{d:'M'+x(.47)+','+y(1)+' Q'+x(.6)+','+y(.55)+' '+x(1)+','+y(.38),fill:'none',stroke:'var(--fig-ink)','stroke-opacity':.45,'stroke-width':1.5,'stroke-dasharray':'5 4'});
    el(svg,'text',{x:x(.99),y:y(.38)+14,'text-anchor':'end',class:'lab'},'decision boundary');
    for(var i=0;i<70;i++){var a=.3+.14*gauss(r),b=.4+.17*gauss(r);a=Math.min(.97,Math.max(.03,a));b=Math.min(.96,Math.max(.04,b));
      var c=el(svg,'circle',{cx:x(a),cy:y(b),r:3.5,class:'c1 mk','fill-opacity':.85,stroke:'var(--fig-bg)','stroke-width':1.5});hover(c,'majority class');}
    var mins=[];for(var j=0;j<10;j++){mins.push([.78+.09*gauss(r),.66+.12*gauss(r)]);}
    for(var s=0;s<14;s++){var p=mins[Math.floor(r()*10)],q=mins[Math.floor(r()*10)],t=r();var a2=p[0]+t*(q[0]-p[0]),b2=p[1]+t*(q[1]-p[1]);
      var h=el(svg,'circle',{cx:x(a2),cy:y(b2),r:3.5,fill:'none',class:'s2 mk','stroke-width':2});hover(h,'synthetic minority point');}
    mins.forEach(function(p){var c=el(svg,'circle',{cx:x(p[0]),cy:y(p[1]),r:4.5,class:'c2 mk',stroke:'var(--fig-bg)','stroke-width':1.5});hover(c,'minority class (rare)');});
  })();

  /* ---------- Gridded return-level map ---------- */
  (function(){
    var svg=document.getElementById('hp-fig-map'); if(!svg) return;
    var cols=16,rows=8,L=4,T=4,cw=16.5,ch=14,g=2,r=rng(5),vals=[],mn=1e9,mx=-1e9;
    for(var i=0;i<rows;i++)for(var j=0;j<cols;j++){
      var v=55+22*Math.exp(-(Math.pow((j-11)/4.2,2)+Math.pow((i-2)/2.6,2)))+12*Math.exp(-(Math.pow((j-3)/3,2)+Math.pow((i-6)/2.5,2)))-.8*i+4*gauss(r);
      vals.push([i,j,v]);mn=Math.min(mn,v);mx=Math.max(mx,v);}
    vals.forEach(function(c){var t=(c[2]-mn)/(mx-mn);
      var rect=el(svg,'rect',{x:L+c[1]*(cw+g),y:T+c[0]*(ch+g),width:cw,height:ch,rx:3,class:'c1 mk','fill-opacity':(.1+.9*t).toFixed(2)});
      hover(rect,'cell ('+(c[0]+1)+','+(c[1]+1)+') · 100-yr level '+fmt(c[2])+' mm');});
    var y0=T+rows*(ch+g)+8, w=110, x0=L;
    var defs=el(svg,'defs',{}),lg=document.createElementNS(NS,'linearGradient');lg.setAttribute('id','hp-seq');defs.appendChild(lg);
    [['0%',.1],['100%',1]].forEach(function(s){var st=document.createElementNS(NS,'stop');st.setAttribute('offset',s[0]);st.setAttribute('stop-color','var(--c1)');st.setAttribute('style','stop-color:var(--c1)');st.setAttribute('stop-opacity',s[1]);lg.appendChild(st);});
    el(svg,'rect',{x:x0,y:y0,width:w,height:8,rx:3,fill:'url(#hp-seq)'});
    el(svg,'text',{x:x0,y:y0+21},fmt(mn,0)+' mm');
    el(svg,'text',{x:x0+w,y:y0+21,'text-anchor':'end'},fmt(mx,0)+' mm');
    el(svg,'text',{x:x0+w+10,y:y0+8,class:'lab'},'100-year return level');
  })();

  /* ---------- Reveal on scroll ---------- */
  var els=document.querySelectorAll('.hp-reveal');
  if(!('IntersectionObserver' in window)){els.forEach(function(e){e.classList.add('in')});return;}
  var io=new IntersectionObserver(function(es){es.forEach(function(e){if(e.isIntersecting){e.target.classList.add('in');io.unobserve(e.target);}})},{threshold:.1});
  els.forEach(function(e){io.observe(e)});
})();
</script>
