<!DOCTYPE html>
<html lang="en" translate="no" class="notranslate">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="google" content="notranslate">
<meta http-equiv="Content-Language" content="en">
<title>SUSULAN ULANGAN HARIAN 1 BAHASA INGGRIS KELAS XI - SMA NEGERI 1 SUMPIUH</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Fraunces:opsz,wght@9..144,500;9..144,600;9..144,700&family=Inter:wght@400;500;600;700;800&family=JetBrains+Mono:wght@500;600&display=swap" rel="stylesheet">
<style>
  :root{
    --ink:#1a1e24;
    --paper:#f2f6f5;
    --paper-card:#ffffff;
    --line:#dde5e2;
    --muted:#6e7a78;
    --navy:#0f2a44;
    --cream:#d9ecfb;
    --good:#1f9d68;
    --good-bg:#e7f6ee;
    --bad:#d5473a;
    --bad-bg:#fceceb;

    --t1:#2f6fed;
    --t1-bg:#eaf1fe;
    --t2:#12946a;
    --t2-bg:#e6f7f0;
    --t3:#d97706;
    --t3-bg:#fdf1de;
    --t4:#c2255c;
    --t4-bg:#fce8f1;
  }

  *{box-sizing:border-box;}
  html,body{margin:0;padding:0;}
  body{
    background:var(--paper);
    color:var(--ink);
    font-family:'Inter',system-ui,sans-serif;
    line-height:1.55;
    padding-bottom:96px;
    -webkit-user-select:none;
    -moz-user-select:none;
    -ms-user-select:none;
    user-select:none;
    -webkit-touch-callout:none;
  }
  input, textarea, select{
    -webkit-user-select:text;
    -moz-user-select:text;
    -ms-user-select:text;
    user-select:text;
  }
  img{ -webkit-user-drag:none; pointer-events:none; }

  h1,h2,h3{font-family:'Fraunces',Georgia,serif;margin:0;}
  .wrap{max-width:820px;margin:0 auto;padding:0 20px;}

  .cover{
    background:var(--navy); color:var(--cream);
    padding:40px 0 30px; border-bottom:6px solid var(--t1);
  }
  .eyebrow{
    font-family:'JetBrains Mono',monospace; font-size:12px;
    letter-spacing:.14em; text-transform:uppercase; color:#a9a6c4; margin-bottom:10px;
  }
  .cover h1{
    font-size:clamp(24px,4.2vw,32px); font-weight:600; line-height:1.18; max-width:640px;
  }
  .cover p.desc{ color:#c9c6da; max-width:560px; margin-top:12px; font-size:14.5px; }
  .id-card{
    margin-top:22px; background:rgba(255,255,255,.06); border:1px solid rgba(255,255,255,.16);
    border-radius:14px; padding:16px 18px; display:grid; grid-template-columns:1fr 1fr; gap:14px;
  }
  @media (max-width:520px){ .id-card{grid-template-columns:1fr;} }
  .id-field label{
    display:block; font-family:'JetBrains Mono',monospace; font-size:11px;
    letter-spacing:.08em; text-transform:uppercase; color:#a9a6c4; margin-bottom:6px;
  }
  .id-field input{
    width:100%; background:rgba(255,255,255,.08); border:1px solid rgba(255,255,255,.2);
    border-radius:8px; padding:10px 12px; color:#fff; font-size:16px; font-family:'Inter',sans-serif; outline:none;
  }
  .id-field input::placeholder{color:#8b88a3;}
  .id-field input:focus{border-color:var(--t3);background:rgba(255,255,255,.13);}

  .progress-shell{
    position:sticky; top:0; z-index:30; background:var(--paper);
    border-bottom:1px solid var(--line); padding:10px 0; transition:transform 0.3s ease, opacity 0.3s ease;
  }
  .progress-shell.collapsed{
    transform: translateY(-100%);
    opacity: 0;
    pointer-events: none;
    height: 0;
    padding: 0;
    border: none;
    overflow: hidden;
  }
  .progress-inner{ display:flex; align-items:center; gap:12px; flex-wrap:wrap; }
  .progress-track{ flex:1 1 140px; height:8px; background:var(--line); border-radius:99px; overflow:hidden; min-width:100px; }
  .progress-fill{ height:100%; width:0%; background:linear-gradient(90deg,var(--t1),var(--t4)); transition:width .3s ease; }
  .progress-label{ font-family:'JetBrains Mono',monospace; font-size:12.5px; color:var(--muted); white-space:nowrap; }
  .palette-toggle{
    font-family:'Inter',sans-serif; font-size:12.5px; font-weight:600;
    background:#fff; border:1px solid var(--line); color:var(--ink);
    padding:6px 12px; border-radius:99px; cursor:pointer;
    transition:background .15s ease, border-color .15s ease;
    display:flex; align-items:center; gap:6px;
  }
  .palette-toggle:hover{background:#f3f1ea; border-color:#d7d3c4;}

  /* Tombol hide/show header, diletakkan sebaris di sebelah tombol soal */
  .header-toggle-inline{
    font-family:'Inter',sans-serif; font-size:11px; font-weight:600;
    background:var(--navy); color:#fff; border:1px solid rgba(255,255,255,.2);
    padding:4px 9px; border-radius:99px; cursor:pointer;
    box-shadow: 0 2px 6px rgba(0,0,0,0.12);
    display: inline-flex; align-items: center; gap: 4px;
    transition: background 0.15s ease;
    white-space:nowrap;
  }
  .header-toggle-inline:hover{background:#183e66;}

  /* Rumah tombol saat header disembunyikan, supaya tetap bisa ditekan lagi */
  .header-toggle-home{
    position: fixed;
    top: 10px;
    right: 14px;
    z-index: 50;
  }

  .timer-badge{
    font-family:'JetBrains Mono',monospace; font-size:13px; font-weight:700; color:var(--ink);
    background:#eef0fb; border:1px solid #c9cdf0; padding:6px 12px; border-radius:99px; white-space:nowrap;
  }
  .timer-badge.warn{background:var(--t3-bg); border-color:var(--t3); color:#7a4e0a;}
  .timer-badge.danger{background:var(--bad-bg); border-color:var(--bad); color:var(--bad); animation:timerPulse 1s infinite;}
  .timer-badge.paused{background:#fff3cd; border-color:#ffeeba; color:#856404;}
  @keyframes timerPulse{ 0%,100%{opacity:1;} 50%{opacity:.55;} }

  .online-badge{
    font-family:'JetBrains Mono',monospace; font-size:12.5px; font-weight:700;
    padding:6px 12px; border-radius:99px; white-space:nowrap; display:flex; align-items:center; gap:6px;
  }
  .online-badge .online-dot{ width:8px; height:8px; border-radius:50%; display:inline-block; flex:none; }
  .online-badge.online{ background:var(--good-bg); border:1px solid var(--good); color:var(--good); }
  .online-badge.online .online-dot{ background:var(--good); animation:onlinePulse 1.6s infinite; }
  .online-badge.offline{ background:var(--bad-bg); border:1px solid var(--bad); color:var(--bad); }
  .online-badge.offline .online-dot{ background:var(--bad); }
  @keyframes onlinePulse{ 0%,100%{opacity:1;} 50%{opacity:.4;} }

  .palette-panel{
    display:none; background:var(--paper-card); border:1px solid var(--line); border-radius:12px;
    padding:16px; margin-top:14px;
  }
  .palette-panel.open{display:block;}
  .palette-legend{
    display:flex; gap:14px; flex-wrap:wrap; font-size:11.5px; color:var(--muted);
    margin-bottom:12px; font-family:'JetBrains Mono',monospace;
  }
  .palette-legend span{display:inline-flex; align-items:center; gap:5px;}
  .legend-dot{width:9px; height:9px; border-radius:3px; display:inline-block;}
  .palette-grid{ display:grid; grid-template-columns:repeat(auto-fill,minmax(38px,1fr)); gap:8px; }
  .pnum{
    aspect-ratio:1; border-radius:8px; border:1.5px solid var(--line); background:#fff;
    font-family:'JetBrains Mono',monospace; font-size:13px; font-weight:700; color:var(--muted);
    cursor:pointer; display:flex; align-items:center; justify-content:center; transition:transform .1s ease;
  }
  .pnum:hover{transform:translateY(-1px);}
  .pnum.pn-current{border-color:var(--navy); border-width:2px; color:var(--navy);}
  .pnum.pn-answered{background:#eef0fb; border-color:#c9cdf0; color:var(--navy);}

  .results{
    display:none; background:var(--paper-card); border:1px solid var(--line); border-radius:14px;
    padding:24px 26px; margin:24px 0 6px; text-align:center;
  }
  .results.show{display:block;}
  .results .score-big{ font-family:'Fraunces',serif; font-size:48px; font-weight:700; line-height:1; color:var(--navy); margin-bottom:6px; }
  .results .score-sub{color:var(--muted); font-size:14px; margin-bottom:14px;}
  .results .score-msg{ font-size:15px; font-weight:600; padding:9px 16px; border-radius:99px; display:inline-block; }
  .submit-row{margin-top:18px; display:flex; flex-direction:column; align-items:center; gap:8px;}
  .submit-row .primary{padding:12px 22px; font-size:14.5px;}
  .submit-row .primary:disabled{opacity:.55; cursor:not-allowed; transform:none;}
  .send-note{font-family:'JetBrains Mono',monospace; font-size:12.5px; min-height:16px;}
  .send-note.ok{color:var(--good);}
  .send-note.err{color:var(--bad);}
  .retry-send{border-color:var(--bad); color:var(--bad);}
  .retry-send:hover{background:var(--bad-bg);}

  .stage{margin-top:22px;}
  .stage-head{ display:flex; align-items:center; justify-content:space-between; gap:10px; margin-bottom:14px; flex-wrap:wrap; }
  .genre-tag{
    font-family:'JetBrains Mono',monospace; font-size:11.5px; letter-spacing:.09em; text-transform:uppercase;
    padding:5px 11px; border-radius:99px; font-weight:600;
  }
  .stage-index{ font-family:'JetBrains Mono',monospace; font-size:12.5px; color:var(--muted); }

  .pin-toggle{
    font-family:'Inter',sans-serif; font-size:12px; font-weight:600;
    background:#fff; border:1px solid var(--line); color:var(--ink);
    padding:6px 11px; border-radius:99px; cursor:pointer;
    display:flex; align-items:center; gap:5px; margin-left:auto; flex-shrink:0;
    transition:background .15s ease, border-color .15s ease, color .15s ease;
  }
  .pin-toggle:hover{background:#f3f1ea; border-color:#d7d3c4;}
  .pin-toggle.active{background:var(--t1-bg); border-color:var(--t1); color:var(--t1);}
  .pin-toggle .pin-ic{font-size:13px; line-height:1; transform:rotate(0deg); transition:transform .15s ease;}
  .pin-toggle.active .pin-ic{transform:rotate(35deg);}

  .stage.pin-mode{position:relative;}
  .stage.pin-mode .passage{padding-bottom:54vh;}
  .stage.pin-mode .q-card{
    position:fixed; left:50%; bottom:0; transform:translateX(-50%);
    width:calc(100% - 40px); max-width:780px; margin:0;
    height:50vh; overflow-y:auto; -webkit-overflow-scrolling:touch;
    z-index:35; border-radius:16px 16px 0 0;
    box-shadow:0 -10px 26px rgba(28,27,34,.18);
    padding-bottom:26px;
  }
  @media (max-width:640px){
    .stage.pin-mode .q-card{width:calc(100% - 20px); height:50vh;}
    .stage.pin-mode .passage{padding-bottom:52vh;}
  }

  .passage{
    background:var(--paper-card); border:1px solid var(--line); border-left-width:5px;
    border-radius:10px; padding:20px 22px; margin-bottom:20px; font-size:14.5px;
  }
  .passage h3{font-size:17px; margin-bottom:10px; font-weight:600;}
  .passage p{margin:0 0 11px; color:#33313c; text-align:justify; text-indent:1.5em;}
  .passage p:last-child{margin-bottom:0;}
  .passage-img{width:100%; max-height:340px; object-fit:cover; border-radius:10px; margin:2px 0 14px; display:block;}
  .passage .meta{
    font-family:'JetBrains Mono',monospace; font-size:11.5px; color:var(--muted); margin-bottom:12px; letter-spacing:.03em;
  }

  .q-card{
    background:var(--paper-card); border:1px solid var(--line); border-radius:12px;
    padding:20px 22px 22px; transition:border-color .2s ease, box-shadow .2s ease;
  }
  .q-top{display:flex; gap:12px; align-items:flex-start; margin-bottom:14px; flex-wrap:wrap;}
  .q-num{
    font-family:'JetBrains Mono',monospace; font-weight:700; font-size:14px;
    min-width:32px; height:32px; border-radius:99px; display:flex; align-items:center; justify-content:center; flex-shrink:0;
  }
  .q-prompt{font-size:16px; font-weight:600; padding-top:4px;}
  .q-hint{ font-size:12px; color:var(--muted); font-style:italic; margin:-6px 0 12px 44px; }

  .options{display:flex; flex-direction:column; gap:9px; margin-left:44px;}
  .opt{
    display:flex; align-items:flex-start; gap:10px; padding:10px 13px; border:1px solid var(--line); border-radius:8px;
    cursor:pointer; font-size:14.5px; background:#fff; transition:background .15s ease, border-color .15s ease;
  }
  .opt:hover{background:#faf9f5;}
  .opt input{margin-top:3px; accent-color:currentColor; flex-shrink:0;}
  .opt.selected{background:#f1eefc; border-color:var(--t1);}
  .opt input:disabled{cursor:default;}
  .opt.locked{cursor:default;}

  .matrix{margin-left:44px; border:1px solid var(--line); border-radius:8px; overflow:hidden;}
  .matrix table{width:100%; border-collapse:collapse; font-size:14px; table-layout:fixed;}
  .matrix th{
    font-family:'JetBrains Mono',monospace; font-size:10.5px; text-transform:uppercase; letter-spacing:.06em;
    color:var(--muted); background:#faf9f5; padding:9px 10px; text-align:center; border-bottom:1px solid var(--line);
  }
  .matrix th:first-child{text-align:left;}
  .matrix td{padding:10px; border-bottom:1px solid var(--line); vertical-align:middle;}
  .matrix tr:last-child td{border-bottom:none;}
  .matrix td.stmt{color:#33313c; width:44%;}
  .matrix th:first-child, .matrix td.stmt{width:44%;}
  .matrix td.pick{text-align:center; width:28%;}
  .matrix th:not(:first-child){width:28%;}
  .matrix input{accent-color:currentColor;}

  .answer-note{
    margin:12px 0 0 44px; font-size:13px; padding:9px 12px; border-radius:8px;
    background:var(--bad-bg); color:#8a2e26; display:none;
  }
  .answer-note.show{display:block;}
  .answer-note b{color:var(--bad);}

  @media (max-width:640px){
    .wrap{padding:0 10px;}
    .stage{margin-top:16px;}
    .passage{padding:14px 12px; font-size:15.5px; line-height:1.6;}
    .passage p{text-indent:1.2em;}
    .passage h3{font-size:16.5px;}
    .q-card{padding:16px 14px 18px;}
    .q-top{gap:10px; margin-bottom:12px;}
    .q-num{min-width:28px; height:28px; font-size:13px;}
    .q-prompt{font-size:15.5px; line-height:1.42;}
    .q-hint{margin-left:0; margin-top:2px; line-height:1.4;}
    .options{margin-left:0; gap:8px;}
    .opt{padding:11px 12px; font-size:15px; line-height:1.4; gap:9px;}
    .matrix{margin-left:0; margin-right:0; width:100%;}
    .matrix table{font-size:12.5px;}
    .matrix th{font-size:9px; padding:7px 5px; letter-spacing:.02em;}
    .matrix td{padding:8px 6px;}
    .matrix td.stmt, .matrix th:first-child{width:40%;}
    .matrix td.pick, .matrix th:not(:first-child){width:30%;}
    .answer-note{margin-left:0;}
  }

  .nav-bar{
    position:fixed; bottom:0; left:0; right:0; z-index:40;
    background:var(--navy); border-top:1px solid rgba(255,255,255,.1); padding:8px 0;
  }
  .nav-inner{ display:flex; align-items:center; justify-content:space-between; gap:8px; flex-wrap:nowrap; }
  button.navbtn{
    background:rgba(255,255,255,.08); color:#fff; border:1px solid rgba(255,255,255,.2);
    padding:9px 14px; border-radius:99px; font-size:13px; cursor:pointer;
    font-family:'Inter',sans-serif; font-weight:600; transition:background .15s ease;
    flex:1 1 0; text-align:center; white-space:nowrap;
  }
  button.navbtn:hover{background:rgba(255,255,255,.16);}
  button.navbtn:disabled{opacity:.35; cursor:not-allowed;}
  button.primary{
    background:var(--t3); color:#241a05; border:none; font-weight:700;
    padding:9px 14px; border-radius:99px; font-size:13px; cursor:pointer;
    font-family:'Inter',sans-serif; transition:transform .12s ease, background .15s ease;
    flex:1 1 0; white-space:nowrap;
  }
  button.primary:hover{transform:translateY(-1px); background:#dc9b28;}
  button.primary:disabled{opacity:.5; cursor:not-allowed; transform:none;}
  button.ghost{
    background:transparent; color:#c9c6da; border:1px solid rgba(255,255,255,.25);
    padding:9px 12px; border-radius:99px; font-size:13px; cursor:pointer; font-family:'Inter',sans-serif;
    flex:0 0 auto; white-space:nowrap;
  }
  button.ghost:hover{border-color:rgba(255,255,255,.5); color:#fff;}

  @media (max-width:480px){
    body{padding-bottom:70px;}
    .nav-bar{padding:7px 0;}
    .nav-inner{gap:5px;}
    button.navbtn, button.primary, button.ghost{ padding:8px 6px; font-size:11.5px; }
    button.ghost{flex:0 0 auto; padding:8px 9px;}
  }

  ::selection{background:var(--cream);}

  .gate-screen{
    position:fixed; inset:0; z-index:100; background:var(--navy);
    display:flex; align-items:center; justify-content:center; padding:24px;
  }
  .gate-card{
    background:rgba(255,255,255,.06); border:1px solid rgba(255,255,255,.16); border-radius:16px;
    padding:28px 26px; max-width:400px; width:100%; color:var(--cream);
  }
  .gate-card h1{ font-size:21px; font-weight:600; color:var(--cream); margin:6px 0 8px; line-height:1.3; }
  .gate-card .desc{color:#c9c6da; font-size:14px; margin:0 0 18px;}
  .gate-field{margin-bottom:14px;}
  .gate-field label{
    display:block; font-family:'JetBrains Mono',monospace; font-size:11px;
    letter-spacing:.08em; text-transform:uppercase; color:#a9a6c4; margin-bottom:6px;
  }
  .gate-field input, .gate-field select{
    width:100%; background:rgba(255,255,255,.08); border:1px solid rgba(255,255,255,.2);
    border-radius:8px; padding:10px 12px; color:#fff; font-size:16px; font-family:'Inter',sans-serif; outline:none;
  }
  .gate-field select option{ background: var(--navy); color: #fff; }
  .gate-field input::placeholder{color:#8b88a3;}
  .gate-field input:focus, .gate-field select:focus{border-color:var(--t3);background:rgba(255,255,255,.13);}

  /* Confirmation Modal */
  .confirm-modal{
    position:fixed; inset:0; z-index:200; background:rgba(15, 18, 30, 0.75);
    display:none; align-items:center; justify-content:center; padding:20px;
    backdrop-filter: blur(4px);
  }
  .confirm-modal.show{ display:flex; }
  .confirm-card{
    background:var(--paper-card); border:1px solid var(--line); border-radius:16px;
    padding:24px 26px; max-width:420px; width:100%; box-shadow:0 20px 25px -5px rgba(0,0,0,0.2);
    text-align:center;
  }
  .confirm-card h2{ font-size:20px; font-weight:700; color:var(--navy); margin-bottom:10px; }
  .confirm-card p{ font-size:14.5px; color:var(--muted); margin-bottom:20px; line-height:1.5; }
  .confirm-actions{ display:flex; gap:10px; justify-content:center; }
  .confirm-actions button{ flex:1; padding:10px 16px; font-size:14px; border-radius:99px; font-weight:600; cursor:pointer; font-family:'Inter',sans-serif; }
  .btn-cancel{ background:var(--paper); border:1px solid var(--line); color:var(--ink); }
  .btn-cancel:hover{ background:#e8e5dc; }
  .btn-confirm{ background:var(--good); border:none; color:#fff; }
  .btn-confirm:hover{ background:#198256; }

  .gate-error{ color:#ff8c82; font-size:13px; min-height:18px; margin-bottom:6px; font-family:'JetBrains Mono',monospace; }
  .gate-card .primary{width:100%; margin-top:6px;}
  .gate-notice{ color:#c9c6da; font-size:12.5px; margin:-8px 0 16px; line-height:1.5; }
  .gate-notice b{ color:#ff9f8f; }

  /* Exam rules consent popup */
  .rules-modal{
    position:fixed; inset:0; z-index:400; background:rgba(15, 18, 30, 0.8);
    display:none; align-items:center; justify-content:center; padding:20px;
    backdrop-filter: blur(4px);
  }
  .rules-modal.show{ display:flex; }
  .rules-card{
    background:var(--paper-card); border:1px solid var(--line); border-radius:16px;
    padding:26px 26px 22px; max-width:460px; width:100%;
    box-shadow:0 20px 30px -5px rgba(0,0,0,.35);
    text-align:left;
  }
  .rules-card .ricon{ font-size:34px; margin-bottom:8px; text-align:center; }
  .rules-card h2{ font-size:19px; font-weight:700; color:var(--navy); margin-bottom:12px; text-align:center; }
  .rules-card ul{ margin:0 0 16px; padding-left:20px; }
  .rules-card li{ color:var(--ink); font-size:13.5px; line-height:1.6; margin-bottom:6px; }
  .rules-card li b{ color:var(--bad); }
  .rules-agree{
    display:flex; align-items:flex-start; gap:9px; background:var(--bad-bg);
    border:1px solid var(--bad); border-radius:10px; padding:10px 12px; margin-bottom:16px;
    cursor:pointer;
  }
  .rules-agree input{ margin-top:3px; width:16px; height:16px; flex-shrink:0; accent-color:var(--bad); }
  .rules-agree span{ font-size:13px; color:#4a3530; line-height:1.5; }
  .rules-card button{
    width:100%; padding:12px 16px; font-size:14.5px; font-weight:700; border-radius:99px;
    border:none; cursor:pointer; font-family:'Inter',sans-serif;
    background:var(--navy); color:#fff; transition:opacity .15s;
  }
  .rules-card button:disabled{ opacity:.4; cursor:not-allowed; }
  .rules-card button:not(:disabled):hover{ opacity:.9; }

  /* Violation / anti-cheat */
  .violation-modal{
    position:fixed; inset:0; z-index:300; background:rgba(140,20,20,.55);
    display:none; align-items:center; justify-content:center; padding:20px;
    backdrop-filter: blur(4px);
  }
  .violation-modal.show{ display:flex; }
  .violation-card{
    background:#fff; border:2px solid var(--bad); border-radius:16px;
    padding:26px 24px; max-width:420px; width:100%; text-align:center;
    box-shadow:0 20px 30px -5px rgba(0,0,0,.3);
    animation:shake .4s ease;
  }
  @keyframes shake{
    0%,100%{transform:translateX(0);} 20%{transform:translateX(-8px);}
    40%{transform:translateX(8px);} 60%{transform:translateX(-6px);} 80%{transform:translateX(6px);}
  }
  .violation-card .vicon{font-size:40px; margin-bottom:8px;}
  .violation-card h2{ font-size:19px; font-weight:700; color:var(--bad); margin-bottom:8px; }
  .violation-card p{ font-size:14px; color:#4a3530; margin-bottom:6px; line-height:1.5; }
  .violation-card .vcount{
    font-family:'JetBrains Mono',monospace; font-weight:700; font-size:15px;
    color:var(--bad); background:var(--bad-bg); border-radius:8px; padding:6px 10px; display:inline-block; margin:8px 0 16px;
  }
  .violation-card button{
    width:100%; padding:11px 16px; font-size:14.5px; border-radius:99px; font-weight:700;
    cursor:pointer; font-family:'Inter',sans-serif; background:var(--bad); border:none; color:#fff;
  }
  .violation-card button:hover{background:#b8392e;}
  .violation-card .violation-end-btn{
    background:transparent; border:1px solid #d8b6b1; color:#8a5a53;
    margin-top:8px; font-weight:600;
  }
  .violation-card .violation-end-btn:hover{ background:rgba(140,20,20,.08); }

  .violation-badge{
    font-family:'JetBrains Mono',monospace; font-size:12.5px; font-weight:700;
    padding:6px 12px; border-radius:99px; white-space:nowrap;
    background:var(--bad-bg); border:1px solid var(--bad); color:var(--bad);
    display:none; align-items:center; gap:6px;
  }
  .violation-badge.show{ display:flex; }
</style>
</head>
<body>

<div id="gateScreen" class="gate-screen">
  <div class="gate-card">
    <div class="eyebrow">Ulangan Susulan</div>
    <h1>SUSULAN ULANGAN HARIAN 1<br>BAHASA INGGRIS KELAS XI</h1>
    <p class="desc">NARRATIVE TEXT (LEGEND)<br>SMA NEGERI 1 SUMPIUH</p>
    <p class="gate-notice">⚠️ <b>Ujian ini diawasi.</b> Peraturan ujian akan ditampilkan setelah kamu klik Mulai Ujian.</p>
    <div class="gate-field">
      <label for="gateName">Name</label>
      <input id="gateName" type="text" placeholder="Write your full name" autocomplete="off">
    </div>
    <div class="gate-field">
      <label for="gateClass">Class</label>
      <select id="gateClass" class="gate-select">
        <option value="" disabled selected>Select your class</option>
        <option value="XI D1">XI D1</option>
        <option value="XI D2">XI D2</option>
        <option value="XI E1">XI E1</option>
      </select>
    </div>
    <div class="gate-field">
      <label for="gateToken">Exam Token</label>
      <input id="gateToken" type="text" placeholder="Enter token" autocomplete="off" style="text-transform:uppercase;">
    </div>
    <div class="gate-error" id="gateError"></div>
    <button class="primary" id="gateSubmitBtn" type="button">Start Exam</button>
  </div>
</div>

<!-- Popup Peraturan & Persetujuan Ujian -->
<div id="rulesModal" class="rules-modal">
  <div class="rules-card">
    <div class="ricon">⚠️</div>
    <h2>Peraturan Ujian — Harap Dibaca</h2>
    <ul>
      <li>Tetap dalam <b>mode fullscreen (layar penuh)</b> dan di tab ini selama ujian berlangsung.</li>
      <li>Berpindah tab/aplikasi atau keluar dari fullscreen akan memicu <b>alarm + popup peringatan</b>.</li>
      <li>Setiap pelanggaran mengurangi <b>2 poin</b> dari nilai akhir. Pelanggaran bersifat akumulatif — <b>tidak dihapus/diampuni</b>.</li>
      <li>Ujian <b>TIDAK</b> akan otomatis dikirim karena pelanggaran — kamu tetap bisa lanjut mengerjakan, hanya saja nilai berkurang.</li>
      <li>Jika keluar dari fullscreen, gunakan tombol <b>"⛶ Fullscreen"</b> di bagian atas untuk kembali.</li>
    </ul>
    <label class="rules-agree">
      <input type="checkbox" id="rulesAgreeCheck">
      <span>Saya telah membaca dan memahami peraturan di atas, dan saya setuju untuk mematuhinya selama ujian ini.</span>
    </label>
    <button type="button" id="rulesStartBtn" disabled>Mulai Ujian</button>
  </div>
</div>

<!-- Modal Peringatan Pelanggaran -->
<div id="violationModal" class="violation-modal">
  <div class="violation-card">
    <div class="vicon">⚠️</div>
    <h2>Terdeteksi Pelanggaran!</h2>
    <p id="violationMsg">Kamu meninggalkan layar ujian (berpindah tab/aplikasi, atau keluar dari fullscreen).</p>
    <div class="vcount" id="violationCount">Pelanggaran 1 — Nilai -2</div>
    <button type="button" id="violationOkBtn">Saya Mengerti — Kembali ke Ujian</button>
    <button type="button" id="violationEndBtn" class="violation-end-btn">Sudahi Ujian</button>
  </div>
</div>

<div id="confirmModal" class="confirm-modal">
  <div class="confirm-card">
    <h2 id="confirmTitle">Konfirmasi Submit Ujian</h2>
    <p id="confirmMsg">Apakah kamu yakin ingin mengirim jawabanmu? Jawaban tidak bisa diubah lagi setelah dikirim.</p>
    <div class="confirm-actions">
      <button type="button" class="btn-cancel" id="cancelSubmitBtn">Batal</button>
      <button type="button" class="btn-confirm" id="confirmSubmitBtn">Ya, Kirim Sekarang</button>
    </div>
  </div>
</div>

<div id="appMain" style="display:none;">

<input type="hidden" id="stuName">
<input type="hidden" id="stuClass">

<!-- Rumah tombol hide/show header saat header sedang disembunyikan -->
<div class="header-toggle-home" id="headerToggleHome" style="display:none;"></div>

<div class="progress-shell" id="progressShell">
  <div class="wrap progress-inner">
    <button type="button" class="palette-toggle" id="backToLoginBtn"><span>&larr; Login Menu</span></button>
    <div class="online-badge online" id="onlineBadge"><span class="online-dot"></span>Online</div>
    <div class="violation-badge" id="violationBadge">⚠️ 0 (-0)</div>
    <button type="button" class="palette-toggle" id="fullscreenBtn" style="display:none;"><span>⛶ Layar Penuh</span></button>
    <div class="timer-badge" id="timerBadge">90:00</div>
    <div class="progress-track"><div class="progress-fill" id="progressFill"></div></div>
    <div class="progress-label" id="progressLabel">0 / 30 answered</div>
    <button type="button" class="palette-toggle" id="paletteToggleBtn"><span id="paletteToggleText">Semua Soal</span></button>
    <button type="button" class="header-toggle-inline" id="toggleHeaderBtn">
      <span id="toggleIcon">▲</span> <span id="toggleText">Hide/show Header</span>
    </button>
  </div>
  <div class="wrap">
    <div class="palette-panel" id="palettePanel">
      <div class="palette-legend">
        <span><span class="legend-dot" style="background:#fff;border:1.5px solid var(--line);"></span>Not answered</span>
        <span><span class="legend-dot" style="background:#eef0fb;border:1.5px solid #c9cdf0;"></span>Answered</span>
      </div>
      <div class="palette-grid" id="paletteGrid"></div>
    </div>
  </div>
</div>

<div class="wrap">
  <div id="resultsBox" class="results">
    <div class="score-big" id="scoreBig" style="display:none;">0</div>
    <div class="score-sub" id="scoreSub" style="display:none;">Nilai Akhir (0-100)</div>
    <div class="score-msg" id="scoreMsg">Ujian selesai dikerjakan!</div>
    <div class="submit-row">
      <div class="send-note" id="sendNote"></div>
      <button class="ghost retry-send" id="retrySendBtn" type="button" style="display:none;">Try Sending Again</button>
    </div>
  </div>

  <div class="stage" id="stage"></div>
</div>

<div class="nav-bar">
  <div class="wrap nav-inner">
    <button class="ghost" id="resetBtn" type="button" style="display:none;">Reset</button>
    <button class="navbtn" id="prevBtn" type="button">&larr; Prev</button>
    <button class="navbtn" id="nextBtn" type="button">Next &rarr;</button>
    <button class="primary" id="submitBtn" type="button">Submit</button>
  </div>
</div>

</div>

<script>
const DATA = [
  {
    id:'part1',
    tag:'PART 1',
    color:'var(--t1)',
    bg:'var(--t1-bg)',
    title:`Identifying the Main Sentence`,
    meta:`Narrative Text · Legend · Choose the topic sentence · Questions No. 1-5`,
    questions:[
      { id:'q1', no:1, type:'single', prompt:`Choose the sentence that best expresses the main idea of the paragraph.`,
        options:[{k:'A',t:`The villagers placed flowers beside the old well every morning.`}, {k:'B',t:`The old well stood near a group of houses.`}, {k:'C',t:`The villagers became anxious when the old well suddenly stopped giving water.`}, {k:'D',t:`A mysterious event at the old well caused the village to change its attitude toward water.`}],
        correct:'D' },
      { id:'q2', no:2, type:'single', prompt:`Choose the sentence that best expresses the main idea of the paragraph.`,
        options:[{k:'A',t:`A young trader crossed the eastern hills before sunset.`}, {k:'B',t:`The trader found a strange compass inside an abandoned hut.`}, {k:'C',t:`He usually traveled alone because he disliked crowded roads.`}, {k:'D',t:`The trader's decision to trust a mysterious compass helped him survive a difficult journey.`}],
        correct:'D' },
      { id:'q3', no:3, type:'single', prompt:`Choose the sentence that best expresses the main idea of the paragraph.`,
        options:[{k:'A',t:`Several birds gathered around the ancient tree.`}, {k:'B',t:`The tree had very wide branches.`}, {k:'C',t:`A girl visited the tree after hearing a strange sound.`}, {k:'D',t:`A mysterious tree taught the villagers an important lesson about protecting their forest.`}],
        correct:'D' },
      { id:'q4', no:4, type:'single', prompt:`Choose the sentence that best expresses the main idea of the paragraph.`,
        options:[{k:'A',t:`The prince often visited the northern fields.`}, {k:'B',t:`Farmers planted corn near the palace.`}, {k:'C',t:`The prince owned a collection of silver cups.`}, {k:'D',t:`The prince's selfish choice caused the kingdom to lose a valuable natural blessing.`}],
        correct:'D' },
      { id:'q5', no:5, type:'single', prompt:`Choose the sentence that best expresses the main idea of the paragraph.`,
        options:[{k:'A',t:`The traveler walked beside a narrow river.`}, {k:'B',t:`He carried a small wooden box in his bag.`}, {k:'C',t:`An old woman lived near the river.`}, {k:'D',t:`The traveler learned that helping a stranger could lead to an unexpected reward.`}],
        correct:'D' },
    ]
  },
  {
    id:'text1p2',
    tag:'PART 2 · TEXT 1',
    color:'var(--t2)',
    bg:'var(--t2-bg)',
    title:`The Legend of the Amber Bell`,
    meta:`Narrative Text · Legend · Identifying the main idea · Question No. 6`,
    passage:[
      `Long ago, a village stood between two wooded hills. At the center of the village hung an amber bell that was said to ring whenever the community faced an unseen danger. For many years, the villagers ignored the old story. One evening, a young baker named Sena heard the bell ring although nobody had touched it. She warned the villagers and asked them to move their animals to higher ground. Before midnight, heavy rain caused a nearby stream to overflow. Because the animals had already been moved, the villagers suffered little loss.`,
    ],
    questions:[
      { id:'q6', no:6, type:'single', prompt:`What is the main idea of the text?`,
        options:[{k:'A',t:`A baker discovered a valuable bell in the hills.`}, {k:'B',t:`A mysterious bell warned a village about danger, and a young baker acted on the warning.`}, {k:'C',t:`The villagers built a new stream after a heavy rain.`}, {k:'D',t:`The amber bell was stolen by a group of travelers.`}, {k:'E',t:`The villagers ignored Sena because she wanted to become famous.`}],
        correct:'B' },
    ]
  },
  {
    id:'text2p2',
    tag:'PART 2 · TEXT 2',
    color:'var(--t3)',
    bg:'var(--t3-bg)',
    title:`The Legend of the Moon Orchard`,
    meta:`Narrative Text · Legend · Identifying the main idea · Question No. 7`,
    passage:[
      `According to an old valley legend, fruit trees in a hidden orchard produced fruit only for people who shared what they had. A poor gardener named Orin once found the orchard after helping an exhausted traveler. He picked only a few fruits and brought them home to his neighbors. The next morning, more fruit had appeared on the trees. Orin continued sharing the harvest, and the orchard remained abundant. When another gardener tried to take all the fruit for himself, the trees produced nothing.`,
    ],
    questions:[
      { id:'q7', no:7, type:'single', prompt:`What is the main idea of the text?`,
        options:[{k:'A',t:`A gardener discovered that sharing was connected to the orchard's abundance.`}, {k:'B',t:`A traveler planted fruit trees in a poor valley.`}, {k:'C',t:`The orchard disappeared because Orin stopped gardening.`}, {k:'D',t:`The villagers refused to share fruit with strangers.`}, {k:'E',t:`A gardener became wealthy by selling all the orchard's fruit.`}],
        correct:'A' },
    ]
  },
  {
    id:'text3p2',
    tag:'PART 2 · TEXT 3',
    color:'var(--t4)',
    bg:'var(--t4-bg)',
    title:`The Legend of the Reed Boat`,
    meta:`Narrative Text · Legend · Identifying the main idea · Question No. 8`,
    passage:[
      `In a remote marshland, people told a story about a reed boat that appeared whenever someone was willing to help a stranger. One afternoon, a young fisherman named Vale found an old traveler stranded on a muddy bank. Vale carried the traveler to a dry place and shared his food. As darkness fell, a small boat made of reeds floated toward them. Vale and the traveler used it to cross the marsh safely. The villagers later said the boat was a reward for compassion.`,
    ],
    questions:[
      { id:'q8', no:8, type:'single', prompt:`What is the main idea of the text?`,
        options:[{k:'A',t:`A fisherman learned how to build boats from reeds.`}, {k:'B',t:`A traveler taught villagers how to cross a marsh.`}, {k:'C',t:`A mysterious reed boat appeared after a fisherman showed compassion.`}, {k:'D',t:`The villagers stopped fishing because the marsh became dangerous.`}, {k:'E',t:`A reed boat carried valuable goods across the marsh.`}],
        correct:'C' },
    ]
  },
  {
    id:'text4p2',
    tag:'PART 2 · TEXT 4',
    color:'var(--t1)',
    bg:'var(--t1-bg)',
    title:`The Legend of the Copper Hill`,
    meta:`Narrative Text · Legend · Identifying the main idea · Question No. 9`,
    passage:[
      `Many generations ago, a hill near a farming settlement was covered with small copper-colored stones. The villagers believed the stones protected the soil from becoming dry. During a long drought, a wealthy merchant ordered workers to collect the stones because he thought they were valuable. Soon, the fields around the hill became dusty and difficult to farm. Realizing their mistake, the villagers returned the stones to the hill. After the next rain, the soil slowly became fertile again.`,
    ],
    questions:[
      { id:'q9', no:9, type:'single', prompt:`What is the main idea of the text?`,
        options:[{k:'A',t:`A merchant discovered a copper mine beneath a village.`}, {k:'B',t:`The villagers became wealthy by selling stones.`}, {k:'C',t:`The hill was dangerous because it contained metal.`}, {k:'D',t:`The legend explains how removing the hill's stones harmed the land and why they were restored.`}, {k:'E',t:`Farmers abandoned their fields during a long drought.`}],
        correct:'D' },
    ]
  },
  {
    id:'text5p2',
    tag:'PART 2 · TEXT 5',
    color:'var(--t2)',
    bg:'var(--t2-bg)',
    title:`The Legend of the Star Weaver`,
    meta:`Narrative Text · Legend · Identifying the main idea · Question No. 10`,
    passage:[
      `An old coastal legend tells of a woman named Ilya who wove fishing nets for poor families. One winter, the sea became unusually dark, and fishermen could not see the shoreline at night. Ilya placed tiny shells that reflected moonlight along the beach. The fishermen could then find their way home. The villagers later said that, on clear nights, the shells appeared like small stars. The tradition of placing shells along the shore continued for generations.`,
    ],
    questions:[
      { id:'q10', no:10, type:'single', prompt:`What is the main idea of the text?`,
        options:[{k:'A',t:`A woman created a tradition that helped fishermen find their way home at night.`}, {k:'B',t:`Fishermen discovered a new source of valuable shells.`}, {k:'C',t:`The sea became bright because of a magical storm.`}, {k:'D',t:`The villagers stopped fishing during winter.`}, {k:'E',t:`Ilya became a famous trader because she sold shells.`}],
        correct:'A' },
    ]
  },
  {
    id:'textAp3',
    tag:'PART 3 · TEXT A',
    color:'var(--t3)',
    bg:'var(--t3-bg)',
    title:`The Legend of the Echoing Fig Tree`,
    meta:`Narrative Text · Legend · Textual & inferential information · Questions No. 11-12`,
    passage:[
      `In a hillside settlement, an enormous fig tree stood beside an old footpath. People said that the tree repeated the last kind words spoken beneath its branches. Most villagers considered the story a children's tale. One afternoon, a boy named Raka found an elderly traveler struggling with a heavy basket. Raka helped carry the basket to the village and thanked the traveler for trusting him. As they passed the fig tree on the way home, the tree seemed to repeat Raka's words. The villagers were surprised. From then on, they began to speak more kindly to one another beneath the tree, hoping its echo would remind them of the value of kindness.`,
    ],
    questions:[
      { id:'q11', no:11, type:'single', prompt:`Why did Raka help the elderly traveler?`,
        options:[{k:'A',t:`He wanted to receive a valuable gift.`}, {k:'B',t:`He was asked by the village chief to help the traveler.`}, {k:'C',t:`He noticed that the traveler was struggling with a heavy basket.`}, {k:'D',t:`He wanted to test whether the fig tree could speak.`}, {k:'E',t:`He needed the traveler to show him a hidden path.`}],
        correct:'C' },
      { id:'q12', no:12, type:'single', prompt:`What did the villagers do after the fig tree seemed to repeat Raka's words?`,
        options:[{k:'A',t:`They cut down the fig tree.`}, {k:'B',t:`They began speaking more kindly to one another.`}, {k:'C',t:`They stopped using the old footpath.`}, {k:'D',t:`They asked Raka to leave the village.`}, {k:'E',t:`They planted a new fig tree beside the river.`}],
        correct:'B' },
    ]
  },
  {
    id:'textBp3',
    tag:'PART 3 · TEXT B',
    color:'var(--t4)',
    bg:'var(--t4-bg)',
    title:`The Legend of the Misty Path`,
    meta:`Narrative Text · Legend · Textual & inferential information · Questions No. 13-15`,
    passage:[
      `A merchant named Elian once traveled through a mountain valley where thick mist often covered the roads. Local people believed that a pale bird appeared to travelers who were about to choose an unsafe path. One evening, Elian saw the bird flying toward a narrow road. He followed it in the opposite direction and reached a small settlement before dark. The next morning, he learned that a rockslide had blocked the narrow road during the night. Elian believed the bird had guided him away from danger.`,
    ],
    questions:[
      { id:'q13', no:13, type:'single', prompt:`What can be inferred about the pale bird?`,
        options:[{k:'A',t:`It probably appeared as a warning to travelers.`}, {k:'B',t:`It belonged to Elian.`}, {k:'C',t:`It always flew over the safest road in the valley.`}, {k:'D',t:`It wanted to lead travelers toward rockslides.`}, {k:'E',t:`It appeared only during the rainy season.`}],
        correct:'A' },
      { id:'q14', no:14, type:'single', prompt:`Why did Elian believe the bird had helped him?`,
        options:[{k:'A',t:`The bird carried him to the settlement.`}, {k:'B',t:`The bird told him about the rockslide.`}, {k:'C',t:`He later learned that the road he avoided had been blocked.`}, {k:'D',t:`The villagers said that Elian owned the bird.`}, {k:'E',t:`He found food near the bird's nest.`}],
        correct:'C' },
      { id:'q15', no:15, type:'single', prompt:`Which statement best describes Elian's decision?`,
        options:[{k:'A',t:`He ignored the unusual sign and continued on the narrow road.`}, {k:'B',t:`He followed the bird directly into the mist.`}, {k:'C',t:`He changed his route after noticing the bird's behavior.`}, {k:'D',t:`He returned to the market to buy another map.`}, {k:'E',t:`He asked the villagers to remove the mountain road.`}],
        correct:'C' },
    ]
  },
  {
    id:'textAp4',
    tag:'PART 4 · TEXT A',
    color:'var(--t1)',
    bg:'var(--t1-bg)',
    title:`The Legend of the Silver Seed`,
    meta:`Narrative Text · Legend · Multiple choice, multiple answers · Questions No. 16-18`,
    passage:[
      `In a dry farming village, a girl named Nemi received one silver seed from a quiet stranger. The stranger told her that the seed would grow only if its harvest was shared. Nemi planted it near the village well. A month later, a tall plant grew and produced enough grain for many families. Nemi kept a small portion for her own family and distributed the rest. The following season, the plant disappeared, but the villagers began sharing their harvests more willingly because they remembered Nemi's example.`,
    ],
    questions:[
      { id:'q16', no:16, type:'multi', prompt:`Which statements are supported by the text?`, hint:`Choose more than one answer!`,
        options:[{k:'A',t:`Nemi received one silver seed.`}, {k:'B',t:`The stranger told Nemi to keep the harvest for herself.`}, {k:'C',t:`The plant produced enough grain for many families.`}, {k:'D',t:`Nemi distributed part of the harvest.`}],
        correct:['A','C','D'] },
      { id:'q17', no:17, type:'multi', prompt:`Which lessons can be learned from the legend?`, hint:`Choose more than one answer!`,
        options:[{k:'A',t:`Sharing can strengthen a community.`}, {k:'B',t:`A person should always keep unexpected gifts.`}, {k:'C',t:`One person's example can influence others.`}, {k:'D',t:`Helping others is useful only when a reward is guaranteed.`}],
        correct:['A','C'] },
      { id:'q18', no:18, type:'multi', prompt:`Which events happened in the story?`, hint:`Choose more than one answer!`,
        options:[{k:'A',t:`Nemi planted the silver seed.`}, {k:'B',t:`The plant produced grain.`}, {k:'C',t:`The villagers sold the entire harvest to a merchant.`}, {k:'D',t:`The plant disappeared after the following season.`}],
        correct:['A','B','D'] },
    ]
  },
  {
    id:'textBp4',
    tag:'PART 4 · TEXT B',
    color:'var(--t2)',
    bg:'var(--t2-bg)',
    title:`The Legend of the Listening Cave`,
    meta:`Narrative Text · Legend · Multiple choice, multiple answers · Questions No. 19-20`,
    passage:[
      `A cave beside a mountain was believed to repeat only truthful words. A young hunter named Sava entered the cave while searching for a lost goat. Inside, he found an old traveler who asked whether Sava had seen a hidden path. Sava honestly said that he had not. The cave repeated his answer clearly. Later, Sava discovered the traveler was looking for a safe route to the village. Sava then returned and guided him there. The villagers remembered the story as a lesson that honesty could build trust.`,
    ],
    questions:[
      { id:'q19', no:19, type:'multi', prompt:`Which statements are true according to the text?`, hint:`Choose more than one answer!`,
        options:[{k:'A',t:`Sava entered the cave while searching for a goat.`}, {k:'B',t:`Sava lied about seeing a hidden path.`}, {k:'C',t:`The cave repeated Sava's truthful answer.`}, {k:'D',t:`Sava later helped the traveler find a safe route.`}],
        correct:['A','C','D'] },
      { id:'q20', no:20, type:'multi', prompt:`Which ideas are implied by the legend?`, hint:`Choose more than one answer!`,
        options:[{k:'A',t:`Honesty can help people trust one another.`}, {k:'B',t:`Truthful answers may be valuable even when they seem simple.`}, {k:'C',t:`Sava helped the traveler only because he wanted money.`}, {k:'D',t:`The villagers considered honesty an important quality.`}],
        correct:['A','B','D'] },
    ]
  },
  {
    id:'text1p5',
    tag:'PART 5 · TEXT 1',
    color:'var(--t3)',
    bg:'var(--t3-bg)',
    title:`The Legend of the Glass Kite`,
    meta:`Narrative Text · Legend · True or False · Questions No. 21-22`,
    passage:[
      `A village near the sea once suffered because fishermen could not tell when strong winds were approaching. A girl named Mara made a kite from thin cloth and pieces of clear glass. Whenever the wind became dangerous, the kite produced a sharp sound. The villagers used the sound as a warning and brought their boats closer to shore. After Mara grew older, the villagers taught younger children how to make similar warning kites.`,
    ],
    questions:[
      { id:'q21', no:21, type:'single', prompt:`Mara made the first warning kite from cloth and pieces of glass.`,
        options:[{k:'A',t:`True`}, {k:'B',t:`False`}],
        correct:'A' },
      { id:'q22', no:22, type:'single', prompt:`The kite was used mainly to entertain children during calm weather.`,
        options:[{k:'A',t:`True`}, {k:'B',t:`False`}],
        correct:'B' },
    ]
  },
  {
    id:'text2p5',
    tag:'PART 5 · TEXT 2',
    color:'var(--t4)',
    bg:'var(--t4-bg)',
    title:`The Legend of the Sleeping Lake`,
    meta:`Narrative Text · Legend · True or False · Questions No. 23-24`,
    passage:[
      `An old legend says that a lake became completely still whenever people forgot to care for the land around it. One summer, villagers cut many trees near the lake and left rubbish along its shore. The water soon became unusually quiet. A farmer named Tera organized a clean-up and encouraged the villagers to plant new trees. Over time, the lake became lively again, and the villagers believed it had awakened.`,
    ],
    questions:[
      { id:'q23', no:23, type:'single', prompt:`The villagers improved the area around the lake by cleaning it and planting trees.`,
        options:[{k:'A',t:`True`}, {k:'B',t:`False`}],
        correct:'A' },
      { id:'q24', no:24, type:'single', prompt:`The lake became still because the villagers planted too many trees.`,
        options:[{k:'A',t:`True`}, {k:'B',t:`False`}],
        correct:'B' },
    ]
  },
  {
    id:'text3p5',
    tag:'PART 5 · TEXT 3',
    color:'var(--t1)',
    bg:'var(--t1-bg)',
    title:`The Legend of the Bronze Sparrow`,
    meta:`Narrative Text · Legend · True or False · Questions No. 25-26`,
    passage:[
      `A bronze statue of a sparrow stood above the gate of an ancient town. According to local legend, the statue turned toward the direction from which danger would come. One morning, it faced west even though danger had never come from that direction before. The town leader sent scouts west and discovered that a bridge had collapsed on the main road. Travelers were redirected to a safer route.`,
    ],
    questions:[
      { id:'q25', no:25, type:'single', prompt:`The statue's unusual movement led the town leader to investigate the western road.`,
        options:[{k:'A',t:`True`}, {k:'B',t:`False`}],
        correct:'A' },
      { id:'q26', no:26, type:'single', prompt:`The collapsed bridge was discovered on the eastern road.`,
        options:[{k:'A',t:`True`}, {k:'B',t:`False`}],
        correct:'B' },
    ]
  },
  {
    id:'text4p5',
    tag:'PART 5 · TEXT 4',
    color:'var(--t2)',
    bg:'var(--t2-bg)',
    title:`The Legend of the Rain Drum`,
    meta:`Narrative Text · Legend · True or False · Questions No. 27-28`,
    passage:[
      `In a mountain village, a large drum was kept in a small wooden shelter. People believed that the drum would sound when the first rain of the season was near. One year, the villagers heard the drum at dawn. Instead of waiting, they repaired the channels that carried water to their fields. Heavy rain arrived two days later, and the repaired channels helped prevent the fields from flooding.`,
    ],
    questions:[
      { id:'q27', no:27, type:'single', prompt:`The villagers repaired the water channels after hearing the drum.`,
        options:[{k:'A',t:`True`}, {k:'B',t:`False`}],
        correct:'A' },
      { id:'q28', no:28, type:'single', prompt:`The heavy rain arrived on the same day that the drum sounded.`,
        options:[{k:'A',t:`True`}, {k:'B',t:`False`}],
        correct:'B' },
    ]
  },
  {
    id:'text5p5',
    tag:'PART 5 · TEXT 5',
    color:'var(--t3)',
    bg:'var(--t3-bg)',
    title:`The Legend of the Willow Lantern`,
    meta:`Narrative Text · Legend · True or False · Questions No. 29-30`,
    passage:[
      `A river village once used lanterns to guide boats through a bend that was difficult to navigate at night. A young carpenter named Lio noticed that the old lantern posts were too weak. He built new wooden frames and placed them higher above the riverbank. During the next storm, the new frames remained standing and continued to guide the boats. The villagers later said that Lio's careful work had protected the community.`,
    ],
    questions:[
      { id:'q29', no:29, type:'single', prompt:`Lio strengthened the lantern posts before the next storm.`,
        options:[{k:'A',t:`True`}, {k:'B',t:`False`}],
        correct:'A' },
      { id:'q30', no:30, type:'single', prompt:`The new lantern frames fell into the river during the storm.`,
        options:[{k:'A',t:`True`}, {k:'B',t:`False`}],
        correct:'B' },
    ]
  }
];

const CLASS_TOKENS = { 'XI D1':'SUSULAN', 'XI D2':'SUSULAN', 'XI E1':'SUSULAN' };

function shuffleArray(array) {
  for (let i = array.length - 1; i > 0; i--) {
    const j = Math.floor(Math.random() * (i + 1));
    [array[i], array[j]] = [array[j], array[i]];
  }
  return array;
}

let FLAT = [];
function buildFlat(savedOrder = null, savedOptions = {}, savedMatrix = {}){
  FLAT = [];
  
  DATA.forEach(section => {
    let sectionQs = [...section.questions];
    
    // Jika belum ada urutan tersimpan untuk section ini, acak urutan soalnya
    if (savedOrder && savedOrder[section.id]) {
      sectionQs = savedOrder[section.id].map(id => section.questions.find(q => q.id === id)).filter(Boolean);
    } else {
      shuffleArray(sectionQs);
    }

    sectionQs.forEach(q => {
      const qCopy = Object.assign({}, q, { _section: section });
      
      if (Array.isArray(q.options)) {
        let opts = [...q.options];
        if (savedOptions && savedOptions[q.id]) {
          opts = savedOptions[q.id].map(k => q.options.find(o => o.k === k)).filter(Boolean);
        } else {
          shuffleArray(opts);
        }
        qCopy.options = opts;
      }

      if (q.type === 'matrix') {
        let stmts = [...q.statements];
        if (savedMatrix && savedMatrix[q.id]) {
          stmts = savedMatrix[q.id].map(idx => q.statements[idx]).filter(Boolean);
          qCopy._matrixOrder = savedMatrix[q.id];
        } else {
          const indices = stmts.map((_, idx) => idx);
          shuffleArray(indices);
          stmts = indices.map(idx => q.statements[idx]);
          qCopy._matrixOrder = indices;
        }
        qCopy.statements = stmts;
      }

      FLAT.push(qCopy);
    });
  });
}

let answers = {};
let submitted = false;
let currentIndex = 0;
let paletteOpen = false;
let questionOrderMap = {};
let optionOrderMap = {};
let matrixOrderMap = {};

function isAnsweredQ(q){
  if(q.type==='matrix'){
    const a = answers[q.id]||{};
    return Object.keys(a).length===q.statements.length;
  }
  if(q.type==='multi'){
    return !!(answers[q.id] && answers[q.id].length>0);
  }
  return !!answers[q.id];
}

function computeResult(q){
  if(q.type==='single'){
    const correct = answers[q.id]===q.correct;
    return {correct, earned: correct?1:0, total:1};
  }
  if(q.type==='multi'){
    const chosen = answers[q.id]||[];
    const correctArr = q.correct;
    let earned = 0;
    chosen.forEach(c => {
      if(correctArr.includes(c)) earned++;
    });
    earned = Math.max(0, earned);
    return {correct: arraysEqual(chosen, correctArr), earned, total: correctArr.length};
  }
  if(q.type==='matrix'){
    const chosenMap = answers[q.id]||{};
    let earned = 0;
    q.statements.forEach((s,i)=>{
      if(chosenMap[i]===s.correct) earned++;
    });
    return {correct: earned===q.statements.length, earned, total: q.statements.length};
  }
}

function arraysEqual(a,b){
  if(a.length!==b.length) return false;
  const sa=[...a].sort(), sb=[...b].sort();
  return sa.every((v,i)=>v===sb[i]);
}

const stage = document.getElementById('stage');
let pinEnabled = false;

function applyPinLayout(){
  const card = stage.querySelector('.q-card');
  const passageEl = stage.querySelector('.passage');
  if(pinEnabled){
    stage.classList.add('pin-mode');
    const navBar = document.querySelector('.nav-bar');
    const navH = navBar ? navBar.offsetHeight : 0;
    if(card) card.style.bottom = navH+'px';
    requestAnimationFrame(()=>{
      if(card && passageEl){
        passageEl.style.paddingBottom = (card.offsetHeight + navH + 20)+'px';
      }
    });
  } else {
    stage.classList.remove('pin-mode');
    if(card) card.style.bottom = '';
    if(passageEl) passageEl.style.paddingBottom = '';
  }
}
window.addEventListener('resize', ()=>{ if(pinEnabled) applyPinLayout(); });

function renderStage(){
  const q = FLAT[currentIndex];
  const section = q._section;
  stage.innerHTML = '';
  stage.style.setProperty('--sc', section.color);

  const head = document.createElement('div');
  head.className='stage-head';
  head.innerHTML = `
    <span class="genre-tag" style="background:${section.bg}; color:${section.color};">${section.tag}</span>
    <span class="stage-index">Question ${currentIndex+1} of ${FLAT.length}</span>
  `;
  stage.appendChild(head);

  const passage = document.createElement('div');
  passage.className='passage';
  passage.style.borderLeftColor = section.color;
  passage.innerHTML = `
    <div class="meta">${section.meta}</div>
    <h3>${section.title}</h3>
    ${section.image ? `<img class="passage-img" src="${section.image}" alt="${section.title}">` : ''}
    ${section.passage ? section.passage.map(p=>`<p>${p}</p>`).join('') : ''}
  `;
  stage.appendChild(passage);

  const card = document.createElement('div');
  card.className='q-card';
  card.id='card-'+q.id;

  const top = document.createElement('div');
  top.className='q-top';
  top.innerHTML = `
    <div class="q-num" style="background:${section.bg}; color:${section.color};">${currentIndex+1}</div>
    <div class="q-prompt">${q.prompt}</div>
    <button type="button" class="pin-toggle ${pinEnabled?'active':''}" id="pinToggleBtn">
      <span class="pin-ic">&#128204;</span><span>${pinEnabled ? 'Pinned' : 'Pin'}</span>
    </button>
  `;
  top.querySelector('#pinToggleBtn').addEventListener('click', ()=>{
    pinEnabled = !pinEnabled;
    applyPinLayout();
    const btn = document.getElementById('pinToggleBtn');
    btn.classList.toggle('active', pinEnabled);
    btn.innerHTML = `<span class="pin-ic">&#128204;</span><span>${pinEnabled ? 'Pinned' : 'Pin'}</span>`;
  });
  card.appendChild(top);

  if(q.hint){
    const hint = document.createElement('div');
    hint.className='q-hint';
    hint.textContent = q.hint;
    card.appendChild(hint);
  }

  if(q.type==='single'){
    const opts = document.createElement('div');
    opts.className='options';
    q.options.forEach(o=>{
      const lbl = document.createElement('label');
      lbl.className='opt';
      lbl.dataset.key=o.k;
      const checked = answers[q.id]===o.k ? 'checked' : '';
      lbl.innerHTML = `<input type="radio" name="${q.id}" value="${o.k}" ${checked}> <span>${o.t}</span>`;
      if(answers[q.id]===o.k) lbl.classList.add('selected');
      lbl.querySelector('input').addEventListener('change', ()=>{
        answers[q.id]=o.k;
        refreshOptionSelection(q, card);
        updateProgress();
        renderPalette();
        saveState();
      });
      opts.appendChild(lbl);
    });
    card.appendChild(opts);
  }

  if(q.type==='multi'){
    const opts = document.createElement('div');
    opts.className='options';
    q.options.forEach(o=>{
      const lbl = document.createElement('label');
      lbl.className='opt';
      lbl.dataset.key=o.k;
      const isChecked = (answers[q.id]||[]).includes(o.k);
      lbl.innerHTML = `<input type="checkbox" name="${q.id}" value="${o.k}" ${isChecked?'checked':''}> <span>${o.t}</span>`;
      if(isChecked) lbl.classList.add('selected');
      lbl.querySelector('input').addEventListener('change', ()=>{
        const cur = new Set(answers[q.id]||[]);
        if(lbl.querySelector('input').checked) cur.add(o.k); else cur.delete(o.k);
        answers[q.id]=Array.from(cur);
        refreshOptionSelection(q, card);
        updateProgress();
        renderPalette();
        saveState();
      });
      opts.appendChild(lbl);
    });
    card.appendChild(opts);
  }

  if(q.type==='matrix'){
    const box = document.createElement('div');
    box.className='matrix';
    const table = document.createElement('table');
    table.innerHTML = `<thead><tr><th>Statement</th><th>${q.cols[0]}</th><th>${q.cols[1]}</th></tr></thead>`;
    const tbody = document.createElement('tbody');
    q.statements.forEach((s,i)=>{
      const tr = document.createElement('tr');
      const chosenVal = (answers[q.id]||{})[i];
      tr.innerHTML = `
        <td class="stmt">${i+1}. ${s.t}</td>
        <td class="pick"><input type="radio" name="${q.id}-${i}" value="${q.cols[0]}" ${chosenVal===q.cols[0]?'checked':''}></td>
        <td class="pick"><input type="radio" name="${q.id}-${i}" value="${q.cols[1]}" ${chosenVal===q.cols[1]?'checked':''}></td>
      `;
      tr.querySelectorAll('input').forEach(inp=>{
        inp.addEventListener('change', ()=>{
          if(!answers[q.id]) answers[q.id]={};
          answers[q.id][i]=inp.value;
          updateProgress();
          renderPalette();
          saveState();
        });
      });
      tbody.appendChild(tr);
    });
    table.appendChild(tbody);
    box.appendChild(table);
    card.appendChild(box);
  }

  const note = document.createElement('div');
  note.className='answer-note';
  note.id='note-'+q.id;
  card.appendChild(note);

  stage.appendChild(card);

  if(submitted){
    applyGradingToCard(q, card);
  }

  applyPinLayout();
  updateNavButtons();
}

function refreshOptionSelection(q, card){
  card.querySelectorAll('.opt').forEach(lbl=>{
    const key = lbl.dataset.key;
    const sel = q.type==='multi' ? (answers[q.id]||[]).includes(key) : answers[q.id]===key;
    lbl.classList.toggle('selected', !!sel && !submitted);
  });
}

function applyGradingToCard(q, card){
  if(q.type==='single' || q.type==='multi'){
    card.querySelectorAll('.opt').forEach(lbl=>{
      lbl.querySelector('input').disabled = true;
      lbl.classList.add('locked');
    });
  }
  if(q.type==='matrix'){
    card.querySelectorAll('.matrix input').forEach(inp=>{ inp.disabled = true; });
  }
}

const paletteGrid = document.getElementById('paletteGrid');
function renderPalette(){
  paletteGrid.innerHTML='';
  FLAT.forEach((q,i)=>{
    const btn = document.createElement('button');
    btn.type='button';
    btn.className='pnum';
    btn.textContent = i+1;
    if(i===currentIndex) btn.classList.add('pn-current');
    if(isAnsweredQ(q)){
      btn.classList.add('pn-answered');
    }
    btn.addEventListener('click', ()=>{
      currentIndex = i;
      renderStage();
      renderPalette();
      saveState();
      window.scrollTo({top:0, behavior:'smooth'});
    });
    paletteGrid.appendChild(btn);
  });
}

document.getElementById('paletteToggleBtn').addEventListener('click', ()=>{
  paletteOpen = !paletteOpen;
  document.getElementById('palettePanel').classList.toggle('open', paletteOpen);
  document.getElementById('paletteToggleText').textContent = paletteOpen ? 'Tutup Soal' : 'Semua Soal';
});

let headerHidden = false;
const toggleHeaderBtn = document.getElementById('toggleHeaderBtn');
const headerToggleHome = document.getElementById('headerToggleHome');
const paletteToggleBtnEl = document.getElementById('paletteToggleBtn');

toggleHeaderBtn.addEventListener('click', ()=>{
  headerHidden = !headerHidden;
  const shell = document.getElementById('progressShell');
  const icon = document.getElementById('toggleIcon');

  if(headerHidden){
    shell.classList.add('collapsed');
    icon.textContent = '▼';
    // pindahkan tombol ke pojok agar tetap bisa ditekan saat header hilang
    headerToggleHome.appendChild(toggleHeaderBtn);
    headerToggleHome.style.display = 'flex';
  } else {
    shell.classList.remove('collapsed');
    icon.textContent = '▲';
    // kembalikan tombol ke sebelah tombol "Semua Soal"
    paletteToggleBtnEl.insertAdjacentElement('afterend', toggleHeaderBtn);
    headerToggleHome.style.display = 'none';
  }
});

function updateProgress(){
  const answered = FLAT.filter(isAnsweredQ).length;
  const pct = Math.round((answered/FLAT.length)*100);
  document.getElementById('progressFill').style.width=pct+'%';
  document.getElementById('progressLabel').textContent = `${answered} / ${FLAT.length} answered`;
}

function updateNavButtons(){
  document.getElementById('prevBtn').disabled = currentIndex===0;
  document.getElementById('nextBtn').disabled = currentIndex===FLAT.length-1;
  const isLast = currentIndex===FLAT.length-1;
  document.getElementById('submitBtn').style.display = isLast ? '' : 'none';
}

document.getElementById('prevBtn').addEventListener('click', ()=>{
  if(currentIndex>0){ currentIndex--; renderStage(); renderPalette(); updateProgress(); saveState(); window.scrollTo({top:0, behavior:'smooth'}); }
});
document.getElementById('nextBtn').addEventListener('click', ()=>{
  if(currentIndex<FLAT.length-1){ currentIndex++; renderStage(); renderPalette(); updateProgress(); saveState(); window.scrollTo({top:0, behavior:'smooth'}); }
});

function grade(auto){
  const name = document.getElementById('stuName').value.trim();
  const stuClass = document.getElementById('stuClass').value.trim();
  if(!auto && (!name || !stuClass)){
    const err = document.getElementById('gateError');
    if(err) err.textContent = 'Please fill in Name and Class at the top before checking & submitting.';
    window.scrollTo({top:0, behavior:'smooth'});
    return;
  }
  if(submitted) return;

  stopTimer();
  submitted = true;
  examActive = false;
  updateFullscreenButton();
  updateResetButton();
  document.getElementById('violationModal').classList.remove('show');
  if(isFullscreenActive()){
    const exitFs = document.exitFullscreen || document.webkitExitFullscreen || document.msExitFullscreen;
    if(exitFs) exitFs.call(document).catch(()=>{});
  }

  let earned=0, total=0;
  FLAT.forEach(q=>{
    const r = computeResult(q);
    earned += r.earned;
    total += r.total;
  });

  const penalti = violationCount * VIOLATION_PENALTY; // dicatat di ringkasan saja, tidak memengaruhi nilai
  const nilaiMentah = total > 0 ? (earned / total) * 100 : 0;
  const nilai = Math.max(0, Math.min(100, Math.round(nilaiMentah)));

  const scoreBig = document.getElementById('scoreBig');
  const scoreSub = document.getElementById('scoreSub');
  scoreBig.textContent = nilai;
  scoreSub.textContent = 'Nilai Akhir (0-100)';

  const msg = document.getElementById('scoreMsg');
  msg.textContent = 'Ujian selesai dikerjakan. Terima kasih sudah mengerjakan ujian ini!';
  msg.style.color = 'var(--navy)';
  msg.style.background = '#eef0fb';

  const resultsBox = document.getElementById('resultsBox');
  resultsBox.classList.add('show');

  document.getElementById('submitBtn').disabled = true;
  document.getElementById('timerBadge').textContent = 'Finished';
  document.getElementById('timerBadge').classList.remove('warn','danger','paused');
  renderStage();
  renderPalette();
  saveState();
  resultsBox.scrollIntoView({behavior:'smooth', block:'start'});

  attemptSend(name, stuClass, {nilai, earned, total, penalti, violationCount});
}

function buildAnswerReport(){
  const sorted = FLAT.slice().sort((a,b)=> a.no - b.no );
  const lines = sorted.map(q=>{
    const r = computeResult(q);
    const mark = `${r.earned}/${r.total}`;
    let ansText;
    if(q.type==='single'){
      ansText = answers[q.id] || '-';
    } else if(q.type==='multi'){
      ansText = (answers[q.id]||[]).slice().sort().join(',') || '-';
    } else if(q.type==='matrix'){
      const chosenMap = answers[q.id]||{};
      ansText = q.statements.map((s,i)=> `${i+1}:${chosenMap[i]||'-'}`).join(' | ');
    }
    return `No.${q.no} [Skor: ${mark}] ${ansText}`;
  });
  const header = `Pelanggaran tab/app: ${violationCount} (dicatat saja, tidak mengurangi nilai)`;
  return header + '\n' + lines.join('\n');
}

const GFORM_BASE = 'https://docs.google.com/forms/d/e/1FAIpQLSd_EKjzKKCXSkAX2LTiWR1g0SXmJ5aGemA3RhkH38ujQLQ2ww/formResponse';
const GFORM_ENTRY_NAME = 'entry.1260637593';
const GFORM_ENTRY_CLASS = 'entry.222236056';
const GFORM_ENTRY_ANSWER = 'entry.264164770';
const GFORM_ENTRY_SCORE = 'entry.383580718';
let pendingSend = null;
let resultSent = false;

function isReallyOnline(){
  return new Promise(resolve=>{
    if(!navigator.onLine){ resolve(false); return; }
    let done = false;
    const finish = (val)=>{ if(!done){ done = true; resolve(val); } };
    const timer = setTimeout(()=>finish(false), 4000);
    const img = new Image();
    img.onload = ()=>{ clearTimeout(timer); finish(true); };
    img.onerror = ()=>{ clearTimeout(timer); finish(true); };
    img.src = 'https://www.google.com/favicon.ico?_=' + Date.now();
  });
}

function attemptSend(name, stuClass, score){
  const note = document.getElementById('sendNote');
  const retryBtn = document.getElementById('retrySendBtn');
  pendingSend = {name, stuClass, score};

  note.textContent = 'Checking internet connection...';
  note.className = 'send-note';
  retryBtn.style.display = 'none';

  isReallyOnline().then(online=>{
    if(!online){
      note.textContent = 'Kirim gagal. Tidak ada koneksi internet, jawabanmu belum terkirim.';
      note.className = 'send-note err';
      retryBtn.style.display = 'inline-block';
      return;
    }
    sendResultToForm(pendingSend.name, pendingSend.stuClass, pendingSend.score);
  });
}

document.getElementById('retrySendBtn').addEventListener('click', ()=>{
  if(pendingSend){
    attemptSend(pendingSend.name, pendingSend.stuClass, pendingSend.score);
  }
});

function sendResultToForm(name, stuClass, score){
  const note = document.getElementById('sendNote');
  const retryBtn = document.getElementById('retrySendBtn');
  const answerReport = buildAnswerReport();
  const scoreText = score.penalti>0
    ? `Nilai: ${score.nilai} (Skor: ${score.earned}/${score.total}, dicatat ${score.violationCount} pelanggaran - tidak mengurangi nilai)`
    : `Nilai: ${score.nilai} (Skor: ${score.earned}/${score.total})`;

  const iframeName = 'gform-send-target';
  let iframe = document.getElementById(iframeName);
  if(!iframe){
    iframe = document.createElement('iframe');
    iframe.name = iframeName;
    iframe.id = iframeName;
    iframe.style.display = 'none';
    document.body.appendChild(iframe);
  }

  const form = document.createElement('form');
  form.action = GFORM_BASE;
  form.method = 'POST';
  form.target = iframeName;
  form.style.display = 'none';

  const fields = {
    [GFORM_ENTRY_NAME]: name,
    [GFORM_ENTRY_CLASS]: stuClass,
    [GFORM_ENTRY_ANSWER]: answerReport,
    [GFORM_ENTRY_SCORE]: scoreText
  };
  Object.keys(fields).forEach(key=>{
    const input = document.createElement('input');
    input.type = 'hidden';
    input.name = key;
    input.value = fields[key];
    form.appendChild(input);
  });

  document.body.appendChild(form);
  form.submit();
  document.body.removeChild(form);

  pendingSend = null;
  resultSent = true;
  saveState();
  retryBtn.style.display = 'none';
  note.textContent = 'Answers submitted! Thank you.';
  note.className = 'send-note ok';
}

function resetQuiz(){
  localStorage.removeItem(STORAGE_KEY);
  location.reload();
}

function openSubmitConfirm(titleHtml, msgHtml){
  document.getElementById('confirmTitle').innerHTML = titleHtml;
  document.getElementById('confirmMsg').innerHTML = msgHtml;
  document.getElementById('confirmModal').classList.add('show');
}

document.getElementById('submitBtn').addEventListener('click', ()=>{
  if(submitted) return;
  const unanswered = FLAT.length - FLAT.filter(isAnsweredQ).length;
  let msg;
  if(unanswered > 0){
    msg = `Kamu masih punya <b>${unanswered} soal yang belum dijawab</b>.<br>Apakah kamu yakin ingin mengirim jawabanmu sekarang?`;
  } else {
    msg = `Kamu sudah menjawab semua <b>${FLAT.length} soal</b>.<br>Apakah kamu yakin ingin mengirim jawabanmu sekarang?`;
  }
  openSubmitConfirm('Konfirmasi Submit Ujian', msg);
});

document.getElementById('violationEndBtn').addEventListener('click', ()=>{
  document.getElementById('violationModal').classList.remove('show');
  const penalty = violationCount * VIOLATION_PENALTY;
  openSubmitConfirm(
    'Konfirmasi Sudahi Ujian',
    `Kamu sudah mendapat <b>${violationCount} pelanggaran</b> (potongan -${penalty} poin).<br>Apakah kamu yakin ingin <b>mengakhiri ujian sekarang</b>? Jawaban yang sudah kamu isi akan langsung dikirim dan tidak bisa diubah lagi.`
  );
});

document.getElementById('cancelSubmitBtn').addEventListener('click', ()=>{
  document.getElementById('confirmModal').classList.remove('show');
  if(isExamRunning() && !isFullscreenActive()){
    requestExamFullscreen();
  }
});

document.getElementById('confirmSubmitBtn').addEventListener('click', ()=>{
  document.getElementById('confirmModal').classList.remove('show');
  grade(false);
});

document.getElementById('resetBtn').addEventListener('click', resetQuiz);

['copy','cut','contextmenu','selectstart','dragstart'].forEach(evt=>{
  document.addEventListener(evt, e=>{
    if(e.target.tagName==='INPUT' || e.target.tagName==='TEXTAREA' || e.target.tagName==='SELECT') return;
    e.preventDefault();
  });
});

const MAX_VIOLATIONS = 5;
const VIOLATION_PENALTY = 2;
let violationCount = 0;
let lastViolationAt = 0;
let examActive = false;

function isExamRunning(){
  return examActive && !submitted;
}

function updateResetButton(){
  const btn = document.getElementById('resetBtn');
  if(btn) btn.style.display = submitted ? '' : 'none';
}

let audioCtx = null;
function playAlarm(){
  try{
    if(!audioCtx) audioCtx = new (window.AudioContext || window.webkitAudioContext)();
    const now = audioCtx.currentTime;
    [0, 0.35, 0.7].forEach(offset=>{
      const osc = audioCtx.createOscillator();
      const gain = audioCtx.createGain();
      osc.type = 'square';
      osc.frequency.setValueAtTime(880, now+offset);
      gain.gain.setValueAtTime(0.0001, now+offset);
      gain.gain.exponentialRampToValueAtTime(0.25, now+offset+0.02);
      gain.gain.exponentialRampToValueAtTime(0.0001, now+offset+0.28);
      osc.connect(gain).connect(audioCtx.destination);
      osc.start(now+offset);
      osc.stop(now+offset+0.3);
    });
  }catch(err){}
}

function requestExamFullscreen(){
  const el = document.documentElement;
  const req = el.requestFullscreen || el.webkitRequestFullscreen || el.msRequestFullscreen;
  if(req){ req.call(el).catch(()=>{}); }
}

function isFullscreenActive(){
  return !!(document.fullscreenElement || document.webkitFullscreenElement || document.msFullscreenElement);
}

function updateViolationBadge(){
  const badge = document.getElementById('violationBadge');
  if(!badge) return;
  if(violationCount>0){
    badge.textContent = `⚠️ ${violationCount} (-${violationCount*VIOLATION_PENALTY})`;
    badge.classList.add('show');
  } else {
    badge.classList.remove('show');
  }
}

function updateFullscreenButton(){
  const btn = document.getElementById('fullscreenBtn');
  if(!btn) return;
  btn.style.display = (isExamRunning() && !isFullscreenActive()) ? '' : 'none';
}

function registerViolation(reason){
  if(!isExamRunning()) return;
  const now = Date.now();
  if(now - lastViolationAt < 800) return;
  lastViolationAt = now;

  violationCount++;
  updateViolationBadge();
  updateFullscreenButton();
  playAlarm();
  saveState();

  const modal = document.getElementById('violationModal');
  const msg = document.getElementById('violationMsg');
  const countEl = document.getElementById('violationCount');
  msg.textContent = `Terdeteksi: ${reason}. Ujian TIDAK otomatis dikirim, tapi ${VIOLATION_PENALTY} poin telah dikurangi dari nilaimu.`;
  countEl.textContent = `Pelanggaran ke-${violationCount} — Total pengurangan: -${violationCount*VIOLATION_PENALTY} poin`;
  modal.classList.add('show');
}

document.getElementById('violationOkBtn').addEventListener('click', ()=>{
  document.getElementById('violationModal').classList.remove('show');
  requestExamFullscreen();
});

document.getElementById('fullscreenBtn').addEventListener('click', ()=>{
  requestExamFullscreen();
});

document.addEventListener('visibilitychange', ()=>{
  if(document.hidden){
    registerViolation('kamu berpindah tab atau meminimalkan jendela');
  }
});

window.addEventListener('blur', ()=>{
  setTimeout(()=>{
    if(isExamRunning() && document.hidden===false && !document.hasFocus()){
      registerViolation('kamu berpindah ke aplikasi lain');
    }
  }, 150);
});

['fullscreenchange','webkitfullscreenchange','msfullscreenchange'].forEach(evt=>{
  document.addEventListener(evt, ()=>{
    if(isExamRunning() && !isFullscreenActive()){
      registerViolation('kamu keluar dari mode fullscreen');
    }
    updateFullscreenButton();
  });
});

const STORAGE_KEY = 'eng_exam_10_descriptive_v5';

function saveState(){
  try{
    const state = {
      name: document.getElementById('stuName').value,
      cls: document.getElementById('stuClass').value,
      gatePassed: true,
      questionOrder: questionOrderMap,
      optionOrder: optionOrderMap,
      matrixOrder: matrixOrderMap,
      order: FLAT.map(q=>q.id),
      answers: answers,
      currentIndex: currentIndex,
      submitted: submitted,
      endAt: examEndAt,
      remainingTimeMs: isTimerPaused ? remainingTimeMs : (examEndAt ? Math.max(0, examEndAt - Date.now()) : TIMER_MS),
      isTimerPaused: isTimerPaused,
      violationCount: violationCount,
      resultSent: resultSent
    };
    localStorage.setItem(STORAGE_KEY, JSON.stringify(state));
  }catch(e){}
}

function loadState(){
  try{
    const raw = localStorage.getItem(STORAGE_KEY);
    if(!raw) return null;
    const state = JSON.parse(raw);
    if(!state || !state.gatePassed) return null;
    return state;
  }catch(e){ return null; }
}

const TIMER_MINUTES = 90;
const TIMER_MS = TIMER_MINUTES*60*1000;
let timerInterval = null;
let examEndAt = null;
let remainingTimeMs = TIMER_MS;
let isTimerPaused = false;

function formatTime(ms){
  if(ms<0) ms=0;
  const totalSec = Math.floor(ms/1000);
  const m = Math.floor(totalSec/60);
  const s = totalSec%60;
  return String(m).padStart(2,'0')+':'+String(s).padStart(2,'0');
}

function renderTimerDisplay(ms){
  const badge = document.getElementById('timerBadge');
  if(!badge) return;
  badge.classList.remove('warn','danger','paused');
  if(isTimerPaused){
    badge.textContent = formatTime(ms) + ' (PAUSED)';
    badge.classList.add('paused');
  } else {
    badge.textContent = formatTime(ms);
    if(ms<=2*60*1000) badge.classList.add('danger');
    else if(ms<=10*60*1000) badge.classList.add('warn');
  }
}

function stopTimer(){
  if(timerInterval){ clearInterval(timerInterval); timerInterval=null; }
}

function tick(){
  if(isTimerPaused) return;
  const remaining = examEndAt - Date.now();
  if(remaining<=0){
    remainingTimeMs = 0;
    renderTimerDisplay(0);
    stopTimer();
    if(!submitted){
      grade(true);
    }
    return;
  }
  remainingTimeMs = remaining;
  renderTimerDisplay(remaining);
}

function startTimer(endAt){
  examEndAt = endAt;
  remainingTimeMs = Math.max(0, examEndAt - Date.now());
  stopTimer();
  if(!navigator.onLine){
    pauseTimer();
  } else {
    isTimerPaused = false;
    tick();
    timerInterval = setInterval(tick, 1000);
  }
}

function pauseTimer(){
  if(submitted) return;
  if(!isTimerPaused && examEndAt){
    remainingTimeMs = Math.max(0, examEndAt - Date.now());
  }
  isTimerPaused = true;
  stopTimer();
  renderTimerDisplay(remainingTimeMs);
}

function resumeTimer(){
  if(submitted) return;
  if(isTimerPaused || !timerInterval){
    isTimerPaused = false;
    if(remainingTimeMs > 0){
      startTimer(Date.now() + remainingTimeMs);
    } else {
      renderTimerDisplay(0);
    }
  }
}

function updateOnlineBadge(){
  const badge = document.getElementById('onlineBadge');
  if(!badge) return;
  if(navigator.onLine){
    badge.classList.remove('offline');
    badge.classList.add('online');
    badge.innerHTML = '<span class="online-dot"></span>Online';
    if(examEndAt && !submitted && isTimerPaused){
      resumeTimer();
      saveState();
    }
  }else{
    badge.classList.remove('online');
    badge.classList.add('offline');
    badge.innerHTML = '<span class="online-dot"></span>Offline';
    if(examEndAt && !submitted){
      pauseTimer();
      saveState();
    }
  }
}
window.addEventListener('online', updateOnlineBadge);
window.addEventListener('offline', updateOnlineBadge);

const saved = loadState();
if(saved){
  questionOrderMap = saved.questionOrder || {};
  optionOrderMap = saved.optionOrder || {};
  matrixOrderMap = saved.matrixOrder || {};
  
  buildFlat(questionOrderMap, optionOrderMap, matrixOrderMap);

  answers = saved.answers || {};
  currentIndex = Math.min(saved.currentIndex||0, FLAT.length-1);
  submitted = !!saved.submitted;
  resultSent = !!saved.resultSent;
  violationCount = saved.violationCount || 0;
  updateViolationBadge();
  updateResetButton();
  document.getElementById('stuName').value = saved.name || '';
  document.getElementById('stuClass').value = saved.cls || '';
  document.getElementById('gateScreen').style.display = 'none';
  document.getElementById('appMain').style.display = 'block';

  if(submitted){
    let earnedR=0, totalR=0;
    FLAT.forEach(q=>{
      const r = computeResult(q);
      earnedR += r.earned;
      totalR += r.total;
    });
    const nilaiMentahR = totalR > 0 ? (earnedR / totalR) * 100 : 0;
    const nilaiR = Math.max(0, Math.min(100, Math.round(nilaiMentahR)));
    document.getElementById('scoreBig').textContent = nilaiR;
    document.getElementById('scoreSub').textContent = 'Nilai Akhir (0-100)';
    const msg = document.getElementById('scoreMsg');
    msg.textContent = 'Ujian selesai dikerjakan. Terima kasih sudah mengerjakan ujian ini!';
    msg.style.color = 'var(--navy)';
    msg.style.background = '#eef0fb';
    document.getElementById('resultsBox').classList.add('show');
    document.getElementById('submitBtn').disabled = true;
    document.getElementById('timerBadge').textContent = 'Finished';
    const penaltiR = violationCount * VIOLATION_PENALTY;
    if(resultSent){
      const note = document.getElementById('sendNote');
      if(note){ note.textContent = 'Answers submitted! Thank you.'; note.className = 'send-note ok'; }
    } else {
      attemptSend(saved.name || '', saved.cls || '', {nilai: nilaiR, earned: earnedR, total: totalR, penalti: penaltiR, violationCount});
    }
  } else {
    examActive = true;
    requestExamFullscreen();
    updateFullscreenButton();
    let rem = saved.remainingTimeMs;
    if(rem === undefined && saved.endAt){
      rem = saved.endAt - Date.now();
    }
    remainingTimeMs = Math.max(0, rem !== undefined ? rem : TIMER_MS);
    if(remainingTimeMs <= 0){
      renderTimerDisplay(0);
      grade(true);
    } else if(!navigator.onLine || saved.isTimerPaused){
      isTimerPaused = true;
      pauseTimer();
    } else {
      startTimer(Date.now() + remainingTimeMs);
    }
  }
} else {
  DATA.forEach(sec => {
    let qArr = [...sec.questions];
    shuffleArray(qArr);
    questionOrderMap[sec.id] = qArr.map(q => q.id);
    
    sec.questions.forEach(q => {
      if (Array.isArray(q.options)) {
        let optCopy = [...q.options];
        shuffleArray(optCopy);
        optionOrderMap[q.id] = optCopy.map(o => o.k);
      }
      if (q.type === 'matrix') {
        let indices = q.statements.map((_, idx) => idx);
        shuffleArray(indices);
        matrixOrderMap[q.id] = indices;
      }
    });
  });
  buildFlat(questionOrderMap, optionOrderMap, matrixOrderMap);
}

renderStage();
renderPalette();
updateProgress();
updateOnlineBadge();

if(saved && !saved.submitted && (remainingTimeMs <= 0)){
  grade(true);
}

function checkGate(){
  const name = document.getElementById('gateName').value.trim();
  const cls = document.getElementById('gateClass').value.trim();
  const token = document.getElementById('gateToken').value.trim().toUpperCase();
  const err = document.getElementById('gateError');

  if(!name){
    err.textContent = 'Please fill in your Name.';
    return;
  }
  if(!cls){
    err.textContent = 'Please select your Class.';
    return;
  }
  if(!token){
    err.textContent = 'Please enter the Exam Token.';
    return;
  }

  if(token !== CLASS_TOKENS[cls]){
    err.textContent = `Invalid token '${token}' for class ${cls}.`;
    return;
  }

  err.textContent = '';
  document.getElementById('stuName').value = name;
  document.getElementById('stuClass').value = cls;
  document.getElementById('gateScreen').style.display = 'none';
  document.getElementById('appMain').style.display = 'block';
  window.scrollTo({top:0});

  const rulesModal = document.getElementById('rulesModal');
  const rulesCheck = document.getElementById('rulesAgreeCheck');
  const rulesBtn = document.getElementById('rulesStartBtn');
  rulesCheck.checked = false;
  rulesBtn.disabled = true;
  rulesModal.classList.add('show');
}

function beginExamAfterConsent(){
  document.getElementById('rulesModal').classList.remove('show');
  examActive = true;
  requestExamFullscreen();
  updateFullscreenButton();
  startTimer(Date.now()+TIMER_MS);
  saveState();
}

document.getElementById('rulesAgreeCheck').addEventListener('change', function(){
  document.getElementById('rulesStartBtn').disabled = !this.checked;
});

document.getElementById('rulesStartBtn').addEventListener('click', ()=>{
  if(document.getElementById('rulesAgreeCheck').checked){
    beginExamAfterConsent();
  }
});

document.getElementById('backToLoginBtn').addEventListener('click', ()=>{
  saveState();
  stopTimer();
  examActive = false;
  updateFullscreenButton();
  document.getElementById('gateName').value = document.getElementById('stuName').value || '';
  const currentCls = document.getElementById('stuClass').value || '';
  document.getElementById('gateClass').value = currentCls;
  document.getElementById('gateToken').value = '';
  document.getElementById('gateError').textContent = '';
  document.getElementById('appMain').style.display = 'none';
  document.getElementById('gateScreen').style.display = 'flex';
  window.scrollTo({top:0});
});

document.getElementById('gateSubmitBtn').addEventListener('click', checkGate);
document.getElementById('gateToken').addEventListener('keydown', e=>{
  if(e.key === 'Enter') checkGate();
});
document.getElementById('gateName').addEventListener('keydown', e=>{
  if(e.key === 'Enter') key = 'Enter'; checkGate();
});
</script>
</body>
</html>
