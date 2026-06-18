<html lang="en"><head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>eugene.sh</title>
  <meta name="description" content="megalomaniacal jerk degrading collective sense of reality">
  <meta name="robots" content="noindex">
  <link rel="icon" type="image/png" sizes="32x32" href="https://eugene.sh/eugene_sh_32x32.ico">
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="">
  <link href="https://fonts.googleapis.com/css2?family=Oxanium:wght@700;800&amp;family=JetBrains+Mono:wght@400;500&amp;display=swap" rel="stylesheet">

  <style>
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
    :root {
      --bg: #04040a;
      --ink: #ccc8be;
      --ink-dim: #38352e;
      --ink-mid: #6b6660;
      --n1: #ff2a6d;
      --n2: #05d9e8;
      --n3: #c8ff00;
      --n4: #b300ff;
      --n5: #ff9000;
      --deep: #0a0612;
      --bruise: #2a0a3a;
      --mono: 'JetBrains Mono', monospace;
      --display: 'Oxanium', sans-serif;
    }
    html, body { height: 100%; overflow-x: hidden; }
    body {
      min-height: 100dvh; background: var(--bg);
      font-family: var(--mono);
      display: flex; align-items: center; justify-content: center;
      -webkit-font-smoothing: antialiased;
      padding-bottom: 2.4rem;
    }
    #u0 { position: fixed; inset: 0; z-index: 0; width: 100%; height: 100%; }
    .u1 {
      position: fixed; inset: 0; z-index: 2; pointer-events: none;
      background: repeating-linear-gradient(0deg, transparent 0px, transparent 3px, rgba(0,0,0,0.09) 3px, rgba(0,0,0,0.09) 4px);
    }
    .u2 {
      position: fixed; inset: 0; z-index: 3; pointer-events: none;
      background: radial-gradient(ellipse at center, transparent 35%, rgba(0,0,0,0.78) 100%);
    }
    .u3 {
      position: fixed; inset: 0; z-index: 4; pointer-events: none;
      opacity: 0; transition: opacity 0.05s;
      mix-blend-mode: screen;
    }
    .panel {
      position: relative; z-index: 10;
      display: flex; flex-direction: column; align-items: center; text-align: center;
      padding: clamp(2rem, 6vw, 4rem) clamp(1.5rem, 5vw, 3.5rem);
      max-width: min(540px, 95vw); width: 100%;
      overflow: visible;
      animation: a-in 0.9s cubic-bezier(0.16,1,0.3,1) both;
    }
    @keyframes a-in { from { opacity:0; transform:translateY(18px); } to { opacity:1; transform:translateY(0); } }

    .h0 {
      width: 100%;
      display: flex;
      align-items: center;
      justify-content: center;
      position: relative;
      height: clamp(3.6rem, 12vw, 7rem);
      min-height: clamp(3.6rem, 12vw, 7rem);
      max-height: clamp(3.6rem, 12vw, 7rem);
      margin-bottom: 2.5rem;
      contain: layout;
    }
    .h0 .h1 { position: absolute; left: 50%; top: 50%; transform: translate(-50%, -50%); }
    .h1 {
      font-family: var(--display);
      font-size: clamp(2.4rem, 8.5vw, 6rem);
      font-weight: 800;
      line-height: 1;
      color: var(--ink);
      display: flex;
      align-items: baseline;
      justify-content: center;
      white-space: nowrap;
      gap: 0;
      letter-spacing: -0.02em;
      text-transform: lowercase;
      transition: font-size 0.6s cubic-bezier(0.22,1,0.36,1), opacity 0.3s ease, letter-spacing 0.42s cubic-bezier(0.22,1,0.36,1);
      max-width: 100%;
      overflow: visible;
      will-change: font-size, letter-spacing;
    }
    .h1.tight { letter-spacing: -0.085em; }
    .fx-a { animation: fx-a 0.42s steps(2,end) 1, fx-col 0.42s linear 1; }
    .fx-b { animation: fx-b 0.5s steps(1,end) 1,  fx-col 0.5s linear 1; }
    .fx-c { animation: fx-c 0.34s ease-in-out 1,  fx-col 0.34s linear 1; }
    .fx-d { animation: fx-d 0.3s steps(1,end) 1,  fx-col 0.3s linear 1; }
    .fx-e { animation: fx-e 0.46s steps(3,end) 1, fx-col 0.46s linear 1; }

    @keyframes fx-col {
      0%   { color: var(--ink);    text-shadow: none; }
      15%  { color: var(--n1);     text-shadow: 0 0 12px var(--n1), 0 0 2px var(--bruise); }
      30%  { color: var(--n4);     text-shadow: 0 0 16px var(--n4), 0 0 3px var(--deep); }
      45%  { color: var(--n2);     text-shadow: 0 0 14px var(--n2), 0 0 4px var(--deep); }
      60%  { color: var(--n3);     text-shadow: 0 0 18px var(--n3), 0 0 3px var(--bruise); }
      75%  { color: var(--n1);     text-shadow: 0 0 12px var(--n1), 0 0 2px var(--deep); }
      90%  { color: var(--n5);     text-shadow: 0 0 10px var(--n5); }
      100% { color: var(--ink);    text-shadow: none; }
    }
    @keyframes fx-a {
      0%,100% { text-shadow:none; transform:none; }
      20% { text-shadow: 4px 0 var(--n1), -4px 0 var(--n2), 0 0 18px var(--n4); transform:translateX(1px); }
      40% { text-shadow:-4px 0 var(--n1), 4px 0 var(--n2), 0 0 20px var(--n4); transform:translateX(-2px); }
      60% { text-shadow: 3px 0 var(--n3), -3px 0 var(--n2), 0 0 16px var(--n3); transform:translateX(1px); }
      80% { text-shadow:-2px 0 var(--n1), 0 0 12px var(--n1); transform:none; }
    }
    @keyframes fx-b {
      0%,100% { clip-path:none; transform:none; text-shadow:none; }
      15% { clip-path: inset(20% 0 55% 0); transform:translateX(-7px); text-shadow:2px 0 var(--n2), 0 0 14px var(--n2); }
      30% { clip-path: inset(62% 0 12% 0); transform:translateX(6px);  text-shadow:0 0 12px var(--n4); }
      45% { clip-path: inset(38% 0 40% 0); transform:translateX(-4px); text-shadow:-2px 0 var(--n1), 0 0 14px var(--n1); }
      60% { clip-path: inset(8% 0 78% 0);  transform:translateX(5px);  text-shadow:0 0 10px var(--n3); }
      75% { clip-path: inset(72% 0 4% 0);  transform:translateX(-3px); text-shadow:0 0 12px var(--n2); }
    }
    @keyframes fx-c {
      0%,100% { transform:none; text-shadow:none; }
      25% { transform:skewX(-9deg) scaleY(1.04); text-shadow:3px 0 var(--n1),-3px 0 var(--n2), 0 0 18px var(--n4); }
      50% { transform:skewX(7deg); text-shadow: 0 0 14px var(--n3); }
      75% { transform:skewX(-3deg) scaleY(0.98); text-shadow:-2px 0 var(--n2), 0 0 12px var(--n2); }
    }
    @keyframes fx-d {
      0%,100% { opacity:1; text-shadow:none; }
      10% { opacity:0.25; text-shadow: 0 0 14px var(--n1); }
      20% { opacity:1; }
      35% { opacity:0.1; text-shadow:0 0 20px var(--n3), 0 0 6px var(--n4); }
      45% { opacity:1; }
      60% { opacity:0.4; text-shadow: 0 0 12px var(--n2); }
      70% { opacity:1; }
      85% { opacity:0.15; text-shadow: 0 0 16px var(--n1); }
    }
    @keyframes fx-e {
      0%,100% { transform:none; text-shadow:none; }
      33% { transform:translate(2px,-2px); text-shadow:-3px 0 var(--n1), 3px 2px var(--n2), 0 0 16px var(--n4); }
      66% { transform:translate(-2px,1px); text-shadow:3px 0 var(--n2), -3px -1px var(--n1), 0 0 14px var(--n3); }
    }
    .sx {
      color: var(--ink-mid);
      font-family: inherit; font-size: inherit; font-weight: inherit;
      line-height: inherit;
      letter-spacing: 0;
      display: inline-block;
      min-width: 0.55em;
      margin: 0 0.04em;
      text-align: center;
      overflow: hidden;
      transition: transform 0.18s ease, margin 0.18s ease, color 0.4s ease;
      animation: none;
      will-change: text-shadow, opacity;
      text-shadow: none;
    }
    .sx.u {
      color: var(--n2);
      animation: sxg 1.05s ease-in-out infinite;
    }
    .sx.k {
      transform: translateY(-0.04em);
      margin: 0 0.02em;
      min-width: 0.22em;
      color: var(--n3);
      animation: sxgk 1.05s ease-in-out infinite;
    }
    .sx.x {
      color: var(--n5);
      min-width: 0.7em;
      margin: 0 0.12em;
      animation: sxgx 1.05s ease-in-out infinite;
    }
    @keyframes sxgx {
      0%,100% { text-shadow: 0 0 3px var(--n5), 0 0 8px rgba(255,144,0,0.45); }
      50%     { text-shadow: 0 0 6px var(--n5), 0 0 18px rgba(255,144,0,0.85), 0 0 26px rgba(255,42,109,0.3); }
    }
    @keyframes sxg {
      0%,100% { text-shadow: 0 0 2px var(--n2), 0 0 6px rgba(5,217,232,0.35); }
      50%     { text-shadow: 0 0 5px var(--n2), 0 0 14px rgba(5,217,232,0.75), 0 0 22px rgba(179,0,255,0.25); }
    }
    @keyframes sxgk {
      0%,100% { text-shadow: 0 0 2px var(--n3), 0 0 6px rgba(200,255,0,0.35); }
      50%     { text-shadow: 0 0 5px var(--n3), 0 0 14px rgba(200,255,0,0.7), 0 0 22px rgba(255,42,109,0.25); }
    }
    .cb {
      color: var(--ink-mid);
      font-family: inherit; font-size: inherit; font-weight: 700; line-height: inherit;
      display: inline-block;
      animation: cb 1.05s step-end infinite;
      margin-left: 0.03em;
    }
    @keyframes cb { 0%,100%{opacity:1} 50%{opacity:0} }

    .nv { display:flex; flex-direction:column; align-items:stretch; gap:0; width:100%; max-width:360px; }
    .it {
      display:flex; align-items:center; gap:0.75rem;
      padding:0.65rem 1rem;
      font-family:var(--mono); font-size:clamp(0.78rem,2vw,0.87rem);
      font-weight:400; letter-spacing:0.05em;
      color:var(--ink-mid); text-decoration:none;
      position:relative; border-radius:2px; overflow:hidden;
      transition:color 120ms ease;
    }
    .it::after { content:''; position:absolute; inset:0; background:var(--n3); transform:scaleX(0); transform-origin:left; transition:transform 160ms cubic-bezier(0.16,1,0.3,1); z-index:-1; border-radius:2px; }
    .it:hover { color:#04040a; }
    .it:hover::after { transform:scaleX(1); }
    .it:hover .ip, .it:hover .ia { color:#04040a; }
    .ip { font-size:0.6rem; letter-spacing:0.14em; color:var(--ink-dim); min-width:2rem; text-align:right; flex-shrink:0; transition:color 120ms ease; }
    .il { flex:1; text-align:left; min-width: 0; }
    .ia { color:var(--ink-dim); flex-shrink:0; transition:color 120ms ease; }
    .dv { height:1px; background:linear-gradient(90deg,transparent,var(--ink-dim) 40%,var(--ink-dim) 60%,transparent); opacity:0.22; margin:0.5rem 0; }

    @media (max-width: 640px) {
      .panel { padding: 1.5rem 1rem; }
      .h1 {
        font-size: clamp(2.2rem, 12vw, 4rem);
        max-width: 92vw;
        flex-wrap: nowrap;
      }
      .h0 { min-height: clamp(3rem, 14vw, 5rem); }
      .nv { max-width: 100%; }
      .it { padding: 0.7rem 0.85rem; font-size: 0.76rem; }
      .il { overflow-wrap: anywhere; word-break: break-word; }
    }
    @media(max-width:380px){ .h1 { font-size: clamp(2rem, 11vw, 3rem); } }
    @media(max-width:280px){ .h1 { font-size: 1.8rem; } }

    body, .panel, .h1, .it, .cd, .cdh, .cdt, #tgw, #lo, #ft { user-select: none; -webkit-user-select: none; -moz-user-select: none; -ms-user-select: none; }
    .il, .ft-c a { user-select: none; -webkit-user-select: none; }

    .h1 .gl {
      color: var(--ink);
      text-shadow:
        -1px 0 rgba(255,42,109,0.85),
        1px 0 rgba(5,217,232,0.85),
        0 0 4px rgba(200,255,0,0.35);
      animation: gl-jit 80ms steps(2) infinite;
      display: inline-block;
    }
    @keyframes gl-jit {
      0%   { transform: translate(0,0); text-shadow: -1px 0 rgba(255,42,109,0.85), 1px 0 rgba(5,217,232,0.85), 0 0 4px rgba(200,255,0,0.3); }
      50%  { transform: translate(0.5px,-0.5px); text-shadow: 1px 0 rgba(255,42,109,0.85), -1px 0 rgba(5,217,232,0.85), 0 0 5px rgba(179,0,255,0.35); }
    }
    .h1 .xo {
      color: var(--n5);
      text-shadow:
        0 0 4px var(--n5),
        0 0 12px rgba(255,144,0,0.7),
        0 0 22px rgba(255,42,109,0.3);
      display: inline-block;
    }
    .sx.gl-sep {
      color: var(--ink) !important;
      text-shadow:
        -1px 0 rgba(255,42,109,0.85),
        1px 0 rgba(5,217,232,0.85),
        0 0 4px rgba(200,255,0,0.35) !important;
      animation: gl-jit 80ms steps(2) infinite !important;
    }

    .eb-wrap {
      display: flex; flex-direction: column; align-items: center; justify-content: center;
      margin-top: 1.6rem; width: 100%; position: relative; z-index: 4; gap: 0.7rem;
    }
    #auth {
      display: flex; flex-direction: column; align-items: center; gap: 0.7rem;
    }
    #auth.off { display: none; }
    #tgh {
      position: relative;
      width: 238px; height: 40px;
      display: flex; justify-content: center; align-items: center;
      transition: opacity 240ms ease;
    }
    #tgh.hidden { display: none; }
    #tgh iframe {
      position: absolute; inset: 0;
      width: 100%; height: 100%;
      opacity: 0;
      border: 0;
      z-index: 2;
    }
    #tgw {
      position: absolute; inset: 0;
      display: flex; align-items: center; justify-content: center;
      gap: 0.55rem;
      background: linear-gradient(180deg, rgba(20,16,36,0.92) 0%, rgba(8,6,16,0.92) 100%);
      border: 1px solid rgba(5,217,232,0.4);
      color: var(--ink); font-family: 'JetBrains Mono', monospace; font-weight: 700;
      letter-spacing: 0.22em; font-size: 0.72rem;
      box-shadow: 0 0 14px rgba(5,217,232,0.22), inset 0 0 10px rgba(5,217,232,0.1);
      backdrop-filter: blur(4px);
      pointer-events: none;
      transition: border-color 220ms ease, box-shadow 220ms ease, color 220ms ease;
      z-index: 1;
    }
    #tgh:hover #tgw {
      border-color: rgba(5,217,232,0.85);
      box-shadow: 0 0 22px rgba(5,217,232,0.45), inset 0 0 14px rgba(5,217,232,0.2);
      color: var(--n2);
    }
    #tgh::before, #tgh::after {
      content:''; position:absolute; pointer-events:none;
      width: 9px; height: 9px; border-color: var(--n2); border-style: solid;
      z-index: 3;
    }
    #tgh::before { top:-1px; left:-1px; border-width: 1px 0 0 1px; }
    #tgh::after { bottom:-1px; right:-1px; border-width: 0 1px 1px 0; }
    #tgh { cursor: pointer; }
    #tgw svg { width: 14px; height: 14px; flex: 0 0 14px; }
    #tgw .tgw-t { display: inline-block; }

    #ft {
      position: fixed; left: 0; right: 0; bottom: 0; z-index: 4;
      padding: 0.9rem 1.2rem;
      font-family: 'JetBrains Mono', monospace;
      font-size: 0.66rem;
      letter-spacing: 0.08em;
      color: var(--ink-dim);
      text-align: center;
      pointer-events: none;
      text-shadow: 0 0 6px rgba(2,2,6,0.9);
    }
    .ft-c { pointer-events: auto; display: inline-block; }
    .ft-c a { color: var(--ink-dim); text-decoration: none; transition: color 200ms ease, text-shadow 200ms ease; }
    .ft-c a:hover { color: var(--n3); text-shadow: 0 0 6px rgba(200,255,0,0.6); }
    .ft-c.is-ua { color: var(--ink-mid); letter-spacing: 0.02em; }

    #av {
      display: none;
      width: 40px; height: 40px;
      margin: 0 auto 1.1rem;
      border-radius: 50%;
      border: 1px solid rgba(5,217,232,0.55);
      box-shadow: 0 0 12px rgba(5,217,232,0.32), inset 0 0 6px rgba(5,217,232,0.18);
      background: #0b0b14 center/cover no-repeat;
      position: relative;
      overflow: hidden;
      opacity: 0;
      transform: scale(0.88);
      transition: opacity 320ms ease, transform 320ms cubic-bezier(0.22,1,0.36,1);
    }
    #av.on { display: block; opacity: 1; transform: scale(1); }
    #avm {
      position: absolute; inset: 0;
      display: flex; align-items: center; justify-content: center;
      font-family: var(--display);
      font-weight: 800;
      font-size: 18px;
      text-transform: uppercase;
      color: var(--n2);
      text-shadow: 0 0 8px rgba(5,217,232,0.55);
      letter-spacing: 0.02em;
    }
    #av.has-img #avm { opacity: 0; }
    #deck {
      display: none;
      grid-template-columns: repeat(3, minmax(0, 1fr));
      gap: 0.85rem;
      width: 100%; max-width: 720px;
    }
    #deck.on { display: grid; }
    .cd {
      position: relative; display: flex; flex-direction: column; justify-content: center;
      padding: 0.85rem 0.95rem 0.95rem;
      background: linear-gradient(180deg, rgba(10,6,18,0.85) 0%, rgba(4,4,10,0.92) 100%);
      border: 1px solid rgba(220,225,235,0.08);
      text-decoration: none; color: var(--ink);
      transition: transform 260ms cubic-bezier(0.22,1,0.36,1), border-color 260ms ease, box-shadow 260ms ease, opacity 360ms ease;
      opacity: 0; transform: translateY(18px) scale(0.97);
      overflow: hidden; min-height: 88px;
    }
    .cd::before { content:''; position:absolute; left:0; right:0; top:0; height:2px; }
    .cd[data-k="seo"]::before { background: linear-gradient(90deg, transparent, var(--n5), transparent); }
    .cd[data-k="lab"]::before { background: linear-gradient(90deg, transparent, var(--n2), transparent); }
    .cd[data-k="n8n"]::before { background: linear-gradient(90deg, transparent, var(--n1), transparent); }
    #deck.on .cd { opacity: 1; transform: translateY(0) scale(1); }
    #deck.on .cd:nth-child(1) { transition-delay: 90ms; }
    #deck.on .cd:nth-child(2) { transition-delay: 220ms; }
    #deck.on .cd:nth-child(3) { transition-delay: 350ms; }
    .cd[data-k="seo"] { border-color: rgba(255,144,0,0.28); }
    .cd[data-k="lab"] { border-color: rgba(5,217,232,0.28); }
    .cd[data-k="n8n"] { border-color: rgba(255,42,109,0.32); }
    .cd[data-k="seo"]:hover { border-color: rgba(255,144,0,0.65); box-shadow: 0 8px 28px rgba(255,144,0,0.22); transform: translateY(-3px) scale(1.01); }
    .cd[data-k="lab"]:hover { border-color: rgba(5,217,232,0.65); box-shadow: 0 8px 28px rgba(5,217,232,0.22); transform: translateY(-3px) scale(1.01); }
    .cd[data-k="n8n"]:hover { border-color: rgba(255,42,109,0.7); box-shadow: 0 8px 28px rgba(255,42,109,0.26); transform: translateY(-3px) scale(1.01); }
    .cdh { display:flex; align-items:center; gap: 0.4rem; font-family: 'JetBrains Mono', monospace; font-size: 0.78rem; color: var(--ink-mid); letter-spacing: 0.02em; margin-bottom: 0.35rem; }
    .cdd { display:inline-block; width: 7px; height: 7px; border-radius: 50%; flex: 0 0 7px; }
    .cd[data-k="seo"] .cdd { background: var(--n5); box-shadow: 0 0 8px var(--n5); }
    .cd[data-k="lab"] .cdd { background: var(--n2); box-shadow: 0 0 8px var(--n2); }
    .cd[data-k="n8n"] .cdd { background: var(--n1); box-shadow: 0 0 8px var(--n1); }
    .cdn { font-weight: 700; }
    .cd[data-k="seo"] .cdn { color: var(--n5); text-shadow: 0 0 4px rgba(255,144,0,0.65), 0 0 12px rgba(255,144,0,0.4); }
    .cd[data-k="lab"] .cdn { color: var(--n2); text-shadow: 0 0 4px rgba(5,217,232,0.7), 0 0 12px rgba(5,217,232,0.45); }
    .cd[data-k="n8n"] .cdn { color: var(--n1); text-shadow: 0 0 4px rgba(255,42,109,0.7), 0 0 12px rgba(255,42,109,0.45); }
    .cdt { display:block; font-size: 0.86rem; font-weight: 700; color: var(--ink); letter-spacing: -0.01em; }

    #lo {
      display: none;
      margin-top: 0.9rem;
      background: transparent; border: none;
      font-family: 'JetBrains Mono', monospace; font-weight: 700;
      letter-spacing: 0.28em; font-size: 0.62rem;
      color: var(--ink-dim);
      padding: 0.35rem 0.6rem;
      cursor: pointer;
      transition: color 200ms ease, text-shadow 200ms ease;
    }
    #lo.on { display: inline-block; }
    #lo:hover { color: var(--n2); text-shadow: 0 0 8px rgba(5,217,232,0.55); }
    #lo::before { content: '[ '; opacity: 0.55; }
    #lo::after { content: ' ]'; opacity: 0.55; }

    @media (max-width: 640px) {
      #deck { grid-template-columns: 1fr; max-width: 360px; }
      .cd { min-height: 70px; padding: 0.75rem 0.9rem 0.85rem; }
    }

    @media(prefers-reduced-motion:reduce){*,*::before,*::after{animation:none!important;transition-duration:0.01ms!important;}}
  </style>
