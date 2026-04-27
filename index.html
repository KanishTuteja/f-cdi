<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>f-cdi Task War Room</title>

  <script src="https://cdn.tailwindcss.com"></script>
  <script crossorigin src="https://unpkg.com/react@18/umd/react.development.js"></script>
  <script crossorigin src="https://unpkg.com/react-dom@18/umd/react-dom.development.js"></script>
  <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>

  <script src="https://www.gstatic.com/firebasejs/10.12.2/firebase-app-compat.js"></script>
  <script src="https://www.gstatic.com/firebasejs/10.12.2/firebase-firestore-compat.js"></script>
  <script src="https://www.gstatic.com/firebasejs/10.12.2/firebase-storage-compat.js"></script>
  <script src="https://www.gstatic.com/firebasejs/10.12.2/firebase-auth-compat.js"></script>
  <script src="https://www.gstatic.com/firebasejs/10.12.2/firebase-database-compat.js"></script>

  <script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js"></script>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/xlsx/0.18.5/xlsx.full.min.js"></script>
  <script src="https://unpkg.com/pdf-lib@1.17.1/dist/pdf-lib.min.js"></script>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/chess.js/0.10.3/chess.min.js"></script>

  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&family=Playfair+Display:wght@500;600;700;800;900&family=JetBrains+Mono:wght@400;500;600;700&family=Bebas+Neue&display=swap" rel="stylesheet" />

  <style>
    /* ═══════════════════════════════════════════════════════════
       DESIGN TOKENS — Dark Mode (default)
    ═══════════════════════════════════════════════════════════ */
    :root {
      --bg:        #1c1c1c;
      --bg-2:      #232323;
      --bg-3:      #2a2a2a;
      --line:      #303030;
      --line-2:    #404040;
      --text:      #f4f4f4;
      --muted:     #9a9a9a;
      --faint:     #666666;
      --orange:    #fb923c;
      --orange-2:  #f97316;
      --blue:      #60a5fa;
      --green:     #4ade80;
      --red:       #f87171;
      --pink:      #fb7185;
      --input-bg:  #232323;
      --shadow:    rgba(0,0,0,.4);
      --card-hover:#2f2f2f;
      --topbar-bg: #1c1c1c;
    }

    /* ═══ Light Mode ═══ */
    [data-theme="light"] {
      --bg:        #f0ece4;
      --bg-2:      #ffffff;
      --bg-3:      #e8e4dc;
      --line:      #d5d0c8;
      --line-2:    #c0bab0;
      --text:      #1a1a1a;
      --muted:     #6b6560;
      --faint:     #9a9490;
      --orange:    #e87b20;
      --orange-2:  #d96a10;
      --blue:      #3b82f6;
      --green:     #16a34a;
      --red:       #dc2626;
      --pink:      #e11d48;
      --input-bg:  #ffffff;
      --shadow:    rgba(0,0,0,.1);
      --card-hover:#f5f1ea;
      --topbar-bg: #f0ece4;
    }

    /* Rage mode for Month End */
    .rage-mode {
      --bg:#0c0606; --bg-2:#1a0606; --bg-3:#220808;
      --line:rgba(255,80,0,.18); --line-2:rgba(255,80,0,.35);
      --text:#f0d0c0; --muted:#a07060; --faint:#604030;
      --input-bg:#1a0606; --topbar-bg:#0c0606;
    }
    [data-theme="light"] .rage-mode {
      --bg:#fdf5f0; --bg-2:#fff8f4; --bg-3:#f5ebe4;
      --line:rgba(200,80,0,.18); --line-2:rgba(200,80,0,.35);
      --text:#3a1a0a; --muted:#8a5a40; --faint:#a08070;
      --input-bg:#fff8f4; --topbar-bg:#fdf5f0;
    }

    *{box-sizing:border-box;}
    html,body,#root{margin:0;padding:0;width:100%;min-height:100vh;}
    html,body{background:var(--bg);color:var(--text);font-family:'Inter',system-ui,sans-serif;-webkit-font-smoothing:antialiased;transition:background 200ms,color 200ms;}

    /* Typography */
    .serif{font-family:'Playfair Display',Georgia,serif;letter-spacing:-.015em;}
    .mono{font-family:'JetBrains Mono',ui-monospace,monospace;}
    .rage-font{font-family:'Bebas Neue',sans-serif;letter-spacing:.06em;}

    .label{font-family:'JetBrains Mono',ui-monospace,monospace;font-size:11px;text-transform:uppercase;letter-spacing:.16em;color:var(--muted);font-weight:500;}

    .wordmark{font-family:'Playfair Display',Georgia,serif;font-weight:600;font-size:20px;letter-spacing:-.01em;}

    .card{background:var(--bg-2);border:1px solid var(--line);border-radius:14px;transition:border-color 180ms ease,background 180ms ease,transform 180ms ease;}
    .card:hover{border-color:var(--line-2);}
    .card-flat{background:var(--bg-2);border:1px solid var(--line);border-radius:12px;}

    .btn{display:inline-flex;align-items:center;gap:8px;padding:8px 16px;border-radius:8px;font-weight:500;font-size:13px;border:1px solid var(--line);background:transparent;color:var(--text);cursor:pointer;transition:all 160ms ease;font-family:inherit;}
    .btn:hover{background:var(--bg-3);border-color:var(--line-2);}
    .btn-primary{background:#3b82f6;border-color:#3b82f6;color:#fff;}
    .btn-primary:hover{background:#2563eb;border-color:#2563eb;}
    .btn-orange{background:var(--orange-2);border-color:var(--orange-2);color:#fff;}
    .btn-orange:hover{background:#ea580c;}
    .btn-danger{background:var(--red);border-color:var(--red);color:#fff;}
    .btn-danger:hover{opacity:.85;}
    .btn-ghost{background:transparent;border:none;color:var(--text);padding:6px 12px;}
    .btn-ghost:hover{color:var(--orange);background:transparent;}
    .btn-link{background:transparent;border:none;color:var(--blue);padding:0;font-size:13px;text-decoration:none;cursor:pointer;font-family:inherit;}
    .btn-link:hover{text-decoration:underline;}

    .topbar{display:flex;align-items:center;justify-content:space-between;padding:14px 24px;border-bottom:1px solid var(--line);position:sticky;top:0;z-index:50;background:var(--topbar-bg);transition:background 200ms;}

    .input{background:var(--input-bg);border:1px solid var(--line);border-radius:8px;padding:8px 12px;color:var(--text);font-family:inherit;font-size:13px;outline:none;transition:border-color 160ms ease,background 200ms,color 200ms;}
    .input:focus{border-color:var(--orange);}
    .input:disabled{opacity:.5;cursor:not-allowed;}
    input[type=number]::-webkit-outer-spin-button,input[type=number]::-webkit-inner-spin-button{-webkit-appearance:none;margin:0;}
    input[type=number]{-moz-appearance:textfield;}
    select.input{cursor:pointer;}

    .chat-panel{position:fixed;top:0;left:0;width:380px;max-width:92vw;height:100vh;background:var(--bg-2);border-right:1px solid var(--line);z-index:60;display:flex;flex-direction:column;transform:translateX(0);transition:transform 280ms cubic-bezier(.4,0,.2,1);}
    .chat-panel.closed{transform:translateX(-110%);}

    .chat-fab{position:fixed;bottom:24px;right:24px;z-index:55;width:52px;height:52px;border-radius:50%;background:var(--bg-2);border:1px solid var(--line-2);display:flex;align-items:center;justify-content:center;cursor:pointer;box-shadow:0 8px 24px var(--shadow);transition:transform 200ms,border-color 200ms;}
    .chat-fab:hover{transform:scale(1.06);border-color:var(--orange);}
    .chat-fab-badge{position:absolute;top:-4px;right:-4px;min-width:20px;height:20px;border-radius:999px;background:var(--orange-2);color:#fff;font-size:10px;font-weight:700;display:flex;align-items:center;justify-content:center;padding:0 5px;border:2px solid var(--bg);}

    @keyframes pulse-orange{0%,100%{box-shadow:0 0 0 0 rgba(251,146,60,.5),0 8px 24px var(--shadow);}50%{box-shadow:0 0 0 10px rgba(251,146,60,0),0 8px 24px var(--shadow);}}
    .pulse-orange{animation:pulse-orange 1.6s ease-in-out infinite;}
    @keyframes dot-pulse{0%,100%{opacity:1;}50%{opacity:.4;}}
    .dot-pulse{animation:dot-pulse 1.8s ease-in-out infinite;}
    @keyframes fade-in{from{opacity:0;transform:translateY(6px);}to{opacity:1;transform:none;}}
    .fade-in{animation:fade-in 200ms ease-out forwards;}

    .scroll::-webkit-scrollbar{width:6px;height:6px;}
    .scroll::-webkit-scrollbar-track{background:transparent;}
    .scroll::-webkit-scrollbar-thumb{background:var(--line-2);border-radius:99px;}
    .scroll::-webkit-scrollbar-thumb:hover{background:var(--faint);}

    .modal-bg{position:fixed;inset:0;z-index:1000;background:rgba(0,0,0,.65);backdrop-filter:blur(2px);display:flex;align-items:center;justify-content:center;padding:24px;}
    .modal{width:min(440px,100%);background:var(--bg-2);border:1px solid var(--line-2);border-radius:14px;padding:24px;}

    .dropzone{border:1.5px dashed var(--line-2);border-radius:12px;transition:all 180ms ease;background:var(--bg-2);}
    .dropzone.over{border-color:var(--orange);background:rgba(251,146,60,.05);}

    .seg{display:inline-flex;background:var(--bg-2);border:1px solid var(--line);border-radius:999px;padding:3px;}
    .seg-btn{padding:6px 16px;border-radius:999px;font-size:12px;font-weight:500;color:var(--muted);background:transparent;border:none;cursor:pointer;transition:all 160ms ease;font-family:inherit;}
    .seg-btn.on{background:var(--orange-2);color:#fff;}
    .seg-btn:hover:not(.on){color:var(--text);}

    .member-tile{position:relative;padding:18px;border-radius:14px;background:var(--bg-2);border:1px solid var(--line);transition:all 180ms ease;}
    .member-tile.me{border-color:var(--orange);}
    .member-tile.drag-over{border-color:var(--orange);background:rgba(251,146,60,.05);}

    .bar{position:relative;height:4px;border-radius:99px;background:var(--bg-3);overflow:hidden;}
    .bar-fill{position:absolute;left:0;top:0;bottom:0;border-radius:99px;transition:width 380ms cubic-bezier(.4,0,.2,1);}

    .chip{display:inline-flex;align-items:center;gap:8px;padding:6px 14px;border-radius:999px;font-size:13px;font-weight:500;cursor:grab;user-select:none;border:1px solid;transition:transform 160ms;}
    .chip:active{cursor:grabbing;}
    .chip:hover{transform:translateY(-2px);}

    .tracker-wrap{display:grid;grid-template-columns:1fr 1fr;gap:12px;}
    @media(max-width:900px){.tracker-wrap{grid-template-columns:1fr;}}

    .no-scroll::-webkit-scrollbar{display:none;}

    .hr{height:1px;background:var(--line);margin:24px 0;}

    .pill{display:inline-block;padding:2px 8px;border-radius:99px;font-size:10px;font-weight:600;font-family:'JetBrains Mono',monospace;text-transform:uppercase;letter-spacing:.08em;}

    /* Folder tab buttons */
    .folder-tab{padding:10px 20px;border-radius:10px 10px 0 0;font-size:13px;font-weight:600;border:1px solid var(--line);border-bottom:none;background:var(--bg);color:var(--muted);cursor:pointer;transition:all 160ms;font-family:inherit;position:relative;bottom:-1px;}
    .folder-tab.active{background:var(--bg-2);color:var(--text);border-color:var(--line);}

    /* Theme toggle */
    .theme-toggle{width:38px;height:22px;border-radius:99px;background:var(--bg-3);border:1px solid var(--line);cursor:pointer;position:relative;transition:all 200ms;flex-shrink:0;}
    .theme-toggle .knob{position:absolute;top:2px;left:2px;width:16px;height:16px;border-radius:50%;background:var(--orange);transition:transform 200ms;}
    [data-theme="light"] .theme-toggle .knob{transform:translateX(16px);}

    /* File item row */
    .file-item{display:flex;align-items:center;justify-content:space-between;padding:6px 10px;border-radius:6px;background:var(--bg);border:1px solid var(--line);margin-bottom:4px;font-size:12px;gap:8px;}
    .file-item .file-name{white-space:nowrap;overflow:hidden;text-overflow:ellipsis;flex:1;min-width:0;}
    .file-item .remove-btn{background:none;border:none;color:var(--red);cursor:pointer;font-size:14px;flex-shrink:0;padding:0 4px;}


    /* Notifications, Chess, and Financial Inquiry */
    .toast-stack{position:fixed;top:76px;right:18px;z-index:2000;display:flex;flex-direction:column;gap:8px;max-width:340px;}
    .toast{background:var(--bg-2);border:1px solid var(--line-2);border-left:4px solid var(--orange);border-radius:12px;padding:12px 14px;box-shadow:0 12px 30px var(--shadow);animation:fade-in 180ms ease-out forwards;}
    .ping{color:var(--orange);font-weight:800;background:rgba(251,146,60,.12);border-radius:6px;padding:1px 4px;}

    .chess-modal{width:min(1120px,96vw);max-height:92vh;overflow:auto;background:linear-gradient(145deg,var(--bg-2),var(--bg));border:1px solid var(--line-2);border-radius:24px;padding:22px;box-shadow:0 28px 90px rgba(0,0,0,.52);}
    .chess-layout{display:grid;grid-template-columns:minmax(320px,520px) minmax(300px,1fr);gap:20px;align-items:start;}
    .chess-board-shell{padding:14px;border-radius:24px;background:linear-gradient(145deg,rgba(251,146,60,.16),rgba(96,165,250,.08));border:1px solid var(--line-2);box-shadow:inset 0 1px 0 rgba(255,255,255,.04),0 16px 40px var(--shadow);}
    .chess-player-card{display:flex;align-items:center;justify-content:space-between;gap:12px;padding:10px 12px;border:1px solid var(--line);border-radius:16px;background:rgba(255,255,255,.03);margin:8px 0;}
    [data-theme="light"] .chess-player-card{background:rgba(255,255,255,.75);}
    .chess-board{display:grid;grid-template-columns:repeat(8,minmax(0,1fr));grid-template-rows:repeat(8,minmax(0,1fr));width:min(72vw,492px);max-width:100%;aspect-ratio:1/1;border:1px solid var(--line-2);border-radius:18px;overflow:hidden;box-shadow:0 18px 46px rgba(0,0,0,.32);background:#111;}
    .chess-square{position:relative;display:flex;align-items:center;justify-content:center;width:100%;height:100%;aspect-ratio:1/1;padding:0;margin:0;border:0;line-height:1;font-size:clamp(24px,5.2vw,46px);cursor:pointer;transition:transform 120ms,box-shadow 120ms,filter 120ms;background:#f3dfbf;color:#15100b;font-family:'Segoe UI Symbol','Apple Color Emoji','Noto Color Emoji',serif;}
    .chess-square.dark{background:#8a6248;}
    .chess-square:hover:not(:disabled){filter:brightness(1.08);}
    .chess-square:disabled{cursor:not-allowed;opacity:1;}
    .chess-square.selected{box-shadow:inset 0 0 0 4px var(--orange), inset 0 0 24px rgba(251,146,60,.28);z-index:2;}
    .chess-square.legal:after{content:'';width:22%;height:22%;border-radius:50%;background:rgba(74,222,128,.78);position:absolute;box-shadow:0 0 0 6px rgba(74,222,128,.14);}
    .chess-square.legal:not(:empty):after{width:82%;height:82%;background:transparent;border:4px solid rgba(74,222,128,.72);box-shadow:none;}
    .chess-square.last{box-shadow:inset 0 0 0 4px rgba(96,165,250,.8), inset 0 0 22px rgba(96,165,250,.22);z-index:1;}
    .chess-side{display:flex;flex-direction:column;gap:12px;min-width:min(380px,100%);}
    .move-list{max-height:190px;overflow:auto;background:var(--bg);border:1px solid var(--line);border-radius:14px;padding:12px;font-size:12px;line-height:1.8;white-space:pre-wrap;}

    .inquiry-card{position:relative;overflow:hidden;}
    .inquiry-card:before{content:'';position:absolute;inset:0;background:radial-gradient(circle at top right,rgba(251,146,60,.16),transparent 42%);pointer-events:none;}
    .inquiry-grid{display:grid;grid-template-columns:1.05fr 1.95fr;gap:14px;align-items:stretch;position:relative;}
    .inquiry-now{padding:18px;border-radius:16px;background:linear-gradient(145deg,rgba(251,146,60,.14),rgba(96,165,250,.06));border:1px solid var(--line-2);}
    .inquiry-roster{display:grid;grid-template-columns:repeat(4,minmax(130px,1fr));gap:8px;}
    .inquiry-slot{padding:10px;border:1px solid var(--line);background:var(--bg);border-radius:12px;display:flex;align-items:center;gap:8px;min-width:0;}
    .inquiry-slot.active{border-color:var(--orange);background:rgba(251,146,60,.10);box-shadow:0 0 0 1px rgba(251,146,60,.14);}
    .inquiry-slot.next{border-color:rgba(96,165,250,.45);}
    .inquiry-progress{height:9px;border-radius:999px;background:var(--bg-3);overflow:hidden;border:1px solid var(--line);}
    .inquiry-progress-fill{height:100%;border-radius:999px;background:linear-gradient(90deg,var(--orange),var(--green));transition:width 500ms ease;}


    .lunch-card{position:relative;overflow:hidden;}
    .lunch-card:before{content:'';position:absolute;inset:0;background:radial-gradient(circle at top left,rgba(251,191,36,.16),transparent 42%);pointer-events:none;}
    .lunch-wrap{display:grid;grid-template-columns:minmax(260px,.9fr) minmax(320px,1.6fr);gap:14px;position:relative;}
    .lunch-control{padding:18px;border:1px solid var(--line-2);border-radius:16px;background:linear-gradient(145deg,rgba(251,191,36,.14),rgba(251,146,60,.07));}
    .lunch-toggle{width:100%;justify-content:center;padding:11px 14px;border-radius:14px;font-weight:800;}
    .lunch-toggle.on{background:var(--orange-2);border-color:var(--orange-2);color:#fff;box-shadow:0 12px 30px rgba(249,115,22,.22);}
    .lunch-active-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(210px,1fr));gap:10px;}
    .lunch-person{padding:12px;border:1px solid var(--line);border-radius:14px;background:var(--bg);display:flex;align-items:flex-start;gap:10px;min-width:0;}
    .lunch-person.live{border-color:rgba(251,146,60,.62);background:rgba(251,146,60,.09);box-shadow:0 0 0 1px rgba(251,146,60,.12);}
    .lunch-message{font-size:12px;color:var(--muted);line-height:1.45;margin-top:4px;}
    .lunch-empty{padding:18px;border:1px dashed var(--line-2);border-radius:14px;background:var(--bg);color:var(--muted);font-size:13px;text-align:center;}


    .payment-card{position:relative;overflow:hidden;}
    .payment-card:before{content:'';position:absolute;inset:0;background:radial-gradient(circle at top right,rgba(34,197,94,.13),transparent 42%);pointer-events:none;}
    .payment-toolbar{display:flex;align-items:center;justify-content:space-between;gap:10px;flex-wrap:wrap;position:relative;}
    .payment-grid{display:grid;grid-template-columns:minmax(280px,.72fr) minmax(380px,1.6fr);gap:14px;position:relative;}
    .payment-upload{padding:16px;border:1px solid var(--line-2);border-radius:16px;background:linear-gradient(145deg,rgba(34,197,94,.12),rgba(251,146,60,.05));}
    .payment-table-wrap{border:1px solid var(--line);border-radius:14px;overflow:auto;background:var(--bg);max-height:460px;}
    .payment-table{width:100%;border-collapse:separate;border-spacing:0;font-size:12px;min-width:1120px;}
    .payment-table th{position:sticky;top:0;background:var(--bg-2);z-index:1;text-align:left;padding:9px 10px;border-bottom:1px solid var(--line);color:var(--text);font-weight:800;font-family:'Inter',system-ui,sans-serif;font-size:11px;white-space:normal;line-height:1.25;}
    .payment-table td{padding:9px 10px;border-bottom:1px solid var(--line);vertical-align:top;color:var(--text);}
    .payment-table tr:hover td{background:rgba(34,197,94,.05);}
    .payment-table tr.ready td{background:rgba(251,191,36,.07);}
    .payment-table tr.processed td{background:rgba(74,222,128,.12);}
    .payment-table tr.active td{box-shadow:inset 3px 0 0 var(--orange);}
    .payment-panel{margin-top:14px;display:grid;grid-template-columns:minmax(300px,.9fr) minmax(360px,1.1fr);gap:12px;}
    .payment-box{border:1px solid var(--line);border-radius:14px;background:var(--bg);padding:12px;min-height:150px;}
    @media(max-width:1050px){.payment-grid,.payment-panel{grid-template-columns:1fr}.payment-table-wrap{max-height:360px}}
    /* WorkEasy Hub — Midnight Forest */
    .workeasy-shell{display:grid;grid-template-columns:240px minmax(0,1fr);gap:18px;margin-bottom:48px;background:#101815;border:1px solid rgba(110,231,183,.18);border-radius:22px;padding:16px;box-shadow:0 22px 55px rgba(0,0,0,.28);}
    .workeasy-sidebar{background:#0b1210;border:1px solid rgba(110,231,183,.16);border-radius:18px;padding:16px;display:flex;flex-direction:column;gap:10px;min-height:520px;position:sticky;top:82px;align-self:start;}
    .workeasy-brand{font-family:'Playfair Display',Georgia,serif;font-size:24px;font-weight:800;color:#ecfdf5;line-height:1;}
    .workeasy-nav{width:100%;text-align:left;padding:12px 13px;border-radius:13px;border:1px solid rgba(110,231,183,.14);background:#13201b;color:#c7f9df;cursor:pointer;font-weight:800;font-size:13px;font-family:inherit;transition:all 160ms ease;}
    .workeasy-nav:hover,.workeasy-nav.active{background:#10b981;color:#052e23;border-color:#34d399;box-shadow:0 10px 28px rgba(16,185,129,.20);}
    .workeasy-stat{display:flex;align-items:center;justify-content:space-between;border:1px solid rgba(110,231,183,.13);background:#111b17;border-radius:12px;padding:10px 12px;color:#a7b5ad;font-size:12px;margin-top:4px;}
    .workeasy-stat strong{color:#d1fae5;font-size:18px;}
    .workeasy-main{min-width:0;}
    .workeasy-header{display:flex;justify-content:space-between;align-items:flex-start;gap:14px;flex-wrap:wrap;background:linear-gradient(145deg,#14211c,#0d1713);border:1px solid rgba(110,231,183,.16);border-radius:18px;padding:18px;color:#ecfdf5;margin-bottom:12px;}
    .workeasy-controls{display:flex;align-items:center;gap:8px;flex-wrap:wrap;margin-bottom:12px;background:#0d1713;border:1px solid rgba(110,231,183,.12);border-radius:15px;padding:10px;}
    .workeasy-search{flex:1;min-width:260px;background:#0b1210;border:1px solid rgba(110,231,183,.20);border-radius:12px;padding:11px 13px;color:#ecfdf5;font-size:13px;outline:none;}
    .workeasy-search:focus,.workeasy-inline-input:focus,.workeasy-notes:focus{border-color:#34d399;box-shadow:0 0 0 3px rgba(52,211,153,.11);}
    .workeasy-btn,.workeasy-small,.workeasy-mini-btn{border:none;border-radius:12px;background:#10b981;color:#052e23;font-weight:900;cursor:pointer;font-family:inherit;transition:all 160ms ease;}
    .workeasy-btn{padding:10px 14px;font-size:13px;}.workeasy-small{padding:9px 11px;font-size:12px;}.workeasy-mini-btn{padding:7px 9px;font-size:11px;border-radius:10px;white-space:nowrap;}
    .workeasy-btn:hover,.workeasy-small:hover,.workeasy-mini-btn:hover{filter:brightness(1.08);transform:translateY(-1px);}
    .workeasy-btn.secondary,.workeasy-mini-btn.muted{background:#1f352d;color:#bbf7d0;border:1px solid rgba(110,231,183,.20);}.workeasy-btn.danger{background:#7f1d1d;color:#fee2e2;}
    .workeasy-empty{border:1px dashed rgba(110,231,183,.25);border-radius:16px;background:#0d1713;color:#a7b5ad;text-align:center;padding:48px 18px;font-size:14px;}
    .workeasy-master-grid,.workeasy-payment-grid{display:grid;grid-template-columns:minmax(0,1.55fr) minmax(360px,.8fr);gap:12px;align-items:start;}
    .workeasy-table-wrap{background:#0b1210;border:1px solid rgba(110,231,183,.15);border-radius:16px;overflow:auto;max-height:680px;}
    .workeasy-table{width:100%;border-collapse:separate;border-spacing:0;min-width:1600px;color:#ecfdf5;font-size:12px;}.payment-mode-table{min-width:980px;}
    .workeasy-table th{position:sticky;top:0;z-index:2;background:#15251f;color:#d1fae5;text-align:left;padding:10px;border-bottom:1px solid rgba(110,231,183,.18);font-size:11px;line-height:1.25;white-space:normal;}
    .workeasy-table td{padding:9px 10px;border-bottom:1px solid rgba(110,231,183,.09);vertical-align:top;max-width:260px;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;color:#edfdf5;}
    .workeasy-table tr:hover td{background:rgba(16,185,129,.08);}.workeasy-table tr.active td{box-shadow:inset 3px 0 0 #34d399;background:rgba(16,185,129,.10);}.workeasy-table tr.ready td{background:rgba(250,204,21,.10);}.workeasy-table tr.processed td{background:rgba(34,197,94,.18);}
    .workeasy-table .notes-cell{min-width:360px;max-width:520px;white-space:normal;line-height:1.45;}
    .workeasy-focus{background:#0b1210;border:1px solid rgba(110,231,183,.16);border-radius:16px;padding:14px;color:#ecfdf5;min-width:0;}
    .workeasy-notes{width:100%;min-height:260px;background:#101b17;border:1px solid rgba(110,231,183,.18);border-radius:14px;color:#ecfdf5;padding:13px;resize:vertical;font-size:13px;line-height:1.65;outline:none;}
    .workeasy-detail-list{margin-top:12px;max-height:270px;overflow:auto;display:grid;gap:6px;}.workeasy-detail-row{display:grid;grid-template-columns:150px minmax(0,1fr);gap:10px;border-bottom:1px solid rgba(110,231,183,.10);padding-bottom:6px;font-size:12px;}.workeasy-detail-row span{font-family:'JetBrains Mono',monospace;color:#7dd3ae;font-size:10px;text-transform:uppercase;letter-spacing:.06em;}.workeasy-detail-row p{margin:0;white-space:pre-wrap;color:#ecfdf5;}
    .workeasy-inline-input{width:100%;min-width:150px;background:#101b17;border:1px solid rgba(110,231,183,.20);border-radius:10px;color:#ecfdf5;padding:8px 9px;outline:none;font-size:12px;}
    @media(max-width:1100px){.workeasy-shell{grid-template-columns:1fr}.workeasy-sidebar{position:relative;top:0;min-height:auto}.workeasy-master-grid,.workeasy-payment-grid{grid-template-columns:1fr}}


    @media(max-width:1050px){.lunch-wrap{grid-template-columns:1fr}}
    @media(max-width:1050px){.inquiry-grid{grid-template-columns:1fr}.inquiry-roster{grid-template-columns:repeat(2,minmax(130px,1fr))}}
    @media(max-width:900px){.topbar{flex-wrap:wrap;gap:10px}.chess-modal{padding:14px}.chess-layout{grid-template-columns:1fr;align-items:center}.chess-board{width:86vw}.toast-stack{left:14px;right:14px;max-width:none}}


    /* ================= WORK EASY HUB ================= */
    .workeasy-page-wrap{max-width:1560px;margin:0 auto;padding:34px 28px 80px;}
    .workeasy-page-hero{border:1px solid rgba(34,211,238,.22);background:linear-gradient(135deg,rgba(34,211,238,.10),rgba(167,139,250,.08),var(--bg-2));border-radius:24px;padding:28px;margin-bottom:18px;box-shadow:0 16px 44px var(--shadow);}
    .workeasy-release-card{margin-top:18px;padding:22px;border-radius:24px;border:1px solid rgba(34,211,238,.20);background:linear-gradient(145deg,var(--bg-2),rgba(34,211,238,.035));}
    .workeasy-release-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(230px,1fr));gap:10px;}
    .workeasy-release-row{padding:14px;border:1px solid var(--line);border-radius:16px;background:var(--bg);}
    .workeasy-release-row.me{border-color:#22d3ee;box-shadow:0 0 0 1px rgba(34,211,238,.14);}

    /* ================= WORK EASY HUB ================= */
    /* Modern compact dashboard, theme-aware, normalized typography */
    .we-wrap{max-width:1340px;margin:0 auto;padding:24px 24px 64px;}
    .we-head{display:flex;align-items:flex-start;justify-content:space-between;gap:16px;flex-wrap:wrap;border:1px solid var(--line);background:var(--bg-2);border-radius:18px;padding:18px 20px;margin-bottom:14px;box-shadow:0 6px 22px var(--shadow);}
    .we-head h1{font-family:'Inter',system-ui,sans-serif;font-size:22px;font-weight:700;letter-spacing:-.02em;line-height:1.2;margin:6px 0 4px;color:var(--text);}
    .we-head p{font-size:13px;line-height:1.55;color:var(--muted);margin:0;max-width:680px;}
    .we-tabs{display:inline-flex;background:var(--bg-2);border:1px solid var(--line);border-radius:12px;padding:3px;gap:2px;}
    .we-tab{appearance:none;border:none;background:transparent;color:var(--muted);font-family:inherit;font-size:12px;font-weight:600;padding:8px 14px;border-radius:9px;cursor:pointer;transition:all 160ms ease;letter-spacing:.01em;}
    .we-tab:hover{color:var(--text);}
    .we-tab.active{background:#22d3ee;color:#06181d;box-shadow:0 4px 14px rgba(34,211,238,.22);}
    [data-theme="light"] .we-tab.active{background:#0891b2;color:#fff;}
    .we-card{border:1px solid var(--line);background:var(--bg-2);border-radius:18px;padding:18px;box-shadow:0 6px 22px var(--shadow);}
    .we-card h2{font-family:'Inter',system-ui,sans-serif;font-size:16px;font-weight:700;letter-spacing:-.01em;margin:0 0 4px;color:var(--text);}
    .we-card-head{display:flex;align-items:flex-start;justify-content:space-between;gap:12px;flex-wrap:wrap;margin-bottom:14px;}
    .we-actions{display:flex;gap:8px;flex-wrap:wrap;align-items:center;}
    .we-btn{appearance:none;border:1px solid var(--line);background:var(--bg);color:var(--text);font-family:inherit;font-size:12px;font-weight:600;padding:8px 12px;border-radius:9px;cursor:pointer;transition:all 160ms ease;letter-spacing:.01em;display:inline-flex;align-items:center;gap:6px;}
    .we-btn:hover{border-color:#22d3ee;color:#22d3ee;}
    [data-theme="light"] .we-btn:hover{color:#0891b2;border-color:#0891b2;}
    .we-btn.primary{background:#22d3ee;border-color:#22d3ee;color:#06181d;}
    .we-btn.primary:hover{filter:brightness(1.06);color:#06181d;}
    [data-theme="light"] .we-btn.primary{background:#0891b2;border-color:#0891b2;color:#fff;}
    .we-btn.subtle{background:transparent;}
    .we-btn.danger{color:var(--red);border-color:var(--line);}
    .we-btn.danger:hover{background:rgba(248,113,113,.10);border-color:var(--red);color:var(--red);}
    .we-btn:disabled{opacity:.42;cursor:not-allowed;filter:none;}
    .we-btn:disabled:hover{border-color:var(--line);color:var(--text);}
    .we-upload{border:1.5px dashed var(--line-2);background:var(--bg);border-radius:14px;padding:28px;text-align:center;cursor:pointer;transition:all 160ms ease;}
    .we-upload:hover{border-color:#22d3ee;background:rgba(34,211,238,.04);}
    .we-upload-title{font-size:14px;font-weight:600;color:var(--text);margin-top:6px;}
    .we-upload-hint{font-size:12px;color:var(--muted);margin-top:4px;line-height:1.5;}
    .we-toolbar{display:grid;grid-template-columns:minmax(220px,1fr) auto;gap:10px;align-items:center;margin-bottom:12px;}
    .we-search{width:100%;background:var(--input-bg);border:1px solid var(--line);border-radius:10px;color:var(--text);font-family:inherit;font-size:13px;padding:9px 12px;outline:none;transition:border-color 160ms ease;}
    .we-search:focus{border-color:#22d3ee;}
    .we-input{width:100%;min-width:120px;background:var(--input-bg);border:1px solid var(--line);border-radius:8px;color:var(--text);font-family:inherit;font-size:12px;padding:7px 9px;outline:none;transition:border-color 160ms ease;}
    .we-input:focus{border-color:#22d3ee;}
    .we-stats{display:flex;gap:8px;flex-wrap:wrap;margin-bottom:12px;}
    .we-pill{display:inline-flex;align-items:center;gap:6px;border-radius:999px;border:1px solid var(--line);background:var(--bg);color:var(--muted);font-size:11px;font-weight:600;padding:4px 10px;letter-spacing:.02em;}
    .we-pill.ready{border-color:rgba(251,191,36,.4);color:#d97706;background:rgba(251,191,36,.08);}
    [data-theme="dark"] .we-pill.ready{color:#fbbf24;}
    .we-pill.done{border-color:rgba(34,197,94,.4);color:#15803d;background:rgba(34,197,94,.08);}
    [data-theme="dark"] .we-pill.done{color:#4ade80;}
    .we-table-wrap{border:1px solid var(--line);border-radius:14px;overflow:auto;background:var(--bg);max-height:560px;}
    .we-table{width:100%;border-collapse:separate;border-spacing:0;min-width:1040px;font-size:12px;}
    .we-table th{position:sticky;top:0;z-index:2;background:var(--bg-2);color:var(--muted);text-align:left;padding:10px 12px;border-bottom:1px solid var(--line);font-size:10px;font-weight:600;text-transform:uppercase;letter-spacing:.07em;white-space:nowrap;}
    .we-table td{padding:9px 12px;border-bottom:1px solid var(--line);vertical-align:middle;color:var(--text);}
    .we-table tr:last-child td{border-bottom:none;}
    .we-table tr:hover td{background:rgba(34,211,238,.04);}
    .we-table tr.ready td{background:rgba(251,191,36,.06);}
    .we-table tr.processed td{background:rgba(34,197,94,.10);}
    .we-name{font-weight:600;font-size:13px;color:var(--text);}
    .we-sub{font-size:11px;color:var(--muted);}
    .we-toast{position:fixed;left:50%;bottom:32px;transform:translateX(-50%);background:var(--bg-2);color:var(--text);border:1px solid #22d3ee;border-radius:12px;padding:10px 16px;font-size:13px;font-weight:500;box-shadow:0 12px 30px var(--shadow);z-index:120;animation:fade-in 180ms ease;}
    .we-preview{border:1px solid var(--line);background:var(--bg);border-radius:14px;padding:14px;margin-bottom:14px;}
    .we-preview-head{display:flex;align-items:center;justify-content:space-between;gap:10px;margin-bottom:10px;flex-wrap:wrap;}
    .we-preview-grid{display:grid;grid-template-columns:minmax(180px,.4fr) minmax(0,1fr);gap:12px;align-items:stretch;}
    .we-preview-meta{border:1px solid var(--line);background:var(--bg-2);border-radius:10px;padding:10px 12px;font-size:12px;}
    .we-preview-meta .label{margin-bottom:3px;}
    .we-preview-meta-row{margin-bottom:10px;word-break:break-word;color:var(--text);font-size:12.5px;}
    .we-preview-body{width:100%;min-height:230px;background:var(--input-bg);border:1px solid var(--line);border-radius:10px;color:var(--text);padding:12px;font-family:'JetBrains Mono',ui-monospace,monospace;font-size:12px;line-height:1.55;white-space:pre-wrap;resize:vertical;outline:none;}
    .we-preview-body:focus{border-color:#22d3ee;}
    .we-placeholder{border:1px dashed var(--line-2);background:var(--bg);border-radius:14px;padding:36px 22px;text-align:center;color:var(--muted);}
    .we-placeholder strong{display:block;font-size:14px;font-weight:700;color:var(--text);margin-bottom:6px;}
    @media(max-width:900px){.we-wrap{padding:16px 14px 60px}.we-head{padding:14px}.we-head h1{font-size:19px}.we-toolbar{grid-template-columns:1fr}.we-preview-grid{grid-template-columns:1fr}}

    /* Legacy V2 alias — keep so any older we-v2-* references render acceptably */
    .we-v2-wrap{max-width:1340px;margin:0 auto;padding:24px 24px 64px;}

  </style>
</head>
<body>
<div id="root"></div>

<!-- FIREBASE CONFIGURATION -->
<script>
  const FIREBASE_CONFIG = {
    apiKey:            "AIzaSyD6WtpGafpwnevz48Pfab-Jj1xnUfikG94",
    authDomain:        "f-cdi-48592.firebaseapp.com",
    databaseURL:       "https://f-cdi-48592-default-rtdb.firebaseio.com",
    projectId:         "f-cdi-48592",
    storageBucket:     "f-cdi-48592.firebasestorage.app",
    messagingSenderId: "563727887409",
    appId:             "1:563727887409:web:67b42c37e9046d03703910",
    measurementId:     "G-77LGG0ZG3S"
  };

  let firebaseApp, db, storage, realtimeDb;
  const HAS_FIREBASE_CONFIG = Object.values(FIREBASE_CONFIG).every(v => v && !String(v).includes('PASTE_'));

  try {
    if(!HAS_FIREBASE_CONFIG) throw new Error('Firebase config placeholders detected');

    firebaseApp = firebase.initializeApp(FIREBASE_CONFIG);
    db          = firebase.firestore();
    storage     = firebase.storage();
    realtimeDb  = firebase.database ? firebase.database() : null;

    console.log('%c Firebase connected: Firestore + Storage + Realtime Database ready','color:#4ade80;font-weight:bold');
  } catch(e) {
    console.warn('Firebase not configured — LOCAL DEMO mode.', e.message);
  }
</script>

<script type="text/babel">
  const { useEffect, useMemo, useRef, useState, useCallback } = React;

  /* ─── Constants ──────────────────────────────────────────── */
  const TEAM_MEMBERS = [
    { name:'Rushi',    accent:'#22d3ee', avatar:'https://api.dicebear.com/7.x/adventurer/svg?seed=Rushi&backgroundColor=232323' },
    { name:'Nancy',    accent:'#fb7185', avatar:'https://api.dicebear.com/7.x/adventurer/svg?seed=Nancy&backgroundColor=232323' },
    { name:'Parveen',  accent:'#fbbf24', avatar:'https://api.dicebear.com/7.x/adventurer/svg?seed=Parveen&backgroundColor=232323' },
    { name:'Viren',    accent:'#34d399', avatar:'https://api.dicebear.com/7.x/adventurer/svg?seed=Viren&backgroundColor=232323' },
    { name:'Aastha',   accent:'#c084fc', avatar:'https://api.dicebear.com/7.x/adventurer/svg?seed=Aastha&backgroundColor=232323' },
    { name:'Kanish',   accent:'#fb923c', avatar:'https://api.dicebear.com/7.x/adventurer/svg?seed=Kanish&backgroundColor=232323' },
    { name:'Devanshi', accent:'#5eead4', avatar:'https://api.dicebear.com/7.x/adventurer/svg?seed=Devanshi&backgroundColor=232323' },
    { name:'Jhanvi',   accent:'#e879f9', avatar:'https://api.dicebear.com/7.x/adventurer/svg?seed=Jhanvi&backgroundColor=232323' },
  ];
  const TASK_POOL = [
    { id:'gradFiles',       name:'Grad Files',       group:'File Closing', color:'#f87171' },
    { id:'dropFiles',       name:'Drop Files',        group:'File Closing', color:'#fb7185' },
    { id:'agreements',      name:'Agreements',        group:'Admissions',   color:'#60a5fa' },
    { id:'sparAgreement',   name:'SPAR Agreement',    group:'Admissions',   color:'#a78bfa' },
    { id:'bonusReferrals',  name:'Bonus Referrals',   group:'Finance',      color:'#fbbf24' },
    { id:'gac',             name:'GAC',               group:'Finance',      color:'#34d399' },
    { id:'overpayment',     name:'Overpayment',       group:'Finance',      color:'#fb7185' },
    { id:'advanceStanding', name:'Advance Standing',  group:'Academics',    color:'#22d3ee' },
    { id:'midpoints',       name:'Midpoints',         group:'OSAP',         color:'#c084fc' },
    { id:'firstRelease',    name:'First Release',     group:'OSAP',         color:'#4ade80' },
    { id:'yr2Releases',     name:'Yr 2 Releases',     group:'OSAP',         color:'#f472b6' },
  ];
  const FINANCE_INQUIRY_SCHEDULE = [
    { name:'Jhanvi', start:9,  end:10, label:'9–10 AM' },
    { name:'Devanshi', start:10, end:11, label:'10–11 AM' },
    { name:'Kanish', start:11, end:12, label:'11 AM–12 PM' },
    { name:'Viren', start:12, end:13, label:'12–1 PM' },
    { name:'Rushi', start:13, end:14, label:'1–2 PM' },
    { name:'Aastha', start:14, end:15, label:'2–3 PM' },
    { name:'Parveen', start:15, end:16, label:'3–4 PM' },
    { name:'Nancy', start:16, end:17, label:'4–5 PM' },
  ];

  const LUNCH_MESSAGES = {
    Rushi: ['Rushi is refueling. Please keep all technical mysteries warm until return.','Lunch mode active: Rushi is temporarily unavailable and emotionally committed to food.','Rushi stepped away for lunch. The dashboard is holding the fort.'],
    Nancy: ['Nancy is on lunch. Standards remain high, replies are temporarily paused.','Lunch mode active: Nancy has left the checklist unsupervised for one brave hour.','Nancy is refueling. Please keep chaos in draft mode.'],
    Parveen: ['Parveen is on lunch. Calm energy is charging in the background.','Lunch mode active: Parveen is away, but the spreadsheet pressure remains.','Parveen stepped out for food. Pending items should use this time wisely.'],
    Viren: ['Viren is on lunch. Finance questions are being asked to form a line.','Lunch mode active: Viren is temporarily unavailable and fully committed to recovery.','Viren stepped away. Please do not create a mystery until he returns.'],
    Aastha: ['Aastha is on lunch. The organized energy is temporarily recharging.','Lunch mode active: Aastha is away, so please keep the notes clean.','Aastha stepped out for lunch. The checklist has been asked to behave.'],
    Kanish: ['Kanish is on lunch. CEO-level digestion in progress.','Lunch mode active: Kanish has temporarily left the war room for strategic refueling.','Kanish is away for lunch. Please keep PDFs clean and drama low.'],
    Devanshi: ['Devanshi is on lunch. Calm productivity is taking a scheduled break.','Lunch mode active: Devanshi stepped away, but the files should still act civilized.','Devanshi is refueling. Please keep surprise errors away until return.'],
    Jhanvi: ['Jhanvi is on lunch. Morning power is officially recharging.','Lunch mode active: Jhanvi stepped away, but the first-hour discipline remains.','Jhanvi is refueling. The dashboard has been told to stay productive.']
  };

  function getLunchMessage(userName) {
    const list = LUNCH_MESSAGES[userName] || [userName + ' is on lunch. Professional refueling in progress.'];
    const key = 'fcdi_lunch_message_index_' + userName;
    const previous = Number(localStorage.getItem(key) || '-1');
    const next = (previous + 1) % list.length;
    localStorage.setItem(key, String(next));
    return list[next];
  }

  function formatLunchTime(ts) {
    if(!ts) return 'just now';
    try { return new Date(ts).toLocaleTimeString('en-US', { hour:'numeric', minute:'2-digit' }); }
    catch(e) { return 'just now'; }
  }


  const PERSONAL_WELCOMES = {
    Rushi: ['Rushi has entered the productivity arena.','Rushi is online. Someone hide the pending files.','Welcome back, Rushi. The dashboard was behaving until now.','Rushi logged in. Time to pretend this was the plan all along.'],
    Nancy: ['Nancy is here. The office suddenly has standards.','Welcome back, Nancy. The chaos has requested supervision.','Nancy logged in. Everyone act organized.','Nancy is online. Pending tasks are now nervous.'],
    Parveen: ['Parveen has joined. The files better start cooperating.','Welcome back, Parveen. Another day, another spreadsheet battle.','Parveen is online. Calm energy, dangerous productivity.','Parveen logged in. The dashboard feels safer already.'],
    Viren: ['Viren is here. The finance queue has been warned.','Welcome back, Viren. Time to turn confusion into completed tasks.','Viren logged in. Professional mode: activated.','Viren is online. The pending list just got uncomfortable.'],
    Aastha: ['Aastha has entered. The dashboard just got more responsible.','Welcome back, Aastha. Time to make the checklist behave.','Aastha is online. Everyone pretend the files are organized.','Aastha logged in. The war room now has adult supervision.'],
    Kanish: ['Kanish is back. The war room CEO has arrived.','Welcome back, Kanish. Time to professionally fight the pending list.','Kanish logged in. The dashboard is now under new management.','Kanish is online. Someone give this man a clean PDF and peace.'],
    Devanshi: ['Devanshi is here. The task list has officially lost its attitude.','Welcome back, Devanshi. Calm, collected, and ready to clear files.','Devanshi logged in. The dashboard just became more civilized.','Devanshi is online. Pending work should start apologizing.'],
    Jhanvi: ['Jhanvi has arrived. Morning shift energy unlocked.','Welcome back, Jhanvi. The 9 AM files are shaking.','Jhanvi is online. The dashboard got its early-bird warning.','Jhanvi logged in. Time to make the first hour count.']
  };

  function getRotatingWelcome(userName) {
    const list = PERSONAL_WELCOMES[userName] || [`Welcome back, ${userName}.`];
    const key = `fcdi_welcome_index_${userName}`;
    const previous = Number(localStorage.getItem(key) || '-1');
    const next = (previous + 1) % list.length;
    localStorage.setItem(key, String(next));
    return list[next];
  }


  const PERSONAL_MOODS = {
    Rushi: [
      'Tech support energy with a side of calm chaos.',
      'Quietly productive, loudly allergic to messy lists.',
      'Dashboard mood: fixing things nobody admitted were broken.',
      'Professional mode on. Random surprises under review.'
    ],
    Nancy: [
      'Organized, alert, and politely judging the pending list.',
      'Office standards department has entered the chat.',
      'Calm face, serious checklist energy.',
      'Professional kindness with audit-level attention.'
    ],
    Parveen: [
      'Spreadsheet patience with deadline pressure in the background.',
      'Soft voice, strong follow-up energy.',
      'Today’s plan: clear files and avoid unnecessary drama.',
      'Professional calm, but the pending list should not test it.'
    ],
    Viren: [
      'Finance mode: focused, practical, slightly suspicious of missing details.',
      'Ready to solve problems that should have been simple.',
      'Dashboard mood: controlled chaos with receipts.',
      'Polite on the outside, checking everything twice on the inside.'
    ],
    Aastha: [
      'Responsible energy with a strong dislike for unfinished notes.',
      'Organized enough to scare the checklist into behaving.',
      'Professional, focused, and not here for random errors.',
      'Today’s vibe: clean entries, clean folders, clean finish.'
    ],
    Kanish: [
      'Manager mindset, employee login, CEO-level expectations.',
      'Today’s vibe: clean PDFs, zero confusion, full control.',
      'Professional chaos controller with a suspicious eye on pending work.',
      'Dashboard mood: productivity, caffeine, and unnecessary confidence.'
    ],
    Devanshi: [
      'Calm productivity with a very low tolerance for messy files.',
      'Professional, steady, and ready to make the queue behave.',
      'Today’s vibe: smooth work, clear notes, no surprise errors.',
      'Soft energy, strong completion rate.'
    ],
    Jhanvi: [
      'Morning shift power with early-bird discipline.',
      'Fresh start energy, but the 9 AM files are already being watched.',
      'Today’s vibe: first hour, first impact, no excuses.',
      'Professional sunrise mode activated.'
    ]
  };

  function getRotatingMood(userName) {
    const list = PERSONAL_MOODS[userName] || ['Fresh login, fresh joke, same pending list.'];
    const key = `fcdi_mood_index_${userName}`;
    const previous = Number(localStorage.getItem(key) || '-1');
    const next = (previous + 1) % list.length;
    localStorage.setItem(key, String(next));
    return list[next];
  }

  const EMOJIS = ['😀','😃','😄','😁','😆','😅','😂','🤣','😊','😎','😍','🥰','😉','🙂','🤩','🥳','😤','🤔','🫡','🤝','👏','🙌','👍','💪','🔥','✨','⚡','💯','✅','📌','📎','📣','💬','🧠','🎯','🏆','🚀','⏳','📈','📊','🗂️','📝','💻','☕','🎉','🎊','🏁','😭','😴','🤯','😬','🙏','👀','💡','🔔','⭐','🌟'];
  const GIFS = [
    { label:'Nice',        url:'https://media.giphy.com/media/111ebonMs90YLu/giphy.gif' },
    { label:'Office hype', url:'https://media.giphy.com/media/xT9IgG50Fb7Mi0prBC/giphy.gif' },
    { label:'Done',        url:'https://media.giphy.com/media/l0MYt5jPR6QX5pnqM/giphy.gif' },
    { label:'Teamwork',    url:'https://media.giphy.com/media/3o7abldj0b3rxrZUxW/giphy.gif' },
    { label:'Focus',       url:'https://media.giphy.com/media/l0HlBO7eyXzSZkJri/giphy.gif' },
    { label:'Approved',    url:'https://media.giphy.com/media/26u4lOMA8JKSnL9Uk/giphy.gif' },
  ];

  const MEMBER_MAP  = Object.fromEntries(TEAM_MEMBERS.map(m=>[m.name,m]));
  const TASKS_BY_ID = Object.fromEntries(TASK_POOL.map(t=>[t.id,t]));
  const isFirebaseConfigFilled = () => !!window.HAS_FIREBASE_CONFIG || Object.values(FIREBASE_CONFIG).every(v => v && !String(v).includes('PASTE_'));
  const isFirebaseReady = ()=>!!db && isFirebaseConfigFilled();
  const isRealtimeReady = ()=>!!realtimeDb && isFirebaseConfigFilled();
  const getTime = ()=>new Date().toLocaleTimeString('en-US',{hour:'numeric',minute:'2-digit'});
  const clamp = (v,min,max)=>{const n=Number(v); return !isFinite(n)?min:Math.max(min,Math.min(max,Math.round(n)));};

  const readLocal = (key, fallback=[]) => { try { return JSON.parse(localStorage.getItem(key) || JSON.stringify(fallback)); } catch(e) { return fallback; } };
  const writeLocal = (key, value) => localStorage.setItem(key, JSON.stringify(value));
  const localId = (prefix) => `${prefix}_${Date.now()}_${Math.random().toString(16).slice(2)}`;
  const pingTargetFromText = (text='') => TEAM_MEMBERS.find(m => new RegExp(`(^|\\s)@${m.name}\\b`, 'i').test(text))?.name || null;

  const dateKeyFromDate = (inputDate = new Date()) => {
    const d = inputDate instanceof Date ? inputDate : new Date(inputDate);
    const y = d.getFullYear();
    const m = String(d.getMonth() + 1).padStart(2, '0');
    const day = String(d.getDate()).padStart(2, '0');
    return `${y}-${m}-${day}`;
  };

  const lastNDates = (count = 7) => {
    const out = [];
    const base = new Date();
    for (let i = count - 1; i >= 0; i--) {
      const d = new Date(base);
      d.setDate(base.getDate() - i);
      out.push(dateKeyFromDate(d));
    }
    return out;
  };

  const formatHistoryDate = (key) => {
    const [y, m, d] = String(key).split('-').map(Number);
    if(!y || !m || !d) return key;
    return new Date(y, m - 1, d).toLocaleDateString('en-US', { weekday:'short', month:'short', day:'numeric' });
  };

  const flattenDailyLog = (log = {}) => {
    const rows = [];
    Object.entries(log || {}).forEach(([member, tasks]) => {
      Object.entries(tasks || {}).forEach(([taskId, record]) => {
        const done = typeof record === 'number' ? record : Number(record?.done || 0);
        if(done > 0) rows.push({ member, taskId, done, updatedAt: record?.updatedAt || null });
      });
    });
    return rows;
  };

  const fbSet = async(col,id,data,merge=true)=>{
    if(!isFirebaseReady()) return;
    try{ if(id) await db.collection(col).doc(id).set(data,{merge}); else await db.collection(col).add(data); }
    catch(e){ console.warn(col,e); }
  };

  /* ─── Theme helper ──────────────────────────────────────── */
  function useTheme() {
    const [theme, setTheme] = useState(() => localStorage.getItem('fcdi_theme') || 'dark');
    useEffect(() => {
      document.documentElement.setAttribute('data-theme', theme);
      localStorage.setItem('fcdi_theme', theme);
    }, [theme]);
    const toggle = () => setTheme(t => t === 'dark' ? 'light' : 'dark');
    return { theme, toggle };
  }

  /* ─── PDF helpers ──────────────────────────────────────── */
  function fileToDataUrl(file) {
    return new Promise((resolve, reject) => {
      const r = new FileReader();
      r.onload  = () => resolve(r.result);
      r.onerror = () => reject(new Error('Read failed: ' + (file?.name || 'file')));
      r.readAsDataURL(file);
    });
  }

  async function urlToDataUrl(url) {
    if (typeof url === 'string' && url.startsWith('data:')) return url;
    const resp = await fetch(url);
    const blob = await resp.blob();
    return await fileToDataUrl(blob);
  }

  function decodeDataUrl(dataUrl) {
    const m = /^data:([^;]+);base64,(.*)$/.exec(dataUrl);
    if (!m) throw new Error('Bad data URL');
    const mime = m[1];
    const bin = atob(m[2]);
    const bytes = new Uint8Array(bin.length);
    for (let i = 0; i < bin.length; i++) bytes[i] = bin.charCodeAt(i);
    return { mime, bytes };
  }

  function loadImage(dataUrl) {
    return new Promise((resolve, reject) => {
      const img = new Image();
      img.onload  = () => resolve(img);
      img.onerror = () => reject(new Error('Image load failed'));
      img.src = dataUrl;
    });
  }

  async function imagesToPdfBlob(imageSources) {
    const { jsPDF } = window.jspdf;
    const doc = new jsPDF({ orientation: 'portrait', unit: 'pt', format: 'a4' });
    const PAGE_W = doc.internal.pageSize.getWidth();
    const PAGE_H = doc.internal.pageSize.getHeight();
    const MARGIN = 24;

    let first = true;
    for (const src of imageSources) {
      const dataUrl = await urlToDataUrl(src);
      const img = await loadImage(dataUrl);
      const iW = img.naturalWidth || 800;
      const iH = img.naturalHeight || 600;
      const fmt = /^data:image\/png/i.test(dataUrl) ? 'PNG' : 'JPEG';
      const availW = PAGE_W - MARGIN * 2;
      const availH = PAGE_H - MARGIN * 2;
      const scale = Math.min(availW / iW, availH / iH);
      const w = iW * scale;
      const h = iH * scale;
      const x = (PAGE_W - w) / 2;
      const y = (PAGE_H - h) / 2;

      if (!first) doc.addPage();
      first = false;
      doc.addImage(dataUrl, fmt, x, y, w, h, undefined, 'FAST');
    }

    return doc.output('blob');
  }

  async function mergePdfBlobs(pdfSources) {
    const { PDFDocument } = window.PDFLib;
    const out = await PDFDocument.create();
    for (const src of pdfSources) {
      let buf;
      if (src instanceof ArrayBuffer) buf = src;
      else if (src instanceof Uint8Array) buf = src.buffer;
      else if (src instanceof Blob) buf = await src.arrayBuffer();
      else buf = src;
      try {
        const sub = await PDFDocument.load(buf, { ignoreEncryption: true });
        const pages = await out.copyPages(sub, sub.getPageIndices());
        pages.forEach(p => out.addPage(p));
      } catch(e) { console.warn('Skipping invalid PDF:', e.message); }
    }
    const bytes = await out.save();
    return new Blob([bytes], { type: 'application/pdf' });
  }

  function sanitizeFilenamePart(s) {
    return String(s || '')
      .replace(/[\\/:*?"<>|]+/g, '')
      .replace(/\s+/g, ' ')
      .trim()
      .slice(0, 80);
  }

  function buildPdfFilename(studentNumber, studentName, purpose) {
    const num  = sanitizeFilenamePart(studentNumber);
    const name = sanitizeFilenamePart(studentName) || 'Student';
    const pur  = sanitizeFilenamePart(purpose)    || 'Document';
    return num
      ? `${num} - ${name} - ${pur}.pdf`
      : `${name} - ${pur}.pdf`;
  }

  // DIRECT BROWSER DOWNLOAD ONLY — no showSaveFilePicker
  function saveBlob(blob, filename) {
    const url = URL.createObjectURL(blob);
    const a = document.createElement('a');
    a.href = url;
    a.download = filename;
    document.body.appendChild(a);
    a.click();
    a.remove();
    setTimeout(() => URL.revokeObjectURL(url), 3000);
  }

  // Build a folder key from student data — uses number as primary key when available.
  function makeFolderKey(student) {
    if (student.number && student.number.trim()) return student.number.trim().replace(/\s+/g,'_');
    return (student.name || 'unknown').replace(/\s+/g,'_') + '_' + (student.id || '').slice(-6);
  }

  /* ═══════════════════════════════════════════════════════════
     THEME TOGGLE BUTTON
  ═══════════════════════════════════════════════════════════ */
  function ThemeToggle({ theme, onToggle }) {
    return (
      <button onClick={onToggle} className="theme-toggle" title={`Switch to ${theme==='dark'?'light':'dark'} mode`}>
        <span className="knob" />
      </button>
    );
  }

  /* ═══════════════════════════════════════════════════════════
     LOGIN
  ═══════════════════════════════════════════════════════════ */
  function LoginPage({ onLogin, theme, onToggleTheme }) {
    return (
      <div style={{minHeight:'100vh',background:'var(--bg)',display:'flex',flexDirection:'column'}}>
        <div className="topbar">
          <span className="wordmark">f-cdi</span>
          <div style={{display:'flex',alignItems:'center',gap:'12px'}}>
            <span style={{fontSize:'12px',color:'var(--muted)'}}>{theme==='dark'?'☾':'☀'}</span>
            <ThemeToggle theme={theme} onToggle={onToggleTheme}/>
            <span className="label">Sign in</span>
          </div>
        </div>
        <div style={{flex:1,display:'flex',flexDirection:'column',justifyContent:'center',padding:'48px 24px',maxWidth:'1100px',width:'100%',margin:'0 auto'}}>
          <h1 className="serif" style={{fontSize:'clamp(40px,6vw,72px)',fontWeight:600,lineHeight:1.05,marginBottom:'10px'}}>Welcome back.</h1>
          <p className="mono" style={{color:'var(--muted)',fontSize:'13px',marginBottom:'56px'}}>Choose your name to enter the war room.</p>

          <div className="label" style={{marginBottom:'18px'}}>Roster</div>
          <div style={{display:'grid',gridTemplateColumns:'repeat(auto-fill,minmax(150px,1fr))',gap:'12px'}}>
            {TEAM_MEMBERS.map(m => (
              <button key={m.name} onClick={()=>onLogin(m.name)}
                className="card"
                style={{padding:'18px 16px',display:'flex',alignItems:'center',gap:'12px',cursor:'pointer',textAlign:'left'}}>
                <div style={{position:'relative',flexShrink:0}}>
                  <img src={m.avatar} alt={m.name} style={{width:'36px',height:'36px',borderRadius:'10px',objectFit:'cover',background:m.accent+'22'}} onError={e=>{e.target.style.display='none';}}/>
                  <span style={{position:'absolute',bottom:'-2px',right:'-2px',width:'10px',height:'10px',borderRadius:'50%',background:'#4ade80',border:'2px solid var(--bg-2)'}} className="dot-pulse"></span>
                </div>
                <div style={{minWidth:0}}>
                  <div style={{fontWeight:500,fontSize:'14px'}}>{m.name}</div>
                  <div className="mono" style={{fontSize:'10px',color:'var(--faint)',textTransform:'uppercase',letterSpacing:'.1em'}}>Online</div>
                </div>
              </button>
            ))}
          </div>
        </div>
      </div>
    );
  }

  /* ─── Avatar ─────────────────────────────────────────────── */
  function Avatar({name, size=32}) {
    const m = MEMBER_MAP[name] || {};
    return (
      <div style={{width:size,height:size,minWidth:size,borderRadius:'8px',background:m.accent||'#fb923c',overflow:'hidden',flexShrink:0,display:'flex',alignItems:'center',justifyContent:'center',color:'#fff',fontWeight:700,fontSize:`${size*0.4}px`}}>
        {m.avatar
          ? <img src={m.avatar} alt={name} style={{width:'100%',height:'100%',objectFit:'cover'}} onError={e=>{e.target.style.display='none';}}/>
          : (name?.[0]||'?')
        }
      </div>
    );
  }


  /* ═══════════════════════════════════════════════════════════
     CHAT PANEL
  ═══════════════════════════════════════════════════════════ */
  function renderMessageText(text='') {
    const parts = String(text).split(/(@[A-Za-z]+)/g);
    return parts.map((part, idx) => {
      const name = part.startsWith('@') ? part.slice(1) : '';
      return MEMBER_MAP[name]
        ? <span key={idx} className="ping">{part}</span>
        : <React.Fragment key={idx}>{part}</React.Fragment>;
    });
  }

  function ChatPanel({ currentUser, open, onToggle, unread, onClearUnread, notifyUser }) {
    const [messages, setMessages] = useState([]);
    const [input, setInput] = useState('');
    const [picker, setPicker] = useState(null);
    const [loading, setLoading] = useState(true);
    const endRef = useRef(null);
    const seenPingIds = useRef(new Set());
    const accent = MEMBER_MAP[currentUser]?.accent || '#fb923c';

    const loadLocalMessages = () => {
      const local = readLocal('fcdi_chat_messages', []);
      if(local.length === 0) {
        const demo = [{id:'demo_notice',author:'System',text:'Firebase is not configured — local demo mode is active. Chat will work in this browser for testing.',time:'now',timestamp:Date.now()}];
        writeLocal('fcdi_chat_messages', demo);
        return demo;
      }
      return local;
    };

    useEffect(() => {
      setLoading(true);
      if(isRealtimeReady()){
        const ref = realtimeDb.ref('chat');
        const query = ref.orderByChild('timestamp').limitToLast(200);
        const handler = snap => {
          const val = snap.val() || {};
          const arr = Object.entries(val).map(([id,data]) => ({id, ...data})).sort((a,b)=>(a.timestamp||0)-(b.timestamp||0));
          setMessages(arr);
          setLoading(false);
        };
        const errHandler = err => {
          console.warn('Realtime chat failed. Falling back to local demo mode.', err);
          setMessages(loadLocalMessages());
          setLoading(false);
        };
        query.on('value', handler, errHandler);
        return () => query.off('value', handler);
      }
      if(isFirebaseReady()){
        const unsub = db.collection('chat').orderBy('timestamp','asc').limitToLast(200).onSnapshot(snap => {
          setMessages(snap.docs.map(d=>({id:d.id,...d.data()})));
          setLoading(false);
        }, err => {
          console.warn('Firestore chat failed. Falling back to local demo mode.', err);
          setMessages(loadLocalMessages());
          setLoading(false);
        });
        return () => unsub();
      }
      setMessages(loadLocalMessages());
      setLoading(false);
      const timer = setInterval(()=>setMessages(loadLocalMessages()), 1200);
      return () => clearInterval(timer);
    }, []);

    useEffect(()=>{
      messages.forEach(msg => {
        if(msg.pingTarget === currentUser && msg.author !== currentUser && !seenPingIds.current.has(msg.id)){
          seenPingIds.current.add(msg.id);
          notifyUser?.(`${msg.author} mentioned you in chat`, msg.text || 'Open team chat', msg.author);
        }
      });
    }, [messages, currentUser]);

    useEffect(()=>{ 
      if(open) onClearUnread();
      setTimeout(()=>endRef.current?.scrollIntoView({behavior:'smooth'}),50);
    }, [open, messages]);

    const send = useCallback(async (payload={}) => {
      if(!currentUser) return;
      const text = payload.text ?? input.trim();
      if(!text && !payload.gif) return;
      const pingTarget = pingTargetFromText(text || '');
      const msg = { 
        id: localId('chat'),
        author:currentUser,
        text:text||'',
        gif:payload.gif||null,
        time:getTime(),
        timestamp:Date.now(),
        pingTarget,
        accent
      };
      setMessages(p => [...p, msg]);
      if(isRealtimeReady()) {
        try { await realtimeDb.ref('chat').push(msg); }
        catch(e) {
          console.warn('Realtime chat write failed. Saving locally.', e);
          const next = [...loadLocalMessages().filter(m => m.id !== 'demo_notice'), msg];
          writeLocal('fcdi_chat_messages', next);
        }
      } else if(isFirebaseReady()) {
        await fbSet('chat', null, {...msg, ts:firebase.firestore.FieldValue.serverTimestamp()});
      } else {
        const next = [...loadLocalMessages().filter(m => m.id !== 'demo_notice'), msg];
        writeLocal('fcdi_chat_messages', next);
      }
      setInput(''); setPicker(null);
    }, [currentUser, input, accent]);

    return (
      <>
        {!open && (
          <button onClick={onToggle} className={`chat-fab ${unread>0?'pulse-orange':''}`} title="Open chat">
            <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="var(--orange)" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"/></svg>
            {unread > 0 && <span className="chat-fab-badge">{unread > 99 ? '99+' : unread}</span>}
          </button>
        )}
        <aside className={`chat-panel ${open?'':'closed'}`}>
          <div style={{display:'flex',alignItems:'center',justifyContent:'space-between',padding:'14px 18px',borderBottom:'1px solid var(--line)'}}>
            <div style={{display:'flex',alignItems:'center',gap:'10px'}}>
              <span className="wordmark" style={{fontSize:'15px'}}>Team Chat</span>
              <span style={{width:'7px',height:'7px',borderRadius:'50%',background:isFirebaseReady()?'#4ade80':'var(--orange)'}} className="dot-pulse"></span>
            </div>
            <button onClick={onToggle} className="btn-ghost" style={{padding:'4px 8px',fontSize:'14px'}}>✕</button>
          </div>
          {!isRealtimeReady() && !isFirebaseReady() && (
            <div style={{margin:'10px 14px 0',padding:'8px 10px',border:'1px solid rgba(251,146,60,.35)',background:'rgba(251,146,60,.08)',borderRadius:'10px',fontSize:'11px',color:'var(--orange)'}}>
              Local demo mode: Firebase is not connected. Chat will still work in this browser.
            </div>
          )}
          <div className="scroll" style={{flex:1,overflowY:'auto',padding:'14px',display:'flex',flexDirection:'column',gap:'10px'}}>
            {loading && <div className="mono" style={{fontSize:'11px',textAlign:'center',padding:'20px',color:'var(--muted)'}}>Loading…</div>}
            {messages.map(msg => {
              const isOwn = msg.author === currentUser;
              const isSystem = msg.author === 'System';
              const m = MEMBER_MAP[msg.author];
              return (
                <div key={msg.id} className="fade-in" style={{display:'flex',gap:'8px',flexDirection:isOwn?'row-reverse':'row',justifyContent:isSystem?'center':'flex-start'}}>
                  {!isOwn && !isSystem && <Avatar name={msg.author} size={28}/>}
                  <div style={{maxWidth:isSystem?'94%':'76%',display:'flex',flexDirection:'column',alignItems:isOwn?'flex-end':'flex-start',gap:'2px'}}>
                    {!isOwn && !isSystem && <span className="mono" style={{fontSize:'10px',color:m?.accent||'var(--muted)',fontWeight:600}}>{msg.author}</span>}
                    <div style={{padding:'8px 12px',borderRadius:'12px',fontSize:'13px',lineHeight:1.4,wordBreak:'break-word',background:isSystem?'rgba(251,146,60,.08)':(isOwn?accent+'22':'var(--bg-3)'),border:`1px solid ${isSystem?'rgba(251,146,60,.25)':(isOwn?accent+'44':'var(--line)')}`}}>
                      {msg.gif ? <img src={msg.gif} alt="gif" style={{maxWidth:'200px',borderRadius:'8px',display:'block'}}/> : renderMessageText(msg.text)}
                    </div>
                    {!isSystem && <span className="mono" style={{fontSize:'9px',color:'var(--faint)'}}>{msg.time}</span>}
                  </div>
                </div>
              );
            })}
            <div ref={endRef}/>
          </div>
          {picker && (
            <div style={{padding:'0 14px 8px'}}>
              {picker === 'emoji' && (
                <div className="card-flat scroll" style={{padding:'8px',maxHeight:'140px',overflowY:'auto',display:'flex',flexWrap:'wrap',gap:'4px'}}>
                  {EMOJIS.map(e => <button key={e} onClick={()=>send({text:e})} style={{fontSize:'20px',background:'none',border:'none',cursor:'pointer',padding:'2px',transition:'transform 100ms'}} onMouseOver={e=>e.currentTarget.style.transform='scale(1.3)'} onMouseOut={e=>e.currentTarget.style.transform='none'}>{e}</button>)}
                </div>
              )}
              {picker === 'gif' && (
                <div className="card-flat scroll" style={{padding:'6px',maxHeight:'180px',overflowY:'auto',display:'grid',gridTemplateColumns:'repeat(3,1fr)',gap:'4px'}}>
                  {GIFS.map(g => <button key={g.label} onClick={()=>send({gif:g.url})} style={{padding:0,border:'none',background:'none',borderRadius:'6px',overflow:'hidden',cursor:'pointer'}}><img src={g.url} alt={g.label} style={{width:'100%',height:'70px',objectFit:'cover'}}/></button>)}
                </div>
              )}
            </div>
          )}
          <div style={{padding:'10px 14px 14px'}}>
            <div style={{display:'flex',alignItems:'center',gap:'6px',background:'var(--input-bg)',border:'1px solid var(--line)',borderRadius:'24px',padding:'4px 6px'}}>
              <button type="button" onClick={()=>setPicker(picker==='emoji'?null:'emoji')} style={{width:'28px',height:'28px',background:'none',border:'none',cursor:'pointer',fontSize:'15px'}}>😊</button>
              <button type="button" onClick={()=>setPicker(picker==='gif'?null:'gif')} className="mono" style={{padding:'2px 8px',background:'none',border:'none',cursor:'pointer',fontSize:'10px',color:'var(--muted)',fontWeight:700}}>GIF</button>
              <input value={input} onChange={e=>setInput(e.target.value)} onKeyDown={e=>{if(e.key==='Enter'&&!e.shiftKey){e.preventDefault();send();}}}
                placeholder="Message team… use @Name to ping" style={{flex:1,minWidth:0,background:'transparent',border:'none',outline:'none',fontSize:'13px',color:'var(--text)',padding:'4px',fontFamily:'inherit'}}/>
              <button type="button" onClick={()=>send()} style={{width:'28px',height:'28px',borderRadius:'50%',background:'var(--orange-2)',border:'none',color:'#fff',cursor:'pointer',fontSize:'12px',display:'flex',alignItems:'center',justifyContent:'center'}}>➤</button>
            </div>
          </div>
        </aside>
      </>
    );
  }


  /* ═══════════════════════════════════════════════════════════
     ASSIGN MODAL
  ═══════════════════════════════════════════════════════════ */
  function AssignModal({ task, memberName, onConfirm, onCancel }) {
    const [goal, setGoal] = useState('');
    const m = MEMBER_MAP[memberName];
    const submit = () => { if(Number(goal) > 0) onConfirm(Number(goal)); };

    return (
      <div className="modal-bg" onClick={onCancel}>
        <div className="modal" onClick={e=>e.stopPropagation()}>
          <div className="label" style={{marginBottom:'10px'}}>Assign Task</div>
          <h3 className="serif" style={{fontSize:'24px',fontWeight:600,marginBottom:'6px'}}>How many?</h3>
          <p style={{fontSize:'13px',color:'var(--muted)',marginBottom:'20px'}}>
            Assigning <span style={{color:task.color,fontWeight:600}}>{task.name}</span> to <span style={{color:m?.accent,fontWeight:600}}>{memberName}</span>
          </p>
          <input type="number" min="1" value={goal} onChange={e=>setGoal(e.target.value)}
            onKeyDown={e=>{if(e.key==='Enter') submit();}} autoFocus
            placeholder="Enter goal number"
            className="input" style={{width:'100%',fontSize:'18px',padding:'12px 16px',borderColor:task.color,marginBottom:'16px'}}/>
          <div style={{display:'flex',gap:'8px',justifyContent:'flex-end'}}>
            <button onClick={onCancel} className="btn">Cancel</button>
            <button onClick={submit} className="btn btn-orange">Assign</button>
          </div>
        </div>
      </div>
    );
  }

  /* ═══════════════════════════════════════════════════════════
     DONE INPUT
  ═══════════════════════════════════════════════════════════ */
  function DoneInput({ committedValue, max, color, locked, onCommit }) {
    const [draft, setDraft] = useState(String(committedValue || 0));
    const [focused, setFocused] = useState(false);
    useEffect(() => { if(!focused) setDraft(String(committedValue || 0)); }, [committedValue, focused]);
    const commit = () => {
      const next = clamp(draft, 0, max);
      setDraft(String(next));
      if(next !== Number(committedValue || 0)) onCommit(next);
    };

    return (
      <input type="number" min="0" max={max} value={draft} disabled={locked}
        onFocus={()=>setFocused(true)} onChange={e=>setDraft(e.target.value)}
        onBlur={()=>{ setFocused(false); commit(); }}
        onKeyDown={e=>{
          if(e.key === 'Enter'){ e.preventDefault(); commit(); e.target.blur(); }
          if(e.key === 'Escape'){ setDraft(String(committedValue||0)); e.target.blur(); }
        }}
        className="input mono"
        style={{width:'100%',fontWeight:700,fontSize:'14px',borderColor: locked ? 'var(--line)' : color,opacity: locked ? .55 : 1}}
      />
    );
  }


  /* ═══════════════════════════════════════════════════════════
     NOTIFICATIONS + CHESS
  ═══════════════════════════════════════════════════════════ */
  function NotificationButton({ notifyUser }) {
    const [permission, setPermission] = useState(() => localStorage.getItem('fcdi_notify_permission') || (window.Notification?.permission || 'unsupported'));
    const request = async () => {
      if(!('Notification' in window)){
        setPermission('unsupported');
        notifyUser?.('Notifications unavailable', 'This browser does not support browser notifications.');
        return;
      }
      const result = await Notification.requestPermission();
      localStorage.setItem('fcdi_notify_permission', result);
      setPermission(result);
      notifyUser?.(result === 'granted' ? 'Notifications enabled' : 'Notifications not enabled', result === 'granted' ? 'You can now receive chat and chess alerts.' : 'Browser notifications are blocked, but in-app alerts still work.');
    };
    return <button onClick={request} className="btn" style={{fontSize:'12px',padding:'7px 10px'}}>{permission === 'granted' ? 'Notifications On' : 'Enable Notifications'}</button>;
  }

  function ToastHost({ toasts, onClose }) {
    return (
      <div className="toast-stack">
        {toasts.map(t => (
          <div key={t.id} className="toast">
            <div style={{display:'flex',justifyContent:'space-between',gap:'10px'}}>
              <div style={{fontWeight:700,fontSize:'13px'}}>{t.title}</div>
              <button onClick={()=>onClose(t.id)} className="btn-ghost" style={{padding:'0 4px',fontSize:'12px'}}>×</button>
            </div>
            {t.body && <div style={{fontSize:'12px',color:'var(--muted)',marginTop:'4px'}}>{t.body}</div>}
          </div>
        ))}
      </div>
    );
  }

  const PIECES = {
    wp:'♙', wn:'♘', wb:'♗', wr:'♖', wq:'♕', wk:'♔',
    bp:'♟', bn:'♞', bb:'♝', br:'♜', bq:'♛', bk:'♚'
  };

  function ChessPanel({ currentUser, open, onClose, notifyUser }) {
    const [invites, setInvites] = useState([]);
    const [games, setGames] = useState([]);
    const [selected, setSelected] = useState(null);
    const [legalTargets, setLegalTargets] = useState([]);
    const seenEvents = useRef(new Set());
    const panelOpenRef = useRef(open);
    useEffect(()=>{ panelOpenRef.current = open; }, [open]);

    const myGame = games.find(g => g.status === 'active' && (g.whitePlayer === currentUser || g.blackPlayer === currentUser)) || games.find(g => g.status === 'active') || null;
    const pendingForMe = invites.filter(i => i.toUser === currentUser && i.status === 'pending');
    const myPendingSent = invites.filter(i => i.fromUser === currentUser && i.status === 'pending');

    const loadLocal = () => {
      setInvites(readLocal('fcdi_chess_invites', []));
      setGames(readLocal('fcdi_chess_games', []));
    };

    useEffect(() => {
      if(isRealtimeReady()){
        const invitesQuery = realtimeDb.ref('chessInvites').orderByChild('createdAt').limitToLast(50);
        const gamesQuery = realtimeDb.ref('chessGames').orderByChild('updatedAt').limitToLast(20);
        const invitesHandler = snap => {
          const val = snap.val() || {};
          setInvites(Object.entries(val).map(([id,data]) => ({id, ...data})).sort((a,b)=>(b.createdAt||0)-(a.createdAt||0)));
        };
        const gamesHandler = snap => {
          const val = snap.val() || {};
          setGames(Object.entries(val).map(([id,data]) => ({id, ...data})).sort((a,b)=>(b.updatedAt||0)-(a.updatedAt||0)));
        };
        const errHandler = err => { console.warn('Realtime chess failed. Falling back to local demo mode.', err); loadLocal(); };
        invitesQuery.on('value', invitesHandler, errHandler);
        gamesQuery.on('value', gamesHandler, errHandler);
        return () => { invitesQuery.off('value', invitesHandler); gamesQuery.off('value', gamesHandler); };
      }
      if(isFirebaseReady()){
        const u1 = db.collection('chessInvites').orderBy('createdAt','desc').limit(50).onSnapshot(snap => setInvites(snap.docs.map(d=>({id:d.id,...d.data()}))), err => { console.warn('Firestore chess invites failed.', err); loadLocal(); });
        const u2 = db.collection('chessGames').orderBy('updatedAt','desc').limit(20).onSnapshot(snap => setGames(snap.docs.map(d=>({id:d.id,...d.data()}))), err => { console.warn('Firestore chess games failed.', err); loadLocal(); });
        return () => { u1(); u2(); };
      }
      loadLocal();
      const timer = setInterval(loadLocal, 1000);
      return () => clearInterval(timer);
    }, []);

    useEffect(() => {
      invites.forEach(inv => {
        if(inv.status === 'pending' && inv.toUser === currentUser && !seenEvents.current.has(`invite_${inv.id}`)){
          seenEvents.current.add(`invite_${inv.id}`);
          notifyUser?.(`${inv.fromUser} invited you to play chess`, 'Open the chess panel to accept or decline.', inv.fromUser);
        }
        if(inv.status === 'accepted' && inv.fromUser === currentUser && !seenEvents.current.has(`accepted_${inv.id}`)){
          seenEvents.current.add(`accepted_${inv.id}`);
          notifyUser?.(`${inv.toUser} accepted your chess invite`, 'Chess game started.', inv.toUser);
        }
      });
    }, [invites, currentUser]);

    useEffect(() => {
      games.forEach(g => {
        if(g.status !== 'active') return;
        const whoseTurn = g.turn === 'w' ? g.whitePlayer : g.blackPlayer;
        const lastMover = g.turn === 'w' ? g.blackPlayer : g.whitePlayer;
        const key = `turn_${g.id}_${g.fen}`;
        if(whoseTurn === currentUser && lastMover !== currentUser && !seenEvents.current.has(key)){
          seenEvents.current.add(key);
          if(!panelOpenRef.current || document.hidden) notifyUser?.("It's your move in Chess", `${g.whitePlayer} vs ${g.blackPlayer}`, lastMover);
        }
      });
    }, [games, currentUser]);

    const saveInvite = async (invite) => {
      if(isRealtimeReady()) {
        try { await realtimeDb.ref('chessInvites/' + invite.id).set(invite); }
        catch(e) { console.warn('Realtime invite save failed. Saving locally.', e); const list = readLocal('fcdi_chess_invites', []); writeLocal('fcdi_chess_invites', [invite, ...list.filter(i => i.id !== invite.id)]); loadLocal(); }
      } else if(isFirebaseReady()) await fbSet('chessInvites', invite.id, invite, false);
      else {
        const list = readLocal('fcdi_chess_invites', []);
        writeLocal('fcdi_chess_invites', [invite, ...list.filter(i => i.id !== invite.id)]);
        loadLocal();
      }
    };
    const saveGame = async (game) => {
      if(isRealtimeReady()) {
        try { await realtimeDb.ref('chessGames/' + game.id).set(game); }
        catch(e) { console.warn('Realtime game save failed. Saving locally.', e); const list = readLocal('fcdi_chess_games', []); writeLocal('fcdi_chess_games', [game, ...list.filter(g => g.id !== game.id)]); loadLocal(); }
      } else if(isFirebaseReady()) await fbSet('chessGames', game.id, game, false);
      else {
        const list = readLocal('fcdi_chess_games', []);
        writeLocal('fcdi_chess_games', [game, ...list.filter(g => g.id !== game.id)]);
        loadLocal();
      }
    };

    const invitePlayer = async (name) => {
      if(name === currentUser) return;
      const invite = { id:localId('invite'), fromUser:currentUser, toUser:name, status:'pending', createdAt:Date.now() };
      await saveInvite(invite);
      notifyUser?.(`Invite sent to ${name}`, 'They will see it inside the app.', currentUser);
    };

    const declineInvite = async (inv) => saveInvite({...inv, status:'declined', updatedAt:Date.now()});

    const acceptInvite = async (inv) => {
      const chess = new Chess();
      const game = {
        id:localId('game'),
        whitePlayer:inv.fromUser,
        blackPlayer:inv.toUser,
        fen:chess.fen(),
        pgn:chess.pgn(),
        turn:'w',
        status:'active',
        winner:null,
        lastMove:null,
        updatedAt:Date.now()
      };
      await saveInvite({...inv, status:'accepted', updatedAt:Date.now(), gameId:game.id});
      await saveGame(game);
    };

    const playerColor = (game) => game?.whitePlayer === currentUser ? 'w' : (game?.blackPlayer === currentUser ? 'b' : null);
    const chessFromGame = (game) => {
      try { return new Chess(game?.fen); } catch(e) { return new Chess(); }
    };
    const gameStatusText = (game) => {
      if(!game) return 'No active game';
      const chess = chessFromGame(game);
      if(game.status === 'resigned') return `${game.winner} won by resignation`;
      if(chess.in_checkmate()) return `Checkmate — ${game.winner || (game.turn === 'w' ? game.blackPlayer : game.whitePlayer)} wins`;
      if(chess.in_stalemate()) return 'Stalemate';
      if(chess.in_draw()) return 'Draw';
      if(chess.in_check()) return 'Check';
      return `${game.turn === 'w' ? game.whitePlayer : game.blackPlayer}'s turn`;
    };

    const chooseSquare = async (square) => {
      if(!myGame || myGame.status !== 'active') return;
      const myColor = playerColor(myGame);
      if(!myColor || myGame.turn !== myColor) return;
      const chess = chessFromGame(myGame);
      const piece = chess.get(square);
      if(!selected){
        if(piece && piece.color === myColor){
          setSelected(square);
          setLegalTargets(chess.moves({square, verbose:true}).map(m => m.to));
        }
        return;
      }
      if(selected === square){ setSelected(null); setLegalTargets([]); return; }
      const move = chess.move({from:selected, to:square, promotion:'q'});
      if(!move){
        if(piece && piece.color === myColor){
          setSelected(square);
          setLegalTargets(chess.moves({square, verbose:true}).map(m => m.to));
        }
        return;
      }
      let status = 'active', winner = null;
      if(chess.in_checkmate()){ status = 'checkmate'; winner = myColor === 'w' ? myGame.whitePlayer : myGame.blackPlayer; }
      else if(chess.in_stalemate()) status = 'stalemate';
      else if(chess.in_draw()) status = 'draw';
      await saveGame({...myGame, fen:chess.fen(), pgn:chess.pgn(), turn:chess.turn(), status, winner, lastMove:{from:move.from,to:move.to,san:move.san,by:currentUser}, updatedAt:Date.now()});
      setSelected(null); setLegalTargets([]);
    };

    const resign = async () => {
      if(!myGame || !playerColor(myGame)) return;
      const winner = myGame.whitePlayer === currentUser ? myGame.blackPlayer : myGame.whitePlayer;
      await saveGame({...myGame, status:'resigned', winner, updatedAt:Date.now()});
    };
    const newGame = async () => {
      if(!myGame) return;
      const chess = new Chess();
      await saveGame({...myGame, fen:chess.fen(), pgn:chess.pgn(), turn:'w', status:'active', winner:null, lastMove:null, updatedAt:Date.now()});
    };

    if(!open) return null;

    const chess = myGame ? chessFromGame(myGame) : null;
    const board = chess ? chess.board() : [];
    const files = ['a','b','c','d','e','f','g','h'];
    const canMove = myGame && myGame.status === 'active' && playerColor(myGame) === myGame.turn;

    return (
      <div className="modal-bg">
        <div className="chess-modal">
          <div style={{display:'flex',justifyContent:'space-between',alignItems:'center',gap:'12px',marginBottom:'16px'}}>
            <div>
              <div className="label">Chess Break</div>
              <h2 className="serif" style={{fontSize:'28px',fontWeight:700,marginTop:'4px'}}>Click this if you’re bored</h2>
            </div>
            <button onClick={onClose} className="btn">Close</button>
          </div>

          {!isRealtimeReady() && !isFirebaseReady() && <div style={{padding:'10px 12px',border:'1px solid rgba(251,146,60,.3)',background:'rgba(251,146,60,.08)',borderRadius:'12px',fontSize:'12px',color:'var(--orange)',marginBottom:'14px'}}>Chess is running in local demo mode. Firebase config is required for real team multiplayer syncing.</div>}

          <div className="chess-layout">
            <div className="chess-board-shell">
              {myGame ? (
                <>
                  <div className="chess-player-card">
                    <div style={{display:'flex',alignItems:'center',gap:'10px'}}><Avatar name={myGame.blackPlayer} size={30}/><div><strong>Black · {myGame.blackPlayer}</strong><div className="mono" style={{fontSize:'10px',color:'var(--muted)'}}>{myGame.turn === 'b' ? 'To move' : 'Waiting'}</div></div></div>
                    <span className="pill" style={{background:chess?.in_check() && myGame.turn === 'b' ? 'rgba(248,113,113,.16)' : 'var(--bg-3)', color:chess?.in_check() && myGame.turn === 'b' ? 'var(--red)' : 'var(--muted)'}}>{chess?.in_check() && myGame.turn === 'b' ? 'Check' : 'Black'}</span>
                  </div>
                  <div className="chess-board">
                    {board.map((row, r) => row.map((piece, f) => {
                      const square = files[f] + (8 - r);
                      const dark = (r + f) % 2 === 1;
                      const isLast = myGame.lastMove && (myGame.lastMove.from === square || myGame.lastMove.to === square);
                      return (
                        <button key={square} disabled={!canMove && !(selected && legalTargets.includes(square))} onClick={()=>chooseSquare(square)}
                          className={`chess-square ${dark?'dark':''} ${selected===square?'selected':''} ${legalTargets.includes(square)?'legal':''} ${isLast?'last':''}`}
                          title={square}>
                          {piece ? PIECES[piece.color + piece.type] : ''}
                        </button>
                      );
                    }))}
                  </div>
                  <div className="chess-player-card">
                    <div style={{display:'flex',alignItems:'center',gap:'10px'}}><Avatar name={myGame.whitePlayer} size={30}/><div><strong>White · {myGame.whitePlayer}</strong><div className="mono" style={{fontSize:'10px',color:canMove?'var(--green)':'var(--muted)'}}>{canMove ? 'Your move' : (playerColor(myGame) ? 'Waiting' : 'Viewing only')}</div></div></div>
                    <span className="pill" style={{background:chess?.in_check() && myGame.turn === 'w' ? 'rgba(248,113,113,.16)' : 'var(--bg-3)', color:chess?.in_check() && myGame.turn === 'w' ? 'var(--red)' : 'var(--muted)'}}>{chess?.in_check() && myGame.turn === 'w' ? 'Check' : 'White'}</span>
                  </div>
                </>
              ) : (
                <div className="card" style={{padding:'24px',width:'min(72vw,492px)',minHeight:'300px',display:'flex',alignItems:'center',justifyContent:'center',textAlign:'center',borderRadius:'20px'}}>
                  <div>
                    <div className="serif" style={{fontSize:'24px',fontWeight:700}}>No active game</div>
                    <p style={{color:'var(--muted)',fontSize:'13px',marginTop:'6px'}}>Invite a teammate to start a clean, legal chess game.</p>
                  </div>
                </div>
              )}
            </div>

            <div className="chess-side">
              <div className="card" style={{padding:'14px'}}>
                <div className="label" style={{marginBottom:'10px'}}>Invite Player</div>
                <div style={{display:'grid',gridTemplateColumns:'repeat(2,1fr)',gap:'8px'}}>
                  {TEAM_MEMBERS.filter(m => m.name !== currentUser).map(m => (
                    <button key={m.name} onClick={()=>invitePlayer(m.name)} className="btn" style={{justifyContent:'flex-start'}}>
                      <Avatar name={m.name} size={24}/> {m.name}
                    </button>
                  ))}
                </div>
              </div>

              <div className="card" style={{padding:'14px'}}>
                <div className="label" style={{marginBottom:'10px'}}>Pending Invites</div>
                {pendingForMe.length === 0 && myPendingSent.length === 0 && <div style={{fontSize:'12px',color:'var(--muted)'}}>No pending invites.</div>}
                {pendingForMe.map(inv => (
                  <div key={inv.id} style={{padding:'10px',border:'1px solid var(--line)',borderRadius:'10px',marginBottom:'8px'}}>
                    <div style={{fontSize:'13px',marginBottom:'8px'}}><strong>{inv.fromUser}</strong> invited you.</div>
                    <div style={{display:'flex',gap:'8px'}}><button onClick={()=>acceptInvite(inv)} className="btn btn-orange">Accept</button><button onClick={()=>declineInvite(inv)} className="btn">Decline</button></div>
                  </div>
                ))}
                {myPendingSent.map(inv => <div key={inv.id} style={{fontSize:'12px',color:'var(--muted)',padding:'8px 0'}}>Waiting for {inv.toUser}…</div>)}
              </div>

              {myGame && (
                <div className="card" style={{padding:'14px'}}>
                  <div className="label" style={{marginBottom:'10px'}}>Game Controls</div>
                  <div style={{fontSize:'13px',fontWeight:700,marginBottom:'10px',padding:'10px 12px',border:'1px solid var(--line)',borderRadius:'12px',background:'var(--bg)'}}>{gameStatusText(myGame)}</div>
                  <div style={{display:'flex',gap:'8px',flexWrap:'wrap',marginBottom:'10px'}}>
                    <button onClick={resign} className="btn btn-danger" disabled={!playerColor(myGame) || myGame.status !== 'active'}>Resign</button>
                    <button onClick={newGame} className="btn" disabled={myGame.status === 'active'}>New Game</button>
                  </div>
                  <div className="move-list scroll">
                    {myGame.pgn ? myGame.pgn : 'Move history will appear here.'}
                  </div>
                </div>
              )}
            </div>
          </div>
        </div>
      </div>
    );
  }


  /* ═══════════════════════════════════════════════════════════
     FINANCIAL INQUIRY SCHEDULE
  ═══════════════════════════════════════════════════════════ */
  function FinancialInquiryPanel({ currentUser, notifyUser }) {
    const [now, setNow] = useState(() => new Date());
    const notifiedKeyRef = useRef('');

    useEffect(() => {
      const tick = () => setNow(new Date());
      tick();
      const timer = setInterval(tick, 15000);
      return () => clearInterval(timer);
    }, []);

    const minutesNow = now.getHours() * 60 + now.getMinutes() + now.getSeconds() / 60;
    const todayKey = now.toISOString().slice(0,10);
    const activeSlot = FINANCE_INQUIRY_SCHEDULE.find(s => minutesNow >= s.start * 60 && minutesNow < s.end * 60) || null;
    const nextSlot = FINANCE_INQUIRY_SCHEDULE.find(s => minutesNow < s.start * 60) || FINANCE_INQUIRY_SCHEDULE[0];
    const activeProgress = activeSlot ? Math.min(100, Math.max(0, ((minutesNow - activeSlot.start * 60) / 60) * 100)) : 0;
    const remainingMinutes = activeSlot ? Math.max(0, Math.ceil(activeSlot.end * 60 - minutesNow)) : null;

    useEffect(() => {
      if(!activeSlot || activeSlot.name !== currentUser) return;
      const key = 'finance_inquiry_' + todayKey + '_' + currentUser + '_' + activeSlot.start;
      if(localStorage.getItem(key) === 'sent' || notifiedKeyRef.current === key) return;
      const startWindow = minutesNow - activeSlot.start * 60;
      if(startWindow >= 0 && startWindow < 2.5){
        notifiedKeyRef.current = key;
        localStorage.setItem(key, 'sent');
        notifyUser?.('Financial inquiry time started', currentUser + ', your finance inquiry slot is now active: ' + activeSlot.label + '.', 'system');
      }
    }, [activeSlot?.name, activeSlot?.start, currentUser, todayKey, Math.floor(minutesNow)]);

    return (
      <div className="card inquiry-card" style={{padding:'18px',marginBottom:'48px'}}>
        <div style={{display:'flex',alignItems:'baseline',justifyContent:'space-between',gap:'12px',marginBottom:'14px',position:'relative'}}>
          <div>
            <div className="label">Financial Inquiry Time</div>
            <div className="serif" style={{fontSize:'28px',fontWeight:700,marginTop:'4px'}}>Daily finance coverage</div>
          </div>
          <div className="mono" style={{fontSize:'11px',color:'var(--muted)',textAlign:'right'}}>{now.toLocaleTimeString('en-US',{hour:'numeric',minute:'2-digit'})}</div>
        </div>

        <div className="inquiry-grid">
          <div className="inquiry-now">
            <div className="label" style={{marginBottom:'8px'}}>{activeSlot ? 'Active now' : 'No active slot'}</div>
            {activeSlot ? (
              <>
                <div style={{display:'flex',alignItems:'center',gap:'10px',marginBottom:'12px'}}>
                  <Avatar name={activeSlot.name} size={42}/>
                  <div>
                    <div style={{fontSize:'20px',fontWeight:800}}>{activeSlot.name}</div>
                    <div className="mono" style={{fontSize:'11px',color:'var(--muted)'}}>{activeSlot.label} · {remainingMinutes} min left</div>
                  </div>
                </div>
                <div className="inquiry-progress"><div className="inquiry-progress-fill" style={{width:activeProgress + '%'}} /></div>
                <div style={{display:'flex',justifyContent:'space-between',marginTop:'8px',fontSize:'11px',color:'var(--muted)'}}>
                  <span>Started</span><strong style={{color:'var(--text)'}}>{Math.round(activeProgress)}%</strong><span>Complete</span>
                </div>
              </>
            ) : (
              <div style={{fontSize:'13px',color:'var(--muted)'}}>The next finance inquiry slot is <strong style={{color:'var(--text)'}}>{nextSlot.name}</strong> at {nextSlot.label}.</div>
            )}
          </div>

          <div className="inquiry-roster">
            {FINANCE_INQUIRY_SCHEDULE.map(slot => {
              const isActive = activeSlot?.name === slot.name;
              const isNext = !activeSlot && nextSlot?.name === slot.name;
              return (
                <div key={slot.name} className={'inquiry-slot ' + (isActive ? 'active' : isNext ? 'next' : '')}>
                  <Avatar name={slot.name} size={30}/>
                  <div style={{minWidth:0}}>
                    <div style={{fontSize:'13px',fontWeight:700,whiteSpace:'nowrap',overflow:'hidden',textOverflow:'ellipsis'}}>{slot.name}</div>
                    <div className="mono" style={{fontSize:'10px',color:'var(--muted)'}}>{slot.label}</div>
                  </div>
                  {isActive && <span className="pill" style={{marginLeft:'auto',background:'rgba(74,222,128,.14)',color:'var(--green)'}}>Live</span>}
                </div>
              );
            })}
          </div>
        </div>
      </div>
    );
  }



  /* ═══════════════════════════════════════════════════════════
     LUNCH MODE
  ═══════════════════════════════════════════════════════════ */
  function LunchModePanel({ currentUser, notifyUser }) {
    const [lunchStatus, setLunchStatus] = useState({});
    const [now, setNow] = useState(() => Date.now());
    const latestRef = useRef({});
    const initializedRef = useRef(false);

    useEffect(() => {
      const timer = setInterval(() => setNow(Date.now()), 30000);
      return () => clearInterval(timer);
    }, []);

    useEffect(() => {
      const applyStatus = (data = {}) => {
        const cleaned = data || {};
        if(initializedRef.current) {
          Object.entries(cleaned).forEach(([name, status]) => {
            const wasActive = !!latestRef.current?.[name]?.active;
            const isActive = !!status?.active;
            if(isActive && !wasActive && name !== currentUser) {
              notifyUser?.('Lunch mode activated', name + ' is on lunch — ' + (status.message || 'professional refueling in progress.'), name);
            }
          });
        } else {
          initializedRef.current = true;
        }
        latestRef.current = cleaned;
        setLunchStatus(cleaned);
      };

      if(isRealtimeReady()) {
        const ref = realtimeDb.ref('lunchStatus');
        const handler = snap => applyStatus(snap.val() || {});
        ref.on('value', handler, e => console.warn('Lunch status sync failed', e));
        return () => ref.off('value', handler);
      }

      const read = () => applyStatus(readLocal('fcdi_lunch_status', {}));
      read();
      const timer = setInterval(read, 1500);
      return () => clearInterval(timer);
    }, [currentUser, notifyUser]);

    const currentStatus = lunchStatus?.[currentUser] || {};
    const isOnLunch = !!currentStatus.active;
    const activeLunches = TEAM_MEMBERS
      .map(m => ({ ...m, status: lunchStatus?.[m.name] || {} }))
      .filter(m => m.status.active);

    const toggleLunch = async () => {
      const turningOn = !isOnLunch;
      const nextStatus = turningOn
        ? { active:true, name:currentUser, startedAt:Date.now(), updatedAt:Date.now(), message:getLunchMessage(currentUser) }
        : { active:false, name:currentUser, endedAt:Date.now(), updatedAt:Date.now(), message:'' };

      const nextAll = { ...(lunchStatus || {}), [currentUser]: nextStatus };
      setLunchStatus(nextAll);
      latestRef.current = nextAll;

      if(isRealtimeReady()) realtimeDb.ref('lunchStatus/' + currentUser).set(nextStatus).catch(console.warn);
      else writeLocal('fcdi_lunch_status', nextAll);

      notifyUser?.(
        turningOn ? 'Lunch mode on' : 'Lunch mode off',
        turningOn ? currentUser + ' is on lunch — ' + nextStatus.message : currentUser + ' is back from lunch.',
        currentUser
      );
    };

    const myStartedAt = currentStatus.startedAt;
    const lunchMinutes = myStartedAt ? Math.max(0, Math.floor((now - myStartedAt) / 60000)) : 0;

    return (
      <div className="card lunch-card" style={{padding:'18px',marginBottom:'48px'}}>
        <div style={{display:'flex',alignItems:'baseline',justifyContent:'space-between',gap:'12px',marginBottom:'14px',position:'relative',flexWrap:'wrap'}}>
          <div>
            <div className="label">Lunch Mode</div>
            <div className="serif" style={{fontSize:'28px',fontWeight:700,marginTop:'4px'}}>Team break status</div>
          </div>
          {activeLunches.length > 0 && <div className="pill" style={{background:'rgba(251,146,60,.14)',color:'var(--orange)'}}>{activeLunches.length} on lunch</div>}
        </div>

        <div className="lunch-wrap">
          <div className="lunch-control">
            <div style={{display:'flex',alignItems:'center',gap:'10px',marginBottom:'14px'}}>
              <Avatar name={currentUser} size={42}/>
              <div>
                <div style={{fontSize:'18px',fontWeight:800}}>{currentUser}</div>
                <div className="mono" style={{fontSize:'11px',color:'var(--muted)'}}>{isOnLunch ? 'On lunch since ' + formatLunchTime(myStartedAt) + ' · ' + lunchMinutes + ' min' : 'Available to the team'}</div>
              </div>
            </div>
            <button onClick={toggleLunch} className={'btn lunch-toggle ' + (isOnLunch ? 'on' : '')}>
              {isOnLunch ? 'I’m back from lunch' : 'Turn on Lunch Mode'}
            </button>
            <div style={{fontSize:'12px',color:'var(--muted)',lineHeight:1.45,marginTop:'12px'}}>
              {isOnLunch ? currentStatus.message : 'When you turn this on, everyone can see you are away and gets the funny lunch status.'}
            </div>
          </div>

          <div>
            {activeLunches.length === 0 ? (
              <div className="lunch-empty">Nobody is on lunch right now. Either the team is productive, or everyone forgot this button exists.</div>
            ) : (
              <div className="lunch-active-grid">
                {activeLunches.map(person => (
                  <div key={person.name} className="lunch-person live">
                    <Avatar name={person.name} size={34}/>
                    <div style={{minWidth:0}}>
                      <div style={{display:'flex',alignItems:'center',gap:'8px',flexWrap:'wrap'}}>
                        <strong style={{fontSize:'14px'}}>{person.name}</strong>
                        <span className="pill" style={{background:'rgba(251,146,60,.14)',color:'var(--orange)'}}>Lunch</span>
                      </div>
                      <div className="mono" style={{fontSize:'10px',color:'var(--faint)',marginTop:'2px'}}>Since {formatLunchTime(person.status.startedAt)}</div>
                      <div className="lunch-message">{person.status.message || person.name + ' is on lunch. Professional refueling in progress.'}</div>
                    </div>
                  </div>
                ))}
              </div>
            )}
          </div>
        </div>
      </div>
    );
  }



  /* ═══════════════════════════════════════════════════════════
     STUDENT PAYMENT COMMUNICATION TOOL — Excel import + mailto drafts
  ═══════════════════════════════════════════════════════════ */
  function WorkEasyHubPanel({ currentUser, notifyUser }) {
    const [mode, setMode] = useState('payment');
    const [paymentRows, setPaymentRows] = useState(() => readLocal('fcdi_we_payment_rows_v3', []));
    const [query, setQuery] = useState('');
    const [selectedIds, setSelectedIds] = useState(() => new Set(readLocal('fcdi_we_payment_selected_v3', [])));
    const [loading, setLoading] = useState(false);
    const [draftPreview, setDraftPreview] = useState(null);
    const [copyToast, setCopyToast] = useState('');
    const fileInputRef = useRef(null);

    useEffect(() => {
      if(!copyToast) return;
      const t = setTimeout(()=>setCopyToast(''), 2400);
      return () => clearTimeout(t);
    }, [copyToast]);

    useEffect(() => { writeLocal('fcdi_we_payment_selected_v3', Array.from(selectedIds)); }, [selectedIds]);

    const savePaymentRows = (nextRows) => {
      setPaymentRows(nextRows);
      writeLocal('fcdi_we_payment_rows_v3', nextRows);
      if(isRealtimeReady()) {
        realtimeDb.ref('workeasyPaymentMailerV3').set({ rows: nextRows, updatedAt: Date.now(), updatedBy: currentUser || 'Unknown' }).catch(e => console.warn('Payment mailer sync failed', e));
      }
    };

    const normalizeCell = (v) => String(v ?? '').replace(/\s+/g, ' ').trim();
    // Keep '#' in keys so 'Student #' stays distinct from 'Student'.
    const normalizeKey = (v) => normalizeCell(v).toLowerCase().replace(/[^a-z0-9#]/g, '');

    const detectHeaderRow = (aoa) => {
      let best = 0, bestScore = -999;
      aoa.slice(0, 25).forEach((row, idx) => {
        const keys = (row || []).map(normalizeKey).filter(Boolean);
        const joined = keys.join(' ');
        let score = 0;
        if(keys.some(k => ['studentname','name','fullname'].includes(k) || (k.includes('student') && k.includes('name')))) score += 10;
        if(keys.some(k => k === 'email' || k.includes('emailaddress') || k.includes('studentemail'))) score += 10;
        if(joined.includes('year2applicationtracker')) score -= 20;
        score += Math.min(keys.length, 8) * 0.25;
        if(score > bestScore) { bestScore = score; best = idx; }
      });
      return best;
    };

    const findColumnIndex = (headers, names, options = {}) => {
      const forbidRaw = (options.forbid || []).map(s => s.toLowerCase());
      const clean = headers.map((h, i) => ({ i, key: normalizeKey(h), raw: normalizeCell(h).toLowerCase() }))
        .filter(x => !forbidRaw.some(f => x.raw.includes(f)));
      // Pass 1: exact match, in seed order. Always allowed for every seed.
      for(const name of names) {
        const needle = normalizeKey(name);
        const exact = clean.find(x => x.key === needle);
        if(exact) return exact.i;
      }
      // Pass 2: loose match, but skip seeds in `exactOnly`.
      const exactOnly = (options.exactOnly || []).map(normalizeKey);
      for(const name of names) {
        const needle = normalizeKey(name);
        if(exactOnly.includes(needle)) continue;
        const loose = clean.find(x => x.key && (x.key.includes(needle) || (!options.noReverseLoose && needle.includes(x.key) && x.key.length >= 5)));
        if(loose) return loose.i;
      }
      return -1;
    };

    const findEmailColumnIndex = (headers) => {
      const clean = headers.map((h, i) => ({ i, key: normalizeKey(h), raw: normalizeCell(h).toLowerCase() }));
      const exact = clean.find(x => ['email','studentemail','emailaddress','studentemailaddress'].includes(x.key));
      if(exact) return exact.i;
      const contains = clean.find(x => x.key.includes('email') || x.raw.includes('e-mail') || x.raw.includes('email'));
      return contains ? contains.i : -1;
    };

    const makePaymentRowId = (name, email, idx) => {
      const base = (email || name || 'student').toLowerCase().replace(/[^a-z0-9]+/g, '_').replace(/^_|_$/g, '');
      return `${base || 'student'}_${idx}`;
    };

    const importPaymentExcel = async (file) => {
      if(!file) return;
      setLoading(true);
      try {
        const buffer = await file.arrayBuffer();
        const wb = XLSX.read(buffer, { type:'array', cellDates:false, raw:false });
        const sheet = wb.Sheets[wb.SheetNames[0]];
        const aoa = XLSX.utils.sheet_to_json(sheet, { header:1, defval:'', raw:false, blankrows:false });
        if(!aoa.length) { notifyUser?.('Import failed', 'The selected Excel file looks empty.'); return; }
        const headerIndex = detectHeaderRow(aoa);
        const headers = aoa[headerIndex] || [];
        // Student Name detection — narrow seeds; 'Name' / 'Student' are EXACT-only so they never grab 'First Name' / 'Student #'.
        const nameIndex = findColumnIndex(
          headers,
          ['Student Name', 'Full Name', 'Name', 'Student'],
          { noReverseLoose:true, forbid:['number','#','id','first','last','email'], exactOnly:['Name','Student'] }
        );
        const firstNameIndex = findColumnIndex(headers, ['First Name', 'Given Name', 'First'], { noReverseLoose:true });
        const lastNameIndex = findColumnIndex(headers, ['Last Name', 'Surname', 'Family Name', 'Last'], { noReverseLoose:true });
        // Student Number detection — 'ID' and 'Number' kept exact-only to avoid grabbing 'Student Name'.
        const studentNumberIndex = findColumnIndex(
          headers,
          ['Student Number', 'Student #', 'Student ID', 'Student No', 'ID', 'Number'],
          { noReverseLoose:true, forbid:['name','email'], exactOnly:['ID','Number'] }
        );
        const emailIndex = findEmailColumnIndex(headers);
        const amountIndex = findColumnIndex(headers, ['Outstanding Amount', 'Owing Amount', 'Outstanding Balance', 'Balance', 'Amount'], { noReverseLoose:true });
        if((nameIndex < 0 && firstNameIndex < 0 && lastNameIndex < 0)) {
          notifyUser?.('Import failed', 'Could not find a name column. Looked for: Student Name, Full Name, Name, First Name + Last Name. Please rename the header in Excel.');
          console.warn('[Payment Import] No name column found in headers:', headers);
          return;
        }
        if(emailIndex < 0) {
          notifyUser?.('Import warning', 'No Email column was found. Rows will import but Generate Email will be disabled until you add an email manually.');
          console.warn('[Payment Import] No email column found in headers:', headers);
        }
        const imported = aoa.slice(headerIndex + 1).map((row, idx) => {
          const first = firstNameIndex >= 0 ? normalizeCell(row?.[firstNameIndex]) : '';
          const last = lastNameIndex >= 0 ? normalizeCell(row?.[lastNameIndex]) : '';
          const fullName = nameIndex >= 0 ? normalizeCell(row?.[nameIndex]) : '';
          const combined = normalizeCell(fullName || [first, last].filter(Boolean).join(' '));
          const email = emailIndex >= 0 ? normalizeCell(row?.[emailIndex]) : '';
          const studentNumber = studentNumberIndex >= 0 ? normalizeCell(row?.[studentNumberIndex]) : '';
          // Guard: never let the student number leak into the name column.
          const name = (combined && combined !== studentNumber) ? combined : '';
          // Skip merged title rows like "Year 2 Application Tracker".
          const joined = (row || []).map(normalizeCell).filter(Boolean).join(' ').toLowerCase();
          if(/year\s*2\s*application\s*tracker/.test(joined) && !email && !studentNumber) return null;
          const owingAmount = amountIndex >= 0 ? normalizeCell(row?.[amountIndex]).replace(/^\$\s*/, '') : '';
          return {
            _id: makePaymentRowId(name, email || studentNumber, idx),
            studentName: name,
            studentNumber,
            email,
            owingAmount,
            paymentLink: '',
            processedAt: '',
            copiedAt: '',
            sourceFile: file.name
          };
        }).filter(r => r && (r.studentName || r.email || r.studentNumber));
        savePaymentRows(imported);
        setSelectedIds(new Set());
        setQuery('');
        notifyUser?.('Payment list loaded', imported.length + ' student row(s) imported from ' + file.name + '.');
      } catch(e) {
        console.error(e);
        notifyUser?.('Import failed', e.message || 'Could not read the Excel file.');
      } finally {
        setLoading(false);
        if(fileInputRef.current) fileInputRef.current.value = '';
      }
    };

    const filteredPaymentRows = useMemo(() => {
      const q = query.trim().toLowerCase();
      if(!q) return paymentRows;
      return paymentRows.filter(r => [r.studentName, r.studentNumber, r.email, r.owingAmount, r.paymentLink].some(v => String(v || '').toLowerCase().includes(q)));
    }, [paymentRows, query]);

    const patchPaymentRow = (id, patch) => savePaymentRows(paymentRows.map(r => r._id === id ? { ...r, ...patch } : r));

    const toggleSelected = (id) => {
      setSelectedIds(prev => {
        const next = new Set(prev);
        next.has(id) ? next.delete(id) : next.add(id);
        return next;
      });
    };

    const selectedRows = paymentRows.filter(r => selectedIds.has(r._id));
    const selectVisible = () => setSelectedIds(new Set(filteredPaymentRows.map(r => r._id)));
    const clearSelection = () => setSelectedIds(new Set());

    const buildPaymentEmail = (row) => {
      const name = normalizeCell(row.studentName) || 'Student';
      const amount = normalizeCell(row.owingAmount).replace(/^\$/,'');
      const link = normalizeCell(row.paymentLink);
      const subject = `Important: Outstanding Balance Reminder - ${name}`;
      const body = [
        'Dear student,',
        '',
        'This email serves as a reminder to pay your outstanding balance on your AGREEMENT.',
        '',
        `Outstanding Amount: $${amount}`,
        '',
        `Please find the payment link: ${link}`,
        '',
        'Use this options if you are selecting BILL PAYMENT option for making payment',
        '',
        `—> Click the link - ${link}`,
        '—> Fill in the required details (refer to the Flywire Payment Instruction Sheet).',
        '—> Select Bill Payment as the payment method.',
        '—> You will receive the reference number which starts with CDRXXXXXX- note down the number',
        '—> Login to your bank account —> Select Bill payment Option —> Add payee —> Payee Name : FLYWIRE —> ACCOUNT NUMBER WILL BE THE REFERENCE NUMBER — CDRXXXXXXX',
        '—> After adding the payee, proceed to make the payment.',
        '',
        "Note: You won't be able to receive Graduation Credentials with your studies without completing your payments"
      ].join('\n');
      return { subject, body };
    };

    const generateEmail = (row) => {
      const email = normalizeCell(row.email);
      if(!email) { notifyUser?.('Missing email', 'This row does not have an email address.'); return; }
      if(!normalizeCell(row.owingAmount)) { notifyUser?.('Missing amount', 'Add the owing amount before generating the email.'); return; }
      if(!normalizeCell(row.paymentLink)) { notifyUser?.('Missing payment link', 'Paste the unique payment link before generating the email.'); return; }
      const draft = buildPaymentEmail(row);
      setDraftPreview({ to: email, studentName: row.studentName || 'Student', ...draft });
      const mailto = `mailto:${encodeURIComponent(email)}?subject=${encodeURIComponent(draft.subject)}&body=${encodeURIComponent(draft.body)}`;
      patchPaymentRow(row._id, { processedAt: getTime(), processedBy: currentUser || 'User' });
      window.location.href = mailto;
    };

    const copyDraft = async (row) => {
      if(!normalizeCell(row.owingAmount)) { notifyUser?.('Missing amount', 'Add the owing amount before copying the draft.'); return; }
      if(!normalizeCell(row.paymentLink)) { notifyUser?.('Missing payment link', 'Paste the unique payment link before copying the draft.'); return; }
      const draft = buildPaymentEmail(row);
      setDraftPreview({ to: normalizeCell(row.email), studentName: row.studentName || 'Student', ...draft });
      const text = `To: ${normalizeCell(row.email)}\nSubject: ${draft.subject}\n\n${draft.body}`;
      try {
        await navigator.clipboard.writeText(text);
        patchPaymentRow(row._id, { copiedAt: getTime(), processedAt: row.processedAt || getTime(), processedBy: currentUser || 'User' });
        setCopyToast('Draft copied to clipboard');
        notifyUser?.('Draft copied', (row.studentName || 'Student') + ' payment email copied.');
      } catch(e) {
        notifyUser?.('Copy failed', 'Clipboard permission was blocked.');
      }
    };

    const exportSelectedPaymentRows = () => {
      if(selectedRows.length === 0) { notifyUser?.('Nothing selected', 'Select at least one student to export.'); return; }
      const data = selectedRows.map(r => {
        const ready = normalizeCell(r.owingAmount) && normalizeCell(r.paymentLink);
        const status = r.processedAt ? 'Processed' : (ready ? 'Ready' : 'Needs amount/link');
        return {
          'Student Name':  r.studentName || '',
          'Email':         r.email || '',
          'Owing Amount':  r.owingAmount || '',
          'Payment Link':  r.paymentLink || '',
          'Status':        status
        };
      });
      const ws = XLSX.utils.json_to_sheet(data);
      const wb = XLSX.utils.book_new();
      XLSX.utils.book_append_sheet(wb, ws, 'Payment Emails');
      XLSX.writeFile(wb, 'Payment_Email_Selected_Students.xlsx');
    };

    const clearPaymentData = () => {
      if(!confirm('Clear the loaded payment email data from this browser?')) return;
      savePaymentRows([]);
      setSelectedIds(new Set());
      setQuery('');
      notifyUser?.('Payment data cleared', 'The payment email list was removed.');
    };

    return (
      <div>
        {/* ================= WORK EASY HUB ================= */}
        {/* ================= PAYMENT EMAILS ================= */}
        <div style={{display:'flex',alignItems:'center',justifyContent:'space-between',gap:'12px',flexWrap:'wrap',marginBottom:'14px'}}>
          <div className="we-tabs" role="tablist">
            <button onClick={()=>setMode('payment')} className={`we-tab ${mode==='payment'?'active':''}`} role="tab" aria-selected={mode==='payment'}>Payment Emails</button>
            <button onClick={()=>setMode('yr2')} className={`we-tab ${mode==='yr2'?'active':''}`} role="tab" aria-selected={mode==='yr2'}>Yr 2 Tracker</button>
          </div>
          <div style={{fontSize:'11px',color:'var(--muted)',letterSpacing:'.04em'}}>
            {mode==='payment' ? 'Excel-driven payment reminders' : 'Separate Excel-driven workspace'}
          </div>
        </div>

        {mode === 'payment' ? (
          <section className="we-card">
            <div className="we-card-head">
              <div>
                <div className="label" style={{color:'#22d3ee',marginBottom:'2px'}}>Payment Emails</div>
                <h2>Generate payment reminder emails</h2>
                <p style={{fontSize:'12.5px',color:'var(--muted)',margin:'4px 0 0',maxWidth:'640px',lineHeight:1.55}}>
                  Upload an Excel sheet with student name and email. Add the owing amount and unique payment link inline, then generate or copy the pre-filled Flywire email.
                </p>
              </div>
              <div className="we-actions">
                <button onClick={()=>fileInputRef.current?.click()} className="we-btn primary">⬆ Upload Excel</button>
                <button onClick={exportSelectedPaymentRows} className="we-btn" disabled={selectedRows.length===0}>Export selected ({selectedRows.length})</button>
                <button onClick={clearPaymentData} className="we-btn danger" disabled={paymentRows.length===0}>Clear</button>
                <input ref={fileInputRef} type="file" accept=".xlsx,.xls" style={{display:'none'}} onChange={e=>importPaymentExcel(e.target.files?.[0])}/>
              </div>
            </div>

            {paymentRows.length === 0 ? (
              <div className="we-upload" onClick={()=>fileInputRef.current?.click()}>
                <div style={{fontSize:'26px',color:'#22d3ee'}}>↥</div>
                <div className="we-upload-title">Upload your payment Excel file</div>
                <div className="we-upload-hint">Accepted: .xlsx, .xls. We auto-detect Student Name / First Name + Last Name, Student #, Email, and Amount headers.</div>
                {loading && <div className="mono" style={{fontSize:'11px',color:'#22d3ee',marginTop:'10px'}}>Importing…</div>}
              </div>
            ) : (
              <>
                <div className="we-toolbar">
                  <input value={query} onChange={e=>setQuery(e.target.value)} className="we-search" placeholder="Search by name, email, amount, or payment link…"/>
                  <div className="we-actions" style={{justifyContent:'flex-end'}}>
                    <button onClick={selectVisible} className="we-btn">Select visible</button>
                    <button onClick={clearSelection} className="we-btn subtle">Clear selection</button>
                  </div>
                </div>

                <div className="we-stats">
                  <span className="we-pill">{paymentRows.length} loaded</span>
                  <span className="we-pill">{filteredPaymentRows.length} showing</span>
                  <span className="we-pill ready">{paymentRows.filter(r=>normalizeCell(r.owingAmount)&&normalizeCell(r.paymentLink)&&!r.processedAt).length} ready</span>
                  <span className="we-pill done">{paymentRows.filter(r=>r.processedAt).length} processed</span>
                </div>

                {draftPreview && (
                  <div className="we-preview">
                    <div className="we-preview-head">
                      <div>
                        <div className="label" style={{color:'#22d3ee',marginBottom:'2px'}}>Generated Email Preview</div>
                        <div style={{fontWeight:600,fontSize:'14px'}}>{draftPreview.studentName}</div>
                      </div>
                      <button onClick={()=>setDraftPreview(null)} className="we-btn subtle">Hide preview</button>
                    </div>
                    <div className="we-preview-grid">
                      <div className="we-preview-meta">
                        <div className="label">To</div>
                        <div className="we-preview-meta-row">{draftPreview.to || '—'}</div>
                        <div className="label">Subject</div>
                        <div className="we-preview-meta-row" style={{marginBottom:0}}>{draftPreview.subject}</div>
                      </div>
                      <textarea className="we-preview-body" value={draftPreview.body} readOnly/>
                    </div>
                  </div>
                )}

                <div className="we-table-wrap scroll">
                  <table className="we-table">
                    <thead>
                      <tr>
                        <th style={{width:'38px'}}></th>
                        <th>Student Name</th>
                        <th>Student #</th>
                        <th>Email</th>
                        <th style={{width:'150px'}}>Owing Amount</th>
                        <th style={{width:'280px'}}>Payment Link</th>
                        <th>Status</th>
                        <th style={{width:'200px'}}>Actions</th>
                      </tr>
                    </thead>
                    <tbody>
                      {filteredPaymentRows.map(row => {
                        const ready = normalizeCell(row.owingAmount) && normalizeCell(row.paymentLink);
                        const processed = !!row.processedAt;
                        const canGenerate = !!normalizeCell(row.email) && ready;
                        return (
                          <tr key={row._id} className={processed ? 'processed' : (ready ? 'ready' : '')}>
                            <td><input type="checkbox" checked={selectedIds.has(row._id)} onChange={()=>toggleSelected(row._id)}/></td>
                            <td><div className="we-name">{row.studentName || <span style={{color:'var(--muted)'}}>Name missing</span>}</div></td>
                            <td><div className="we-sub">{row.studentNumber || '—'}</div></td>
                            <td><div className="we-sub" style={{wordBreak:'break-all'}}>{row.email || <span style={{color:'var(--red)'}}>missing</span>}</div></td>
                            <td><input value={row.owingAmount || ''} onChange={e=>patchPaymentRow(row._id,{owingAmount:e.target.value})} className="we-input" placeholder="e.g. 766.00"/></td>
                            <td><input value={row.paymentLink || ''} onChange={e=>patchPaymentRow(row._id,{paymentLink:e.target.value})} className="we-input" placeholder="Paste unique payment link"/></td>
                            <td>
                              {processed ? <span className="we-pill done">Processed</span>
                                : ready ? <span className="we-pill ready">Ready</span>
                                : <span className="we-pill">Needs amount/link</span>}
                            </td>
                            <td>
                              <div className="we-actions">
                                <button onClick={()=>generateEmail(row)} className="we-btn primary" disabled={!canGenerate} title={!canGenerate ? 'Email, amount and payment link are required' : 'Generate Email'}>Generate</button>
                                <button onClick={()=>copyDraft(row)} className="we-btn" disabled={!ready} title={!ready ? 'Add amount and payment link first' : 'Copy Draft'}>Copy</button>
                              </div>
                            </td>
                          </tr>
                        );
                      })}
                    </tbody>
                  </table>
                </div>
              </>
            )}
          </section>
        ) : (
          /* ================= YR 2 TRACKER PLACEHOLDER ================= */
          <section className="we-card">
            <div className="we-card-head">
              <div>
                <div className="label" style={{color:'#a78bfa',marginBottom:'2px'}}>Yr 2 Tracker</div>
                <h2>Separate workspace for Year 2 data</h2>
                <p style={{fontSize:'12.5px',color:'var(--muted)',margin:'4px 0 0',maxWidth:'640px',lineHeight:1.55}}>
                  This is a clean placeholder. Yr 2 Tracker will use its own Excel upload, its own data structure, its own export workflow, and its own localStorage. Nothing here will read from or write to the Payment Emails data.
                </p>
              </div>
            </div>
            <div className="we-placeholder">
              <strong>Ready for the next instructions.</strong>
              Send the columns you want, the workflow you want, and any export rules. I&apos;ll wire this tab end-to-end without touching Payment Emails.
            </div>
          </section>
        )}

        {copyToast && <div className="we-toast">{copyToast}</div>}
      </div>
    );
  }

  /* ═══════════════════════════════════════════════════════════
     TASK WAR ROOM
  ═══════════════════════════════════════════════════════════ */
  function TaskWarRoom({ currentUser, onSwitchUser, onNavigate, theme, onToggleTheme }) {
    const [chatOpen, setChatOpen] = useState(false);
    const [chessOpen, setChessOpen] = useState(false);
    const [unread, setUnread] = useState(0);
    const [toasts, setToasts] = useState([]);
    const [masterGoals, setMasterGoals] = useState(() => Object.fromEntries(TASK_POOL.map(t=>[t.id,0])));
    const [memberTasks, setMemberTasks] = useState(() => Object.fromEntries(TEAM_MEMBERS.map(m=>[m.name,[]])));
    const [todayKey, setTodayKey] = useState(() => dateKeyFromDate());
    const [dailyTaskLog, setDailyTaskLog] = useState({});
    const [weeklyTaskHistory, setWeeklyTaskHistory] = useState({});
    const [draggedTask, setDraggedTask] = useState(null);
    const [hoveredMember, setHoveredMember] = useState(null);
    const [assignPending, setAssignPending] = useState(null);
    const [editingGoal, setEditingGoal] = useState(null);
    const [goalDraft, setGoalDraft] = useState('');
    const [welcomeLine] = useState(() => getRotatingWelcome(currentUser));
    const [moodLine] = useState(() => getRotatingMood(currentUser));
    const [showDevResetPanel, setShowDevResetPanel] = useState(false);
    const lastMsgCount = useRef(0);

    const notifyUser = useCallback((title, body='', actor=null) => {
      const id = localId('toast');
      setToasts(p => [{id, title, body}, ...p].slice(0, 5));
      setTimeout(() => setToasts(p => p.filter(t => t.id !== id)), 6500);
      const allowed = localStorage.getItem('fcdi_notify_permission') === 'granted' || window.Notification?.permission === 'granted';
      if(allowed && actor !== currentUser && 'Notification' in window) {
        try { new Notification(title, { body }); } catch(e) { console.warn(e); }
      }
    }, [currentUser]);

    useEffect(()=>{ document.body.className=''; },[]);

    useEffect(() => {
      const timer = setInterval(() => {
        const next = dateKeyFromDate();
        if(next !== todayKey) setTodayKey(next);
      }, 60000);
      return () => clearInterval(timer);
    }, [todayKey]);

    useEffect(() => {
      const emptyTasks = () => Object.fromEntries(TEAM_MEMBERS.map(m=>[m.name,[]]));

      if(isRealtimeReady()) {
        const goalsRef = realtimeDb.ref('config/masterGoals');
        const tasksRef = realtimeDb.ref('dailyTeamRosters/' + todayKey + '/tasks');
        const todayRef = realtimeDb.ref('dailyTaskHistory/' + todayKey);
        const historyRef = realtimeDb.ref('dailyTaskHistory');

        const goalsHandler = snap => setMasterGoals(snap.val() || Object.fromEntries(TASK_POOL.map(t=>[t.id,0])));
        const tasksHandler = snap => {
          const raw = snap.val() || {};
          const next = emptyTasks();
          Object.entries(raw).forEach(([id,data]) => {
            if(data && next[data.member]) next[data.member].push({...data, id});
          });
          setMemberTasks(next);
        };
        const todayHandler = snap => setDailyTaskLog(snap.val() || {});
        const historyHandler = snap => {
          const all = snap.val() || {};
          const wanted = new Set(lastNDates(7));
          const compact = {};
          Object.entries(all).forEach(([date, log]) => { if(wanted.has(date)) compact[date] = log || {}; });
          setWeeklyTaskHistory(compact);
        };
        const err = e => console.warn('Realtime task sync failed', e);
        goalsRef.on('value', goalsHandler, err);
        tasksRef.on('value', tasksHandler, err);
        todayRef.on('value', todayHandler, err);
        historyRef.on('value', historyHandler, err);
        return () => {
          goalsRef.off('value', goalsHandler);
          tasksRef.off('value', tasksHandler);
          todayRef.off('value', todayHandler);
          historyRef.off('value', historyHandler);
        };
      }

      if(isFirebaseReady()) {
        const u1 = db.collection('config').doc('masterGoals').onSnapshot(doc=>{ if(doc.exists) setMasterGoals(doc.data()); });
        const u2 = db.collection('dailyTeamRosters').doc(todayKey).collection('tasks').onSnapshot(snap => {
          const next = emptyTasks();
          snap.docs.forEach(d => { const data = d.data(); if(next[data.member]) next[data.member].push({...data,id:d.id}); });
          setMemberTasks(next);
        });
        return () => { u1(); u2(); };
      }

      setMasterGoals(readLocal('fcdi_master_goals', Object.fromEntries(TASK_POOL.map(t=>[t.id,0]))));
      setMemberTasks(readLocal('fcdi_member_tasks_' + todayKey, emptyTasks()));
      setDailyTaskLog(readLocal('fcdi_daily_log_' + todayKey, {}));
      const compact = {};
      lastNDates(7).forEach(k => compact[k] = readLocal('fcdi_daily_log_' + k, {}));
      setWeeklyTaskHistory(compact);
    }, [todayKey]);

    useEffect(() => {
      if(chatOpen){ lastMsgCount.current = 0; return; }

      if(isRealtimeReady()){
        const ref = realtimeDb.ref('chat').orderByChild('timestamp').limitToLast(200);
        const handler = snap => {
          const val = snap.val() || {};
          const messages = Object.values(val).filter(m => m && m.author && m.author !== currentUser && m.author !== 'System');
          const count = messages.length;
          if(lastMsgCount.current && count > lastMsgCount.current) setUnread(p => p + (count - lastMsgCount.current));
          lastMsgCount.current = count;
        };
        ref.on('value', handler, e => console.warn('Unread chat listener failed', e));
        return () => ref.off('value', handler);
      }

      if(isFirebaseReady()){
        const u = db.collection('chat').orderBy('timestamp','asc').limitToLast(200).onSnapshot(snap => {
          const docs = snap.docs.map(d => d.data());
          const visibleCount = docs.filter(m => m.author !== currentUser && m.author !== 'System').length;
          if(lastMsgCount.current && visibleCount > lastMsgCount.current) setUnread(p => p + (visibleCount - lastMsgCount.current));
          lastMsgCount.current = visibleCount;
        });
        return () => u();
      }

      const check = () => {
        const local = readLocal('fcdi_chat_messages', []).filter(m => m.author !== currentUser && m.author !== 'System');
        if(lastMsgCount.current && local.length > lastMsgCount.current) setUnread(p => p + (local.length - lastMsgCount.current));
        lastMsgCount.current = local.length;
      };
      check();
      const timer = setInterval(check, 1200);
      return () => clearInterval(timer);
    }, [chatOpen, currentUser]);

    const getDailyDone = (memberName, taskId) => {
      const record = dailyTaskLog?.[memberName]?.[taskId];
      return typeof record === 'number' ? record : Number(record?.done || 0);
    };

    const totals = useMemo(() => {
      const dbt = {};
      TASK_POOL.forEach(t => { dbt[t.id] = 0; });
      flattenDailyLog(dailyTaskLog).forEach(entry => { dbt[entry.taskId] = (dbt[entry.taskId]||0) + Number(entry.done||0); });
      const tg = TASK_POOL.reduce((s,t) => s + Number(masterGoals[t.id]||0), 0);
      const td = TASK_POOL.reduce((s,t) => s + Number(dbt[t.id]||0), 0);
      return { doneByTask:dbt, totalGoal:tg, totalDone:td, totalPending:Math.max(tg-td,0), officeProgress: tg ? Math.min(100,Math.round(td/tg*100)) : 0 };
    }, [dailyTaskLog, masterGoals]);

    const weeklySummary = useMemo(() => {
      return lastNDates(7).map(date => {
        const rows = flattenDailyLog(weeklyTaskHistory[date] || {});
        const total = rows.reduce((sum, row) => sum + Number(row.done || 0), 0);
        const byMember = {};
        rows.forEach(row => { byMember[row.member] = (byMember[row.member] || 0) + Number(row.done || 0); });
        const topMember = Object.entries(byMember).sort((a,b)=>b[1]-a[1])[0];
        return { date, total, topMember };
      });
    }, [weeklyTaskHistory]);

    const getMemberStats = name => {
      const tasks = memberTasks[name] || [];
      const done = tasks.reduce((s,i) => s + getDailyDone(name, i.taskId), 0);
      const goal = tasks.reduce((s,i) => s + Number(i.goalNumber||0), 0);
      return { count:tasks.length, done, assignedGoal:goal, progress: goal ? Math.min(100,Math.round(done/goal*100)) : 0 };
    };

    const updateGoal = (taskId, val) => {
      const next = { ...masterGoals, [taskId]: clamp(val, 0, 99999) };
      setMasterGoals(next);
      if(isRealtimeReady()) realtimeDb.ref('config/masterGoals').set(next).catch(console.warn);
      else if(isFirebaseReady()) fbSet('config','masterGoals',next,false);
      else writeLocal('fcdi_master_goals', next);
    };

    const handleDragStart = task => e => { setDraggedTask(task); e.dataTransfer.effectAllowed='copy'; e.dataTransfer.setData('text/plain', task.id); };
    const handleDrop = memberName => e => {
      e.preventDefault();
      const task = draggedTask || TASKS_BY_ID[e.dataTransfer.getData('text/plain')];
      if(!task) return;
      if((memberTasks[memberName]||[]).some(i=>i.taskId===task.id)){ setDraggedTask(null); setHoveredMember(null); return; }
      setAssignPending({ task, memberName });
      setDraggedTask(null); setHoveredMember(null);
    };

    const confirmAssign = goalNumber => {
      if(!assignPending) return;
      const { task, memberName } = assignPending;
      const docId = `${memberName}_${task.id}`;
      const data = { taskId:task.id, taskName:task.name, member:memberName, goalNumber, createdAt:Date.now(), updatedAt:Date.now() };
      const nextTasks = {...memberTasks, [memberName]:[...(memberTasks[memberName] || []), {id:docId,...data}]};
      setMemberTasks(nextTasks);
      if(isRealtimeReady()) realtimeDb.ref('dailyTeamRosters/' + todayKey + '/tasks/' + docId).set(data).catch(console.warn);
      else if(isFirebaseReady()) db.collection('dailyTeamRosters').doc(todayKey).collection('tasks').doc(docId).set(data).catch(console.warn);
      else writeLocal('fcdi_member_tasks_' + todayKey, nextTasks);
      setAssignPending(null);
    };

    const removeTask = (memberName, docId) => {
      if(memberName !== currentUser) return;
      const nextTasks = {...memberTasks, [memberName]: (memberTasks[memberName] || []).filter(i => i.id !== docId)};
      setMemberTasks(nextTasks);
      if(isRealtimeReady()) realtimeDb.ref('dailyTeamRosters/' + todayKey + '/tasks/' + docId).remove().catch(console.warn);
      else if(isFirebaseReady()) db.collection('dailyTeamRosters').doc(todayKey).collection('tasks').doc(docId).delete().catch(console.warn);
      else writeLocal('fcdi_member_tasks_' + todayKey, nextTasks);
    };

    const resetTodayRoster = async (askConfirm = true) => {
      if(askConfirm) {
        const ok = window.confirm('Reset today\'s team roster? This clears today\'s assigned roster only. Daily completed history stays saved.');
        if(!ok) return;
      }
      const emptyTasks = Object.fromEntries(TEAM_MEMBERS.map(m=>[m.name,[]]));
      setMemberTasks(emptyTasks);
      if(isRealtimeReady()) {
        realtimeDb.ref('dailyTeamRosters/' + todayKey + '/tasks').remove().catch(console.warn);
      } else if(isFirebaseReady()) {
        try {
          const snap = await db.collection('dailyTeamRosters').doc(todayKey).collection('tasks').get();
          const batch = db.batch();
          snap.docs.forEach(doc => batch.delete(doc.ref));
          await batch.commit();
        } catch(e) { console.warn(e); }
      } else {
        writeLocal('fcdi_member_tasks_' + todayKey, emptyTasks);
      }
    };


    const deleteFirestoreCollection = async (collectionName) => {
      if(!isFirebaseReady()) return;
      try {
        const snap = await db.collection(collectionName).get();
        let batch = db.batch();
        let count = 0;
        for (const doc of snap.docs) {
          batch.delete(doc.ref);
          count++;
          if (count % 450 === 0) { await batch.commit(); batch = db.batch(); }
        }
        if (count % 450 !== 0) await batch.commit();
      } catch(e) { console.warn('Could not delete Firestore collection:', collectionName, e); }
    };

    const askDevConfirm = (label, details) => {
      if(currentUser !== 'Kanish') return false;
      return window.confirm(`Kanish dev reset: ${label}\n\n${details}\n\nContinue?`);
    };

    const clearLocalKeys = (matcher) => {
      Object.keys(localStorage).forEach(key => {
        if(matcher(key)) localStorage.removeItem(key);
      });
    };

    const resetDevMasterGoals = async () => {
      if(!askDevConfirm('Reset War Room master goals', 'This clears the editable target numbers only. Team roster and completed history stay saved.')) return;
      const empty = Object.fromEntries(TASK_POOL.map(t=>[t.id,0]));
      setMasterGoals(empty);
      if(isRealtimeReady()) await realtimeDb.ref('config/masterGoals').remove().catch(console.warn);
      else if(isFirebaseReady()) await db.collection('config').doc('masterGoals').delete().catch(console.warn);
      clearLocalKeys(k => k === 'fcdi_master_goals');
      alert('Master goals reset.');
    };

    const resetDevTodayRoster = async () => {
      if(!askDevConfirm('Reset today\'s team roster', 'This clears today\'s assigned roster only. Completed numbers and weekly history stay saved.')) return;
      await resetTodayRoster(false);
      alert('Today roster reset.');
    };

    const resetDevTodayTaskHistory = async () => {
      if(!askDevConfirm('Reset today\'s completed task numbers', 'This clears today\'s completed counts only. Assigned roster and master goals stay saved.')) return;
      setDailyTaskLog({});
      setWeeklyTaskHistory(p => ({ ...(p || {}), [todayKey]: {} }));
      if(isRealtimeReady()) await realtimeDb.ref('dailyTaskHistory/' + todayKey).remove().catch(console.warn);
      clearLocalKeys(k => k === 'fcdi_daily_log_' + todayKey);
      alert('Today completed task numbers reset.');
    };

    const resetDevAllTaskHistory = async () => {
      if(!askDevConfirm('Reset all daily / weekly task history', 'This clears every saved daily completion log. Master goals and assigned rosters stay saved.')) return;
      setDailyTaskLog({});
      setWeeklyTaskHistory({});
      if(isRealtimeReady()) await realtimeDb.ref('dailyTaskHistory').remove().catch(console.warn);
      clearLocalKeys(k => k.startsWith('fcdi_daily_log_'));
      alert('All task history reset.');
    };

    const resetDevChat = async () => {
      if(!askDevConfirm('Reset team chat', 'This clears chat messages and unread count only.')) return;
      setUnread(0);
      if(isRealtimeReady()) await realtimeDb.ref('chat').remove().catch(console.warn);
      if(isFirebaseReady()) await deleteFirestoreCollection('chat');
      clearLocalKeys(k => k === 'fcdi_chat_messages');
      alert('Chat reset.');
    };

    const resetDevChess = async () => {
      if(!askDevConfirm('Reset chess games and invites', 'This clears active chess games and chess invites only.')) return;
      if(isRealtimeReady()) await Promise.all([
        realtimeDb.ref('chessGames').remove(),
        realtimeDb.ref('chessInvites').remove()
      ].map(p => p.catch(console.warn)));
      if(isFirebaseReady()) {
        await deleteFirestoreCollection('chessGames');
        await deleteFirestoreCollection('chessInvites');
      }
      clearLocalKeys(k => k === 'fcdi_chess_games' || k === 'fcdi_chess_invites');
      alert('Chess data reset.');
    };

    const resetDevLunch = async () => {
      if(!askDevConfirm('Reset lunch statuses', 'This clears everyone\'s active lunch status only.')) return;
      if(isRealtimeReady()) await realtimeDb.ref('lunchStatus').remove().catch(console.warn);
      clearLocalKeys(k => k === 'fcdi_lunch_status' || k.startsWith('fcdi_lunch_message_index_'));
      alert('Lunch statuses reset.');
    };

    const resetDevWorkEasy = async () => {
      if(!askDevConfirm('Reset WorkEasy data', 'This clears WorkEasy payment email rows, selected rows, notes/preview cache, and synced WorkEasy data only.')) return;
      if(isRealtimeReady()) await realtimeDb.ref('workeasyPaymentMailerV3').remove().catch(console.warn);
      clearLocalKeys(k => k.startsWith('fcdi_we_'));
      alert('WorkEasy data reset. Reload WorkEasy Hub to see the clean state.');
    };

    const resetDevMonthEndExcel = async () => {
      if(!askDevConfirm('Reset Month End Excel roster', 'This clears imported Month End students and tracker marks. SPAR/GAC/Overpayment packages are session-based and will also be clean after reload.')) return;
      if(isFirebaseReady()) await deleteFirestoreCollection('monthend_students');
      clearLocalKeys(k => k.startsWith('fcdi_monthend_'));
      alert('Month End Excel roster reset. Reload Month End Mode before uploading a new roster.');
    };

    const resetDevLocalCache = async () => {
      if(!askDevConfirm('Reset local cache on this browser', 'This clears saved f-cdi browser data on this device, but keeps the logged-in user, theme, and notification permission. Cloud data is not touched.')) return;
      const keepUser = localStorage.getItem('fcdi_user');
      const keepTheme = localStorage.getItem('fcdi_theme');
      const keepNotify = localStorage.getItem('fcdi_notify_permission');
      clearLocalKeys(k => k.startsWith('fcdi_'));
      if(keepUser) localStorage.setItem('fcdi_user', keepUser);
      if(keepTheme) localStorage.setItem('fcdi_theme', keepTheme);
      if(keepNotify) localStorage.setItem('fcdi_notify_permission', keepNotify);
      alert('Local cache reset. Reloading now.');
      window.location.reload();
    };

    const updateDone = (memberName, docId, taskId, val) => {
      if(memberName !== currentUser) return;
      const taskRow = (memberTasks[memberName]||[]).find(i => i.id === docId);
      const goal = taskRow?.goalNumber || 0;
      const done = clamp(val, 0, Number(goal));
      const record = { done, taskName: taskRow?.taskName || TASKS_BY_ID[taskId]?.name || taskId, updatedAt: Date.now(), updatedBy: currentUser };
      const nextDaily = {
        ...(dailyTaskLog || {}),
        [memberName]: {
          ...(dailyTaskLog?.[memberName] || {}),
          [taskId]: record
        }
      };
      setDailyTaskLog(nextDaily);
      if(isRealtimeReady()) realtimeDb.ref(`dailyTaskHistory/${todayKey}/${memberName}/${taskId}`).set(record).catch(console.warn);
      else writeLocal('fcdi_daily_log_' + todayKey, nextDaily);
    };

    const startEditGoal = (taskId, currentGoal) => { setEditingGoal(taskId); setGoalDraft(String(currentGoal||0)); };
    const commitGoal = (taskId) => { updateGoal(taskId, goalDraft); setEditingGoal(null); };

    return (
      <div style={{minHeight:'100vh',background:'var(--bg)',position:'relative'}}>
        <ToastHost toasts={toasts} onClose={(id)=>setToasts(p=>p.filter(t=>t.id!==id))} />
        <ChatPanel currentUser={currentUser} open={chatOpen}
          onToggle={()=>{ setChatOpen(p=>!p); if(!chatOpen) setUnread(0); }}
          unread={unread} onClearUnread={()=>setUnread(0)} notifyUser={notifyUser} />
        <ChessPanel currentUser={currentUser} open={chessOpen} onClose={()=>setChessOpen(false)} notifyUser={notifyUser} />

        {/* TOP BAR */}
        <div className="topbar">
          <div style={{display:'flex',alignItems:'center',gap:'14px'}}>
            <span className="wordmark">f-cdi</span>
            <span style={{color:'var(--faint)'}}>/</span>
            <span className="label">Task War Room</span>
          </div>
          <div style={{display:'flex',alignItems:'center',gap:'10px'}}>
            <button onClick={()=>setChessOpen(true)} className="btn btn-orange" style={{fontSize:'12px',padding:'7px 10px'}}>Click this if you’re bored</button>
            {currentUser === 'Kanish' && <button onClick={()=>setShowDevResetPanel(p=>!p)} className="btn" style={{fontSize:'12px',padding:'7px 10px',borderColor:'var(--orange)',color:'var(--orange)'}}>Dev Reset Tools</button>}
            <NotificationButton notifyUser={notifyUser}/>
            <span style={{fontSize:'12px',color:'var(--muted)'}}>{theme==='dark'?'☾':'☀'}</span>
            <ThemeToggle theme={theme} onToggle={onToggleTheme}/>
            <div className="seg">
              <button className="seg-btn on" onClick={()=>onNavigate('war')}>War Room</button>
              <button className="seg-btn" onClick={()=>onNavigate('workeasy')}>WorkEasy Hub</button>
              <button className="seg-btn" onClick={()=>onNavigate('monthend')}>Month End</button>
            </div>
            <div style={{display:'flex',alignItems:'center',gap:'8px',padding:'4px 10px 4px 4px',background:'var(--bg-2)',border:'1px solid var(--line)',borderRadius:'24px'}}>
              <Avatar name={currentUser} size={26}/>
              <span style={{fontSize:'13px',fontWeight:500}}>{currentUser}</span>
              <span style={{width:'6px',height:'6px',borderRadius:'50%',background:'#4ade80'}} className="dot-pulse"></span>
            </div>
            <button onClick={onSwitchUser} className="btn-link" title="Switch user">Switch user</button>
          </div>
        </div>

        {/* MAIN CONTENT */}
        <div style={{maxWidth:'1400px',margin:'0 auto',padding:'48px 32px 80px'}}>
          <div style={{display:'flex',alignItems:'flex-start',justifyContent:'space-between',gap:'18px',flexWrap:'wrap',marginBottom:'28px'}}>
            <div>
              <h1 className="serif" style={{fontSize:'clamp(36px,5vw,58px)',fontWeight:600,lineHeight:1.05,marginBottom:'8px'}}>{welcomeLine}</h1>
              <p className="mono" style={{color:'var(--muted)',fontSize:'13px'}}>{currentUser} · {new Date().toLocaleDateString('en-US',{weekday:'long',month:'long',day:'numeric'})}</p>
            </div>
            <div className="card-flat" style={{padding:'12px 14px',maxWidth:'310px',background:'linear-gradient(135deg, rgba(251,146,60,.10), var(--bg-2))'}}>
              <div className="label" style={{marginBottom:'5px'}}>Today’s mood</div>
              <div style={{fontSize:'13px',color:'var(--muted)',lineHeight:1.45}}>{moodLine}</div>
            </div>
          </div>

          {currentUser === 'Kanish' && showDevResetPanel && (
            <div className="card" style={{padding:'16px',marginBottom:'18px',borderColor:'var(--orange)',background:'linear-gradient(135deg, rgba(251,146,60,.08), var(--bg-2))'}}>
              <div style={{display:'flex',alignItems:'flex-start',justifyContent:'space-between',gap:'12px',marginBottom:'12px',flexWrap:'wrap'}}>
                <div>
                  <div className="label" style={{color:'var(--orange)',marginBottom:'5px'}}>Kanish Developer Reset Tools</div>
                  <div style={{fontSize:'13px',color:'var(--muted)',lineHeight:1.45}}>Individual reset buttons only. Each button clears one area and asks for confirmation first.</div>
                </div>
                <button onClick={()=>setShowDevResetPanel(false)} className="btn btn-ghost">Close</button>
              </div>
              <div style={{display:'grid',gridTemplateColumns:'repeat(auto-fit,minmax(220px,1fr))',gap:'10px'}}>
                <button onClick={resetDevMasterGoals} className="btn" style={{justifyContent:'center'}}>Reset Master Goals</button>
                <button onClick={resetDevTodayRoster} className="btn" style={{justifyContent:'center'}}>Reset Today Roster</button>
                <button onClick={resetDevTodayTaskHistory} className="btn" style={{justifyContent:'center'}}>Reset Today Completed</button>
                <button onClick={resetDevAllTaskHistory} className="btn" style={{justifyContent:'center'}}>Reset All Task History</button>
                <button onClick={resetDevChat} className="btn" style={{justifyContent:'center'}}>Reset Team Chat</button>
                <button onClick={resetDevChess} className="btn" style={{justifyContent:'center'}}>Reset Chess Games</button>
                <button onClick={resetDevLunch} className="btn" style={{justifyContent:'center'}}>Reset Lunch Status</button>
                <button onClick={resetDevWorkEasy} className="btn" style={{justifyContent:'center'}}>Reset WorkEasy Data</button>
                <button onClick={resetDevMonthEndExcel} className="btn" style={{justifyContent:'center'}}>Reset Month End Excel</button>
                <button onClick={resetDevLocalCache} className="btn btn-danger" style={{justifyContent:'center'}}>Reset Local Cache</button>
              </div>
            </div>
          )}

          <FinancialInquiryPanel currentUser={currentUser} notifyUser={notifyUser} />
          <LunchModePanel currentUser={currentUser} notifyUser={notifyUser} />

          {/* STATS */}
          <div className="label" style={{marginBottom:'14px'}}>At a glance</div>
          <div style={{display:'grid',gridTemplateColumns:'repeat(auto-fit,minmax(180px,1fr))',gap:'12px',marginBottom:'48px'}}>
            {[
              { label:'Pending',   value:totals.totalPending.toLocaleString(),  color:'var(--orange)' },
              { label:'Completed', value:totals.totalDone.toLocaleString(),     color:'var(--green)' },
              { label:'Total Goal',value:totals.totalGoal.toLocaleString(),     color:'var(--text)' },
              { label:'Progress',  value:`${totals.officeProgress}%`,           color:totals.officeProgress > 75 ? 'var(--green)' : 'var(--orange)', bar:true },
            ].map(s => (
              <div key={s.label} className="card" style={{padding:'18px'}}>
                <div className="label" style={{marginBottom:'10px'}}>{s.label}</div>
                <div className="serif" style={{fontSize:'32px',fontWeight:600,color:s.color,lineHeight:1}}>{s.value}</div>
                {s.bar && <div className="bar" style={{marginTop:'12px'}}><div className="bar-fill" style={{width:`${totals.officeProgress}%`,background:'linear-gradient(90deg,var(--orange),var(--green))'}}/></div>}
              </div>
            ))}
          </div>

          {/* TOTAL TASKS */}
          <div style={{display:'flex',alignItems:'baseline',justifyContent:'space-between',marginBottom:'14px'}}>
            <div className="label">Daily Total Tasks</div>
            <div style={{fontSize:'12px',color:'var(--muted)'}}>Today: {formatHistoryDate(todayKey)} · completed numbers reset by date and stay saved in history.</div>
          </div>
          <div style={{display:'grid',gridTemplateColumns:'repeat(auto-fit,minmax(220px,1fr))',gap:'12px',marginBottom:'48px'}}>
            {TASK_POOL.map(task => {
              const goal = Number(masterGoals[task.id]||0);
              const done = Number(totals.doneByTask[task.id]||0);
              const pct = goal ? Math.min(100,Math.round(done/goal*100)) : 0;
              const editing = editingGoal === task.id;
              return (
                <div key={task.id} className="card" style={{padding:'16px'}}>
                  <div style={{display:'flex',alignItems:'flex-start',justifyContent:'space-between',gap:'8px',marginBottom:'12px'}}>
                    <div>
                      <div className="mono" style={{fontSize:'10px',textTransform:'uppercase',letterSpacing:'.12em',color:task.color,marginBottom:'2px'}}>{task.group}</div>
                      <div style={{fontSize:'15px',fontWeight:600}}>{task.name}</div>
                    </div>
                    <button onClick={()=>{ if(editing){ commitGoal(task.id); } else { startEditGoal(task.id, goal); } }} className="btn-ghost" style={{padding:'2px 8px',fontSize:'12px'}}>{editing?'✓':'✎'}</button>
                  </div>
                  {editing
                    ? <input type="number" min="0" value={goalDraft}
                        onChange={e=>setGoalDraft(e.target.value)}
                        onKeyDown={e=>{ if(e.key==='Enter'){commitGoal(task.id);} if(e.key==='Escape'){setEditingGoal(null);} }}
                        onBlur={()=>commitGoal(task.id)}
                        autoFocus className="input" style={{width:'100%',fontSize:'18px',fontWeight:700,borderColor:task.color}}/>
                    : <div style={{display:'flex',alignItems:'baseline',justifyContent:'space-between',gap:'12px'}}>
                        <div>
                          <div className="serif" style={{fontSize:'26px',fontWeight:600,lineHeight:1}}>{goal.toLocaleString()}</div>
                          <div className="mono" style={{fontSize:'10px',color:'var(--faint)',textTransform:'uppercase',letterSpacing:'.1em',marginTop:'2px'}}>Goal</div>
                        </div>
                        <div style={{textAlign:'right'}}>
                          <div style={{fontSize:'15px',fontWeight:600,color:'var(--orange)'}}>{Math.max(goal-done,0).toLocaleString()}</div>
                          <div className="mono" style={{fontSize:'10px',color:'var(--faint)',textTransform:'uppercase',letterSpacing:'.1em'}}>Today Pending</div>
                        </div>
                      </div>
                  }
                  <div className="bar" style={{marginTop:'14px'}}><div className="bar-fill" style={{width:`${pct}%`,background:task.color}}/></div>
                </div>
              );
            })}
          </div>

          <div className="card" style={{padding:'18px',marginBottom:'48px'}}>
            <div style={{display:'flex',alignItems:'baseline',justifyContent:'space-between',gap:'12px',marginBottom:'14px',flexWrap:'wrap'}}>
              <div>
                <div className="label" style={{marginBottom:'6px'}}>Weekly Task History</div>
                <div style={{fontSize:'13px',color:'var(--muted)'}}>Last 7 days of completed daily tasks saved in Firebase.</div>
              </div>
              <div className="pill" style={{background:'rgba(251,146,60,.12)',color:'var(--orange)'}}>Today: {totals.totalDone}</div>
            </div>
            <div style={{display:'grid',gridTemplateColumns:'repeat(auto-fit,minmax(145px,1fr))',gap:'10px'}}>
              {weeklySummary.map(day => (
                <div key={day.date} style={{padding:'12px',border:'1px solid var(--line)',borderRadius:'12px',background:day.date===todayKey?'rgba(251,146,60,.08)':'var(--bg)'}}>
                  <div className="mono" style={{fontSize:'10px',color:'var(--muted)',textTransform:'uppercase',letterSpacing:'.08em'}}>{formatHistoryDate(day.date)}</div>
                  <div className="serif" style={{fontSize:'28px',fontWeight:700,lineHeight:1.1,marginTop:'6px',color:day.date===todayKey?'var(--orange)':'var(--text)'}}>{day.total}</div>
                  <div style={{fontSize:'11px',color:'var(--faint)',marginTop:'4px'}}>
                    {day.topMember ? `Top: ${day.topMember[0]} (${day.topMember[1]})` : 'No completed tasks'}
                  </div>
                </div>
              ))}
            </div>
          </div>


          {/* TASK POOL */}
          <div style={{display:'flex',alignItems:'baseline',justifyContent:'space-between',marginBottom:'14px'}}>
            <div className="label">Task Pool</div>
            <div style={{fontSize:'12px',color:'var(--muted)'}}>Drag a task onto a roster card to assign it for today only.</div>
          </div>
          <div className="card" style={{padding:'18px',marginBottom:'48px'}}>
            <div style={{display:'flex',flexWrap:'wrap',gap:'8px'}}>
              {TASK_POOL.map(task => (
                <div key={task.id} draggable
                  onDragStart={handleDragStart(task)}
                  onDragEnd={()=>{ setDraggedTask(null); setHoveredMember(null); }}
                  className="chip"
                  style={{background:`${task.color}15`,borderColor:`${task.color}55`,color:task.color}}>
                  <span style={{opacity:.5,fontSize:'11px'}}>⋮⋮</span> {task.name}
                </div>
              ))}
            </div>
          </div>

          {/* TEAM ROSTER */}
          <div style={{display:'flex',alignItems:'center',justifyContent:'space-between',gap:'12px',marginBottom:'14px',flexWrap:'wrap'}}>
            <div>
              <div className="label">Daily Team Roster</div>
              <div style={{fontSize:'12px',color:'var(--muted)',marginTop:'4px'}}>Roster assignments are now saved separately for each day: {formatHistoryDate(todayKey)}.</div>
            </div>
            <button onClick={resetTodayRoster} className="btn" style={{fontSize:'12px',padding:'7px 10px'}}>↻ Reset Today Roster</button>
          </div>
          <div style={{display:'grid',gridTemplateColumns:'repeat(auto-fill,minmax(260px,1fr))',gap:'14px'}}>
            {TEAM_MEMBERS.map(member => {
              const stats = getMemberStats(member.name);
              const isMe = currentUser === member.name;
              const isHovered = hoveredMember === member.name;
              return (
                <div key={member.name}
                  onDragOver={e=>{e.preventDefault();setHoveredMember(member.name);}}
                  onDragLeave={e=>{if(!e.currentTarget.contains(e.relatedTarget))setHoveredMember(null);}}
                  onDrop={handleDrop(member.name)}
                  className={`member-tile ${isMe?'me':''} ${isHovered?'drag-over':''}`}>
                  <div style={{display:'flex',alignItems:'center',justifyContent:'space-between',marginBottom:'14px'}}>
                    <div style={{display:'flex',alignItems:'center',gap:'10px'}}>
                      <Avatar name={member.name} size={36}/>
                      <div>
                        <div style={{display:'flex',alignItems:'center',gap:'6px'}}>
                          <span style={{fontWeight:600,fontSize:'14px'}}>{member.name}</span>
                          {isMe && <span className="pill" style={{background:'rgba(74,222,128,.15)',color:'var(--green)'}}>You</span>}
                        </div>
                        <div className="mono" style={{fontSize:'10px',color:'var(--faint)',marginTop:'2px'}}>{isMe?'Editing unlocked':'View only'}</div>
                      </div>
                    </div>
                    <div className="serif" style={{fontSize:'24px',fontWeight:600,color:member.accent,lineHeight:1}}>{stats.progress}%</div>
                  </div>
                  <div className="bar" style={{marginBottom:'14px'}}><div className="bar-fill" style={{width:`${stats.progress}%`,background:member.accent}}/></div>
                  <div style={{display:'grid',gridTemplateColumns:'repeat(3,1fr)',gap:'4px',padding:'10px',background:'var(--bg)',border:'1px solid var(--line)',borderRadius:'8px',marginBottom:'14px'}}>
                    {[{v:stats.count,l:'Tasks'},{v:stats.done,l:'Done'},{v:stats.assignedGoal,l:'Goal'}].map(s=>(
                      <div key={s.l} style={{textAlign:'center'}}>
                        <div className="serif" style={{fontSize:'18px',fontWeight:600,lineHeight:1}}>{s.v}</div>
                        <div className="mono" style={{fontSize:'9px',color:'var(--faint)',textTransform:'uppercase',letterSpacing:'.1em',marginTop:'3px'}}>{s.l}</div>
                      </div>
                    ))}
                  </div>
                  <div style={{display:'flex',flexDirection:'column',gap:'8px',minHeight:'120px'}}>
                    {(memberTasks[member.name]||[]).length === 0 ? (
                      <div style={{flex:1,minHeight:'120px',border:`1.5px dashed ${isHovered?member.accent:'var(--line)'}`,borderRadius:'10px',display:'flex',alignItems:'center',justifyContent:'center',textAlign:'center',padding:'16px',background:isHovered?member.accent+'0a':'transparent',transition:'all 180ms'}}>
                        <div>
                          <div className="mono" style={{fontSize:'11px',fontWeight:600,color:isHovered?member.accent:'var(--muted)',textTransform:'uppercase',letterSpacing:'.1em'}}>{isHovered?'Drop here':'Empty roster'}</div>
                          <div style={{fontSize:'11px',color:'var(--faint)',marginTop:'4px'}}>No tasks assigned for today</div>
                        </div>
                      </div>
                    ) : (memberTasks[member.name]||[]).map(item => {
                      const task = TASKS_BY_ID[item.taskId];
                      if(!task) return null;
                      const locked = !isMe;
                      return (
                        <div key={item.id} style={{padding:'10px',background:'var(--bg)',border:'1px solid var(--line)',borderRadius:'10px'}}>
                          <div style={{display:'flex',alignItems:'center',justifyContent:'space-between',gap:'6px',marginBottom:'8px'}}>
                            <div style={{minWidth:0}}>
                              <div style={{fontSize:'13px',fontWeight:600,color:task.color,whiteSpace:'nowrap',overflow:'hidden',textOverflow:'ellipsis'}}>{task.name}</div>
                              <div className="mono" style={{fontSize:'10px',color:'var(--faint)',marginTop:'2px'}}>Goal: {item.goalNumber||0}</div>
                            </div>
                            {isMe && <button onClick={()=>removeTask(member.name,item.id)} style={{width:'22px',height:'22px',background:'none',border:'none',color:'var(--red)',cursor:'pointer',fontSize:'14px',borderRadius:'50%'}} onMouseOver={e=>e.currentTarget.style.background='rgba(248,113,113,.1)'} onMouseOut={e=>e.currentTarget.style.background='none'}>×</button>}
                          </div>
                          <div style={{display:'flex',alignItems:'center',gap:'8px'}}>
                            <DoneInput committedValue={getDailyDone(member.name, item.taskId)} max={item.goalNumber||9999} color={task.color} locked={locked} onCommit={val => updateDone(member.name, item.id, item.taskId, val)} />
                            <span className="mono" style={{fontSize:'10px',color:'var(--faint)',textTransform:'uppercase',letterSpacing:'.1em',flexShrink:0}}>Today</span>
                          </div>
                        </div>
                      );
                    })}
                  </div>
                </div>
              );
            })}
          </div>
        </div>
        {assignPending && <AssignModal task={assignPending.task} memberName={assignPending.memberName} onConfirm={confirmAssign} onCancel={()=>setAssignPending(null)}/>}
      </div>
    );
  }

  /* ═══════════════════════════════════════════════════════════
     MONTH END — Tracker Column
  ═══════════════════════════════════════════════════════════ */
  function TrackerColumn({ title, accentColor, students, folders, currentUser, onMarkCompleted, trackerKey }) {
    const [search, setSearch] = useState('');
    const filtered = students.filter(s => {
      const q = search.toLowerCase();
      return (s.name || '').toLowerCase().includes(q) || (s.number || '').toString().toLowerCase().includes(q);
    });
    const done = filtered.filter(s=>s[`${trackerKey}_completed`]).length;
    const statusFor = s => {
      if(s[`${trackerKey}_completed`]) return 'Completed';
      const fk = makeFolderKey(s);
      return folders[fk] ? 'Files added' : 'Pending';
    };
    const statusColor = st => ({Completed:'var(--green)','Files added':'var(--orange)','Pending':'var(--faint)'})[st] || 'var(--faint)';

    return (
      <div className="card" style={{display:'flex',flexDirection:'column',height:'100%',minHeight:0}}>
        <div style={{padding:'14px 14px 10px',borderBottom:'1px solid var(--line)',flexShrink:0}}>
          <div className="label" style={{color:accentColor,marginBottom:'8px'}}>{title}</div>
          <input value={search} onChange={e=>setSearch(e.target.value)} placeholder="Search name or number…" className="input" style={{width:'100%',fontSize:'12px'}}/>
          <div className="mono" style={{fontSize:'10px',marginTop:'8px',color:'var(--faint)'}}>{done}/{filtered.length} done</div>
        </div>
        <div className="scroll" style={{flex:1,overflowY:'auto',padding:'10px',display:'flex',flexDirection:'column',gap:'6px'}}>
          {filtered.length === 0 && <div className="mono" style={{fontSize:'11px',padding:'14px',textAlign:'center',color:'var(--faint)'}}>Import Excel first.</div>}
          {filtered.map(s => {
            const isDone = !!s[`${trackerKey}_completed`];
            const completedBy = s[`${trackerKey}_completedBy`] || '';
            const st = statusFor(s);
            const primary = s.name && s.name.trim() ? s.name : 'Name missing';
            return (
              <div key={s.id} style={{padding:'10px 12px',border:'1px solid var(--line)',borderRadius:'8px',background:'var(--bg)'}}>
                <div style={{fontSize:'13px',fontWeight:600,color:'var(--text)',whiteSpace:'nowrap',overflow:'hidden',textOverflow:'ellipsis'}}>{primary}</div>
                {s.number && <div className="mono" style={{fontSize:'10px',color:'var(--faint)',marginTop:'2px'}}>{s.number}</div>}
                <div style={{display:'flex',alignItems:'center',justifyContent:'space-between',gap:'6px',marginTop:'8px'}}>
                  <span className="pill" style={{background:statusColor(st)+'22',color:statusColor(st)}}>{st}</span>
                  {!isDone
                    ? <button onClick={()=>onMarkCompleted(s.id, trackerKey)} className="btn" style={{padding:'2px 10px',fontSize:'10px',color:'var(--green)',borderColor:'var(--green)'}}>Mark Done ✓</button>
                    : <span className="mono" style={{fontSize:'10px',color:'var(--green)'}}>✓ {completedBy}</span>
                  }
                </div>
              </div>
            );
          })}
        </div>
      </div>
    );
  }

  /* ═══════════════════════════════════════════════════════════
     MONTH END MODE — MAIN
  ═══════════════════════════════════════════════════════════ */
  function MonthEndMode({ currentUser, onSwitchUser, onNavigate, theme, onToggleTheme }) {
    const [students, setStudents] = useState([]);
    // SPAR: staging files before moving to GAC/Overpayment
    const [sparFiles, setSparFiles] = useState([]);           // {file, preview, type:'image'|'pdf', name}
    const [sparStudent, setSparStudent] = useState(null);
    const [sparSearch, setSparSearch] = useState('');
    const [sparDragOver, setSparDragOver] = useState(false);

    // GAC / Overpayment packages: folderKey -> { studentName, studentNumber, sparFiles:[], extraFiles:[], purpose }
    const [gacPackages, setGacPackages] = useState({});
    const [opPackages, setOpPackages] = useState({});

    // Active folder tab
    const [activeTab, setActiveTab] = useState('spar');
    // Currently viewing/editing package key
    const [activeGacKey, setActiveGacKey] = useState(null);
    const [activeOpKey, setActiveOpKey] = useState(null);

    // Excel mapping
    const [showMapping, setShowMapping] = useState(false);
    const [rawHeaders, setRawHeaders] = useState([]);
    const [rawRows, setRawRows] = useState([]);
    const [colMap, setColMap] = useState({name:'',num:''});

    const [pdfGenerating, setPdfGenerating] = useState(false);

    const sparFileRef = useRef(null);
    const excelRef = useRef(null);

    useEffect(() => {
      document.body.className = 'rage-mode';
      return () => { document.body.className = ''; };
    }, []);

    useEffect(() => {
      if(!isFirebaseReady()) return;
      const u1 = db.collection('monthend_students').orderBy('importedAt','asc').onSnapshot(snap=>{
        setStudents(snap.docs.map(d=>({id:d.id,...d.data()})));
      }, console.warn);
      return () => { u1(); };
    }, []);

    // Paste handler
    const handlePaste = useCallback(async e => {
      if (activeTab !== 'spar') return;
      const items = Array.from(e.clipboardData?.items || []);
      const imgs = items.filter(i => i.type.startsWith('image/')).map(i => i.getAsFile()).filter(Boolean);
      for (const f of imgs) {
        try {
          const dataUrl = await fileToDataUrl(f);
          setSparFiles(p => [...p, { file: f, preview: dataUrl, type: 'image', name: f.name || 'pasted-image.png' }]);
        } catch(err) { console.warn('Paste read failed', err); }
      }
    }, [activeTab]);
    useEffect(() => { window.addEventListener('paste', handlePaste); return () => window.removeEventListener('paste', handlePaste); }, [handlePaste]);

    // Add files to SPAR (images + PDFs)
    const addSparFiles = async files => {
      const arr = Array.from(files || []);
      for (const f of arr) {
        if (f.type.startsWith('image/')) {
          try {
            const dataUrl = await fileToDataUrl(f);
            setSparFiles(p => [...p, { file: f, preview: dataUrl, type: 'image', name: f.name }]);
          } catch(err) { console.warn('Image read failed', err); }
        } else if (f.type === 'application/pdf' || /\.pdf$/i.test(f.name)) {
          setSparFiles(p => [...p, { file: f, preview: null, type: 'pdf', name: f.name }]);
        }
      }
    };

    // Excel handling — smart header detection for clean Excel files where headers start on row 2+.
    const normalizeHeader = (h='') => String(h || '').replace(/\s+/g,' ').trim();
    const headerScore = row => {
      const cells = (row || []).map(normalizeHeader);
      const joined = cells.join(' | ').toLowerCase();
      let score = 0;
      if (/student\s*(#|number|no\.?|id)/i.test(joined)) score += 4;
      if (/first\s*name/i.test(joined)) score += 3;
      if (/last\s*name/i.test(joined)) score += 3;
      if (/student\s*name|full\s*name/i.test(joined)) score += 3;
      if (/program/i.test(joined)) score += 1;
      if (/start\s*date|status|rep|assigned\s*to/i.test(joined)) score += 1;
      return score;
    };

    const detectHeaderRowIndex = data => {
      let bestIdx = 0;
      let bestScore = -1;
      data.slice(0, 30).forEach((row, idx) => {
        const score = headerScore(row);
        if (score > bestScore) { bestScore = score; bestIdx = idx; }
      });
      return bestIdx;
    };

    const handleExcelFile = file => {
      if(!file) return;
      const reader = new FileReader();
      reader.onload = e => {
        try{
          const wb = XLSX.read(e.target.result,{type:'binary'});
          const ws = wb.Sheets[wb.SheetNames[0]];
          const data = XLSX.utils.sheet_to_json(ws,{header:1, defval:''});
          if(!data.length) return;

          const headerRowIdx = detectHeaderRowIndex(data);
          const headers = (data[headerRowIdx] || []).map(normalizeHeader);
          const rows = data.slice(headerRowIdx + 1).filter(r => (r || []).some(c => String(c || '').trim() !== ''));

          setRawHeaders(headers);
          setRawRows(rows);

          // Flexible auto-detection. In the Year 2 Application Tracker, this picks:
          // Student # = number, First Name + Last Name = full student name.
          const firstNameIdx = headers.findIndex(h => /^first\s*name$/i.test(h));
          const fullNameIdx = headers.findIndex(h => /^(student\s*(full\s*)?name|full\s*name|student\s*name|name)$/i.test(h));
          const looseNameIdx = headers.findIndex(h => /name/i.test(h) && !/^last\s*name$/i.test(h));
          const nameIdx = fullNameIdx >= 0 ? fullNameIdx : (firstNameIdx >= 0 ? firstNameIdx : looseNameIdx);

          const numberIdx = headers.findIndex(h => /^(student\s*(#|number|no\.?|id)|student#|student id|student number|stud\s*id|id|number)$/i.test(h));
          const looseNumberIdx = numberIdx >= 0 ? numberIdx : headers.findIndex(h => /(student.*#|student.*num|student.*id|\bnum\b|\bid\b|#)/i.test(h));

          setColMap({
            name: (nameIdx >= 0 ? nameIdx : '').toString(),
            num: (looseNumberIdx >= 0 ? looseNumberIdx : '').toString()
          });
          setShowMapping(true);
        }catch(err){ alert('Cannot read file: '+err.message); }
      };
      reader.readAsBinaryString(file);
    };

    const confirmImport = async () => {
      if (colMap.name === '') { alert('Please select the name column first.'); return; }

      const nameIdx = Number(colMap.name);
      const numIdx = colMap.num === '' ? -1 : Number(colMap.num);
      const selectedHeader = (rawHeaders[nameIdx] || '').toLowerCase();

      const lastNameIdx = rawHeaders.findIndex(h => /^last\s*name$/i.test(String(h || '').trim()));
      const firstNameIdx = rawHeaders.findIndex(h => /^first\s*name$/i.test(String(h || '').trim()));
      const useFirstLast = /first\s*name/i.test(selectedHeader) && lastNameIdx >= 0;

      const imported = rawRows.map((row, idx) => {
        const firstPart = String(row[nameIdx] || '').trim();
        const lastPart = useFirstLast ? String(row[lastNameIdx] || '').trim() : '';
        const combinedName = useFirstLast ? `${firstPart} ${lastPart}`.trim() : firstPart;
        const studentNumber = numIdx >= 0 ? String(row[numIdx] || '').trim() : '';
        return {
          id: studentNumber || `student_${Date.now()}_${idx}`,
          name: combinedName,
          number: studentNumber,
          firstName: firstNameIdx >= 0 ? String(row[firstNameIdx] || '').trim() : (useFirstLast ? firstPart : ''),
          lastName: lastNameIdx >= 0 ? String(row[lastNameIdx] || '').trim() : '',
          importedAt: Date.now() + idx
        };
      }).filter(s => (s.name && s.name.trim()) || (s.number && s.number.trim()));

      if (!imported.length) { alert('No valid student rows found. Please check the selected columns.'); return; }

      if (isFirebaseReady()) {
        try {
          const oldSnap = await db.collection('monthend_students').get();
          let batch = db.batch();
          let count = 0;
          for (const doc of oldSnap.docs) {
            batch.delete(doc.ref);
            count++;
            if (count % 450 === 0) { await batch.commit(); batch = db.batch(); }
          }
          for (const st of imported) {
            const docId = String(st.id || localId('student')).replace(/[\/#[\]?]/g, '_');
            batch.set(db.collection('monthend_students').doc(docId), st, { merge:false });
            count++;
            if (count % 450 === 0) { await batch.commit(); batch = db.batch(); }
          }
          await batch.commit();
        } catch(e) {
          console.warn('Firebase import failed. Using local roster for this session.', e);
          setStudents(imported);
        }
      } else {
        setStudents(imported);
      }

      setShowMapping(false);
      setRawHeaders([]);
      setRawRows([]);
      resetSpar();
      setGacPackages({});
      setOpPackages({});
      setActiveGacKey(null);
      setActiveOpKey(null);
      if (excelRef.current) excelRef.current.value = '';
    };

    // Move SPAR files to GAC or Overpayment
    const moveToSection = (section) => {
      if (!sparStudent) { alert('Select a student first.'); return; }
      if (!sparFiles.length) { alert('Add at least one file to SPAR first.'); return; }
      const student = students.find(s => s.id === sparStudent);
      if (!student) return;
      const fk = makeFolderKey(student);
      const pkg = {
        studentName: student.name || 'Name missing',
        studentNumber: student.number || '',
        studentId: student.id,
        folderKey: fk,
        purpose: section === 'gac' ? 'GAC' : 'Overpayment',
        sparFiles: [...sparFiles],
        extraFiles: [],
        createdAt: Date.now(),
      };
      if (section === 'gac') {
        setGacPackages(p => {
          const existing = p[fk];
          if (existing) {
            return { ...p, [fk]: { ...existing, sparFiles: [...existing.sparFiles, ...sparFiles] } };
          }
          return { ...p, [fk]: pkg };
        });
        setActiveGacKey(fk);
      } else {
        setOpPackages(p => {
          const existing = p[fk];
          if (existing) {
            return { ...p, [fk]: { ...existing, sparFiles: [...existing.sparFiles, ...sparFiles] } };
          }
          return { ...p, [fk]: pkg };
        });
        setActiveOpKey(fk);
      }
      // Clear SPAR
      setSparFiles([]);
      setSparStudent(null);
      setSparSearch('');
      setActiveTab(section === 'gac' ? 'gac' : 'overpayment');
    };

    // Add extra files to a GAC/Overpayment package
    const addExtraFiles = async (fk, section, files) => {
      const arr = Array.from(files || []);
      const newEntries = [];
      for (const f of arr) {
        if (f.type.startsWith('image/')) {
          try {
            const dataUrl = await fileToDataUrl(f);
            newEntries.push({ file: f, preview: dataUrl, type: 'image', name: f.name });
          } catch(err) { console.warn(err); }
        } else if (f.type === 'application/pdf' || /\.pdf$/i.test(f.name)) {
          newEntries.push({ file: f, preview: null, type: 'pdf', name: f.name });
        }
      }
      if (!newEntries.length) return;
      const setter = section === 'gac' ? setGacPackages : setOpPackages;
      setter(p => {
        const pkg = p[fk];
        if (!pkg) return p;
        return { ...p, [fk]: { ...pkg, extraFiles: [...pkg.extraFiles, ...newEntries] } };
      });
    };

    // Remove a file from a package
    const removeFileFromPackage = (fk, section, source, idx) => {
      const setter = section === 'gac' ? setGacPackages : setOpPackages;
      setter(p => {
        const pkg = p[fk];
        if (!pkg) return p;
        if (source === 'spar') {
          return { ...p, [fk]: { ...pkg, sparFiles: pkg.sparFiles.filter((_,i) => i !== idx) } };
        } else {
          return { ...p, [fk]: { ...pkg, extraFiles: pkg.extraFiles.filter((_,i) => i !== idx) } };
        }
      });
    };

    // Download merged PDF package
    const downloadPackage = async (fk, section) => {
      const packages = section === 'gac' ? gacPackages : opPackages;
      const pkg = packages[fk];
      if (!pkg) return;

      const allFiles = [...pkg.sparFiles, ...pkg.extraFiles];
      if (!allFiles.length) { alert('No files in this package.'); return; }

      setPdfGenerating(true);
      try {
        const pdfBlobs = [];

        // Collect images first (SPAR files, then extras)
        const images = allFiles.filter(f => f.type === 'image');
        if (images.length) {
          const imgSrcs = images.map(f => f.preview);
          const imgPdf = await imagesToPdfBlob(imgSrcs);
          pdfBlobs.push(imgPdf);
        }

        // Collect PDFs
        const pdfs = allFiles.filter(f => f.type === 'pdf');
        for (const f of pdfs) {
          pdfBlobs.push(f.file);
        }

        if (!pdfBlobs.length) {
          alert('No valid files to merge.');
          setPdfGenerating(false);
          return;
        }

        const finalBlob = pdfBlobs.length === 1 ? pdfBlobs[0] : await mergePdfBlobs(pdfBlobs);
        // Handle case where single "blob" is actually a File not a Blob
        let downloadBlob = finalBlob;
        if (!(finalBlob instanceof Blob)) {
          downloadBlob = new Blob([await finalBlob.arrayBuffer()], {type:'application/pdf'});
        }

        const fname = buildPdfFilename(pkg.studentNumber, pkg.studentName, pkg.purpose);
        saveBlob(downloadBlob, fname);
      } catch(e) {
        console.error(e);
        alert('Error generating PDF: ' + e.message);
      }
      setPdfGenerating(false);
    };

    // Reset functions
    const resetSpar = () => {
      setSparFiles([]);
      setSparStudent(null);
      setSparSearch('');
    };

    const resetGacPackage = (fk) => {
      setGacPackages(p => { const n = {...p}; delete n[fk]; return n; });
      if (activeGacKey === fk) setActiveGacKey(null);
    };

    const resetOpPackage = (fk) => {
      setOpPackages(p => { const n = {...p}; delete n[fk]; return n; });
      if (activeOpKey === fk) setActiveOpKey(null);
    };

    // Reset the imported Excel roster so a fresh file can be uploaded cleanly.
    const resetExcelImport = async () => {
      if (!students.length && !rawRows.length && !showMapping) { alert('No Excel roster is currently loaded.'); return; }
      const ok = confirm('Reset the imported Excel roster? This will clear loaded students, column mapping, SPAR files, GAC/Overpayment packages, and tracker completion marks so you can upload a new Excel file.');
      if (!ok) return;

      setShowMapping(false);
      setRawHeaders([]);
      setRawRows([]);
      setColMap({name:'',num:''});
      resetSpar();
      setGacPackages({});
      setOpPackages({});
      setActiveGacKey(null);
      setActiveOpKey(null);
      if (excelRef.current) excelRef.current.value = '';

      if (isFirebaseReady()) {
        try {
          const snap = await db.collection('monthend_students').get();
          let batch = db.batch();
          let count = 0;
          for (const doc of snap.docs) {
            batch.delete(doc.ref);
            count++;
            if (count % 450 === 0) { await batch.commit(); batch = db.batch(); }
          }
          await batch.commit();
        } catch(e) { console.warn('Could not clear Firebase monthend_students:', e); }
      } else {
        setStudents([]);
      }
    };

    // Reset the current Month End document workspace without touching imported students or tracker completion data.
    const resetCurrentDocument = () => {
      if (activeTab === 'spar') {
        if (!sparStudent && !sparFiles.length) { alert('SPAR is already empty.'); return; }
        if (confirm('Reset the current SPAR document? This will clear the selected student and staged files only.')) resetSpar();
        return;
      }

      const sectionLabel = activeTab === 'gac' ? 'GAC' : 'Overpayment';
      const activeKey = activeTab === 'gac' ? activeGacKey : activeOpKey;
      const packages = activeTab === 'gac' ? gacPackages : opPackages;
      const resetOne = activeTab === 'gac' ? resetGacPackage : resetOpPackage;
      const packageKeys = Object.keys(packages || {});

      if (activeKey && packages[activeKey]) {
        const pkg = packages[activeKey];
        if (confirm(`Reset ${pkg.studentName}'s ${sectionLabel} document package? This will remove the package files only.`)) resetOne(activeKey);
        return;
      }

      if (packageKeys.length === 1) {
        const onlyKey = packageKeys[0];
        const pkg = packages[onlyKey];
        if (confirm(`Reset ${pkg.studentName}'s ${sectionLabel} document package? This will remove the package files only.`)) resetOne(onlyKey);
        return;
      }

      if (packageKeys.length > 1) {
        alert(`Open one ${sectionLabel} package first, then use Reset Document. This protects other students' packages from being cleared by mistake.`);
        return;
      }

      alert(`No ${sectionLabel} document package to reset.`);
    };

    const markCompleted = async (studentId, trackerKey) => {
      const now = new Date().toLocaleString();
      const data = { [`${trackerKey}_completed`]:true, [`${trackerKey}_completedBy`]:currentUser, [`${trackerKey}_completedTime`]:now };
      if(isFirebaseReady()) await db.collection('monthend_students').doc(studentId).update(data).catch(console.warn);
      else setStudents(p => p.map(s => s.id === studentId ? {...s,...data} : s));
    };

    const exportExcel = () => {
      const rows = students.map(s => {
        const fk = makeFolderKey(s);
        return {
          'Student Name':s.name||'', 'Student Number':s.number||'',
          'GAC Package': gacPackages[fk] ? 'Yes' : 'No',
          'Overpayment Package': opPackages[fk] ? 'Yes' : 'No',
          'GAC Completed':s.gac_completed?'Yes':'No', 'GAC By':s.gac_completedBy||'',
          'OP Completed':s.overpayment_completed?'Yes':'No', 'OP By':s.overpayment_completedBy||'',
        };
      });
      const ws = XLSX.utils.json_to_sheet(rows);
      const wb = XLSX.utils.book_new();
      XLSX.utils.book_append_sheet(wb, ws, 'Month End');
      XLSX.writeFile(wb, 'Month_End_Tracker.xlsx');
    };

    const dropdownStudents = students.filter(s =>
      (s.name||'').toLowerCase().includes(sparSearch.toLowerCase()) ||
      (s.number||'').toString().toLowerCase().includes(sparSearch.toLowerCase())
    );

    // Counts
    const gacCount = Object.keys(gacPackages).length;
    const opCount = Object.keys(opPackages).length;

    // All folders for tracker
    const allFolders = {...gacPackages, ...opPackages};

    return (
      <div style={{minHeight:'100vh',background:'var(--bg)'}}>
        <div className="topbar">
          <div style={{display:'flex',alignItems:'center',gap:'14px'}}>
            <span className="rage-font" style={{fontSize:'22px',color:'#ff6030',letterSpacing:'.06em'}}>MONTH END MODE</span>
            <span className="mono" style={{fontSize:'10px',color:'var(--muted)',textTransform:'uppercase',letterSpacing:'.2em'}}>High Pressure</span>
          </div>
          <div style={{display:'flex',alignItems:'center',gap:'10px',flexWrap:'wrap'}}>
            <span style={{fontSize:'12px',color:'var(--muted)'}}>{theme==='dark'?'☾':'☀'}</span>
            <ThemeToggle theme={theme} onToggle={onToggleTheme}/>
            <div className="seg">
              <button className="seg-btn" onClick={()=>onNavigate('war')} style={{color:'var(--muted)'}}>War Room</button>
              <button className="seg-btn" onClick={()=>onNavigate('workeasy')} style={{color:'var(--muted)'}}>WorkEasy Hub</button>
              <button className="seg-btn on" style={{background:'#c00'}}>Month End</button>
            </div>
            <button onClick={exportExcel} className="btn" style={{background:'#c00',color:'#fff',border:'none',fontSize:'11px'}}>⬇ Export</button>
            <div style={{display:'flex',alignItems:'center',gap:'8px',padding:'4px 10px 4px 4px',background:'var(--bg-2)',border:'1px solid var(--line)',borderRadius:'24px'}}>
              <Avatar name={currentUser} size={26}/>
              <span style={{fontSize:'13px',fontWeight:500}}>{currentUser}</span>
            </div>
            <button onClick={onSwitchUser} className="btn-link" title="Switch user">Switch</button>
          </div>
        </div>

        <div style={{display:'grid',gridTemplateColumns:'1fr 540px',gap:'20px',padding:'24px 32px',maxWidth:'1600px',margin:'0 auto',height:'calc(100vh - 60px)'}}>

          {/* LEFT: Main workflow */}
          <div className="scroll" style={{overflowY:'auto',display:'flex',flexDirection:'column',gap:'16px'}}>

            <h1 className="serif" style={{fontSize:'36px',fontWeight:600,lineHeight:1.05,color:'#ff6030'}}>Crunch time.</h1>
            <p className="mono" style={{color:'var(--muted)',fontSize:'12px',marginTop:'-12px'}}>Import → SPAR → Move → Download.</p>

            {/* Excel import */}
            <div className="card" style={{padding:'18px'}}>
              <div style={{display:'flex',alignItems:'center',justifyContent:'space-between',gap:'10px',marginBottom:'10px',flexWrap:'wrap'}}>
                <div className="label" style={{color:'#ff8060'}}>Excel Import</div>
                <div style={{display:'flex',gap:'8px',flexWrap:'wrap'}}>
                  <button onClick={()=>excelRef.current?.click()} className="btn" style={{background:'#c00',color:'#fff',border:'none',fontSize:'11px'}}>Upload .xlsx / .csv</button>
                  <button onClick={resetExcelImport} className="btn" style={{color:'var(--red)',borderColor:'var(--red)',fontSize:'11px'}}>↻ Reset Excel</button>
                </div>
                <input ref={excelRef} type="file" accept=".xlsx,.xls,.csv" style={{display:'none'}} onChange={e=>handleExcelFile(e.target.files[0])}/>
              </div>
              <p style={{fontSize:'12px',color:'var(--muted)'}}>
                Upload your student roster.
                {students.length > 0 && <span style={{color:'var(--green)',marginLeft:'6px'}}>{students.length} students loaded.</span>}
              </p>
              {showMapping && (
                <div style={{marginTop:'14px',padding:'14px',border:'1px solid var(--line-2)',borderRadius:'10px',background:'var(--bg)'}}>
                  <div className="label" style={{color:'#ff8060',marginBottom:'12px'}}>Map columns</div>
                  <div style={{display:'grid',gridTemplateColumns:'1fr 1fr',gap:'10px',marginBottom:'10px'}}>
                    {[{k:'name',l:'Name column (First Name is okay)'},{k:'num',l:'Student Number'}].map(f => (
                      <div key={f.k}>
                        <div className="mono" style={{fontSize:'10px',color:'var(--muted)',marginBottom:'4px'}}>{f.l}</div>
                        <select value={colMap[f.k]} onChange={e=>setColMap(p=>({...p,[f.k]:e.target.value}))} className="input" style={{width:'100%'}}>
                          <option value="">— {f.k==='num'?'none':'select'} —</option>
                          {rawHeaders.map((h,i)=><option key={i} value={i}>{h||`Col ${i+1}`}</option>)}
                        </select>
                      </div>
                    ))}
                  </div>
                  <div className="scroll" style={{overflowX:'auto',marginBottom:'10px'}}>
                    <table style={{fontSize:'10px',color:'var(--muted)',width:'100%'}}>
                      <thead><tr>{rawHeaders.map((h,i)=><th key={i} style={{textAlign:'left',padding:'4px 8px',borderBottom:'1px solid var(--line)'}}>{h}</th>)}</tr></thead>
                      <tbody>{rawRows.slice(0,3).map((r,i)=><tr key={i}>{rawHeaders.map((_,j)=><td key={j} style={{padding:'4px 8px'}}>{r[j]||''}</td>)}</tr>)}</tbody>
                    </table>
                  </div>
                  <div style={{display:'flex',gap:'8px'}}>
                    <button onClick={()=>setShowMapping(false)} className="btn">Cancel</button>
                    <button onClick={confirmImport} disabled={colMap.name===''} className="btn" style={{background:'#c00',color:'#fff',border:'none',opacity:(colMap.name==='' ? .5 : 1)}}>Import {rawRows.length} students</button>
                  </div>
                </div>
              )}
            </div>

            {/* ═══ FOLDER TABS ═══ */}
            <div>
              <div style={{display:'flex',gap:'4px',paddingLeft:'8px'}}>
                <button className={`folder-tab ${activeTab==='spar'?'active':''}`} onClick={()=>setActiveTab('spar')}
                  style={activeTab==='spar'?{color:'#ff8060',borderColor:'rgba(255,128,96,.4)'}:{}}>
                  📋 SPAR {sparFiles.length > 0 && <span className="pill" style={{background:'rgba(255,128,96,.15)',color:'#ff8060',marginLeft:'6px'}}>{sparFiles.length}</span>}
                </button>
                <button className={`folder-tab ${activeTab==='gac'?'active':''}`} onClick={()=>setActiveTab('gac')}
                  style={activeTab==='gac'?{color:'#34d399',borderColor:'rgba(52,211,153,.4)'}:{}}>
                  📁 GAC {gacCount > 0 && <span className="pill" style={{background:'rgba(52,211,153,.15)',color:'#34d399',marginLeft:'6px'}}>{gacCount}</span>}
                </button>
                <button className={`folder-tab ${activeTab==='overpayment'?'active':''}`} onClick={()=>setActiveTab('overpayment')}
                  style={activeTab==='overpayment'?{color:'#fb7185',borderColor:'rgba(251,113,133,.4)'}:{}}>
                  📁 Overpayment {opCount > 0 && <span className="pill" style={{background:'rgba(251,113,133,.15)',color:'#fb7185',marginLeft:'6px'}}>{opCount}</span>}
                </button>
              </div>

              <div className="card" style={{borderTopLeftRadius:0,padding:'20px'}}>

                {/* ═══ SPAR TAB ═══ */}
                {activeTab === 'spar' && (
                  <div>
                    <div className="label" style={{color:'#ff8060',marginBottom:'14px'}}>SPAR — Intake / Staging</div>

                    {/* Student selector */}
                    <div style={{position:'relative',marginBottom:'14px'}}>
                      <div className="mono" style={{fontSize:'10px',color:'var(--muted)',marginBottom:'4px'}}>Select Student (name or number)</div>
                      <input value={sparSearch} onChange={e=>{setSparSearch(e.target.value);setSparStudent(null);}}
                        placeholder="Type name or number…" className="input" style={{width:'100%'}}/>
                      {sparSearch && !sparStudent && dropdownStudents.length > 0 && (
                        <div className="scroll" style={{position:'absolute',zIndex:30,width:'100%',marginTop:'2px',background:'var(--bg-2)',border:'1px solid var(--line-2)',borderRadius:'8px',maxHeight:'180px',overflowY:'auto'}}>
                          {dropdownStudents.map(s => (
                            <button key={s.id} onClick={()=>{setSparStudent(s.id);setSparSearch(`${s.name||'Name missing'}${s.number?` — ${s.number}`:''}`);}}
                              style={{width:'100%',textAlign:'left',padding:'8px 12px',fontSize:'12px',background:'none',border:'none',color:'var(--text)',cursor:'pointer'}}
                              onMouseOver={e=>e.currentTarget.style.background='var(--bg-3)'} onMouseOut={e=>e.currentTarget.style.background='none'}>
                              <span style={{fontWeight:600}}>{s.name || 'Name missing'}</span>
                              {s.number && <span style={{color:'var(--muted)',marginLeft:'6px',fontSize:'11px'}}>#{s.number}</span>}
                            </button>
                          ))}
                        </div>
                      )}
                      {!students.length && <p className="mono" style={{fontSize:'10px',color:'var(--faint)',marginTop:'4px'}}>Import Excel first.</p>}
                    </div>

                    {/* Drop zone for images AND PDFs */}
                    <div className={`dropzone ${sparDragOver?'over':''}`}
                      onDragOver={e=>{e.preventDefault();setSparDragOver(true);}}
                      onDragLeave={()=>setSparDragOver(false)}
                      onDrop={e=>{e.preventDefault();setSparDragOver(false);addSparFiles(e.dataTransfer.files);}}
                      onClick={()=>sparFileRef.current?.click()}
                      style={{padding:'24px',textAlign:'center',cursor:'pointer',marginBottom:'14px'}}>
                      <div style={{fontSize:'24px',marginBottom:'4px'}}>📋</div>
                      <div className="mono" style={{fontSize:'11px',fontWeight:600,color:'#ff8060',textTransform:'uppercase',letterSpacing:'.1em'}}>Drop screenshots or PDFs here</div>
                      <div style={{fontSize:'11px',color:'var(--muted)',marginTop:'4px'}}>or click to browse · Ctrl+V to paste images</div>
                      <input ref={sparFileRef} type="file" accept="image/*,application/pdf,.pdf" multiple style={{display:'none'}} onChange={e=>addSparFiles(e.target.files)}/>
                    </div>

                    {/* File list */}
                    {sparFiles.length > 0 && (
                      <div style={{marginBottom:'14px'}}>
                        <div className="mono" style={{fontSize:'10px',color:'var(--muted)',marginBottom:'6px'}}>{sparFiles.length} file(s) staged</div>
                        <div style={{display:'grid',gridTemplateColumns:'repeat(auto-fill,minmax(90px,1fr))',gap:'6px'}}>
                          {sparFiles.map((f,i) => (
                            <div key={i} style={{position:'relative',aspectRatio:f.type==='image'?'4/3':'auto',borderRadius:'6px',overflow:'hidden',background:'var(--bg)',border:'1px solid var(--line)',display:'flex',alignItems:'center',justifyContent:'center',padding:f.type==='pdf'?'10px 6px':0}}>
                              {f.type === 'image' ? (
                                <img src={f.preview} alt="" style={{width:'100%',height:'100%',objectFit:'cover'}}/>
                              ) : (
                                <div style={{textAlign:'center'}}>
                                  <div style={{fontSize:'20px'}}>📄</div>
                                  <div className="mono" style={{fontSize:'8px',color:'var(--muted)',marginTop:'2px',wordBreak:'break-all'}}>{f.name?.slice(0,20)}</div>
                                </div>
                              )}
                              <button onClick={()=>setSparFiles(p=>p.filter((_,j)=>j!==i))} style={{position:'absolute',top:'2px',right:'2px',width:'16px',height:'16px',borderRadius:'50%',background:'#c00',color:'#fff',fontSize:'10px',border:'none',cursor:'pointer'}}>×</button>
                            </div>
                          ))}
                        </div>
                      </div>
                    )}

                    {/* Action buttons */}
                    <div style={{display:'flex',gap:'8px',flexWrap:'wrap'}}>
                      <button onClick={()=>moveToSection('gac')} disabled={!sparStudent || !sparFiles.length}
                        className="btn" style={{flex:1,justifyContent:'center',background:'#166534',color:'#fff',border:'none',padding:'10px',opacity:(!sparStudent||!sparFiles.length)?.4:1,minWidth:'140px'}}>
                        → Move to GAC
                      </button>
                      <button onClick={()=>moveToSection('op')} disabled={!sparStudent || !sparFiles.length}
                        className="btn" style={{flex:1,justifyContent:'center',background:'#9f1239',color:'#fff',border:'none',padding:'10px',opacity:(!sparStudent||!sparFiles.length)?.4:1,minWidth:'140px'}}>
                        → Move to Overpayment
                      </button>
                      <button onClick={resetSpar} disabled={!sparStudent && !sparFiles.length}
                        className="btn" style={{justifyContent:'center',padding:'10px 14px',opacity:(!sparStudent && !sparFiles.length)?.4:1}}
                        title="Clear SPAR files and selected student only">
                        ↻ Reset SPAR
                      </button>
                    </div>
                  </div>
                )}

                {/* ═══ GAC TAB ═══ */}
                {activeTab === 'gac' && (
                  <PackageSection
                    title="GAC Packages"
                    accentColor="#34d399"
                    packages={gacPackages}
                    section="gac"
                    activeKey={activeGacKey}
                    setActiveKey={setActiveGacKey}
                    onAddFiles={addExtraFiles}
                    onRemoveFile={removeFileFromPackage}
                    onDownload={downloadPackage}
                    onReset={resetGacPackage}
                    pdfGenerating={pdfGenerating}
                  />
                )}

                {/* ═══ OVERPAYMENT TAB ═══ */}
                {activeTab === 'overpayment' && (
                  <PackageSection
                    title="Overpayment Packages"
                    accentColor="#fb7185"
                    packages={opPackages}
                    section="overpayment"
                    activeKey={activeOpKey}
                    setActiveKey={setActiveOpKey}
                    onAddFiles={addExtraFiles}
                    onRemoveFile={removeFileFromPackage}
                    onDownload={downloadPackage}
                    onReset={resetOpPackage}
                    pdfGenerating={pdfGenerating}
                  />
                )}
              </div>
            </div>
          </div>

          {/* RIGHT: trackers */}
          <div className="tracker-wrap" style={{height:'100%',minHeight:0}}>
            <TrackerColumn title="GAC Tracker" accentColor="#34d399" students={students} folders={gacPackages} currentUser={currentUser} onMarkCompleted={markCompleted} trackerKey="gac"/>
            <TrackerColumn title="Overpayment Tracker" accentColor="#fb7185" students={students} folders={opPackages} currentUser={currentUser} onMarkCompleted={markCompleted} trackerKey="overpayment"/>
          </div>
        </div>
      </div>
    );
  }

  /* ═══════════════════════════════════════════════════════════
     PACKAGE SECTION — Reusable for GAC and Overpayment
  ═══════════════════════════════════════════════════════════ */
  function PackageSection({ title, accentColor, packages, section, activeKey, setActiveKey, onAddFiles, onRemoveFile, onDownload, onReset, pdfGenerating }) {
    const [dragKey, setDragKey] = useState(null);
    const fileRefs = useRef({});
    const list = Object.values(packages);

    if (list.length === 0) {
      return (
        <div>
          <div className="label" style={{color:accentColor,marginBottom:'8px'}}>{title}</div>
          <p style={{fontSize:'13px',color:'var(--muted)'}}>No packages yet. Use SPAR to move files here.</p>
        </div>
      );
    }

    return (
      <div>
        <div className="label" style={{color:accentColor,marginBottom:'14px'}}>{title}</div>
        <div style={{display:'grid',gridTemplateColumns:'repeat(auto-fill,minmax(280px,1fr))',gap:'12px'}}>
          {list.map(pkg => {
            const fk = pkg.folderKey;
            const isOpen = activeKey === fk;
            const isDragging = dragKey === fk;
            const totalFiles = pkg.sparFiles.length + pkg.extraFiles.length;

            return (
              <div key={fk} style={{padding:'14px',border:`1px solid ${isOpen?accentColor+'55':'var(--line)'}`,borderRadius:'10px',background:'var(--bg)',transition:'border-color 180ms'}}>
                {/* Header */}
                <div style={{marginBottom:'10px'}}>
                  <div style={{fontSize:'14px',fontWeight:700,color:'var(--text)'}}>{pkg.studentName}</div>
                  {pkg.studentNumber && <div className="mono" style={{fontSize:'10px',color:'var(--faint)',marginTop:'2px'}}>#{pkg.studentNumber}</div>}
                  <div className="mono" style={{fontSize:'10px',color:'var(--faint)',marginTop:'4px'}}>
                    {pkg.sparFiles.length} from SPAR · {pkg.extraFiles.length} added · {totalFiles} total
                  </div>
                  <div style={{marginTop:'4px'}}>
                    <span className="pill" style={{background:accentColor+'22',color:accentColor}}>{pkg.purpose}</span>
                    {totalFiles > 0 && <span className="pill" style={{background:'rgba(74,222,128,.15)',color:'var(--green)',marginLeft:'6px'}}>Ready</span>}
                  </div>
                </div>

                {/* Toggle open */}
                <button onClick={()=>setActiveKey(isOpen?null:fk)}
                  className="btn" style={{width:'100%',marginBottom:'8px',justifyContent:'center',fontSize:'11px',color:accentColor,borderColor:accentColor+'55'}}>
                  {isOpen?'▲ Close':'▼ Open Package'}
                </button>

                {isOpen && (
                  <div style={{marginBottom:'8px'}}>
                    {/* SPAR files */}
                    {pkg.sparFiles.length > 0 && (
                      <div style={{marginBottom:'8px'}}>
                        <div className="mono" style={{fontSize:'9px',color:'var(--muted)',marginBottom:'4px',textTransform:'uppercase',letterSpacing:'.1em'}}>From SPAR</div>
                        {pkg.sparFiles.map((f,i) => (
                          <div key={'s'+i} className="file-item">
                            <span style={{fontSize:'14px',flexShrink:0}}>{f.type==='image'?'🖼':'📄'}</span>
                            <span className="file-name">{f.name}</span>
                            <button className="remove-btn" onClick={()=>onRemoveFile(fk, section, 'spar', i)}>×</button>
                          </div>
                        ))}
                      </div>
                    )}

                    {/* Extra files */}
                    {pkg.extraFiles.length > 0 && (
                      <div style={{marginBottom:'8px'}}>
                        <div className="mono" style={{fontSize:'9px',color:'var(--muted)',marginBottom:'4px',textTransform:'uppercase',letterSpacing:'.1em'}}>Added manually</div>
                        {pkg.extraFiles.map((f,i) => (
                          <div key={'e'+i} className="file-item">
                            <span style={{fontSize:'14px',flexShrink:0}}>{f.type==='image'?'🖼':'📄'}</span>
                            <span className="file-name">{f.name}</span>
                            <button className="remove-btn" onClick={()=>onRemoveFile(fk, section, 'extra', i)}>×</button>
                          </div>
                        ))}
                      </div>
                    )}

                    {/* Add more files */}
                    <div
                      className={`dropzone ${isDragging?'over':''}`}
                      onDragOver={e=>{e.preventDefault(); setDragKey(fk);}}
                      onDragLeave={()=>setDragKey(null)}
                      onDrop={e=>{e.preventDefault(); setDragKey(null); onAddFiles(fk, section, e.dataTransfer.files);}}
                      onClick={()=>fileRefs.current[fk]?.click()}
                      style={{padding:'14px',textAlign:'center',cursor:'pointer',marginBottom:'8px'}}>
                      <div style={{fontSize:'16px',marginBottom:'2px'}}>+</div>
                      <div className="mono" style={{fontSize:'10px',fontWeight:600,color:accentColor,textTransform:'uppercase',letterSpacing:'.08em'}}>Add Files to Package</div>
                      <div style={{fontSize:'10px',color:'var(--muted)',marginTop:'2px'}}>images or PDFs</div>
                    </div>
                    <input
                      ref={el => { fileRefs.current[fk] = el; }}
                      type="file" accept="image/*,application/pdf,.pdf" multiple
                      style={{display:'none'}}
                      onChange={e => { onAddFiles(fk, section, e.target.files); e.target.value = ''; }}
                    />
                  </div>
                )}

                {/* Action buttons */}
                <div style={{display:'flex',gap:'6px'}}>
                  <button onClick={()=>onDownload(fk, section)} disabled={pdfGenerating || totalFiles === 0}
                    className="btn btn-orange"
                    style={{flex:1,justifyContent:'center',fontSize:'11px',opacity:(pdfGenerating||totalFiles===0)?.5:1}}>
                    {pdfGenerating ? 'Generating…' : `⬇ Download ${pkg.purpose} PDF`}
                  </button>
                  <button onClick={()=>{if(confirm(`Reset ${pkg.studentName}'s ${pkg.purpose} document package?`)) onReset(fk);}}
                    className="btn" style={{fontSize:'11px',color:'var(--red)',borderColor:'var(--red)',padding:'8px 12px',whiteSpace:'nowrap'}}
                    title={`Reset only this ${pkg.purpose} document package`}>
                    ↻ Reset Document
                  </button>
                </div>
              </div>
            );
          })}
        </div>
      </div>
    );
  }



  /* ================= WORK EASY HUB ================= */
  function WorkEasyYr2ReleasesTracker({ currentUser, notifyUser }) {
    return null;
  }

  function WorkEasyHubPage({ currentUser, onSwitchUser, onNavigate, theme, onToggleTheme }) {
    const [chatOpen, setChatOpen] = useState(false);
    const [unread, setUnread] = useState(0);
    const [toasts, setToasts] = useState([]);
    const notifyUser = useCallback((title, body='', sourceUser='') => {
      const toast = { id:localId('toast'), title, body, createdAt:Date.now() };
      setToasts(p => [toast, ...p].slice(0, 4));
      setTimeout(()=>setToasts(p=>p.filter(t=>t.id!==toast.id)), 7000);
      if('Notification' in window && Notification.permission === 'granted' && document.hidden) {
        try { new Notification(title, { body, tag:title + sourceUser }); } catch(e) {}
      }
      if(!chatOpen && /chat|mentioned|ping/i.test(title + ' ' + body)) setUnread(u => u + 1);
    }, [chatOpen]);

    return (
      <div style={{minHeight:'100vh',background:'var(--bg)',position:'relative'}}>
        <ToastHost toasts={toasts} onClose={(id)=>setToasts(p=>p.filter(t=>t.id!==id))} />
        <ChatPanel currentUser={currentUser} open={chatOpen}
          onToggle={()=>{ setChatOpen(p=>!p); if(!chatOpen) setUnread(0); }}
          unread={unread} onClearUnread={()=>setUnread(0)} notifyUser={notifyUser} />

        {/* Topbar — consistent with War Room and Month End */}
        <div className="topbar">
          <div style={{display:'flex',alignItems:'center',gap:'14px'}}>
            <span className="wordmark">f-cdi</span>
            <span style={{color:'var(--faint)'}}>/</span>
            <span className="label">WorkEasy Hub</span>
          </div>
          <div style={{display:'flex',alignItems:'center',gap:'10px',flexWrap:'wrap'}}>
            <NotificationButton notifyUser={notifyUser}/>
            <ThemeToggle theme={theme} onToggle={onToggleTheme}/>
            <div className="seg">
              <button className="seg-btn" onClick={()=>onNavigate('war')}>War Room</button>
              <button className="seg-btn on" style={{background:'#22d3ee',color:'#06181d'}}>WorkEasy Hub</button>
              <button className="seg-btn" onClick={()=>onNavigate('monthend')}>Month End</button>
            </div>
            <div style={{display:'flex',alignItems:'center',gap:'8px',padding:'4px 10px 4px 4px',background:'var(--bg-2)',border:'1px solid var(--line)',borderRadius:'24px'}}>
              <Avatar name={currentUser} size={26}/>
              <span style={{fontSize:'13px',fontWeight:500}}>{currentUser}</span>
            </div>
            <button onClick={onSwitchUser} className="btn-link">Switch user</button>
          </div>
        </div>

        {/* Compact head — no giant hero, normalized typography */}
        <main className="we-wrap">
          <div className="we-head">
            <div>
              <div className="label" style={{color:'#22d3ee',marginBottom:'2px'}}>WorkEasy Hub</div>
              <h1>Excel-driven tools, focused workspace</h1>
              <p>
                Two separate workspaces: <strong style={{color:'var(--text)'}}>Payment Emails</strong> for outstanding-balance reminders, and <strong style={{color:'var(--text)'}}>Yr 2 Tracker</strong> for Year 2 application data. Each tab uses its own Excel file, its own data, and its own export.
              </p>
            </div>
            <div className="we-actions" style={{alignSelf:'flex-end'}}>
              <button onClick={()=>onNavigate('war')} className="we-btn subtle">← Back to War Room</button>
            </div>
          </div>

          <WorkEasyHubPanel currentUser={currentUser} notifyUser={notifyUser} />
        </main>
      </div>
    );
  }

  /* ═══════════════════════════════════════════════════════════
     ROOT
  ═══════════════════════════════════════════════════════════ */
  function App() {
    const [currentUser, setCurrentUser] = useState(() => localStorage.getItem('fcdi_user') || null);
    const [page, setPage] = useState('war');
    const { theme, toggle: toggleTheme } = useTheme();

    const handleLogin = name => { setCurrentUser(name); localStorage.setItem('fcdi_user', name); };
    const handleSwitchUser = () => { setCurrentUser(null); localStorage.removeItem('fcdi_user'); document.body.className=''; };

    if(!currentUser) return <LoginPage onLogin={handleLogin} theme={theme} onToggleTheme={toggleTheme}/>;

    if(page === 'workeasy') return <WorkEasyHubPage currentUser={currentUser} onSwitchUser={handleSwitchUser} onNavigate={setPage} theme={theme} onToggleTheme={toggleTheme}/>;
    if(page === 'monthend') return <MonthEndMode currentUser={currentUser} onSwitchUser={handleSwitchUser} onNavigate={setPage} theme={theme} onToggleTheme={toggleTheme}/>;
    return <TaskWarRoom currentUser={currentUser} onSwitchUser={handleSwitchUser} onNavigate={setPage} theme={theme} onToggleTheme={toggleTheme}/>;
  }

  ReactDOM.createRoot(document.getElementById('root')).render(<App/>);
</script>
</body>
</html>
