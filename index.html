<!DOCTYPE html>
<html lang="ku">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>TECH RELL</title>
    <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/@emailjs/browser@3/dist/email.min.js"></script>
    <style>
        :root {
            --bg-main: #06070d;
            --bg-card: rgba(13, 16, 27, 0.85);
            --accent-pink: #ff0055;
            --accent-cyan: #00f0ff;
            --text-white: #ffffff;
            --text-gray: #64748b;
            --border-color: rgba(255, 255, 255, 0.06);
            --glow-cyan: rgba(0, 240, 255, 0.15);
        }

        * { box-sizing: border-box; margin: 0; padding: 0; font-family: 'Segoe UI', system-ui, sans-serif; }
        
        body { 
            background-color: var(--bg-main);
            color: var(--text-white); 
            min-height: 100vh; 
            display: flex; 
            justify-content: center; 
            align-items: center;
            overflow-x: hidden;
        }
        
        .app-container { 
            width: 100vw;
            height: 100vh;
            max-width: 100%;
            background-color: var(--bg-card); 
            position: relative; 
            display: flex; 
            flex-direction: column; 
            justify-content: center;
        }

        .screen { display: none; opacity: 0; transform: translateY(15px);
            transition: all 0.35s cubic-bezier(0.34, 1.56, 0.64, 1); padding: 30px 20px;
        }
        .screen.active { display: block; opacity: 1; transform: translateY(0);
        }
        
        #splash-screen { position: absolute;
            top: 0; left: 0; width: 100%; height: 100%; display: none; flex-direction: column; justify-content: center; align-items: center; background-color: var(--bg-main); z-index: 10;
            padding: 0; }
        #splash-screen.active { display: flex; opacity: 1;
        }
        
        .logo-box { width: 95px;
            height: 95px; margin: 0 auto 20px auto; animation: floatAnim 3s ease-in-out infinite;
        }
        @keyframes floatAnim { 0%, 100% { transform: translateY(0);
            } 50% { transform: translateY(-8px); } }
        .logo-svg { width: 100%; height: 100%;
            filter: drop-shadow(0px 0px 15px rgba(0, 240, 255, 0.4)); }
        
        .brand-name { font-size: 36px;
            font-weight: 900; letter-spacing: 4px; text-transform: uppercase; background: linear-gradient(45deg, var(--accent-cyan), #ffffff, var(--accent-pink)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; text-align: center;
        }
        
        .card-panel {
            background: rgba(255, 255, 255, 0.02);
            border: 1px solid var(--border-color);
            border-radius: 20px;
            padding: 30px 20px;
            box-shadow: 0 15px 35px rgba(0,0,0,0.4);
        }

        h2 { font-size: 26px; font-weight: 800; margin-bottom: 6px; text-align: center; letter-spacing: 0.5px;
        }
        .subtitle { font-size: 13px; color: var(--text-gray); text-align: center; margin-bottom: 25px; line-height: 1.5;
        }
        
        input, select, textarea { 
            width: 100%;
            padding: 15px 18px; 
            background-color: rgba(0, 0, 0, 0.4); 
            border: 1px solid var(--border-color); 
            border-radius: 12px; 
            color: var(--text-white); 
            font-size: 15px; 
            outline: none;
            transition: all 0.25s ease;
        }
        input:focus, select:focus, textarea:focus { border-color: var(--accent-cyan);
            box-shadow: 0 0 15px var(--glow-cyan); background-color: rgba(0,0,0,0.6); }
        .form-group { margin-bottom: 18px;
        }
        .form-group label { display: block; font-size: 11px; color: var(--text-gray); margin-bottom: 8px;
            font-weight: 700; letter-spacing: 1.5px; text-transform: uppercase; }
        .form-row { display: grid;
            grid-template-columns: 1fr 1fr; gap: 12px; }
        
        .btn { 
            width: 100%;
            padding: 16px; 
            background: linear-gradient(90deg, #00e5ff, #00aeff); 
            border: none; 
            border-radius: 12px; 
            color: #04060a; 
            font-size: 15px; 
            font-weight: 800; 
            cursor: pointer; 
            margin-top: 10px;
            box-shadow: 0 5px 20px rgba(0, 229, 255, 0.25);
            transition: all 0.25s ease;
            text-transform: uppercase;
            letter-spacing: 1px;
        }
        .btn:hover { transform: translateY(-2px); box-shadow: 0 7px 25px rgba(0, 229, 255, 0.4);
        }
        .btn-secondary { background: transparent; border: 1px solid var(--border-color); color: #cbd5e1; margin-top: 12px;
            box-shadow: none; }
        .forget-link { display: block; text-align: right; margin-top: -8px; margin-bottom: 20px;
            font-size: 12px; color: var(--accent-pink); cursor: pointer; font-weight: 600; }
        
        /* 📱 MAIN APP SCREEN */
        #main-app-screen { position: absolute;
            top:0; left:0; width:100%; height:100%; padding:0; display:none; background-color:#000; overflow:hidden; }
        #main-app-screen.active { display: flex;
            flex-direction: column; opacity: 1; transform: none; }
        
        .app-content-area { flex: 1;
            display: flex; justify-content: center; align-items: center; position: relative; width: 100%; height: 100%;
        }
        .tab-content { width: 100%; height: 100%; display: none; flex-direction: column; justify-content: center;
            align-items: center; }
        .tab-content.active { display: flex;
        }

        /* 📸 CAMERA INTERFACE CSS */
        .camera-container { width: 100%;
            height: 100%; position: relative; background: #000; display: flex; flex-direction: column; justify-content: space-between;
        }
        #camera-stream { width: 100%; height: 100%; object-fit: cover; position: absolute; top: 0;
            left: 0; z-index: 1; transition: filter 0.3s ease, transform 0.2s ease;
        }
        
        #screen-flash-overlay { display: none;
            position: absolute; top: 0; left: 0; width: 100%; height: 100%; background: #ffffff; z-index: 9;
        }

        .camera-overlay { position: absolute; top: 0; left: 0; width: 100%; height: 100%;
            z-index: 2; display: flex; flex-direction: column; justify-content: space-between; padding: 20px;
            background: linear-gradient(to bottom, rgba(0,0,0,0.3) 0%, transparent 25%, transparent 65%, rgba(0,0,0,0.8) 100%);
        }
        
        .camera-top-actions { display: flex;
            justify-content: space-between; align-items: flex-start; width: 100%; padding-top: 10px; position: relative; z-index: 10;
        }
        .camera-top-right-group { display: flex; flex-direction: column; gap: 15px; align-items: flex-end;
        }
        
        .add-music-center-container {
            position: absolute;
            left: 50%;
            top: 25px;
            transform: translateX(-50%);
            z-index: 10;
        }
        .add-music-btn {
            background: rgba(20, 20, 20, 0.75);
            border: 1px solid rgba(255, 255, 255, 0.3);
            padding: 10px 18px;
            border-radius: 30px;
            color: #ffffff;
            font-size: 13px;
            font-weight: 700;
            display: flex;
            align-items: center;
            gap: 6px;
            cursor: pointer;
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
            transition: all 0.2s ease;
            box-shadow: 0 4px 12px rgba(0,0,0,0.4);
            white-space: nowrap;
        }
        .add-music-btn:active { transform: scale(0.95) translateX(-52%); background: rgba(0,0,0,0.9);
        }

        .cam-icon-btn { background: rgba(0, 0, 0, 0.55); border: none; width: 45px;
            height: 45px; border-radius: 50%; color: white; display: flex; align-items: center; justify-content: center; cursor: pointer; font-size: 20px; backdrop-filter: blur(5px);
            border: 1px solid rgba(255,255,255,0.25); box-shadow: 0 4px 10px rgba(0,0,0,0.3); transition: all 0.2s ease; position: relative; overflow: hidden;
        }
        .cam-icon-btn:active { transform: scale(0.9); transition: transform 0.1s;
        }
        
        .flash-off-line::after { content: "";
            position: absolute; width: 3px; height: 28px; background-color: #ff0055; transform: rotate(45deg); top: 8px; left: 20px;
            box-shadow: 0 0 4px rgba(255, 0, 85, 0.6); }
        .cam-icon-btn.flash-on { background: rgba(0, 0, 0, 0.7) !important;
            color: #ffea00 !important; border-color: #ffea00; filter: drop-shadow(0 0 8px #ffea00);
        }
        .cam-icon-btn.flash-on::after { display: none;
        }
        
        .timer-active-btn { border-color: var(--accent-cyan);
            color: var(--accent-cyan); filter: drop-shadow(0 0 5px var(--accent-cyan)); }
        .timer-options-shelf { display: none;
            background: rgba(0, 0, 0, 0.85); border-radius: 12px; border: 1px solid rgba(255,255,255,0.2); padding: 5px; position: absolute; right: 55px; top: 135px;
            flex-direction: row; gap: 8px; z-index: 10; backdrop-filter: blur(5px); }
        .timer-opt-btn { background: transparent;
            border: none; color: white; font-weight: bold; font-size: 13px; padding: 8px 12px; border-radius: 8px; cursor: pointer; transition: all 0.2s;
        }
        .timer-opt-btn.selected { background: var(--accent-cyan); color: #000;
        }

        .countdown-overlay-display { display: none; position: absolute; top: 50%; left: 50%;
            transform: translate(-50%, -50%); font-size: 90px; font-weight: 900; color: #fff; text-shadow: 0 0 30px rgba(0, 240, 255, 0.8); z-index: 8;
            animation: pulseCountdown 0.5s ease-in-out infinite alternate; }
        @keyframes pulseCountdown { 0% { transform: translate(-50%, -50%) scale(0.9);
            } 100% { transform: translate(-50%, -50%) scale(1.1); } }

        .camera-control-row { display: flex;
            flex-direction: column; align-items: center; width: 100%; position: relative; gap: 15px;
        }
        .left-controls-wrapper { position: absolute; left: 10px; bottom: 10px; display: flex; flex-direction: column;
            gap: 12px; align-items: center; z-index: 5; }
        .studio-gallery-btn { width: 45px; height: 45px;
            border-radius: 10px; border: 2px solid #fff; background: rgba(255,255,255,0.2); overflow: hidden; display: flex; flex-direction: column; align-items: center; justify-content: center; cursor: pointer;
            font-size: 10px; font-weight: bold; color: white; text-shadow: 0 1px 3px rgba(0,0,0,0.8); box-shadow: 0 4px 10px rgba(0,0,0,0.4);
        }
        .zoom-circle-btn { width: 42px; height: 42px; border-radius: 50%;
            background: rgba(0, 0, 0, 0.6); border: 1.5px solid rgba(255, 255, 255, 0.6); color: var(--accent-cyan); font-size: 12px; font-weight: 800; display: flex;
            align-items: center; justify-content: center; cursor: pointer; box-shadow: 0 4px 8px rgba(0,0,0,0.4); transition: all 0.2s ease; backdrop-filter: blur(5px);
        }

        .filters-horizontal-container { display: none; width: 100vw; overflow-x: auto; white-space: nowrap;
            padding: 10px 20px; scroll-behavior: smooth; -webkit-overflow-scrolling: touch; justify-content: flex-start; }
        .filters-horizontal-container::-webkit-scrollbar { display: none;
        }
        .filter-snap-item { display: inline-flex; flex-direction: column; align-items: center; margin-right: 16px; cursor: pointer;
            transition: transform 0.2s ease; }
        .filter-snap-circle { width: 52px; height: 52px; border-radius: 50%;
            background: linear-gradient(45deg, #111, #333); border: 2.5px solid rgba(255,255,255,0.6); display: flex; align-items: center; justify-content: center; font-size: 22px;
            box-shadow: 0 4px 12px rgba(0,0,0,0.5); transition: all 0.2s ease; }
        .filter-snap-item.active .filter-snap-circle { border-color: var(--accent-cyan);
            box-shadow: 0 0 15px var(--accent-cyan); transform: scale(1.1); }
        .filter-snap-label { font-size: 10px;
            color: #ffffff; font-weight: 700; margin-top: 5px; text-shadow: 0 1px 4px rgba(0,0,0,1);
        }

        .camera-bottom-actions { display: flex; flex-direction: column; align-items: center; gap: 12px; width: 100%;
            padding-bottom: 20px; z-index: 3; }
        .capture-trigger-btn { width: 74px; height: 74px; border-radius: 50%;
            background: white; border: 6px solid rgba(255, 255, 255, 0.35); cursor: pointer; transition: all 0.2s; flex-shrink: 0;
            box-shadow: 0 0 15px rgba(0,0,0,0.5); z-index: 6; }
        .capture-trigger-btn:active { transform: scale(0.9);
            background: #ddd; }
        .camera-modes { display: flex; gap: 25px; font-size: 13px; font-weight: 700;
            color: rgba(255,255,255,0.5); letter-spacing: 0.5px; margin-top: 5px; }
        .camera-mode-item { cursor: pointer;
            transition: color 0.2s; }
        .camera-mode-item.active { color: #fff; text-shadow: 0 0 8px rgba(255,255,255,0.6);
        }

        /* PREVIEW SCREEN */
        .preview-box { display: none;
            position: absolute; top:0; left:0; width:100%; height:100%; background: #000000; z-index:10; flex-direction:column; justify-content: space-between; padding: 0; overflow: hidden;
        }
        .fullscreen-media-container { width: 100%; height: 100%; position: absolute; top:0; left:0; z-index: 1;
            display: flex; justify-content: center; align-items: center; background: #050505; }
        .fullscreen-media-container img, .fullscreen-media-container video { width: 100%;
            height: 100%; object-fit: contain; max-width: 100%; max-height: 100%; pointer-events: none;
        }
        .movable-emoji { font-size: 55px; cursor: move; user-select: none; touch-action: none; position: absolute;
            z-index: 7; filter: drop-shadow(0 4px 10px rgba(0,0,0,0.3)); }
        .media-overlay-text-display { position: absolute;
            z-index: 5; color: #ffffff; font-size: 24px; font-weight: bold; text-align: center; text-shadow: 0 2px 8px rgba(0,0,0,0.9); background: rgba(0,0,0,0.3); padding: 6px 14px;
            border-radius: 8px; display: none; max-width: 85%; word-wrap: break-word; cursor: move; user-select: none; touch-action: none; top: 40%; left: 10%;
        }
        .preview-top-bar { position: relative; z-index: 6; padding: 20px; display: flex; justify-content: space-between;
            align-items: center; background: linear-gradient(to bottom, rgba(0,0,0,0.7), transparent); }
        .preview-bottom-bar { position: relative;
            z-index: 6; padding: 30px 20px; display: flex; justify-content: space-between; align-items: center; background: linear-gradient(to top, rgba(0,0,0,0.8) 30%, transparent); width: 100%;
        }
        .story-quick-btn { padding: 14px 28px; background: rgba(255, 255, 255, 0.2); color: #ffffff;
            border-radius: 30px; font-weight: 800; font-size: 15px; cursor: pointer; border: 1px solid rgba(255,255,255,0.4); display: flex; align-items: center; gap: 8px; backdrop-filter: blur(10px);
        }
        .next-step-btn { padding: 14px 35px; background: linear-gradient(90deg, var(--accent-cyan), #00aeff); color: #000000;
            border-radius: 30px; font-weight: 800; font-size: 15px; cursor: pointer; border: none; display: flex; align-items: center; gap: 6px;
            box-shadow: 0 4px 15px rgba(0,240,255,0.3); }

        /* DETAILS LAYOUT */
        .details-post-panel { display: none;
            position: absolute; top:0; left:0; width:100%; height:100%; background: #0c0e14; z-index:12; flex-direction:column; padding: 20px; overflow-y: auto;
        }
        .publish-split-layout { display: flex; flex-direction: row; gap: 15px; width: 100%; margin-top: 20px;
        }
        .preview-left-side { flex: 0 0 110px; height: 140px; background: #050505; border-radius: 12px;
            overflow: hidden; display: flex; justify-content: center; align-items: center; border: 1px solid var(--border-color); position: relative;
        }
        .preview-left-side img, .preview-left-side video { width: 100%; height: 100%; object-fit: contain;
        }
        .preview-right-side { flex: 1; display: flex; flex-direction: column;
        }
        
        /* TEXT EDITOR MODAL */
        .text-editor-overlay-modal { display: none;
            position: absolute; top:0; left:0; width:100%; height:100%; background: rgba(0,0,0,0.95); z-index: 20; flex-direction: column; justify-content: center; padding: 20px;
        }
        .full-color-picker-box { display: flex; flex-direction: column; align-items: center; gap: 10px;
            margin: 25px 0; }
        .modern-color-wheel { -webkit-appearance: none; appearance: none; width: 70px;
            height: 45px; background: transparent; border: none; cursor: pointer; }
        .modern-color-wheel::-webkit-color-swatch { border-radius: 10px;
            border: 2px solid #fff; }

        /* EMOJI PICKER MODAL */
        .instagram-emoji-modal { display: none;
            position: absolute; top:0; left:0; width:100%; height:100%; background: rgba(0, 0, 0, 0.65); backdrop-filter: blur(20px); -webkit-backdrop-filter: blur(20px); z-index: 20; flex-direction: column;
            justify-content: flex-end; }
        .emoji-modal-content { background: rgba(25, 25, 25, 0.9); border-top-left-radius: 24px;
            border-top-right-radius: 24px; padding: 20px 15px; max-height: 70vh; overflow-y: auto; border-top: 1px solid rgba(255, 255, 255, 0.08);
        }
        .emoji-grid-viewport { display: grid; grid-template-columns: repeat(6, 1fr); gap: 12px; justify-content: center;
            padding-bottom: 30px; }
        .emoji-item-clickable { font-size: 34px; text-align: center; cursor: pointer; user-select: none;
        }

        .caption-area { position: relative; margin-bottom: 10px;
        }
        .caption-area textarea { height: 120px; resize: none; font-size: 14px; padding: 12px;
            padding-bottom: 25px; }
        .char-counter { position: absolute; bottom: 8px; right: 12px; font-size: 11px;
            color: var(--text-gray); }
        .quick-tags { display: flex; gap: 10px; margin-bottom: 20px;
        }
        .tag-shortcut { padding: 8px 14px; background: rgba(255,255,255,0.07); border-radius: 20px; font-size: 12px;
            cursor: pointer; color: var(--accent-cyan); }

        /* NAV BAR */
        .tiktok-nav { height: 65px;
            background-color: #000000; border-top: 1px solid rgba(255,255,255,0.1); display: grid; grid-template-columns: repeat(5, 1fr); align-items: center; justify-items: center; width: 100%; z-index: 5;
            transition: display 0.2s ease; }
        .nav-item { display: flex; flex-direction: column; align-items: center;
            justify-content: center; color: #777; cursor: pointer; font-size: 11px; font-weight: 600; width: 100%; height: 100%;
        }
        .nav-item svg { width: 22px; height: 22px; fill: currentColor; margin-bottom: 3px;
        }
        .nav-item.active { color: #ffffff;
        }
        .nav-item-add { position: relative;
        }
        .add-btn-design { width: 44px; height: 28px; background: #fff; border-radius: 8px; position: relative;
            display: flex; align-items: center; justify-content: center; color: #000 !important; font-size: 18px; font-weight: bold;
        }
        .add-btn-design::before { content: ''; position: absolute; width: 44px; height: 28px; background: #00f0ff;
            border-radius: 8px; left: -3px; top: 0; z-index: -1; }
        .add-btn-design::after { content: '';
            position: absolute; width: 44px; height: 28px; background: #ff0055; border-radius: 8px; right: -3px; top: 0; z-index: -2;
        }

        /* 📥 INBOX TOP ICONS STYLING */
        .inbox-header-icons {
            display: flex;
            justify-content: center;
            gap: 15px;
            width: 100%;
            margin-bottom: 25px;
            padding: 10px;
        }
        .inbox-square-icon {
            width: 60px;
            height: 60px;
            background-color: rgba(255, 255, 255, 0.05);
            border: 1px solid var(--border-color);
            border-radius: 12px;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            transition: all 0.25s ease;
            font-size: 24px;
        }
        .inbox-square-icon:hover {
            border-color: var(--accent-cyan);
            box-shadow: 0 0 12px var(--glow-cyan);
            transform: translateY(-2px);
        }
    </style>
</head>
<body>

    <div class="app-container">

        <div id="splash-screen" class="screen active">
            <div class="logo-box">
                <svg class="logo-svg" viewBox="0 0 100 100">
                    <polygon points="50,15 82,33 82,67 50,85 18,67 18,33" stroke="url(#cyberGradient)" stroke-width="4" fill="none" />
                    <polygon points="42,35 68,50 42,65" fill="#ffffff" />
                    <defs><linearGradient id="cyberGradient"><stop offset="0%" stop-color="#00f0ff" /><stop offset="100%" stop-color="#ff0055" /></linearGradient></defs>
                </svg>
            </div>
            <h1 class="brand-name">TECH RELL</h1>
        </div>

        <div id="welcome-screen" class="screen">
            <div class="card-panel">
                <div style="text-align: center; margin-bottom: 30px;">
                    <h2>TECH RELL</h2>
                    <p class="subtitle">تۆڕا ڤیدیۆیی یا تەکنەلۆژییا نوی</p>
                </div>
                <button class="btn" onclick="navigateTo('signin-screen')">SIGN IN</button>
                <button class="btn btn-secondary" onclick="navigateTo('signup-screen')">SIGN UP</button>
            </div>
        </div>

        <div id="signin-screen" class="screen">
            <div class="card-panel">
                <h2>SIGN IN</h2>
                <p class="subtitle">بچۆ د ناڤ حسابا خۆ دا</p>
                <form id="signin-form" onsubmit="handleSignIn(event)">
                    <div class="form-group"><label>EMAIL</label><input type="email" id="login-email" required></div>
                    <div class="form-group"><label>PASSWORD</label><input type="password" id="login-pass" required></div>
                    <div class="forget-link" onclick="navigateTo('forget-password-screen')">پاسوۆرد ژبیر کر ل ڤێرە کلیک بکە؟</div>
                    <button type="submit" class="btn">SIGN IN</button>
                </form>
                <button class="btn btn-secondary" onclick="navigateTo('welcome-screen')">← زڤڕین</button>
            </div>
        </div>

        <div id="forget-password-screen" class="screen">
            <div class="card-panel">
                <h2>RESET PASSWORD</h2>
                <p class="subtitle">ناڤێ خۆ بنڤیسە و کۆد دێ بۆ ئیمەیلی چیت</p>
                <form id="forget-form" onsubmit="handleForgetPassword(event)">
                    <div class="form-group"><label>USERNAME</label><input type="text" id="forget-user" required></div>
                    <button type="submit" class="btn">SEND CODE</button>
                </form>
                <button class="btn btn-secondary" onclick="navigateTo('signin-screen')">← زڤڕین</button>
            </div>
        </div>

        <div id="new-password-screen" class="screen">
            <div class="card-panel">
                <h2>ENTER NEW PASSWORD</h2>
                <p class="subtitle">کۆدێ هاتی و پاسوۆردێ نوو داخل بکە</p>
                <form id="reset-final-form" onsubmit="handleFinalReset(event)">
                    <div class="form-group"><label>VERIFICATION CODE</label><input type="text" id="reset-otp" required></div>
                    <div class="form-group"><label>NEW PASSWORD</label><input type="password" id="new-pass" required></div>
                    <button type="submit" class="btn">تمام</button>
                </form>
            </div>
        </div>

        <div id="signup-screen" class="screen">
            <div class="card-panel">
                <h2>SIGN UP</h2>
                <p class="subtitle">حسابەکا نوو تۆمار بکە</p>
                <form id="signup-form" onsubmit="handleSignUp(event)">
                    <div class="form-group"><label>USERNAME</label><input type="text" id="reg-user" required></div>
                    <div class="form-group"><label>NAME</label><input type="text" id="reg-name" required></div>
                    <div class="form-group"><label>EMAIL</label><input type="email" id="reg-email" required></div>
                    <div class="form-group"><label>PASSWORD</label><input type="password" id="reg-pass" required></div>
                    <div class="form-row">
                        <div class="form-group"><label>COUNTRY</label><select id="reg-country"><option value="Iraq">Iraq</option></select></div>
                        <div class="form-group"><label>GENDER</label><select id="reg-gender"><option value="Male">Male</option><option value="Female">Female</option></select></div>
                    </div>
                    <button type="submit" class="btn">SUBMIT & SEND CODE</button>
                </form>
                <button class="btn btn-secondary" onclick="navigateTo('welcome-screen')">← زڤڕین</button>
            </div>
        </div>

        <div id="signup-verify-screen" class="screen">
            <div class="card-panel">
                <h2>EMAIL VERIFICATION</h2>
                <p class="subtitle">کۆدەک بۆ ئیمەیلێ تە چوویە</p>
                <div class="form-group"><input type="text" id="email-otp" placeholder="••••••" maxlength="6" style="text-align:center; font-size:24px;" required></div>
                <button class="btn" onclick="verifyAndSave()">VERIFY & SAVE</button>
            </div>
        </div>

        <div id="main-app-screen" class="screen">
            <div class="app-content-area">
                
                <div id="tab-reels" class="tab-content active">
                    <div style="text-align:center;">
                        <div style="font-size:45px; margin-bottom:10px;">🎬</div>
                        <p style="font-size:18px; font-weight: bold;">بەشێ ڕیڵز (TECH REELS)</p>
                        <p style="color: var(--text-gray); font-size: 14px; margin-top: 5px;">ڤیدیۆ ل ڤێرە دێ دیار بن...</p>
                    </div>
                </div>

                <div id="tab-search" class="tab-content">
                    <div style="width: 100%; padding: 20px;">
                        <h2>SEARCH</h2>
                        <input type="text" placeholder="ناڤەکێ بگەڕێ..." style="margin-top:15px;">
                    </div>
                </div>

                <div id="tab-add" class="tab-content" style="padding:0;">
                    <div class="camera-container">
                        <video id="camera-stream" autoplay playsinline></video>
                        <div id="screen-flash-overlay"></div>
                        <div id="countdown-number" class="countdown-overlay-display">0</div>

                        <div id="gallery-preview-box" class="preview-box">
                            <div class="preview-top-bar">
                                <button class="cam-icon-btn" onclick="closePreview()">❌</button>
                                <div style="display: flex; flex-direction: column; gap: 12px;">
                                    <button class="cam-icon-btn" onclick="openTextEditorModal()" style="font-weight:bold; font-size:22px; color:var(--accent-cyan);">T</button>
                                    <button class="cam-icon-btn" onclick="openEmojiPickerModal()" style="font-size:22px;">😀</button>
                                </div>
                            </div>

                            <div class="fullscreen-media-container" id="media-container-zone">
                                <img id="preview-media" src="" alt="Preview">
                                <video id="preview-video" autoplay loop muted></video>
                                <div id="media-text-overlay" class="media-overlay-text-display" onclick="openTextEditorModal()"></div>
                                <div id="sticker-container-zone" style="position: absolute; top:0; left:0; width:100%; height:100%; pointer-events:none; z-index:6;"></div>
                            </div>

                            <div id="text-editor-modal" class="text-editor-overlay-modal">
                                <h3 style="text-align:center; margin-bottom:15px; color:#fff;">نڤیسین ل سەر پۆستی</h3>
                                <input type="text" id="media-custom-text-input" placeholder="لێرە دەقێ خۆ بنڤیسە..." style="text-align:center; font-size:18px;">
                                <div class="full-color-picker-box">
                                    <label>ڕەنگێ دەقی هەڵبژێرە:</label>
                                    <input type="color" id="html-color-wheel" class="modern-color-wheel" value="#ffffff">
                                </div>
                                <button class="btn" onclick="saveTextOverlay()">Save Text</button>
                                <button class="btn btn-secondary" onclick="closeTextEditorModal()">Cancel</button>
                            </div>

                            <div id="emoji-picker-modal" class="instagram-emoji-modal" onclick="closeEmojiPickerModal()">
                                <div class="emoji-modal-content" onclick="event.stopPropagation()">
                                    <div class="emoji-grid-viewport" id="emoji-grid-container"></div>
                                </div>
                            </div>

                            <div class="preview-bottom-bar">
                                <button class="story-quick-btn" onclick="quickPublishStory()">⏱️ Story</button>
                                <button class="next-step-btn" onclick="openStepTwoDetails()">Next ➡️</button>
                            </div>
                        </div>

                        <div id="details-post-panel" class="details-post-panel">
                            <div style="display:flex; justify-content:space-between; align-items:center; margin-bottom:10px;">
                                <button class="cam-icon-btn" onclick="backToStepOne()">←</button>
                                <h3 style="font-weight:800; color:var(--accent-cyan);">بڵاوکردنەوەی نوو</h3>
                                <div style="width:40px;"></div>
                            </div>
                            <div class="publish-split-layout">
                                <div class="preview-left-side" id="split-media-zone"></div>
                                <div class="preview-right-side">
                                    <div class="caption-area">
                                        <textarea id="post-caption-input" placeholder="تێکست یان تایتل بنڤیسە..." maxlength="999" oninput="updateCharCount()"></textarea>
                                        <div class="char-counter" id="char-counter-txt">999 پیت ماون</div>
                                    </div>
                                    <div class="quick-tags">
                                        <div class="tag-shortcut" onclick="insertAtCursor('@')">@ تاگکرن</div>
                                        <div class="tag-shortcut" onclick="insertAtCursor('#')"># هێشتاگ</div>
                                    </div>
                                </div>
                            </div>
                            <button class="btn" onclick="finalPublishPost()" style="margin-top:30px; background:linear-gradient(90deg, #ff0055, #ff5500); color:white;">Post 📝</button>
                        </div>

                        <div class="camera-overlay">
                            <div class="add-music-center-container">
                                <button class="add-music-btn" onclick="alert('لیستا میوزیکان دێ ل ڤێرە ڤەبیت')"> 🎵 زیادکردنی میوزیک </button>
                            </div>
                            <div class="camera-top-actions">
                                <button class="cam-icon-btn" onclick="exitCameraTab()" style="background: rgba(255, 0, 85, 0.6); border-color: var(--accent-pink);">❌</button>
                                <div class="camera-top-right-group">
                                    <button class="cam-icon-btn" onclick="flipCamera()">🔄</button>
                                    <button class="cam-icon-btn" onclick="toggleFiltersShelf()">🌟</button>
                                    <button class="cam-icon-btn flash-off-line" id="flash-toggle-btn" onclick="toggleFlash()">⚡</button>
                                    <button class="cam-icon-btn" id="timer-toggle-btn" onclick="toggleTimerShelf()">⏱️</button>
                                    <div id="timer-options-shelf" class="timer-options-shelf">
                                        <button class="timer-opt-btn selected" id="opt-0s" onclick="setTimerSecs(0, this)">Off</button>
                                        <button class="timer-opt-btn" id="opt-3s" onclick="setTimerSecs(3, this)">3s</button>
                                        <button class="timer-opt-btn" id="opt-10s" onclick="setTimerSecs(10, this)">10s</button>
                                    </div>
                                </div>
                            </div>

                            <div class="camera-control-row">
                                <div class="left-controls-wrapper">
                                    <div class="studio-gallery-btn" onclick="triggerHiddenGalleryInput()">
                                        <span style="font-size:16px;">🖼️</span>
                                    </div>
                                    <button class="zoom-circle-btn" id="zoom-toggle-btn" onclick="toggleZoomClick()">1x</button>
                                </div>

                                <div class="filters-horizontal-container" id="filters-horizontal-shelf">
                                    <div class="filter-snap-item active" onclick="setCamFilter('', this)"><div class="filter-snap-circle">❌</div><div class="filter-snap-label">Normal</div></div>
                                    <div class="filter-snap-item" onclick="setCamFilter('grayscale(100%)', this)"><div class="filter-snap-circle">🎬</div><div class="filter-snap-label">B&W</div></div>
                                    <div class="filter-snap-item" onclick="setCamFilter('sepia(80%)', this)"><div class="filter-snap-circle">🍂</div><div class="filter-snap-label">Sepia</div></div>
                                    <div class="filter-snap-item" onclick="setCamFilter('hue-rotate(90deg)', this)"><div class="filter-snap-circle">🔮</div><div class="filter-snap-label">Cyber</div></div>
                                    <div class="filter-snap-item" onclick="setCamFilter('contrast(150%) saturate(150%)', this)"><div class="filter-snap-circle">🔥</div><div class="filter-snap-label">Vibrant</div></div>
                                </div>

                                <input type="file" id="hidden-gallery-input" accept="image/*,video/*" style="display: none;" onchange="handleGalleryFileSelected(this)">

                                <div class="camera-bottom-actions">
                                    <button class="capture-trigger-btn" onclick="handleCaptureAction()"></button>
                                    <div class="camera-modes">
                                        <span class="camera-mode-item active" onclick="setCamMode('video', this)">VIDEO</span>
                                        <span class="camera-mode-item" onclick="setCamMode('photo', this)">PHOTO</span>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>

                <div id="tab-inbox" class="tab-content">
                    <div style="width: 100%; padding: 20px; height: 100%; display: flex; flex-direction: column;">
                        <h2 style="margin-bottom: 20px; text-align: center;">INBOX</h2>
                        
                        <div class="inbox-header-icons">
                            <div class="inbox-square-icon" onclick="alert('دەمی فولوه ك بو بكار هينه ری بيت (Follow Alerts)')" title="فۆڵۆوەرێن نوو">
                                👤
                            </div>
                            <div class="inbox-square-icon" onclick="alert('ده می كه سه ك بوستی ته لايك بكه ت يان كومينت بكه ت يان نافي ته ل جهه كي تاك بكه ت يان كوميتا ته لايك بكه ت يان كومنتا ته ريبله ي بكه ت')" title="کۆمێنت و لایک و تاگ">
                                💬
                            </div>
                            <div class="inbox-square-icon" onclick="alert('به شي ره خفه يي نامي بيت كو كه سه ك نامي بوته ريكه ت (Direct Messages)')" title="نامەیێن نوو">
                                ✉️
                            </div>
                        </div>

                        <div style="flex: 1; display: flex; align-items: center; justify-content: center; border: 1px dashed var(--border-color); border-radius: 15px; color: var(--text-gray);">
                            <p>پەیام و ئاگەهدارێن تە دێ ل ڤێرە دیار بن</p>
                        </div>
                    </div>
                </div>

                <div id="tab-profile" class="tab-content">
                    <div style="text-align:center;">
                        <div style="font-size:50px; margin-bottom:10px;">👤</div>
                        <h2>MY PROFILE</h2>
                        <p style="color: var(--text-gray); font-size:14px; margin-top:5px;">@username</p>
                    </div>
                </div>

            </div>

            <div class="tiktok-nav" id="main-tiktok-nav-bar">
                <div class="nav-item active" onclick="switchTab('tab-reels', this)">
                    <svg viewBox="0 0 24 24"><path d="M10 20v-6h4v6h5v-8h3L12 3 2 12h3v8z"/></svg>
                    <span>Home</span>
                </div>
                <div class="nav-item" onclick="switchTab('tab-search', this)">
                    <svg viewBox="0 0 24 24"><path d="M15.5 14h-.79l-.28-.27C15.41 12.59 16 11.11 16 9.5 16 5.91 13.09 3 9.5 3S3 5.91 3 9.5 5.91 16 9.5 16c1.61 0 3.09-.59 4.23-1.57l.27.28v.79l5 4.99L20.49 19l-4.99-5zm-6 0C7.01 14 5 11.99 5 9.5S7.01 5 9.5 5 14 7.01 14 9.5 11.99 14 9.5 14z"/></svg>
                    <span>Discover</span>
                </div>
                <div class="nav-item nav-item-add" onclick="enterCameraTabMode(this)">
                    <div class="add-btn-design">+</div>
                </div>
                <div class="nav-item" onclick="switchTab('tab-inbox', this)">
                    <svg viewBox="0 0 24 24"><path d="M20 2H4c-1.1 0-1.99.9-1.99 2L2 22l4-4h14c1.1 0 2-.9 2-2V4c0-1.1-.9-2-2-2zM6 9h12v2H6V9zm8 5H6v-2h8v2zm4-6H6V6h12v2z"/></svg>
                    <span>Inbox</span>
                </div>
                <div class="nav-item" onclick="switchTab('tab-profile', this)">
                    <svg viewBox="0 0 24 24"><path d="M12 12c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm0 2c-2.67 0-8 1.34-8 4v2h16v-2c0-2.66-5.33-4-8-4z"/></svg>
                    <span>Profile</span>
                </div>
            </div>
        </div>

    </div>

    <script type="text/javascript">
        (function(){ emailjs.init("YOUR_PUBLIC_KEY"); })();

        let currentActiveTabId = "tab-reels";
        let isCameraStreamRunning = false;
        let activeMediaStreamObject = null;
        let selectedFilterStyle = "";
        let flashModeState = false;
        let captureTimerSeconds = 0;
        let zoomLevels = ["1", "2", "4"];
        let zoomIndex = 0;
        let currentCamMode = "video";

        setTimeout(() => {
            document.getElementById('splash-screen').classList.remove('active');
            document.getElementById('welcome-screen').classList.add('active');
        }, 2200);

        function navigateTo(screenId) {
            document.querySelectorAll('.screen').forEach(s => s.classList.remove('active'));
            let target = document.getElementById(screenId);
            if(target) target.classList.add('active');
        }

        function switchTab(tabId, el) {
            document.querySelectorAll('.nav-item').forEach(item => item.classList.remove('active'));
            if(el) el.classList.add('active');
            document.querySelectorAll('.tab-content').forEach(tc => tc.classList.remove('active'));
            document.getElementById(tabId).classList.add('active');
            currentActiveTabId = tabId;
        }

        function enterMainAppAndShowReels() {
            navigateTo('main-app-screen');
            switchTab('tab-reels', document.querySelector('.nav-item'));
        }

        function enterCameraTabMode(navElement) {
            document.querySelectorAll('.nav-item').forEach(item => item.classList.remove('active'));
            navElement.classList.add('active');
            document.querySelectorAll('.tab-content').forEach(tc => tc.classList.remove('active'));
            document.getElementById('tab-add').classList.add('active');
            document.getElementById('main-tiktok-nav-bar').style.display = 'none';
            startLiveCameraProcessing();
        }

        function exitCameraTab() {
            stopLiveCameraProcessing();
            document.getElementById('main-tiktok-nav-bar').style.display = 'grid';
            let firstTabBtn = document.querySelector('.nav-item');
            switchTab('tab-reels', firstTabBtn);
        }

        async function startLiveCameraProcessing() {
            if(isCameraStreamRunning) return;
            try {
                let stream = await navigator.mediaDevices.getUserMedia({ video: { facingMode: "user" }, audio: false });
                activeMediaStreamObject = stream;
                let vWidget = document.getElementById('camera-stream');
                vWidget.srcObject = stream;
                isCameraStreamRunning = true;
            } catch(e) {
                console.log("Camera access error:", e);
                alert("کامێرا کار ناکەت یان مۆڵەت نەدراوە!");
            }
        }

        function stopLiveCameraProcessing() {
            if(activeMediaStreamObject) {
                activeMediaStreamObject.getTracks().forEach(t => t.stop());
                activeMediaStreamObject = null;
            }
            isCameraStreamRunning = false;
        }

        function flipCamera() { alert("گۆڕینی کامێرا بۆ دواوە/پێشەوە"); }
        function toggleFiltersShelf() {
            let shelf = document.getElementById('filters-horizontal-shelf');
            shelf.style.display = (shelf.style.display === 'inline-flex' || shelf.style.display === 'flex') ? 'none' : 'inline-flex';
        }
        function setCamFilter(filterCSS, el) {
            document.querySelectorAll('.filter-snap-item').forEach(i => i.classList.remove('active'));
            el.classList.add('active');
            selectedFilterStyle = filterCSS;
            document.getElementById('camera-stream').style.filter = filterCSS;
        }

        function toggleFlash() {
            flashModeState = !flashModeState;
            let btn = document.getElementById('flash-toggle-btn');
            if(flashModeState) { btn.classList.remove('flash-off-line'); btn.classList.add('flash-on'); }
            else { btn.classList.remove('flash-on'); btn.classList.add('flash-off-line'); }
        }

        function toggleTimerShelf() {
            let shelf = document.getElementById('timer-options-shelf');
            shelf.style.display = (shelf.style.display === 'flex') ? 'none' : 'flex';
        }
        function setTimerSecs(secs, el) {
            document.querySelectorAll('.timer-opt-btn').forEach(b => b.classList.remove('selected'));
            el.classList.add('selected');
            captureTimerSeconds = secs;
            let mainBtn = document.getElementById('timer-toggle-btn');
            if(secs > 0) mainBtn.classList.add('timer-active-btn');
            else mainBtn.classList.remove('timer-active-btn');
            toggleTimerShelf();
        }

        function handleCaptureAction() {
            if(captureTimerSeconds > 0) {
                let count = captureTimerSeconds;
                let overlay = document.getElementById('countdown-number');
                overlay.innerText = count;
                overlay.style.display = 'block';
                let interval = setInterval(() => {
                    count--;
                    if(count <= 0) {
                        clearInterval(interval);
                        overlay.style.display = 'none';
                        executeCoreCapturePipeline();
                    } else { overlay.innerText = count; }
                }, 1000);
            } else { executeCoreCapturePipeline(); }
        }

        function executeCoreCapturePipeline() {
            if(flashModeState) {
                let flash = document.getElementById('screen-flash-overlay');
                flash.style.display = 'block';
                setTimeout(() => { flash.style.display = 'none'; proceedToMockPreviewView(); }, 150);
            } else { proceedToMockPreviewView(); }
        }

        function proceedToMockPreviewView() {
            let pBox = document.getElementById('gallery-preview-box');
            pBox.style.display = 'flex';
            let imgWidget = document.getElementById('preview-media');
            let vidWidget = document.getElementById('preview-video');
            imgWidget.style.filter = selectedFilterStyle;
            vidWidget.style.filter = selectedFilterStyle;
            if(currentCamMode === 'photo') {
                imgWidget.src = "https://images.unsplash.com/photo-1618005182384-a83a8bd57fbe?w=500";
                imgWidget.style.display = 'block'; vidWidget.style.display = 'none';
            } else {
                vidWidget.src = "https://assets.mixkit.co/videos/preview/mixkit-neon-light-from-a-tunnel-41865-large.mp4";
                vidWidget.style.display = 'block'; imgWidget.style.display = 'none';
            }
        }

        function triggerHiddenGalleryInput() { document.getElementById('hidden-gallery-input').click(); }
        function handleGalleryFileSelected(input) {
            if(input.files && input.files[0]) { proceedToMockPreviewView(); }
        }

        function openTextEditorModal() { document.getElementById('text-editor-modal').style.display = 'flex'; }
        function closeTextEditorModal() { document.getElementById('text-editor-modal').style.display = 'none'; }
        function saveTextOverlay() {
            let txt = document.getElementById('media-custom-text-input').value;
            let col = document.getElementById('html-color-wheel').value;
            let display = document.getElementById('media-text-overlay');
            if(txt.trim() !== "") { display.innerText = txt; display.style.color = col; display.style.display = 'block'; }
            closeTextEditorModal();
        }

        function openEmojiPickerModal() {
            let modal = document.getElementById('emoji-picker-modal');
            modal.style.display = 'flex';
            let grid = document.getElementById('emoji-grid-container');
            if(grid.children.length === 0) {
                let emojis = ["😀","😂","🥰","😍","😎","🔥","👏","👍","💯","🎉","❤️","✨","🚀","👑","💀","💩","👽","🤖"];
                emojis.forEach(e => {
                    let item = document.createElement('div');
                    item.className = 'emoji-item-clickable'; item.innerText = e;
                    item.onclick = (event) => { event.stopPropagation(); spawnStickerOnPreview(e); closeEmojiPickerModal(); };
                    grid.appendChild(item);
                });
            }
        }
        function closeEmojiPickerModal() { document.getElementById('emoji-picker-modal').style.display = 'none'; }
        function spawnStickerOnPreview(emojiStr) {
            let st = document.createElement('div'); st.className = 'movable-emoji'; st.innerText = emojiStr;
            st.style.left = '40%'; st.style.top = '45%'; document.getElementById('sticker-container-zone').appendChild(st);
            setupDragAndDropElement(st);
        }

        function setupDragAndDropElement(el) {
            let posX = 0, posY = 0, initialX = 0, initialY = 0;
            el.onmousedown = (e) => { e.preventDefault(); initialX = e.clientX; initialY = e.clientY; document.onmouseup = closeDragElement; document.onmousemove = elementDrag; };
            el.ontouchstart = (e) => { initialX = e.touches[0].clientX; initialY = e.touches[0].clientY; document.ontouchend = closeDragElement; document.ontouchmove = elementTouchDrag; };
            function elementDrag(e) { e.preventDefault(); posX = initialX - e.clientX; posY = initialY - e.clientY; initialX = e.clientX; initialY = e.clientY; el.style.top = (el.offsetTop - posY) + "px"; el.style.left = (el.offsetLeft - posX) + "px"; }
            function elementTouchDrag(e) { posX = initialX - e.touches[0].clientX; posY = initialY - e.touches[0].clientY; initialX = e.touches[0].clientX; initialY = e.touches[0].clientY; el.style.top = (el.offsetTop - posY) + "px"; el.style.left = (el.offsetLeft - posX) + "px"; }
            function closeDragElement() { document.onmouseup = null; document.onmousemove = null; document.ontouchend = null; document.ontouchmove = null; }
        }
        setupDragAndDropElement(document.getElementById('media-text-overlay'));

        function openStepTwoDetails() {
            document.getElementById('details-post-panel').style.display = 'flex';
            let splitZone = document.getElementById('split-media-zone');
            splitZone.innerHTML = "";
            if(currentCamMode === 'photo') { splitZone.innerHTML = `<img src="${document.getElementById('preview-media').src}" style="width:100%;height:100%;object-fit:cover;">`; }
            else { splitZone.innerHTML = `<video src="${document.getElementById('preview-video').src}" autoplay loop muted style="width:100%;height:100%;object-fit:cover;"></video>`; }
        }
        function backToStepOne() { document.getElementById('details-post-panel').style.display = 'none'; }
        function closePreview() { document.getElementById('gallery-preview-box').style.display = 'none'; document.getElementById('details-post-panel').style.display = 'none'; exitCameraTab(); }
        function updateCharCount() {
            let len = document.getElementById('post-caption-input').value.length;
            document.getElementById('char-counter-txt').innerText = (999 - len) + " پیت ماون";
        }
        function insertAtCursor(char) {
            let txtArea = document.getElementById('post-caption-input');
            txtArea.value += char; txtArea.focus(); updateCharCount();
        }
        function finalPublishPost() { alert("Post Shared Successfully!"); closePreview(); }
        function quickPublishStory() { alert("Story Shared Successfully!"); closePreview(); }
        
        function handleSignIn(e) { e.preventDefault(); enterMainAppAndShowReels(); }
        function handleSignUp(e) { e.preventDefault(); navigateTo('signup-verify-screen'); }
        function verifyAndSave() { enterMainAppAndShowReels(); }
        
        function toggleZoomClick() { zoomIndex = (zoomIndex + 1) % zoomLevels.length; document.getElementById('zoom-toggle-btn').innerText = zoomLevels[zoomIndex] + "x"; }
        function setCamMode(mode, el) { document.querySelectorAll('.camera-mode-item').forEach(m => m.classList.remove('active')); el.classList.add('active'); currentCamMode = mode; }
    </script>
</body>
</html>