<style>.keyword-info-container{box-sizing:border-box;width:92%;margin-bottom:20px;font-size:12px;border-bottom:1px solid #dee1e5;border:1px solid #f1f3f4;margin:14px 16px;border-radius:2px;padding:20px;position:relative;-webkit-font-smoothing:antialiased}body[data-dt="1"] .keyword-info-container,html[dark] .keyword-info-container{border-color:#3d4042}.keyword-info-container .title{color:#26282d;font-size:16px;font-weight:bold}.keyword-info-container .tabs{list-style:none;display:flex;justify-content:flex-start;border-bottom:1px solid #dee1e5;margin-top:-10px;padding:0px 16px;align-items:center}.keyword-info-container .tabs.tip{border-color:#f8b199 !important;border-radius:2px;border:1px solid}.keyword-info-container .tabs li{padding:8px;padding-left:0;color:#000;cursor:pointer;font-size:12px}.keyword-info-container .tabs li.small{font-size:10px}.keyword-info-container .tabs li:last-child{overflow:hidden}.keyword-info-container .tabs li.active{color:#4285f4;margin:20px 0}table.keyword-info-table{border-collapse:collapse;width:100%;color:#000;font-size:12px;position:relative}.keyword-info-table thead{height:50px}.keyword-info-table th{padding:10px;padding-left:0;font-weight:bold;color:#000;font-size:12px}.keyword-info-table th:first-child{padding-left:16px}.keyword-info-table th:last-child{padding-right:0px}.keyword-info-table td{border-bottom:1px solid #f1f3f4;padding:10px;padding-left:0;height:50px;box-sizing:border-box}.keyword-info-table tr{border-bottom:1px solid #f1f3f4}body[data-dt="1"] .keyword-info-table td,html[dark] .keyword-info-table td{border-color:#3d4042}body[data-dt="1"] .keyword-info-table tr,html[dark] .keyword-info-table tr{border-color:#3d4042}body[data-dt="1"] .keyword-info-table tfoot tr,body[data-dt="1"] .keyword-info-table tfoot td,html[dark] .keyword-info-table tfoot tr,html[dark] .keyword-info-table tfoot td{border:none}.keyword-info-table td:first-child{padding-left:16px}.keyword-info-table td:last-child{padding-right:0px}.keyword-info-table tfoot tr,.keyword-info-table tfoot td{border:none}.ubersuggest-button{color:#0086f7;font-family:Figtree;font-size:14px;font-weight:bold;line-height:29px;padding:8px 30px;border:1px solid #0086f7;background-color:#fff;border-radius:2px;outline:none;border:none;cursor:pointer;margin:4px}.ubersuggest-logo-wrapper{display:flex;align-items:center;justify-content:flex-end;margin:10px 10px 0 0;font-weight:bold;color:#26282d}.ubersuggest-logo{width:182px;height:33px;cursor:pointer}.keyword-info-container .row{display:flex;justify-content:space-between;align-items:center;margin:0;padding:20px 16px}.header h2{color:#000;font-family:Figtree;font-size:24px;font-weight:500}html[dark] .keyword-info-container .title{color:#fff}html[dark] table.keyword-info-table{color:#fff}html[dark] .keyword-info-table th{color:#fff}html[dark] .keyword-info-table tfoot tr:last-child td .button-arrow{border-color:#fff}body[data-dt="1"] .keyword-info-container .title{color:#fff}body[data-dt="1"] .keyword-info-container .tabs{border-color:rgba(255,255,255,.0509803922)}body[data-dt="1"] table.keyword-info-table{color:#fff}body[data-dt="1"] .keyword-info-table th{color:#fff}</style><style>.tippy-box[data-theme~=tip-dark] .tippy-content,.tippy-box[data-theme~=tip-light] .tippy-content{padding:0}.tippy-box[data-theme~=tip-dark]>.tippy-backdrop{background-color:#fff}.tippy-box[data-theme~=tip-dark]>.tippy-arrow:after{border-color:#fff;border-style:solid}.tippy-box[data-theme~=tip-dark][data-placement^=top]>.tippy-arrow:before{border-top-color:#fff}.tippy-box[data-theme~=tip-dark][data-placement^=top]>.tippy-arrow:after{border-top-color:#fff}.tippy-box[data-theme~=tip-dark][data-placement^=bottom]>.tippy-arrow:before{border-bottom-color:#fff;bottom:16px}.tippy-box[data-theme~=tip-dark][data-placement^=bottom]>.tippy-arrow:after{border-bottom-color:#fff}.tippy-box[data-theme~=tip-dark][data-placement^=left]>.tippy-arrow:before{border-left-color:#fff}.tippy-box[data-theme~=tip-dark][data-placement^=left]>.tippy-arrow:after{border-left-color:#fff}.tippy-box[data-theme~=tip-dark][data-placement^=right]>.tippy-arrow:before{border-right-color:#fff}.tippy-box[data-theme~=tip-dark][data-placement^=right]>.tippy-arrow:after{border-right-color:#fff}.tippy-box[data-theme~=tip-dark]>.tippy-svg-arrow{fill:#fff}.tippy-box[data-theme~=tip-light]>.tippy-backdrop{background-color:#202020}.tippy-box[data-theme~=tip-light]>.tippy-arrow:after{border-color:#202020;border-style:solid}.tippy-box[data-theme~=tip-light][data-placement^=top]>.tippy-arrow:before{border-top-color:#202020}.tippy-box[data-theme~=tip-light][data-placement^=top]>.tippy-arrow:after{border-top-color:#202020}.tippy-box[data-theme~=tip-light][data-placement^=bottom]>.tippy-arrow:before{border-bottom-color:#202020;bottom:16px}.tippy-box[data-theme~=tip-light][data-placement^=bottom]>.tippy-arrow:after{border-bottom-color:#202020}.tippy-box[data-theme~=tip-light][data-placement^=left]>.tippy-arrow:before{border-left-color:#202020}.tippy-box[data-theme~=tip-light][data-placement^=left]>.tippy-arrow:after{border-left-color:#202020}.tippy-box[data-theme~=tip-light][data-placement^=right]>.tippy-arrow:before{border-right-color:#202020}.tippy-box[data-theme~=tip-light][data-placement^=right]>.tippy-arrow:after{border-right-color:#202020}.tippy-box[data-theme~=tip-light]>.tippy-svg-arrow{fill:#202020}</style><style>.tippy-box[data-animation=fade][data-state=hidden]{opacity:0}[data-tippy-root]{max-width:calc(100vw - 10px)}.tippy-box{position:relative;background-color:#333;color:#fff;border-radius:4px;font-size:14px;line-height:1.4;white-space:normal;outline:0;transition-property:transform,visibility,opacity}.tippy-box[data-placement^=top]>.tippy-arrow{bottom:0}.tippy-box[data-placement^=top]>.tippy-arrow:before{bottom:-7px;left:0;border-width:8px 8px 0;border-top-color:initial;transform-origin:center top}.tippy-box[data-placement^=bottom]>.tippy-arrow{top:0}.tippy-box[data-placement^=bottom]>.tippy-arrow:before{top:-7px;left:0;border-width:0 8px 8px;border-bottom-color:initial;transform-origin:center bottom}.tippy-box[data-placement^=left]>.tippy-arrow{right:0}.tippy-box[data-placement^=left]>.tippy-arrow:before{border-width:8px 0 8px 8px;border-left-color:initial;right:-7px;transform-origin:center left}.tippy-box[data-placement^=right]>.tippy-arrow{left:0}.tippy-box[data-placement^=right]>.tippy-arrow:before{left:-7px;border-width:8px 8px 8px 0;border-right-color:initial;transform-origin:center right}.tippy-box[data-inertia][data-state=visible]{transition-timing-function:cubic-bezier(0.54, 1.5, 0.38, 1.11)}.tippy-arrow{width:16px;height:16px;color:#333}.tippy-arrow:before{content:"";position:absolute;border-color:rgba(0,0,0,0);border-style:solid}.tippy-content{position:relative;padding:5px 9px;z-index:1}</style><style>.tippy-box[data-theme~=light]{color:#26323d;box-shadow:0 0 20px 4px rgba(154,161,177,.15),0 4px 80px -8px rgba(36,40,47,.25),0 4px 4px -2px rgba(91,94,105,.15);background-color:#fff}.tippy-box[data-theme~=light][data-placement^=top]>.tippy-arrow:before{border-top-color:#fff}.tippy-box[data-theme~=light][data-placement^=bottom]>.tippy-arrow:before{border-bottom-color:#fff}.tippy-box[data-theme~=light][data-placement^=left]>.tippy-arrow:before{border-left-color:#fff}.tippy-box[data-theme~=light][data-placement^=right]>.tippy-arrow:before{border-right-color:#fff}.tippy-box[data-theme~=light]>.tippy-backdrop{background-color:#fff}.tippy-box[data-theme~=light]>.tippy-svg-arrow{fill:#fff}</style><style id="_goober"> @keyframes go2264125279{from{transform:scale(0) rotate(45deg);opacity:0;}to{transform:scale(1) rotate(45deg);opacity:1;}}@keyframes go3020080000{from{transform:scale(0);opacity:0;}to{transform:scale(1);opacity:1;}}@keyframes go463499852{from{transform:scale(0) rotate(90deg);opacity:0;}to{transform:scale(1) rotate(90deg);opacity:1;}}@keyframes go1268368563{from{transform:rotate(0deg);}to{transform:rotate(360deg);}}@keyframes go1310225428{from{transform:scale(0) rotate(45deg);opacity:0;}to{transform:scale(1) rotate(45deg);opacity:1;}}@keyframes go651618207{0%{height:0;width:0;opacity:0;}40%{height:0;width:6px;opacity:1;}100%{opacity:1;height:10px;}}@keyframes go901347462{from{transform:scale(0.6);opacity:0.4;}to{transform:scale(1);opacity:1;}}.go4109123758{z-index:9999;}.go4109123758 > *{pointer-events:auto;}</style><style>.ubersuggest-header-container{box-sizing:border-box;width:100%;font-size:12px;-webkit-font-smoothing:antialiased}@keyframes slideInFromLeft{from{transform:translateX(100%);opacity:0}to{transform:translateX(-4%);opacity:1}}.ubersuggest-header-container .toast-container{animation:slideInFromLeft .5s ease forwards}.ubersuggest-header-container .row{margin:0;padding:15px 16px 15px 16px;display:flex;justify-content:space-between;align-items:center;min-height:30px}.ubersuggest-header-container .row>div{display:flex;flex-wrap:wrap;gap:8px}.ubersuggest-header-container .row>div:first-child>div{flex-wrap:wrap;align-content:space-around}.ue-enable{display:block}.ue-disable,.ue-enable.hide-settings{display:none !important}.ue-disable.hide-settings{display:flex !important}.ubersuggest-header-container .settings{display:flex;align-items:center}.ubersuggest-header-container .settings-label{margin-right:21px}.ubersuggest-header-container .settings-icon{width:21px;height:21px;margin-right:7px}</style><style>.rr--group{display:flex;width:100%;position:relative}.rr--box{display:flex;width:100%;flex-grow:1;-webkit-tap-highlight-color:rgba(0,0,0,0)}.rr--svg{display:flex;aspect-ratio:1;width:100%;flex-grow:1;overflow:clip;pointer-events:none}@supports not (overflow: clip){.rr--svg{overflow:auto}}.rr--box:focus,.rr--box:focus-visible,.rr-reset:focus-visible,.rr-reset:focus{outline:none;box-shadow:none}.rr--focus-reset{outline:6px double #0079ff}.rr--box:focus-visible .rr--svg{outline:6px double #0079ff;isolation:isolate}.rr--reset{position:absolute;width:1px;height:1px;padding:0;margin:-1px;overflow:hidden;clip:rect(0, 0, 0, 0);white-space:nowrap;border:0;right:0;bottom:50%}[dir=rtl] .rr--reset{left:0;right:auto}.rr--dir-y .rr--reset{bottom:0;right:50%}.rr--disabled{opacity:.5;cursor:not-allowed}.rr--disabled .rr--svg{pointer-events:none}.rr--pointer .rr--box{cursor:pointer}.rr--dir-x{flex-direction:row}.rr--dir-y{flex-direction:column}.rr--space-sm .rr--svg{padding:8%}.rr--space-md .rr--svg{padding:12.5%}.rr--space-lg .rr--svg{padding:17.5%}.rr--dir-x.rr--gap-sm .rr--svg{margin:0 6.25%}.rr--dir-x.rr--gap-sm .rr--box:focus-visible:after{width:87.5%;left:6.25%}.rr--dir-x.rr--gap-md .rr--svg{margin:0 12.5%}.rr--dir-x.rr--gap-md .rr--box:focus-visible:after{width:75%;left:12.5%}.rr--dir-x.rr--gap-lg .rr--svg{margin:0 25%}.rr--dir-x.rr--gap-lg .rr--box:focus-visible:after{width:50%;left:25%}.rr--dir-y.rr--gap-sm .rr--svg{margin:6.25% 0}.rr--dir-y.rr--gap-md .rr--svg{margin:12.5% 0}.rr--dir-y.rr--gap-lg .rr--svg{margin:25% 0}.rr--rx-sm .rr--svg{border-radius:5%}.rr--rx-md .rr--svg{border-radius:15%}.rr--rx-lg .rr--svg{border-radius:20%}.rr--rx-full .rr--svg{border-radius:100%}.rr--has-stroke .rr--svg{stroke-linecap:round;stroke-linejoin:round}.rr--has-border .rr--svg{border-width:var(--rr--border-width);border-style:solid}.rr--on .rr--svg{fill:var(--rr--fill-on-color, none)}.rr--off .rr--svg{fill:var(--rr--fill-off-color, none)}.rr--has-stroke .rr--on .rr--svg{stroke:var(--rr--stroke-on-color, currentColor)}.rr--has-stroke .rr--off .rr--svg{stroke:var(--rr--stroke-off-color, currentColor)}.rr--on .rr--svg{background-color:var(--rr--box-on-color, none)}.rr--off .rr--svg{background-color:var(--rr--box-off-color, none)}.rr--has-border .rr--off .rr--svg{border-color:var(--rr--border-off-color, currentColor)}.rr--has-border .rr--on .rr--svg{border-color:var(--rr--border-on-color, currentColor)}.rr--fx-colors{--rr--easing: .2s cubic-bezier(.61, 1, .88, 1)}.rr--fx-colors .rr--svg{transition-duration:.2s;transition-timing-function:var(--rr--easing);transition-property:background-color,border-color,fill,stroke}.rr--fx-opacity .rr--off{opacity:.35;transition:opacity var(--rr--easing)}.rr--fx-opacity .rr--on{opacity:1}@media(hover: hover){.rr--fx-opacity .rr--box:hover{opacity:1}}@media(hover: hover){.rr--fx-zoom .rr--box{transition:transform var(--rr--easing);transform:scale(1)}.rr--fx-zoom .rr--box:hover{transform:scale(1.2)}}@media(hover: hover)and (prefers-reduced-motion){.rr--fx-zoom .rr--box:hover{transform:scale(1)}}@media(hover: hover){.rr--fx-position .rr--box{transition:transform var(--rr--easing);transform:translateY(0)}.rr--fx-position .rr--box:hover{transform:translateY(-15%)}}@media(hover: hover)and (prefers-reduced-motion){.rr--fx-position .rr--box:hover{transform:translateY(0)}}.rr--svg-stop-1{stop-color:var(--rr--fill-on-color, rgba(0, 0, 0, 0))}[dir=rtl] .rr--svg-stop-1,.rr--svg-stop-2{stop-color:var(--rr--fill-off-color, rgba(0, 0, 0, 0))}[dir=rtl] .rr--svg-stop-2{stop-color:var(--rr--fill-on-color, rgba(0, 0, 0, 0))}.rr--hf-svg-on{fill:var(--rr--fill-on-color, none)}.rr--hf-svg-off{fill:var(--rr--fill-off-color, none)}.rr--has-stroke .rr--hf-svg-on{stroke:var(--rr--stroke-on-color, currentColor)}.rr--has-stroke .rr--hf-svg-off{stroke:var(--rr--stroke-off-color, currentColor)}.rr--hf-svg-on .rr--svg,.rr--hf-svg-off .rr--svg{background-color:var(--rr--box-off-color, none)}.rr--has-border .rr--hf-svg-on .rr--svg{border-color:var(--rr--border-on-color, currentColor)}.rr--has-border .rr--hf-svg-off .rr--svg{border-color:var(--rr--border-off-color, currentColor)}.rr--dir-x .rr--hf-box-int .rr--svg{background:linear-gradient(to right, var(--rr--box-on-color, none) 50%, var(--rr--box-off-color, none) 50%)}[dir=rtl] .rr--dir-x .rr--hf-box-int .rr--svg{background:linear-gradient(to left, var(--rr--box-on-color, none) 50%, var(--rr--box-off-color, none) 50%)}.rr--dir-y .rr--hf-box-int .rr--svg{background:linear-gradient(to bottom, var(--rr--box-on-color, none) 50%, var(--rr--box-off-color, none) 50%)}.rr--hf-box-on .rr--svg{background-color:var(--rr--box-on-color, none)}.rr--hf-box-off .rr--svg{background-color:var(--rr--box-off-color, none)}.rr--hf-box-on .rr--svg,.rr--hf-box-off .rr--svg,.rr--hf-box-int .rr--svg{fill:var(--rr--fill-off-color, none)}.rr--has-stroke .rr--hf-box-on .rr--svg,.rr--has-stroke .rr--hf-box-off .rr--svg,.rr--has-stroke .rr--hf-box-int .rr--svg{stroke:var(--rr--stroke-off-color, currentColor)}.rr--has-border .rr--hf-box-on .rr--svg,.rr--has-border .rr--hf-box-int .rr--svg{border-color:var(--rr--border-on-color, currentColor)}.rr--has-border .rr--hf-box-off .rr--svg{border-color:var(--rr--border-off-color, currentColor)}</style><style>.keyword-info-section{color:#26282d;font-family:Figtree;font-size:12px;height:100%;display:flex;align-items:center;-webkit-font-smoothing:antialiased}.keyword-info-section img{max-width:none}.keyword-info-section>li{font-weight:600;position:relative;display:flex;align-items:center;gap:6px}.keyword-info-section>li:first-child::after{content:"";width:6px;height:6px;background-color:#e8ebec;border-radius:50%;margin:0px 10px 0px 4px}body[data-dt="1"] .keyword-info-section>li:first-child::after{background-color:#636363}.keyword-info-section.hidden{display:none}.keyword-info-section.google{background-color:rgba(0,0,0,0)}.keyword-info-section.youtube{margin-right:15px;padding:0 0 0 10px;height:100%;background-color:#fff}.keyword-info-section.amazon{padding:13px 0;background-color:#fff}</style><style>.kw-overview-container{box-sizing:border-box;width:673px;padding:0;margin:0;margin-top:14px;font-size:12px;font-family:Figtree;-webkit-font-smoothing:antialiased}.kw-overview-container.youtube{box-sizing:border-box;width:645px;padding:0;margin:0;font-size:12px}</style><style>.bl-info-container{box-sizing:border-box;width:100%;padding:0;margin:0;font-size:12px;font-family:"Figtree";-webkit-font-smoothing:antialiased}.bl-info-header{display:flex;min-height:24px;width:100%;padding:0;justify-content:space-between;box-sizing:border-box;margin-bottom:5px}.bl-info-header .row{display:flex;margin:0;width:100%;justify-content:space-between}.bl-info-header .row.youtube{justify-content:flex-start}.bl-info-content,.kw-info-content{width:97%;display:flex;flex-direction:column;border:1px solid #dee1e5;border-radius:4px;padding-block:16px 10px;justify-items:center;align-items:center;margin-bottom:16px;position:relative}body[data-dt="1"] .kw-info-content,body[data-dt="1"] .bl-info-content{background:rgba(0,0,0,0);border-color:#292929}.bl-info-content img.loading{width:50px;margin:0 auto;margin-bottom:10px}.kw-info-content img.loading{width:50px;margin:0 auto;margin-top:10px;margin-bottom:10px}table.bl-info-table,table.kw-info-table{border-collapse:collapse;width:calc(100% - 32px);color:#808185;font-size:12px}body[data-dt="1"] table.bl-info-table,body[data-dt="1"] table.kw-info-table{color:#fff}.bl-info-table thead,.kw-info-table thead{height:50px;background:#f6f7f7}body[data-dt="1"] table.bl-info-table thead,body[data-dt="1"] table.kw-info-table thead{background:#36373a}.bl-info-table tr,.kw-info-table tr{width:100%;max-width:600px}.bl-info-table th,.kw-info-table th{padding:10px;padding-left:0;font-weight:600;color:#000;font-size:12px;border-bottom:1px solid #f6f7f7}body[data-dt="1"] .bl-info-table th,body[data-dt="1"] .kw-info-table th{color:#fff;border-color:#3d4043}.bl-info-table th:first-child,.kw-info-table th:first-child{padding-left:16px}.bl-info-table th:last-child,.kw-info-table th:last-child{border-right:none;padding-right:16px}.bl-info-table td,.kw-info-table td{border-bottom:1px solid #dee1e5;padding:10px;padding-left:0;max-width:0;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;color:#000}body[data-dt="1"] .bl-info-table td,body[data-dt="1"] .kw-info-table td{color:#fff;border-color:#3d4043}.bl-info-table td:first-child,.kw-info-table td:first-child{border-left:none;padding-left:16px}.bl-info-table tfoot td:first-child,.kw-info-table tfoot td:first-child{padding-left:0;padding-top:12px}.bl-info-table tfoot td:last-child,.kw-info-table tfoot td:last-child{padding-right:0;padding-top:12px}.bl-info-table td:last-child,.kw-info-table td:last-child{border-right:none;padding-right:16px}.bl-info-table tfoot tr:last-child td,.kw-info-table tfoot tr:last-child td{border-bottom:none}.bl-info-container .row{display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap}.bl-info-container .row.start{justify-content:flex-start;gap:10px}.bl-info-container .row.start.tip{border:1px solid #f8b199;border-radius:2px;width:fit-content;padding-right:10px}</style><style>.statistics-graph-container{box-sizing:border-box;width:92%;font-size:12px;border-bottom:1px solid #dee1e5;border:1px solid #f1f3f4;margin:24px 16px;border-radius:2px;padding:20px;padding-bottom:10px;position:relative;-webkit-font-smoothing:antialiased}body[data-dt="1"] .statistics-graph-container{border-color:#3d4042}.statistics-graph-container.tip{border:1px solid #f8b199;border-radius:2px}.statistics-graph-container .row{display:flex;justify-content:space-between;align-items:center;margin:0 0 20px 0}.statistics-graph-container .row.closed{margin-bottom:10px}.statistics-graph-container .row .title{color:#26282d;font-size:16px;font-weight:bold}body[data-dt="1"] .statistics-graph-container .row .title{color:#fff}body[data-dt="1"] .statistics-graph-container .tabs{border-bottom:1px solid #dee1e5}body[data-dt="1"] .statistics-graph-container .tabs li{color:#fff}body[data-dt="1"] .statistics-graph-container .tabs li.active{color:#fff;border-bottom:3px solid #fff}</style></head>

<body cz-shortcut-listen="true">
  <canvas id="u0" aria-hidden="true" width="811" height="928"></canvas>
  <div class="u1" aria-hidden="true"></div>
  
  

  <main>
    <div class="panel">
      <div class="h0" aria-label="eugene.sh">
        <div class="h1 tight" id="h1" aria-hidden="true" style="opacity: 1;">
          <span id="ha">eugene</span><span class="sx k" id="hs">.</span><span id="hb">sh</span><span class="cb">|</span>
        </div>
      </div>

      
    </div>

    
  </main>

  

  <script>
  (function(){
    const T = [];
    let visible = !document.hidden;

    function schedule(fn, delay){
      const item = { fn, due: performance.now() + delay, remaining: delay, paused: !visible };
      T.push(item);
      if (!item.paused) item.timer = setTimeout(() => run(item), delay);
      return item;
    }
    function run(item){
      const idx = T.indexOf(item);
      if (idx !== -1) T.splice(idx, 1);
      try { item.fn(); } catch(e){}
    }
    function pauseAll(){
      const now = performance.now();
      for (const item of T){
        if (item.paused) continue;
        clearTimeout(item.timer);
        item.remaining = Math.max(0, item.due - now);
        item.paused = true;
      }
    }
    function resumeAll(){
      const now = performance.now();
      for (const item of T){
        if (!item.paused) continue;
        item.due = now + item.remaining;
        item.paused = false;
        item.timer = setTimeout(() => run(item), item.remaining);
      }
    }
    document.addEventListener('visibilitychange', () => {
      visible = !document.hidden;
      if (visible) resumeAll(); else pauseAll();
    });

    window.__S = { schedule, isVisible: () => visible };
  })();

  window.__BOX = window.__BOX || [];
  function pruneBoxes(){
    const now = performance.now();
    for (let i = window.__BOX.length-1; i >= 0; i--){
      if (window.__BOX[i].exp < now) window.__BOX.splice(i, 1);
    }
  }
  function rectsOverlap(a, b, pad){
    return !(a.x+a.w+pad < b.x || a.x > b.x+b.w+pad || a.y+a.h+pad < b.y || a.y > b.y+b.h+pad);
  }
  function pos(tw, th, pad, life){
    pruneBoxes();
    const W = window.innerWidth, H = window.innerHeight;
    const p = document.querySelector('.panel');
    const r = p ? p.getBoundingClientRect() : {left:0,top:0,width:0,height:0};
    const lifeMs = life || 6000;
    for (let i=0;i<30;i++){
      const x = pad + Math.random()*(W-tw-pad*2);
      const y = pad + Math.random()*(H-th-pad*2);
      if (!(x+tw < r.left-40 || x > r.left+r.width+40 || y+th < r.top-40 || y > r.top+r.height+40)) continue;
      const cand = { x, y, w: tw, h: th };
      let ok = true;
      for (const b of window.__BOX){ if (rectsOverlap(cand, b, 24)){ ok = false; break; } }
      if (ok){
        window.__BOX.push({ x, y, w: tw, h: th, exp: performance.now() + lifeMs });
        return { x, y };
      }
    }
    return {x: pad, y: pad + Math.random()*80};
  }

  (function(){
    const sx = document.getElementById('hs');
    const ha = document.getElementById('ha');
    const hb = document.getElementById('hb');
    const h1 = document.getElementById('h1');

    const POOL = ['·','∙',':',';','!','?','*','-','/','|','°','¦','’','′'];
    const pick = () => POOL[Math.floor(Math.random()*POOL.length)];

    let phase='dot', t0=Date.now(), morphing=false;
    const HOLD=2200, SDUR=720;

    function size(mode){
      if (mode === 'm') h1.style.fontSize = 'clamp(1.5rem, 9vw, 3.6rem)';
      else if (mode === 's') h1.style.fontSize = 'clamp(1.55rem, 8.6vw, 3.3rem)';
      else h1.style.fontSize = '';
    }

    const MGLY = '01アイウエオカキクケコサシスセソタチツテトナニヌネノ░▒▓│┤╡╢╖╣║╗╝└┴┬├─┼╠═╬┘┌@#$%^&*!?<>';
    const scr = (w,p) => w.split('').map(c => {
      if (c === ' ') return c;
      if (c === '\u00d7') return '<span class="xo">\u00d7</span>';
      if (Math.random() < p) {
        const g = MGLY[Math.floor(Math.random()*MGLY.length)];
        return '<span class="gl">' + g + '</span>';
      }
      return c;
    }).join('');

    const FX = ['fx-a','fx-b','fx-c','fx-d','fx-e'];
    const clearFx = () => FX.forEach(c => h1.classList.remove(c));

    function corrupt(){
      clearFx();
      h1.classList.add('fx-a');
      let f = 0;
      const iv = setInterval(() => {
        if (morphing){ clearInterval(iv); return; }
        f++;
        ha.innerHTML = scr('eugene', 0.38);
        hb.innerHTML = scr('sh', 0.5);
        if (f > 5){
          clearInterval(iv);
          ha.textContent = 'eugene';
          hb.textContent = 'sh';
          h1.classList.remove('fx-a');
        }
      }, 40);
    }

    function fire(){
      if (morphing){ next(); return; }
      if (Math.random() < 0.22){
        corrupt();
      } else {
        clearFx();
        const c = FX[Math.floor(Math.random()*FX.length)];
        void h1.offsetWidth;
        h1.classList.add(c);
        h1.addEventListener('animationend', function ae(){ h1.classList.remove(c); h1.removeEventListener('animationend', ae); }, { once:true });
        setTimeout(() => h1.classList.remove(c), 700);
      }
      next();
    }
    function next(){ window.__S.schedule(fire, 3000 + Math.random()*5000); }
    next();

    function morphNext(){ window.__S.schedule(morphPick, 60000 + Math.random()*60000); }
    function morphPick(){ (Math.random() < 0.5 ? morphFull : morphSeo)(); }

    function morphFull(){
      if (morphing){ morphNext(); return; }
      morphing = true;
      clearFx();
      h1.classList.remove('tight');
      h1.style.transition = 'font-size 0.6s cubic-bezier(0.22,1,0.36,1), opacity 0.3s ease';

      h1.style.opacity = '0.18';
      setS('_');
      ha.innerHTML = scr('eugene', 0.7);
      hb.innerHTML = scr('sheremet', 0.8);
      size('m');
      let gf = 0;
      const gi = setInterval(() => {
        gf++;
        ha.innerHTML = scr('eugene', 0.55);
        hb.innerHTML = scr('sheremet', 0.6);
        if (gf > 14){
          clearInterval(gi);
          ha.textContent = 'eugene';
          hb.textContent = 'sheremet';
          setS('_');
          h1.style.opacity = '1';
          setTimeout(() => {
            h1.style.opacity = '0.18';
            let rf = 0;
            const ri = setInterval(() => {
              rf++;
              ha.innerHTML = scr('eugene', 0.55);
              hb.innerHTML = scr('sheremet', 0.6);
              if (rf > 10){
                clearInterval(ri);
                ha.textContent = 'eugene';
                hb.textContent = 'sh';
                setS(phase==='under' ? '_' : '.');
                size('n');
                h1.style.opacity = '1';
                setTimeout(() => {
                  h1.style.transition = '';
                  morphing = false;
                  morphNext();
                }, 680);
              }
            }, 45);
          }, 3000);
        }
      }, 45);
    }

    function setSepX(on){
      sx.classList.remove('k'); sx.classList.remove('u'); sx.classList.remove('gl-sep');
      if (on){ sx.classList.add('x'); sx.textContent = '\u00d7'; }
      else { sx.classList.remove('x'); }
    }

    function morphSeo(){
      if (morphing){ morphNext(); return; }
      morphing = true;
      clearFx();
      h1.classList.remove('tight');
      h1.style.transition = 'font-size 0.6s cubic-bezier(0.22,1,0.36,1), opacity 0.3s ease';

      h1.style.opacity = '0.18';
      sx.classList.remove('k'); sx.classList.remove('u'); sx.classList.remove('x'); sx.classList.remove('gl-sep');
      sx.textContent = '\u00d7';
      sx.classList.add('x');
      ha.innerHTML = scr('SEO', 0.7);
      hb.innerHTML = scr('AI \u00d7 CODING', 0.78);
      size('s');
      let gf = 0;
      const gi = setInterval(() => {
        gf++;
        ha.innerHTML = scr('SEO', 0.5);
        hb.innerHTML = scr('AI \u00d7 CODING', 0.6);
        if (gf > 14){
          clearInterval(gi);
          ha.textContent = 'SEO';
          hb.innerHTML = 'AI <span class="xo">\u00d7</span> CODING';
          h1.style.opacity = '1';
          setTimeout(() => {
            h1.style.opacity = '0.18';
            let rf = 0;
            const ri = setInterval(() => {
              rf++;
              ha.innerHTML = scr('SEO', 0.5);
              hb.innerHTML = scr('AI \u00d7 CODING', 0.55);
              if (rf > 10){
                clearInterval(ri);
                ha.textContent = 'eugene';
                hb.textContent = 'sh';
                setS(phase==='under' ? '_' : '.');
                size('n');
                h1.style.opacity = '1';
                setTimeout(() => {
                  h1.style.transition = '';
                  morphing = false;
                  morphNext();
                }, 680);
              }
            }, 45);
          }, 6000);
        }
      }, 45);
    }
    morphNext();

    function setS(ch){
      sx.textContent = ch;
      sx.classList.remove('x');
      sx.classList.remove('k');
      sx.classList.remove('u');
      sx.classList.remove('gl-sep');
      if (ch === '.') sx.classList.add('k');
      else if (ch === '_') sx.classList.add('u');
      else sx.classList.add('gl-sep');
    }

    function loop(){
      if (morphing){ setTimeout(loop, 100); return; }
      const now = Date.now(), e = now - t0;
      if (phase === 'dot'){
        setS('.');
        h1.classList.add('tight');
        if (e > HOLD){ phase = 's2u'; t0 = now; }
      } else if (phase === 's2u'){
        setS(e > SDUR ? '_' : pick());
        h1.classList.remove('tight');
        if (e > SDUR){ phase = 'under'; t0 = now; }
      } else if (phase === 'under'){
        setS('_');
        h1.classList.remove('tight');
        if (e > HOLD){ phase = 's2d'; t0 = now; }
      } else if (phase === 's2d'){
        setS(e > SDUR ? '.' : pick());
        if (e > SDUR){ phase = 'dot'; t0 = now; }
      }
      setTimeout(loop, (phase==='s2u'||phase==='s2d') ? 35 : 80);
    }
    loop();
  })();

  (function(){
    const canvas = document.getElementById('u0');
    const ctx = canvas.getContext('2d');
    let W, H;
    function resize(){ W = canvas.width = window.innerWidth; H = canvas.height = window.innerHeight; }
    window.addEventListener('resize', resize);
    resize();

    const GLY = '01アイウエオカキクケコサシスセソタチツテトナニヌネノ░▒▓│┤╡╢╖╣║╗╝└┴┬├─┼╠═╬┘┌';
    const CW = 18;
    let cols = [];
    function initCols(){
      cols = [];
      for (let i = 0; i < Math.ceil(W/CW); i++) cols.push({
        x: i*CW, y: Math.random()*-H, speed: 0.35 + Math.random()*1.1,
        len: 5 + Math.floor(Math.random()*18),
        chars: Array.from({length:22}, () => GLY[Math.floor(Math.random()*GLY.length)]),
        opacity: 0.03 + Math.random()*0.07,
        color: Math.random()<0.11 ? '#ff2a6d' : Math.random()<0.07 ? '#05d9e8' : '#c8ff00'
      });
    }
    initCols();
    window.addEventListener('resize', initCols);

    const bars = [];
    function spawnBar(){
      if (Math.random() < 0.35) bars.push({
        x: Math.random()*W, y: Math.random()*H,
        w: 15 + Math.random()*240, h: 1 + Math.random()*3,
        life: 2 + Math.floor(Math.random()*6),
        color: Math.random()<0.5 ? '#ff2a6d' : '#c8ff00',
        alpha: 0.05 + Math.random()*0.13
      });
      window.__S.schedule(spawnBar, 80 + Math.random()*250);
    }
    spawnBar();

    const NODES = Array.from({length:26}, () => ({
      x: Math.random()*1920, y: Math.random()*1080,
      vx: (Math.random()-0.5)*0.12, vy: (Math.random()-0.5)*0.12,
      r: 1 + Math.random()*1.2
    }));
    let scanY = 0;
    function rgba(hex, a){
      const r = parseInt(hex.slice(1,3),16), g = parseInt(hex.slice(3,5),16), b = parseInt(hex.slice(5,7),16);
      return `rgba(${r},${g},${b},${a})`;
    }

    const PH = ['404 not found','null','undefined','page 2 of google','zero-click search','google hates me','keyword stuffing','search intent','content is king','high bounce rate','organic traffic','link equity','results in 30 days','megalomaniacal jerk','crawled - not indexed','google slapped my site','backlink profile','toxic links','core update','spammy links'];
    let pEv = null;
    function pNext(){ window.__S.schedule(pTrig, 30000 + Math.random()*40000); }
    function pTrig(){
      const w = PH[Math.floor(Math.random()*PH.length)];
      const p = pos(w.length*9 + 20, 22, 50, 5200);
      pEv = { w, x:p.x, y:p.y, phase:'type', i:0, alpha:0, t:performance.now(), color: Math.random()<0.3?'#ff2a6d':Math.random()<0.2?'#05d9e8':'#c8ff00' };
      pNext();
    }
    pNext();

    let fEv = null;
    function fNext(){ window.__S.schedule(fTrig, 90000 + Math.random()*120000); }
    function fTrig(){ fEv = { life:18 }; fNext(); }
    fNext();

    const rings = [];
    function rNext(){ window.__S.schedule(rTrig, 45000 + Math.random()*55000); }
    function rTrig(){
      const c = Math.random()<0.5 ? '#c8ff00' : '#05d9e8';
      rings.push({ r:0, max: Math.max(W,H)*0.8, speed:2.5, alpha:0.35, color:c });
      if (Math.random() < 0.4) setTimeout(() => rings.push({ r:0, max: Math.max(W,H)*0.8, speed:2.5, alpha:0.25, color:'#ff2a6d' }), 400);
      rNext();
    }
    rNext();

    let rgbEv = null;
    const u3 = document.getElementById('u3');
    function rgbNext(){ window.__S.schedule(rgbTrig, 60000 + Math.random()*90000); }
    function rgbTrig(){ rgbEv = { y:0, life:60, dir:1 }; rgbNext(); }
    rgbNext();

    let stEv = null;
    function stNext(){ window.__S.schedule(stTrig, 100000 + Math.random()*140000); }
    function stTrig(){ stEv = { life:22 }; stNext(); }
    stNext();

    let cEv = null;
    function cNext(){ window.__S.schedule(cTrig, 75000 + Math.random()*100000); }
    function cTrig(){
      const i = Math.floor(Math.random()*cols.length);
      cEv = { i, life:90, sp: cols[i].speed, op: cols[i].opacity };
      cols[i].speed = 8 + Math.random()*6;
      cols[i].opacity = 0.9;
      cNext();
    }
    cNext();

    const hex = [];
    const HX = '0123456789ABCDEF';
    function rh(){ const n = Math.random()<0.5?4:Math.random()<0.5?6:8; let s = '0x'; for (let i=0;i<n;i++) s += HX[Math.floor(Math.random()*16)]; return s; }
    function hNext(){ window.__S.schedule(hTrig, 18000 + Math.random()*22000); }
    function hTrig(){
      const n = 2 + Math.floor(Math.random()*4);
      for (let i=0;i<n;i++){
        const p = pos(90, 18, 40, 3500);
        hex.push({
          text: rh(), x: p.x, y: p.y+12,
          alpha:0, phase:'in', t: performance.now() + i*120,
          color: Math.random()<0.18 ? '#ff2a6d' : Math.random()<0.2 ? '#05d9e8' : '#c8ff00',
          hold: 1200 + Math.random()*1800
        });
      }
      hNext();
    }
    hNext();

    const LBL = ['SYS://INDEX','CRAWL://NET','SEO.CORE','LINK.GRAPH','RANK.SYNC','NODE.SCAN','CACHE.PURGE','DATA.STREAM'];
    let lEv = null;
    function lNext(){ window.__S.schedule(lTrig, 55000 + Math.random()*70000); }
    function lTrig(){
      const p = pos(220, 46, 40, 6500);
      lEv = {
        label: LBL[Math.floor(Math.random()*LBL.length)],
        x: p.x, y: p.y+14, progress:0, alpha:0,
        phase:'in', t: performance.now(),
        color: Math.random()<0.5 ? '#c8ff00' : '#05d9e8'
      };
      lNext();
    }
    lNext();

    let fkEv = null;
    function fkNext(){ window.__S.schedule(fkTrig, 40000 + Math.random()*60000); }
    function fkTrig(){ fkEv = { life: 6 + Math.floor(Math.random()*5) }; fkNext(); }
    fkNext();

    let wEv = null;
    function wNext(){ window.__S.schedule(wTrig, 70000 + Math.random()*80000); }
    function wTrig(){
      const s = 46 + Math.random()*40;
      const p = pos(s*2.4, s*2.4, 50);
      wEv = {
        x: p.x + s*1.2, y: p.y + s*1.2, s,
        sides: Math.random()<0.5 ? 6 : Math.random()<0.5 ? 3 : 4,
        rot: Math.random()*Math.PI, alpha:0, phase:'in',
        t: performance.now(), color: Math.random()<0.5 ? '#c8ff00' : '#05d9e8'
      };
      wNext();
    }
    wNext();

    let mEv = null;
    function mNext(){ window.__S.schedule(mTrig, 60000 + Math.random()*80000); }
    function mTrig(){ mEv = { life: 10 + Math.floor(Math.random()*12), bands: [] }; mNext(); }
    mNext();

    let sEv = null;
    const SERP_SITES = ['eugene.sh','sitelair.com','yevhen.locker','sheremet.ton.run'];
    function sNext(){ window.__S.schedule(sTrig, 240000 + Math.random()*300000); }
    function sTrig(){
      const rows = SERP_SITES.length;
      const w = 280 + Math.floor(Math.random()*80);
      const rh = 26;
      const h = rows * rh + 24;
      const p = pos(w, h, 50, 7500);
      const items = [];
      const shuffled = SERP_SITES.slice().sort(() => Math.random()-0.5);
      for (let i=0;i<rows;i++){
        items.push({ rank: i+1, site: shuffled[i] });
      }
      sEv = { x:p.x, y:p.y, w, h, rh, items, phase:'in', t: performance.now(), alpha:0, life: 4200, warp:0 };
      sNext();
    }
    sNext();

    function draw(){
      ctx.clearRect(0, 0, W, H);
      ctx.fillStyle = '#04040a';
      ctx.fillRect(0, 0, W, H);

      ctx.strokeStyle = 'rgba(200,255,0,0.022)';
      ctx.lineWidth = 1;
      for (let x=0; x<W; x+=60){ ctx.beginPath(); ctx.moveTo(x,0); ctx.lineTo(x,H); ctx.stroke(); }
      for (let y=0; y<H; y+=60){ ctx.beginPath(); ctx.moveTo(0,y); ctx.lineTo(W,y); ctx.stroke(); }

      for (let i=0; i<NODES.length; i++){
        const a = NODES[i];
        a.x += a.vx; a.y += a.vy;
        if (a.x<0||a.x>W) a.vx *= -1;
        if (a.y<0||a.y>H) a.vy *= -1;
        for (let j=i+1; j<NODES.length; j++){
          const b = NODES[j], d = Math.hypot(a.x-b.x, a.y-b.y);
          if (d < 180){
            ctx.strokeStyle = `rgba(200,255,0,${(1-d/180)*0.07})`;
            ctx.lineWidth = 0.5;
            ctx.beginPath(); ctx.moveTo(a.x,a.y); ctx.lineTo(b.x,b.y); ctx.stroke();
          }
        }
        ctx.fillStyle = 'rgba(200,255,0,0.28)';
        ctx.beginPath(); ctx.arc(a.x, a.y, a.r, 0, Math.PI*2); ctx.fill();
      }

      ctx.font = `${CW-2}px 'JetBrains Mono',monospace`;
      for (const c of cols){
        c.y += c.speed;
        if (c.y > H + c.len*CW){
          c.y = Math.random()*-H*0.5;
          c.speed = 0.35 + Math.random()*1.1;
          if (Math.random() < 0.3) for (let j=0; j<c.chars.length; j++) c.chars[j] = GLY[Math.floor(Math.random()*GLY.length)];
        }
        for (let j=0; j<c.len; j++){
          const cy = c.y - j*CW;
          if (cy < -CW || cy > H + CW) continue;
          const al = c.opacity * (j===0 ? 2.2 : 1 - j/c.len);
          ctx.fillStyle = j===0 ? `rgba(255,255,255,${Math.min(al*2, 0.45)})` : rgba(c.color, al);
          ctx.fillText(c.chars[j], c.x, cy);
          if (Math.random() < 0.003) c.chars[j] = GLY[Math.floor(Math.random()*GLY.length)];
        }
      }

      for (let i = bars.length-1; i >= 0; i--){
        const g = bars[i];
        ctx.globalAlpha = g.alpha; ctx.fillStyle = g.color;
        ctx.fillRect(g.x, g.y, g.w, g.h);
        ctx.globalAlpha = 1;
        if (--g.life <= 0) bars.splice(i, 1);
      }

      scanY = (scanY + 0.35) % H;
      const sg = ctx.createLinearGradient(0, scanY-70, 0, scanY+70);
      sg.addColorStop(0, 'rgba(200,255,0,0)');
      sg.addColorStop(0.5, 'rgba(200,255,0,0.022)');
      sg.addColorStop(1, 'rgba(200,255,0,0)');
      ctx.fillStyle = sg;
      ctx.fillRect(0, scanY-70, W, 140);

      if (pEv){
        const e = pEv, now = performance.now(), D = 80;
        if (e.phase === 'type'){
          e.i = Math.min(Math.floor((now-e.t)/D), e.w.length);
          e.alpha = Math.min(e.i/Math.max(e.w.length,1), 1) * 0.88;
          if (e.i >= e.w.length){ e.phase = 'hold'; e.t = now; }
        } else if (e.phase === 'hold'){
          e.alpha = 0.88;
          if (now-e.t > 2400){ e.phase = 'fade'; e.t = now; }
        } else if (e.phase === 'fade'){
          e.alpha = Math.max(0, 0.88*(1-(now-e.t)/800));
          if (e.alpha <= 0) pEv = null;
        }
        if (e){
          ctx.font = `bold 13px 'JetBrains Mono',monospace`;
          ctx.globalAlpha = e.alpha * (Math.random()<0.04 ? 0.3 : 1);
          ctx.fillStyle = e.color;
          const tx = e.w.slice(0, e.i);
          for (let ci=0; ci<tx.length; ci++){
            const jx = (Math.random()-0.5) * (e.phase==='type' && ci===tx.length-1 ? 2 : 0.3);
            const jy = (Math.random()-0.5) * (e.phase==='type' && ci===tx.length-1 ? 3 : 0.5);
            ctx.fillText(tx[ci], e.x + ci*14 + jx, e.y + jy);
          }
          ctx.globalAlpha = 1;
        }
      }

      if (fEv){
        fEv.life--;
        if (fEv.life > 12){
          const n = Math.floor(Math.random()*6) + 2;
          for (let i=0; i<n; i++){
            ctx.globalAlpha = 0.12 + Math.random()*0.2;
            ctx.fillStyle = Math.random()<0.5 ? '#ff2a6d' : '#c8ff00';
            ctx.fillRect(Math.random()*(W*0.5), Math.random()*H, 80 + Math.random()*(W*0.7), 1 + Math.random()*5);
          }
          if (Math.random() < 0.3){
            ctx.globalAlpha = 0.07; ctx.fillStyle = '#ff2a6d';
            ctx.fillRect(0, Math.floor(Math.random()*H), W, 2 + Math.floor(Math.random()*8));
          }
        } else {
          ctx.globalAlpha = (fEv.life/12) * 0.06;
          ctx.fillStyle = '#c8ff00';
          ctx.fillRect(0, 0, W, H);
        }
        ctx.globalAlpha = 1;
        if (fEv.life <= 0) fEv = null;
      }

      for (let i = rings.length-1; i >= 0; i--){
        const r = rings[i];
        ctx.globalAlpha = r.alpha * (1 - r.r/r.max);
        ctx.strokeStyle = r.color; ctx.lineWidth = 1.5;
        ctx.beginPath(); ctx.arc(W/2, H/2, r.r, 0, Math.PI*2); ctx.stroke();
        ctx.globalAlpha = 1;
        r.r += r.speed;
        r.alpha = Math.max(0, r.alpha - 0.003);
        if (r.r >= r.max || r.alpha <= 0) rings.splice(i, 1);
      }

      if (rgbEv){
        rgbEv.y += 2.5 * rgbEv.dir;
        if (rgbEv.y > H+60 || rgbEv.y < -60){ rgbEv = null; u3.style.opacity = '0'; }
        else {
          const bh = Math.floor(H*0.06) + 2;
          ctx.globalAlpha = 0.07; ctx.fillStyle = '#ff2a6d'; ctx.fillRect(0, rgbEv.y, W, bh);
          ctx.globalAlpha = 0.06; ctx.fillStyle = '#05d9e8'; ctx.fillRect(-4, rgbEv.y-2, W, bh);
          ctx.globalAlpha = 0.18; ctx.fillStyle = '#ffffff'; ctx.fillRect(0, rgbEv.y, W, 1);
          ctx.globalAlpha = 1;
          rgbEv.life--;
          if (rgbEv.life <= 0) rgbEv = null;
        }
      }

      if (stEv){
        stEv.life--;
        const dens = stEv.life > 11 ? 0.003 : 0.0015;
        const ct = Math.floor((W*H/16) * dens);
        for (let p=0; p<ct; p++){
          const sxp = Math.random()*W, syp = Math.random()*H;
          ctx.globalAlpha = 0.08 + Math.random()*0.18;
          const gr = Math.floor(Math.random()*255);
          ctx.fillStyle = `rgb(${gr},${gr},${gr})`;
          ctx.fillRect(sxp, syp, Math.floor(Math.random()*6)+1, Math.floor(Math.random()*6)+1);
        }
        if (Math.random() < 0.25){
          ctx.globalAlpha = 0.05 + Math.random()*0.07;
          ctx.fillStyle = '#ffffff';
          ctx.fillRect(0, Math.floor(Math.random()*H), W, 1 + Math.floor(Math.random()*3));
        }
        ctx.globalAlpha = 1;
        if (stEv.life <= 0) stEv = null;
      }

      if (cEv){
        cEv.life--;
        const col = cols[cEv.i];
        if (cEv.life <= 0 || !col){
          if (col){ col.speed = cEv.sp; col.opacity = cEv.op; }
          cEv = null;
        } else if (cEv.life < 20){
          const t = cEv.life/20;
          col.speed = cEv.sp + (8 - cEv.sp)*t;
          col.opacity = cEv.op + (0.9 - cEv.op)*t;
        }
      }

      if (hex.length){
        ctx.font = `11px 'JetBrains Mono',monospace`;
        const now = performance.now();
        for (let i = hex.length-1; i >= 0; i--){
          const tk = hex[i];
          if (now < tk.t) continue;
          const t = now - tk.t;
          if (tk.phase === 'in'){ tk.alpha = Math.min(t/250, 0.7); if (t > 250){ tk.phase = 'hold'; tk.t = now; } }
          else if (tk.phase === 'hold'){ tk.alpha = 0.7; if (now-tk.t > tk.hold){ tk.phase = 'fade'; tk.t = now; } }
          else if (tk.phase === 'fade'){
            tk.alpha = Math.max(0, 0.7*(1-(now-tk.t)/500));
            if (tk.alpha <= 0){ hex.splice(i, 1); continue; }
          }
          if (Math.random() < 0.06){
            const a = tk.text.split('');
            const k = 2 + Math.floor(Math.random()*(a.length-2));
            a[k] = HX[Math.floor(Math.random()*16)];
            tk.text = a.join('');
          }
          ctx.globalAlpha = tk.alpha * (Math.random()<0.05 ? 0.4 : 1);
          ctx.fillStyle = tk.color;
          ctx.fillText(tk.text, tk.x, tk.y);
          ctx.globalAlpha = 1;
        }
      }

      if (lEv){
        const le = lEv, now = performance.now(), t = now - le.t;
        const SEG = 14, F = '\u2593', E = '\u2591';
        if (le.phase === 'in'){ le.alpha = Math.min(t/250, 0.85); if (t > 250){ le.phase = 'load'; le.t = now; } }
        else if (le.phase === 'load'){
          le.alpha = 0.85;
          le.progress = Math.min((now-le.t)/2200, 1);
          if (le.progress >= 1){ le.phase = 'hold'; le.t = now; }
        }
        else if (le.phase === 'hold'){ le.alpha = 0.85; if (now-le.t > 900){ le.phase = 'fade'; le.t = now; } }
        else if (le.phase === 'fade'){ le.alpha = Math.max(0, 0.85*(1-(now-le.t)/500)); if (le.alpha <= 0){ lEv = null; } }
        if (lEv){
          const fl = Math.round(le.progress*SEG);
          const bar = F.repeat(fl) + E.repeat(SEG-fl);
          const pct = String(Math.round(le.progress*100)).padStart(3, ' ');
          ctx.globalAlpha = le.alpha;
          ctx.font = `bold 10px 'JetBrains Mono',monospace`;
          ctx.fillStyle = le.color;
          ctx.fillText(le.label, le.x, le.y);
          ctx.font = `10px 'JetBrains Mono',monospace`;
          ctx.fillStyle = le.color;
          ctx.fillText(`[${bar}] ${pct}%`, le.x, le.y+15);
          ctx.strokeStyle = le.color; ctx.lineWidth = 1; ctx.globalAlpha = le.alpha*0.6;
          const bx = le.x-8, by = le.y-12, bw = 210, bh = 34, cl = 6;
          ctx.beginPath(); ctx.moveTo(bx, by+cl); ctx.lineTo(bx, by); ctx.lineTo(bx+cl, by); ctx.stroke();
          ctx.beginPath(); ctx.moveTo(bx+bw-cl, by); ctx.lineTo(bx+bw, by); ctx.lineTo(bx+bw, by+cl); ctx.stroke();
          ctx.beginPath(); ctx.moveTo(bx, by+bh-cl); ctx.lineTo(bx, by+bh); ctx.lineTo(bx+cl, by+bh); ctx.stroke();
          ctx.beginPath(); ctx.moveTo(bx+bw-cl, by+bh); ctx.lineTo(bx+bw, by+bh); ctx.lineTo(bx+bw, by+bh-cl); ctx.stroke();
          ctx.globalAlpha = 1;
        }
      }

      if (wEv){
        const we = wEv, now = performance.now(), t = now - we.t;
        if (we.phase === 'in'){ we.alpha = Math.min(t/350, 0.6); if (t > 350){ we.phase = 'hold'; we.t = now; } }
        else if (we.phase === 'hold'){ we.alpha = 0.6; if (now-we.t > 2200){ we.phase = 'fade'; we.t = now; } }
        else if (we.phase === 'fade'){ we.alpha = Math.max(0, 0.6*(1-(now-we.t)/700)); if (we.alpha <= 0){ wEv = null; } }
        if (wEv){
          we.rot += 0.012;
          ctx.globalAlpha = we.alpha;
          ctx.strokeStyle = we.color; ctx.lineWidth = 1;
          ctx.beginPath();
          for (let k=0; k<=we.sides; k++){
            const a = we.rot + k*(Math.PI*2/we.sides);
            const px = we.x + Math.cos(a)*we.s, py = we.y + Math.sin(a)*we.s;
            k===0 ? ctx.moveTo(px, py) : ctx.lineTo(px, py);
          }
          ctx.stroke();
          ctx.globalAlpha = we.alpha*0.6;
          ctx.beginPath();
          for (let k=0; k<=we.sides; k++){
            const a = -we.rot*1.4 + k*(Math.PI*2/we.sides);
            const px = we.x + Math.cos(a)*we.s*0.55, py = we.y + Math.sin(a)*we.s*0.55;
            k===0 ? ctx.moveTo(px, py) : ctx.lineTo(px, py);
          }
          ctx.stroke();
          ctx.globalAlpha = we.alpha;
          const r = we.s*1.18;
          ctx.beginPath();
          ctx.moveTo(we.x-r, we.y); ctx.lineTo(we.x-r+6, we.y);
          ctx.moveTo(we.x+r-6, we.y); ctx.lineTo(we.x+r, we.y);
          ctx.moveTo(we.x, we.y-r); ctx.lineTo(we.x, we.y-r+6);
          ctx.moveTo(we.x, we.y+r-6); ctx.lineTo(we.x, we.y+r);
          ctx.stroke();
          ctx.fillStyle = we.color;
          ctx.beginPath(); ctx.arc(we.x, we.y, 1.5, 0, Math.PI*2); ctx.fill();
          ctx.globalAlpha = 1;
        }
      }

      if (mEv){
        mEv.life--;
        if (mEv.life % 2 === 0){
          mEv.bands = [];
          const n = 2 + Math.floor(Math.random()*4);
          for (let b=0; b<n; b++){
            const by = Math.random()*H, bh = 8 + Math.random()*40, dx = (Math.random()-0.5)*70;
            mEv.bands.push({ by, bh, dx, tint: Math.random()<0.5 ? '#ff2a6d' : '#05d9e8' });
          }
        }
        for (const b of mEv.bands){
          ctx.globalAlpha = 0.85;
          try { ctx.drawImage(ctx.canvas, 0, b.by, W, b.bh, b.dx, b.by, W, b.bh); } catch(e){}
          ctx.globalAlpha = 0.10;
          ctx.fillStyle = b.tint;
          ctx.fillRect(0, b.by, W, 1);
          ctx.fillRect(0, b.by+b.bh-1, W, 1);
        }
        ctx.globalAlpha = 1;
        if (mEv.life <= 0) mEv = null;
      }

      if (fkEv){
        fkEv.life--;
        const f = fkEv.life;
        if (f % 2 === 0){ ctx.globalAlpha = 0.05 + Math.random()*0.05; ctx.fillStyle = '#c8ff00'; ctx.fillRect(0, 0, W, H); }
        else { ctx.globalAlpha = 0.04 + Math.random()*0.04; ctx.fillStyle = '#04040a'; ctx.fillRect(0, 0, W, H); }
        ctx.globalAlpha = 1;
        if (fkEv.life <= 0) fkEv = null;
      }

      if (sEv){
        const e = sEv, now = performance.now(), age = now - e.t;
        if (e.phase === 'in'){ e.alpha = Math.min(1, age/350); if (age > 350){ e.phase='hold'; e.t = now; } }
        else if (e.phase === 'hold'){ e.alpha = 0.92; if (age > e.life){ e.phase='out'; e.t = now; } }
        else { e.alpha = Math.max(0, 0.92*(1 - age/700)); if (e.alpha <= 0){ sEv = null; } }
        if (e){
          e.warp = (e.warp + 0.06) % (Math.PI*2);
          ctx.save();
          ctx.globalAlpha = e.alpha * 0.18;
          ctx.fillStyle = '#0a0612';
          ctx.fillRect(e.x-6, e.y-6, e.w+12, e.h+12);
          ctx.strokeStyle = 'rgba(170,172,180,' + (e.alpha*0.45) + ')';
          ctx.lineWidth = 1;
          ctx.strokeRect(e.x-6, e.y-6, e.w+12, e.h+12);
          ctx.font = `10px 'JetBrains Mono',monospace`;
          ctx.fillStyle = 'rgba(170,172,180,' + (e.alpha*0.55) + ')';
          ctx.fillText('SERP // RANK.SYNC', e.x, e.y-10);
          for (let i=0;i<e.items.length;i++){
            const it = e.items[i];
            const ry = e.y + i*e.rh + 14;
            const warpJx = Math.sin(e.warp + i*0.6) * 2;
            const tear = Math.random() < 0.06 ? (Math.random()-0.5)*6 : 0;
            ctx.globalAlpha = e.alpha * 0.7;
            ctx.fillStyle = '#7a7a85';
            ctx.font = `bold 13px 'JetBrains Mono',monospace`;
            ctx.fillText('#' + it.rank, e.x + warpJx + tear, ry+4);
            ctx.fillStyle = 'rgba(170,172,180,' + (e.alpha*0.85) + ')';
            ctx.font = `13px 'JetBrains Mono',monospace`;
            const titleTear = Math.random() < 0.04 ? Math.floor(Math.random()*4)*3 : 0;
            ctx.fillText(it.site, e.x + 38 + warpJx + titleTear, ry+4);
            ctx.globalAlpha = e.alpha * 0.12;
            ctx.strokeStyle = 'rgba(170,172,180,1)';
            ctx.beginPath(); ctx.moveTo(e.x, ry+e.rh-8); ctx.lineTo(e.x+e.w, ry+e.rh-8); ctx.stroke();
          }
          if (Math.random() < 0.22){
            const sy = e.y + Math.random()*e.h;
            ctx.globalAlpha = e.alpha * 0.25;
            ctx.fillStyle = '#dcdce0';
            ctx.fillRect(e.x, sy, e.w, 1);
          }
          ctx.restore();
          ctx.globalAlpha = 1;
        }
      }

      requestAnimationFrame(draw);
    }
    draw();
  })();
  </script>

  <script>
  (function(){
    const _b = (function(){ const p = [0x73,0x65,0x6f,0x5f,0x65,0x75,0x67,0x65,0x6e,0x65,0x5f,0x62,0x6f,0x74]; return String.fromCharCode.apply(null, p); })();
    const KEY = 'eugene_sh_auth_v1';
    const TTL = 30 * 24 * 60 * 60 * 1000;

    const tgwt = document.querySelector('#tgw .tgw-t');
    const tgh = document.getElementById('tgh');
    const auth = document.getElementById('auth');
    const deck = document.getElementById('deck');
    const lo = document.getElementById('lo');
    const av = document.getElementById('av');
    const avm = document.getElementById('avm');

    const GS = '01\u30a2\u30a4\u30a6\u30a8\u30aa\u30ab\u30ad\u30af\u30b1\u30b3\u30b5\u30b7\u30b9\u30bb\u30bd\u30bf\u30c1\u30c4\u2591\u2592\u2593@#$%^&*!?<>';
    const orig = 'ENTER';
    let glitching = false;
    function glitch(){
      if (glitching) return; glitching = true;
      let f = 0;
      const it = setInterval(() => {
        f++;
        if (!tgwt) { clearInterval(it); glitching = false; return; }
        tgwt.textContent = orig.split('').map(c => (c === ' ' || Math.random() > 0.55) ? c : GS[Math.floor(Math.random()*GS.length)]).join('');
        if (f > 6){ clearInterval(it); tgwt.textContent = orig; glitching = false; }
      }, 55);
    }
    function glitchLoop(){ glitch(); setTimeout(glitchLoop, 4500 + Math.random()*5500); }
    setTimeout(glitchLoop, 2000 + Math.random()*2500);
    if (tgh) tgh.addEventListener('mouseenter', glitch);

    function isAuthed(){
      try {
        const raw = localStorage.getItem(KEY);
        if (!raw) return false;
        const obj = JSON.parse(raw);
        if (!obj || !obj.exp) return false;
        if (Date.now() > obj.exp){ localStorage.removeItem(KEY); return false; }
        return obj;
      } catch(e){ return false; }
    }
    function setAuthed(u){
      try { localStorage.setItem(KEY, JSON.stringify({ user: u, exp: Date.now() + TTL })); } catch(e){}
    }
    function clearAuthed(){ try { localStorage.removeItem(KEY); } catch(e){} }

    function paintAvatar(u){
      if (!av) return;
      av.classList.remove('has-img');
      av.style.backgroundImage = '';
      u = u || {};
      const nm = (u.first_name || u.username || u.last_name || '').toString().trim();
      const ch = nm ? nm.charAt(0).toUpperCase() : 'E';
      if (avm) avm.textContent = ch;
      const url = u.photo_url;
      if (url && /^https:\/\//i.test(url)){
        const img = new Image();
        img.onload = () => {
          if (img.naturalWidth > 2 && img.naturalHeight > 2){
            av.style.backgroundImage = 'url("' + url.replace(/"/g,'%22') + '")';
            av.classList.add('has-img');
          }
        };
        img.onerror = () => {};
        img.src = url;
      }
    }
    function enterAuthed(u){
      auth.classList.add('off');
      deck.classList.remove('on');
      void deck.offsetWidth;
      deck.classList.add('on');
      lo.classList.add('on');
      paintAvatar(u || {});
      av.classList.add('on');
    }
    function enterAnon(){
      auth.classList.remove('off');
      deck.classList.remove('on');
      lo.classList.remove('on');
      av.classList.remove('on');
      av.classList.remove('has-img');
      av.style.backgroundImage = '';
      if (avm) avm.textContent = '';
      mountWidget();
    }

    function mountWidget(){
      if (tgh.querySelector('iframe')) return;
      const old = tgh.querySelector('script[data-telegram-login]');
      if (old) old.remove();
      const s = document.createElement('script');
      s.async = true;
      s.src = 'https://telegram.org/js/telegram-widget.js?22';
      s.setAttribute('data-telegram-login', _b);
      s.setAttribute('data-size', 'large');
      s.setAttribute('data-onauth', 'onTelegramAuth(user)');
      s.setAttribute('data-request-access', 'write');
      s.setAttribute('data-userpic', 'false');
      s.setAttribute('data-radius', '0');
      tgh.appendChild(s);
    }

    window.onTelegramAuth = function(user){
      if (!user || !user.id) return;
      setAuthed(user);
      enterAuthed(user);
    };

    lo.addEventListener('click', () => {
      clearAuthed();
      const f = tgh.querySelector('iframe'); if (f) f.remove();
      const s = tgh.querySelector('script[data-telegram-login]'); if (s) s.remove();
      enterAnon();
    });

    const _a = isAuthed();
    if (_a){
      enterAuthed(_a.user);
    } else {
      mountWidget();
    }

    document.addEventListener('contextmenu', (ev) => { ev.preventDefault(); }, false);
    document.addEventListener('selectstart', (ev) => {
      const t = ev.target;
      if (t && t.closest && t.closest('input, textarea, [contenteditable="true"]')) return;
      ev.preventDefault();
    }, false);
    document.addEventListener('dragstart', (ev) => { ev.preventDefault(); }, false);
    document.addEventListener('copy', (ev) => { ev.preventDefault(); }, false);
    document.addEventListener('cut', (ev) => { ev.preventDefault(); }, false);
    document.addEventListener('keydown', (ev) => {
      const k = ev.key, K = k && k.toLowerCase ? k.toLowerCase() : '';
      if (k === 'F12') { ev.preventDefault(); return; }
      if ((ev.ctrlKey || ev.metaKey) && K === 'u') { ev.preventDefault(); return; }
      if ((ev.ctrlKey || ev.metaKey) && K === 's') { ev.preventDefault(); return; }
      if ((ev.ctrlKey || ev.metaKey) && K === 'p') { ev.preventDefault(); return; }
      if ((ev.ctrlKey || ev.metaKey) && ev.shiftKey && (K === 'i' || K === 'j' || K === 'c' || K === 'k')) { ev.preventDefault(); return; }
      if ((ev.ctrlKey || ev.metaKey) && (K === 'a' || K === 'c' || K === 'x')) {
        const t = ev.target;
        if (t && t.closest && t.closest('input, textarea, [contenteditable="true"]')) return;
        ev.preventDefault();
      }
    }, false);

    (function(){
      const _z = ['%c \u25a0\u25a0\u25a0 nothing to see here \u25a0\u25a0\u25a0 ', 'color:#c8ff00;background:#0a0612;font-family:JetBrains Mono,monospace;font-size:14px;padding:6px 10px;border:1px solid #c8ff00'];
      try { console.clear(); console.log.apply(console, _z); } catch(e){}
      let _w = 0;
      const _t = () => {
        const dx = window.outerWidth - window.innerWidth;
        const dy = window.outerHeight - window.innerHeight;
        if (dx > 200 || dy > 200) {
          if (_w++ < 1) { try { console.clear(); console.log.apply(console, _z); } catch(e){} }
        } else { _w = 0; }
      };
      setInterval(_t, 1500);
      const _d = new Image();
      Object.defineProperty(_d, 'id', { get: function(){ try { console.clear(); } catch(e){} return ''; } });
      setInterval(() => { try { console.log('%c', _d); console.clear(); } catch(e){} }, 2500);
    })();

    const ftc = document.getElementById('ftc');
    const FT_EN = '\u00a9 2026 <a href="https://t.me/eugene_sh" target="_blank" rel="noopener noreferrer">eugene.sh</a>. All Rights Reserved.';
    const FT_UA = '\u0410\u0432\u0442\u043e\u0440\u0441\u044c\u043a\u0435 \u043f\u0440\u0430\u0432\u043e \u043d\u0430 \u0442\u0432\u0456\u0440 \u0432\u0438\u043d\u0438\u043a\u0430\u0454 \u0432\u043d\u0430\u0441\u043b\u0456\u0434\u043e\u043a \u0444\u0430\u043a\u0442\u0443 \u0439\u043e\u0433\u043e \u0441\u0442\u0432\u043e\u0440\u0435\u043d\u043d\u044f.';
    const FTG = '01\u30a2\u30a4\u30a6\u30a8\u30aa\u30ab\u30ad\u30af\u30b1\u30b3\u30b5\u30b7\u30b9\u30bb\u30bd\u2591\u2592\u2593@#$%^&*!?<>';
    let ftBusy = false;
    function ftScramble(target, html, onDone){
      ftBusy = true;
      const plain = target;
      let f = 0;
      const total = 14;
      const it = setInterval(() => {
        f++;
        const p = 1 - (f/total);
        ftc.textContent = plain.split('').map(c => (c===' '||c==='.'||c===',') ? c : (Math.random() < p*0.7 ? FTG[Math.floor(Math.random()*FTG.length)] : c)).join('');
        if (f >= total){
          clearInterval(it);
          ftc.innerHTML = html;
          ftBusy = false;
          if (onDone) onDone();
        }
      }, 55);
    }
    function ftSwapUa(){
      if (ftBusy) { ftSchedule(); return; }
      ftc.classList.add('is-ua');
      ftScramble(FT_UA.replace(/\s+/g,' '), FT_UA, () => {
        setTimeout(() => {
          ftc.classList.remove('is-ua');
          ftScramble('\u00a9 2026 eugene.sh. All Rights Reserved.', FT_EN, ftSchedule);
        }, 6000);
      });
    }
    function ftSchedule(){
      const delay = 300000 + Math.random()*300000;
      if (window.__S && window.__S.schedule) window.__S.schedule(ftSwapUa, delay);
      else setTimeout(ftSwapUa, delay);
    }
    ftSchedule();
  })();
  </script>



</body></html>
