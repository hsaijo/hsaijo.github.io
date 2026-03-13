---
layout: null
---

<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Hikaru Saijo</title>
  <meta name="description" content="Hikaru Saijo is an Associate Professor of Economics at UC Santa Cruz, working on behavioral macroeconomics, diagnostic expectations, and deep learning methods for macro models.">
 
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Instrument+Serif:ital@0;1&family=Karla:wght@300;400;500;600&display=swap" rel="stylesheet">
 
  <style>
    :root {
      --bg: #fafafa;
      --text: #2a2a2a;
      --text-2: #606060;
      --text-3: #9a9a9a;
      --accent: #0e7c6b;
      --rule: #e8e8e8;
      --rule-light: #f0f0f0;
      --serif: 'Instrument Serif', Georgia, serif;
      --sans: 'Karla', system-ui, sans-serif;
      --measure: 680px;
    }
 
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
 
    html {
      font-size: 16.5px;
      -webkit-font-smoothing: antialiased;
      scroll-behavior: smooth;
    }
 
    body {
      font-family: var(--sans);
      color: var(--text);
      background: var(--bg);
      line-height: 1.6;
    }
 
    ::selection { background: var(--accent); color: #fff; }
 
    a { color: var(--text); text-decoration: none; }
 
    /* ─── Layout ─── */
    .container {
      max-width: var(--measure);
      margin: 0 auto;
      padding: 0 1.5rem;
    }
 
    /* ─── Nav ─── */
    nav {
      position: sticky;
      top: 0;
      z-index: 10;
      background: rgba(250,250,250,0.92);
      backdrop-filter: blur(12px);
      -webkit-backdrop-filter: blur(12px);
      border-bottom: 1px solid var(--rule);
    }
 
    .nav-inner {
      max-width: var(--measure);
      margin: 0 auto;
      padding: 0.8rem 1.5rem;
      display: flex;
      justify-content: space-between;
      align-items: baseline;
    }
 
    .nav-name {
      font-family: var(--serif);
      font-size: 1.1rem;
      color: var(--text);
    }
 
    .nav-links {
      list-style: none;
      display: flex;
      gap: 1.5rem;
    }
 
    .nav-links a {
      font-size: 0.78rem;
      font-weight: 500;
      color: var(--text-3);
      letter-spacing: 0.06em;
      text-transform: uppercase;
      transition: color 0.15s;
    }
 
    .nav-links a:hover { color: var(--text); }
 
    /* ─── Hero ─── */
    .hero {
      padding: 5rem 0 3rem;
      display: grid;
      grid-template-columns: 120px 1fr;
      gap: 2rem;
      align-items: start;
    }
 
    .hero-photo {
      width: 120px;
      height: 120px;
      border-radius: 50%;
      object-fit: cover;
      filter: none;
      border: 2px solid var(--rule);
    }
 
    .hero-text h1 {
      font-family: var(--serif);
      font-weight: 400;
      font-size: 2.4rem;
      line-height: 1.1;
      letter-spacing: -0.02em;
    }
 
    .hero-sub {
      font-size: 0.88rem;
      color: var(--accent);
      margin-top: 0.3rem;
    }
 
    .hero-sub a { color: var(--accent); border-bottom: 1px solid transparent; }
    .hero-sub a:hover { border-color: var(--accent); }
 
    .pronunciation {
      font-size: 0.78rem;
      color: var(--text-3);
      font-style: italic;
      margin-top: 0.15rem;
    }
 
    .hero-bio {
      margin-top: 1.25rem;
      font-size: 0.92rem;
      color: var(--text-2);
      line-height: 1.7;
      max-width: 540px;
    }
 
    .hero-bio p + p { margin-top: 0.75rem; }
 
    .hero-links {
      margin-top: 1.25rem;
      display: flex;
      gap: 1.25rem;
      flex-wrap: wrap;
      align-items: center;
    }
 
    .hero-links span:not(.sep) {
      font-size: 0.8rem;
      font-weight: 500;
      color: var(--accent);
    }
 
    .hero-links .sep {
      color: var(--rule);
      user-select: none;
    }
 
    /* ─── Sections ─── */
    section {
      padding: 3rem 0;
      border-top: 1px solid var(--rule);
    }
 
    .section-label {
      font-size: 0.72rem;
      font-weight: 600;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      color: var(--text-3);
      margin-bottom: 2rem;
    }
 
    /* ─── Interests ─── */
    .interests {
      display: flex;
      flex-wrap: wrap;
      gap: 0.5rem;
    }
 
    .interest {
      font-size: 0.8rem;
      font-weight: 500;
      color: var(--text-2);
      padding: 0.3rem 0.7rem;
      border: 1px solid var(--rule);
      border-radius: 3px;
    }
 
    /* ─── Papers ─── */
    .paper {
      margin-bottom: 2rem;
    }
 
    .paper:last-child { margin-bottom: 0; }
 
    .paper-title {
      font-family: var(--serif);
      font-size: 1.12rem;
      font-weight: 400;
      line-height: 1.35;
    }
 
    .paper-title a { transition: color 0.15s; }
    .paper-title a:hover { color: var(--accent); }
 
    .paper-meta {
      font-size: 0.82rem;
      color: var(--text-2);
      margin-top: 0.2rem;
      line-height: 1.5;
    }
 
    .paper-meta a { color: var(--text-2); }
    .paper-meta a:hover { color: var(--accent); }
 
    .paper-journal {
      font-weight: 600;
      color: var(--text);
    }
 
    .paper-status {
      color: var(--accent);
      font-weight: 600;
    }
 
    .paper-abstract {
      font-size: 0.86rem;
      color: var(--text-2);
      margin-top: 0.5rem;
      line-height: 1.65;
    }
 
    .paper-files {
      margin-top: 0.4rem;
      display: flex;
      gap: 0.75rem;
    }
 
    .paper-files a {
      font-size: 0.75rem;
      font-weight: 600;
      color: var(--accent);
      letter-spacing: 0.03em;
      text-transform: uppercase;
      transition: opacity 0.15s;
    }
 
    .paper-files a:hover { opacity: 0.7; }
 
    /* ─── Discussions ─── */
    .disc {
      margin-bottom: 1rem;
      font-size: 0.88rem;
      line-height: 1.55;
    }
 
    .disc:last-child { margin-bottom: 0; }
 
    .disc a { font-weight: 500; transition: color 0.15s; }
    .disc a:hover { color: var(--accent); }
 
    .disc-venue {
      display: block;
      font-size: 0.78rem;
      color: var(--text-3);
      margin-top: 0.1rem;
    }
 
    /* ─── Footer ─── */
    footer {
      border-top: 1px solid var(--rule);
      padding: 2rem 0 4rem;
    }
 
    .footer-inner {
      max-width: var(--measure);
      margin: 0 auto;
      padding: 0 1.5rem;
      font-size: 0.75rem;
      color: var(--text-3);
    }
 
    /* ─── Mobile ─── */
    @media (max-width: 600px) {
      .hero {
        grid-template-columns: 1fr;
        padding: 3rem 0 2rem;
      }
 
      .hero-photo {
        width: 96px;
        height: 96px;
      }
 
      .hero-text h1 { font-size: 1.8rem; }
 
      .nav-links { gap: 1rem; }
      .nav-links a { font-size: 0.7rem; }
    }
  </style>
</head>
<body>
 
  <nav>
    <div class="nav-inner">
      <span class="nav-name">Hikaru Saijo</span>
      <ul class="nav-links">
        <li><a href="#research">Research</a></li>
        <li><a href="#papers">Working Papers</a></li>
        <li><a href="#discussions">Discussions</a></li>
        <li><a href="http://hsaijo.github.io/files/CV_saijo.pdf">CV</a></li>
      </ul>
    </div>
  </nav>
 
  <div class="container">
 
    <div class="hero">
      <img src="https://hsaijo.github.io/assets/img/hsaijo.jpg" alt="Hikaru Saijo" class="hero-photo">
      <div class="hero-text">
        <h1>Hikaru Saijo</h1>
        <p class="hero-sub">Associate Professor of Economics · <a href="https://economics.ucsc.edu/">UC Santa Cruz</a></p>
        <p class="pronunciation">He-Ka-Ru Sigh-Joe</p>
 
        <div class="hero-bio">
          <p>I study how beliefs, uncertainty, and nonlinearities shape macroeconomic fluctuations. My research combines theoretical insights with econometrics and computational tools, drawing on macro, micro, and survey data.</p>
          <p>Current work spans diagnostic expectations in general equilibrium, volatility propagation through production networks, and deep learning methods for solving high-dimensional macro models.</p>
        </div>
 
        <div class="hero-links">
          <span id="e1"></span>
          <span class="sep">·</span>
          <span id="e2"></span>
        </div>
      </div>
    </div>
 
    <script>
      document.getElementById('e1').textContent='hsaijo'+'@'+'ucsc.edu';
      document.getElementById('e2').textContent='hikaru.saijo'+'@'+'gmail.com';
    </script>

    <!-- Interests -->
    <section>
      <div class="section-label">Research Interests</div>
      <div class="interests">
        <span class="interest">Behavioral Macroeconomics</span>
        <span class="interest">Deep Learning for Macro Models</span>
        <span class="interest">Diagnostic Expectations</span>
        <span class="interest">Production Networks</span>
        <span class="interest">Uncertainty & Business Cycles</span>
        <span class="interest">Structural Estimation</span>
      </div>
    </section>

    <!-- Publications -->
    <section id="research">
      <div class="section-label">Publications</div>

      <div class="paper">
        <div class="paper-title"><a href="http://hsaijo.github.io/files/BIS.pdf">Diagnostic Business Cycles</a></div>
        <div class="paper-meta">
          with <a href="https://sites.google.com/view/francescobianchi/home">Francesco Bianchi</a> &amp; <a href="https://sites.google.com/site/cosminilut/">Cosmin Ilut</a><br>
          <span class="paper-journal">Review of Economic Studies</span>, 2024
        </div>
        <p class="paper-abstract">We develop theoretical and methodological framework to apply diagnostic expectations to a large class of recursive macro models, with a focus on implications of memory recall based on distant past.</p>
        <div class="paper-files">
          <a href="http://hsaijo.github.io/files/BIS.pdf">Paper</a>
          <a href="http://hsaijo.github.io/files/BIS_appendix.pdf">Appendix</a>
        </div>
      </div>

      <div class="paper">
        <div class="paper-title"><a href="http://hsaijo.github.io/files/ilut_saijo.pdf">Learning, Confidence, and Business Cycles</a></div>
        <div class="paper-meta">
          with <a href="https://sites.google.com/site/cosminilut/">Cosmin Ilut</a><br>
          <span class="paper-journal">Journal of Monetary Economics</span>, 2021
        </div>
        <p class="paper-abstract">We propose a new propagation mechanism based on firm-level confidence dynamics that challenges and improves upon standard New Keynesian frictions.</p>
        <div class="paper-files">
          <a href="http://hsaijo.github.io/files/ilut_saijo.pdf">Paper</a>
          <a href="http://hsaijo.github.io/files/ilut_saijo_appendix.pdf">Appendix</a>
        </div>
      </div>

      <div class="paper">
        <div class="paper-title"><a href="http://hsaijo.github.io/files/policy_uncertainty.pdf">Redistribution and Fiscal Uncertainty Shocks</a></div>
        <div class="paper-meta">
          <span class="paper-journal">International Economic Review</span>, 2020
        </div>
        <p class="paper-abstract">The interaction of ambiguity aversion and limited capital market participation magnifies the impact of fiscal uncertainty shocks on economic activity because concerns about redistribution have first-order effects.</p>
        <div class="paper-files">
          <a href="http://hsaijo.github.io/files/policy_uncertainty.pdf">Paper</a>
          <a href="http://hsaijo.github.io/files/policy_uncertainty_appendix.pdf">Appendix</a>
        </div>
      </div>

      <div class="paper">
        <div class="paper-title"><a href="http://hsaijo.github.io/files/hours.pdf">Technology Shocks and Hours Revisited: Evidence from Household Data</a></div>
        <div class="paper-meta">
          <span class="paper-journal">Review of Economic Dynamics</span>, 2019
        </div>
        <p class="paper-abstract">Contrary to the aggregate evidence, labor supply responses to technology shocks at the household level indicate that the data is inconsistent with the sticky price view of the business cycle.</p>
        <div class="paper-files">
          <a href="http://hsaijo.github.io/files/hours.pdf">Paper</a>
          <a href="http://hsaijo.github.io/files/hours_wp.pdf">Working paper version with additional results</a>
        </div>
      </div>

      <div class="paper">
        <div class="paper-title"><a href="http://hsaijo.github.io/files/uncertainty_multiplier.pdf">The Uncertainty Multiplier and Business Cycles</a></div>
        <div class="paper-meta">
          <span class="paper-journal">Journal of Economic Dynamics and Control</span>, 2017
        </div>
        <p class="paper-abstract">A dynamic general equilibrium model where agents learn about macro fundamentals through investment. The endogenously countercyclical uncertainty amplifies output fluctuations by 16%.</p>
        <div class="paper-files">
          <a href="http://hsaijo.github.io/files/uncertainty_multiplier.pdf">Paper</a>
        </div>
      </div>

      <div class="paper">
        <div class="paper-title"><a href="http://hsaijo.github.io/files/seasonal_DSGE.pdf">Estimating DSGE Models Using Seasonally Adjusted and Unadjusted Data</a></div>
        <div class="paper-meta">
          <span class="paper-journal">Journal of Econometrics</span>, 2013
        </div>
        <p class="paper-abstract">
        The common practice of estimating dynamic stochastic general equilibrium (DSGE) models using seasonally adjusted data leads to sizeable distortions in estimated parameters.
        </p>
        <div class="paper-files">
          <a href="http://hsaijo.github.io/files/seasonal_DSGE.pdf">Paper</a>
          <a href="http://hsaijo.github.io/files/seasonal_DSGE_appendix.pdf">Appendix</a>
        </div>
      </div>

      <div class="paper">
        <div class="paper-title"><a href="http://hsaijo.github.io/files/japanese_depression.pdf">The Japanese Depression in the Interwar Period: A General Equilibrium Analysis</a></div>
        <div class="paper-meta">
          <span class="paper-journal">The B.E. Journal of Macroeconomics</span>, 2008
        </div>
        <p class="paper-abstract">The increase in markups due to cartelization can explain a substantial fraction of Japan's weak recovery from the Great Depression.</p>
        <div class="paper-files">
          <a href="http://hsaijo.github.io/files/japanese_depression.pdf">Paper</a>
        </div>
      </div>

    </section>

    <!-- Working Papers -->
    <section id="papers">
      <div class="section-label">Working Papers</div>

      <div class="paper">
        <div class="paper-title"><a href="http://hsaijo.github.io/files/SmoothDE_paper.pdf">Smooth Diagnostic Expectations</a></div>
        <div class="paper-meta">
          with <a href="https://sites.google.com/view/francescobianchi/home">Francesco Bianchi</a> &amp; <a href="https://sites.google.com/site/cosminilut/">Cosmin Ilut</a><br>
          <span class="paper-status">R&amp;R</span> · <span class="paper-journal">Review of Economic Studies</span>, 2025.
        </div>
        <p class="paper-abstract">Introducing Smooth Diagnostic Expectations (Smooth DE), featuring an intrinsic connection between uncertainty and overreaction. We provide novel survey evidence that supports the key prediction of Smooth DE: forecasts overreact more when uncertainty is high. We show Smooth DE explains additional stylized facts on surveys, and key features of business cycles.</p>
        <div class="paper-files">
          <a href="http://hsaijo.github.io/files/SmoothDE_paper.pdf">Paper</a>
        </div>
      </div>

      <div class="paper">
        <div class="paper-title"><a href="http://hsaijo.github.io/files/volatility_network.pdf">Volatility Shocks in Networks</a></div>
        <div class="paper-meta">2025</div>
        <p class="paper-abstract">I show that sector-specific volatility shocks propagate through input–output linkages, triggering a network precautionary pricing multiplier that amplifies their impact on the entire economy.</p>
        
        <div class="paper-files">
          <a href="http://hsaijo.github.io/files/volatility_network.pdf">Paper</a>
        </div>
      </div>

    </section>

    <!-- Discussions -->
    <section id="discussions">
      <div class="section-label">Discussions</div>

      <div class="disc">
        <a href="http://hsaijo.github.io/files/wu_xie_discussion.pdf">(Un)Conventional Monetary and Fiscal Policy</a> by Wu &amp; Xie
        <span class="disc-venue">ASSA Meeting, January 2024</span>
      </div>

      <div class="disc">
        <a href="http://hsaijo.github.io/files/MS_slide.pdf">What Do Sectoral Dynamics Tell Us About the Origins of Business Cycles?</a> by Matthes &amp; Schwartzman
        <span class="disc-venue">Workshop on Methods and Applications for DSGE Models, October 2019</span>
      </div>

      <div class="disc">
        <a href="http://hsaijo.github.io/files/BKT_slide.pdf">The Origins and Effects of Uncertainty Shocks</a> by Bianchi, Kung &amp; Tirskikh
        <span class="disc-venue">Workshop on Methods and Applications for DSGE Models, October 2018</span>
      </div>

      <div class="disc">
        <a href="http://hsaijo.github.io/files/boehm_slide.pdf">Are Supply Curves Convex?</a> by Boehm, Flaaen &amp; Pandalai-Nayar
        <span class="disc-venue">West Coast Workshop in International Finance, November 2017</span>
      </div>

      <div class="disc">
        <a href="http://hsaijo.github.io/files/milani_slide.pdf">Sentiment and the Business Cycle</a> by Fabio Milani
        <span class="disc-venue">California Macroeconomics Conference, October 2016</span>
      </div>

    </section>
