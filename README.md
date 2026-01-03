<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>⚡ CYBER GAME BOOSTER PRO | Chuyên Gia Tối Ưu Game</title>
    <meta name="description" content="Công cụ tối ưu game chuyên nghiệp cấp độ hacker - Tăng FPS 200%, fix lag 95%, tiết kiệm pin 60 phút.">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&family=Share+Tech+Mono&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #00ff41;
            --secondary: #0088ff;
            --accent: #ff00ff;
            --danger: #ff3333;
            --warning: #ffaa00;
            --dark: #0a0a0f;
            --darker: #05050a;
            --terminal: #001100;
            --glow: 0 0 20px;
            --transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            -webkit-tap-highlight-color: transparent;
            -webkit-user-drag: none;
            user-select: none;
        }
        
        html, body {
            width: 100%;
            height: 100%;
            overflow: hidden;
            font-family: 'Share Tech Mono', monospace;
            background: var(--dark);
            color: var(--primary);
            position: fixed;
        }
        
        /* Cyber Container */
        .cyber-container {
            width: 100%;
            height: 100%;
            position: relative;
            overflow: hidden;
            background: 
                radial-gradient(circle at 20% 80%, rgba(0, 136, 255, 0.05) 0%, transparent 50%),
                radial-gradient(circle at 80% 20%, rgba(255, 0, 255, 0.05) 0%, transparent 50%),
                linear-gradient(var(--darker), var(--dark));
        }
        
        /* Grid Overlay */
        .grid-overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-image: 
                linear-gradient(rgba(0, 255, 65, 0.03) 1px, transparent 1px),
                linear-gradient(90deg, rgba(0, 255, 65, 0.03) 1px, transparent 1px);
            background-size: 30px 30px;
            pointer-events: none;
            z-index: 1;
        }
        
        /* Scan Lines */
        .scanlines {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(
                to bottom,
                transparent 50%,
                rgba(0, 255, 65, 0.02) 50%
            );
            background-size: 100% 4px;
            pointer-events: none;
            z-index: 2;
            opacity: 0.5;
        }
        
        /* Main App */
        .hacker-app {
            width: 100%;
            height: 100%;
            position: relative;
            z-index: 3;
            display: flex;
            flex-direction: column;
            padding: env(safe-area-inset-top) env(safe-area-inset-right) env(safe-area-inset-bottom) env(safe-area-inset-left);
        }
        
        /* Status Bar - iOS Style */
        .status-bar {
            padding: 10px 15px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            background: rgba(5, 5, 10, 0.95);
            backdrop-filter: blur(20px);
            border-bottom: 1px solid rgba(0, 255, 65, 0.1);
            position: sticky;
            top: 0;
            z-index: 100;
            font-family: -apple-system, BlinkMacSystemFont, sans-serif;
        }
        
        .time {
            font-weight: 600;
            font-size: 15px;
            color: var(--primary);
        }
        
        .signal-info {
            display: flex;
            align-items: center;
            gap: 15px;
            font-size: 14px;
        }
        
        /* Header */
        .cyber-header {
            padding: 25px 20px;
            text-align: center;
            position: relative;
            border-bottom: 1px solid rgba(0, 255, 65, 0.2);
            background: linear-gradient(180deg, rgba(10, 10, 15, 0.9) 0%, rgba(5, 5, 10, 0.7) 100%);
        }
        
        .app-title {
            font-family: 'Orbitron', sans-serif;
            font-size: 2.8rem;
            font-weight: 900;
            background: linear-gradient(135deg, var(--primary) 0%, var(--secondary) 50%, var(--accent) 100%);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            margin-bottom: 10px;
            letter-spacing: 3px;
            text-transform: uppercase;
            position: relative;
        }
        
        .app-title::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 25%;
            width: 50%;
            height: 3px;
            background: linear-gradient(90deg, transparent, var(--primary), transparent);
        }
        
        .app-subtitle {
            color: var(--secondary);
            font-size: 1.1rem;
            letter-spacing: 2px;
            margin-top: 15px;
        }
        
        /* Main Content */
        .main-content {
            flex: 1;
            overflow-y: auto;
            -webkit-overflow-scrolling: touch;
            padding: 20px 15px 100px 15px;
        }
        
        /* Performance Dashboard */
        .dashboard-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 15px;
            margin-bottom: 30px;
        }
        
        .metric-card {
            background: rgba(15, 20, 30, 0.8);
            border: 1px solid rgba(0, 136, 255, 0.3);
            border-radius: 16px;
            padding: 20px;
            position: relative;
            overflow: hidden;
            backdrop-filter: blur(10px);
            transition: var(--transition);
        }
        
        .metric-card:hover {
            transform: translateY(-5px);
            border-color: var(--primary);
            box-shadow: 0 10px 30px rgba(0, 255, 65, 0.2);
        }
        
        .metric-value {
            font-size: 3.5rem;
            font-weight: 700;
            font-family: 'Orbitron', sans-serif;
            color: var(--primary);
            text-shadow: var(--glow) rgba(0, 255, 65, 0.3);
            margin-bottom: 5px;
            line-height: 1;
        }
        
        .metric-label {
            color: var(--secondary);
            font-size: 0.9rem;
            text-transform: uppercase;
            letter-spacing: 1px;
        }
        
        .metric-trend {
            position: absolute;
            top: 15px;
            right: 15px;
            font-size: 0.8rem;
            padding: 3px 8px;
            border-radius: 10px;
            background: rgba(0, 255, 65, 0.1);
            color: var(--primary);
        }
        
        /* Optimization Modules */
        .modules-section {
            margin-bottom: 30px;
        }
        
        .section-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
            padding-bottom: 10px;
            border-bottom: 1px solid rgba(0, 255, 65, 0.1);
        }
        
        .section-title {
            font-size: 1.8rem;
            font-family: 'Orbitron', sans-serif;
            color: var(--primary);
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .modules-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 15px;
        }
        
        .module-card {
            background: rgba(20, 25, 40, 0.8);
            border: 1px solid rgba(0, 136, 255, 0.2);
            border-radius: 12px;
            padding: 20px;
            display: flex;
            align-items: center;
            gap: 15px;
            transition: var(--transition);
            position: relative;
            overflow: hidden;
        }
        
        .module-card:hover {
            transform: translateX(5px);
            border-color: var(--primary);
            background: rgba(25, 30, 45, 0.9);
        }
        
        .module-icon {
            width: 50px;
            height: 50px;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            border-radius: 12px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 24px;
            flex-shrink: 0;
            color: #000;
        }
        
        .module-info {
            flex: 1;
        }
        
        .module-name {
            font-size: 1.2rem;
            font-weight: bold;
            color: var(--primary);
            margin-bottom: 5px;
        }
        
        .module-desc {
            color: var(--secondary);
            font-size: 0.9rem;
            opacity: 0.8;
        }
        
        .module-status {
            font-size: 0.8rem;
            padding: 3px 10px;
            border-radius: 10px;
            background: rgba(0, 255, 65, 0.1);
            color: var(--primary);
        }
        
        /* Cyber Switch */
        .cyber-switch {
            position: relative;
            width: 60px;
            height: 30px;
            flex-shrink: 0;
        }
        
        .cyber-switch input {
            opacity: 0;
            width: 0;
            height: 0;
        }
        
        .switch-slider {
            position: absolute;
            cursor: pointer;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: rgba(0, 136, 255, 0.2);
            border: 2px solid var(--secondary);
            border-radius: 34px;
            transition: var(--transition);
        }
        
        .switch-slider:before {
            position: absolute;
            content: "";
            height: 22px;
            width: 22px;
            left: 2px;
            bottom: 2px;
            background: var(--secondary);
            border-radius: 50%;
            transition: var(--transition);
        }
        
        input:checked + .switch-slider {
            background: rgba(0, 255, 65, 0.3);
            border-color: var(--primary);
            box-shadow: 0 0 10px rgba(0, 255, 65, 0.5);
        }
        
        input:checked + .switch-slider:before {
            transform: translateX(30px);
            background: var(--primary);
            box-shadow: 0 0 10px var(--primary);
        }
        
        /* Progress Bars */
        .progress-section {
            margin: 30px 0;
        }
        
        .progress-item {
            margin-bottom: 20px;
        }
        
        .progress-header {
            display: flex;
            justify-content: space-between;
            margin-bottom: 8px;
            font-size: 1rem;
        }
        
        .progress-bar {
            height: 10px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 5px;
            overflow: hidden;
            position: relative;
        }
        
        .progress-fill {
            height: 100%;
            background: linear-gradient(90deg, var(--primary), var(--secondary));
            border-radius: 5px;
            width: 0%;
            transition: width 1s cubic-bezier(0.4, 0, 0.2, 1);
            position: relative;
            overflow: hidden;
        }
        
        .progress-fill::after {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
            animation: shine 2s infinite;
        }
        
        @keyframes shine {
            0% { transform: translateX(-100%); }
            100% { transform: translateX(100%); }
        }
        
        /* Action Panel */
        .action-panel {
            position: fixed;
            bottom: 0;
            left: 0;
            right: 0;
            background: rgba(5, 5, 10, 0.95);
            backdrop-filter: blur(20px);
            border-top: 1px solid rgba(0, 255, 65, 0.2);
            padding: 20px 15px;
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 15px;
            z-index: 100;
        }
        
        .cyber-button {
            background: linear-gradient(135deg, rgba(0, 136, 255, 0.2), rgba(0, 255, 65, 0.1));
            border: 2px solid var(--secondary);
            border-radius: 12px;
            padding: 18px 10px;
            color: var(--primary);
            font-family: 'Orbitron', sans-serif;
            font-size: 1rem;
            font-weight: bold;
            text-transform: uppercase;
            letter-spacing: 1px;
            cursor: pointer;
            transition: var(--transition);
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 8px;
            position: relative;
            overflow: hidden;
        }
        
        .cyber-button:hover {
            transform: translateY(-3px);
            border-color: var(--primary);
            box-shadow: 0 10px 20px rgba(0, 255, 65, 0.2);
        }
        
        .cyber-button:active {
            transform: translateY(0);
        }
        
        .cyber-button::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.1), transparent);
            transition: left 0.5s;
        }
        
        .cyber-button:hover::before {
            left: 100%;
        }
        
        .cyber-button.primary {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: #000;
            border-color: var(--primary);
            grid-column: span 3;
            padding: 22px 15px;
            font-size: 1.2rem;
        }
        
        .cyber-button.primary:hover {
            box-shadow: 0 10px 30px rgba(0, 255, 65, 0.4);
            background: linear-gradient(135deg, #00ff41, #0088ff, #ff00ff);
            animation: pulse 2s infinite;
        }
        
        @keyframes pulse {
            0%, 100% { box-shadow: 0 10px 30px rgba(0, 255, 65, 0.4); }
            50% { box-shadow: 0 10px 40px rgba(0, 255, 65, 0.6); }
        }
        
        /* Terminal Window */
        .terminal-window {
            background: rgba(0, 10, 5, 0.9);
            border: 1px solid rgba(0, 255, 65, 0.3);
            border-radius: 12px;
            padding: 20px;
            margin-top: 30px;
            font-family: 'Share Tech Mono', monospace;
            font-size: 0.9rem;
            line-height: 1.6;
            max-height: 300px;
            overflow-y: auto;
            position: relative;
        }
        
        .terminal-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 15px;
            padding-bottom: 10px;
            border-bottom: 1px solid rgba(0, 255, 65, 0.2);
        }
        
        .terminal-line {
            margin-bottom: 8px;
            color: var(--secondary);
            animation: typing 0.5s steps(40, end);
        }
        
        .terminal-line::before {
            content: ">> ";
            color: var(--primary);
            font-weight: bold;
        }
        
        .terminal-line.success { color: var(--primary); }
        .terminal-line.warning { color: var(--warning); }
        .terminal-line.error { color: var(--danger); }
        
        @keyframes typing {
            from { width: 0 }
            to { width: 100% }
        }
        
        /* Particle System */
        .particle {
            position: absolute;
            pointer-events: none;
            z-index: 2;
        }
        
        /* Mobile Responsive */
        @media (max-width: 768px) {
            .dashboard-grid {
                grid-template-columns: 1fr;
            }
            
            .modules-grid {
                grid-template-columns: 1fr;
            }
            
            .app-title {
                font-size: 2rem;
            }
            
            .metric-value {
                font-size: 2.8rem;
            }
        }
        
        /* iOS Safe Areas */
        @supports (padding: max(0px)) {
            .hacker-app {
                padding-top: max(env(safe-area-inset-top), 10px);
                padding-bottom: max(env(safe-area-inset-bottom), 10px);
            }
        }
        
        /* Performance Optimization */
        .will-change {
            will-change: transform, opacity;
        }
        
        /* Loading Animation */
        .loading-overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: var(--darker);
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            z-index: 9999;
            transition: opacity 0.5s;
        }
        
        .cyber-loader {
            width: 80px;
            height: 80px;
            position: relative;
            margin-bottom: 30px;
        }
        
        .loader-ring {
            width: 100%;
            height: 100%;
            border: 4px solid transparent;
            border-top-color: var(--primary);
            border-radius: 50%;
            animation: spin 1s linear infinite;
        }
        
        .loader-ring::after {
            content: '';
            position: absolute;
            top: 5px;
            left: 5px;
            right: 5px;
            bottom: 5px;
            border: 3px solid transparent;
            border-top-color: var(--secondary);
            border-radius: 50%;
            animation: spin 1.5s linear infinite reverse;
        }
        
        /* Notification System */
        .cyber-notification {
            position: fixed;
            top: 80px;
            right: 20px;
            background: rgba(0, 20, 10, 0.95);
            border: 1px solid var(--primary);
            border-radius: 12px;
            padding: 20px;
            max-width: 300px;
            transform: translateX(400px);
            transition: transform 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            z-index: 1000;
            backdrop-filter: blur(20px);
        }
        
        .cyber-notification.show {
            transform: translateX(0);
        }
        
        /* Custom Scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
        }
        
        ::-webkit-scrollbar-track {
            background: rgba(0, 255, 65, 0.05);
            border-radius: 4px;
        }
        
        ::-webkit-scrollbar-thumb {
            background: linear-gradient(var(--primary), var(--secondary));
            border-radius: 4px;
        }
    </style>
</head>
<body>
    <!-- Loading Screen -->
    <div class="loading-overlay" id="loadingScreen">
        <div class="cyber-loader">
            <div class="loader-ring"></div>
        </div>
        <h2 style="color: var(--primary); margin-bottom: 15px; font-family: 'Orbitron';">CYBER BOOSTER PRO</h2>
        <p style="color: var(--secondary); text-align: center; padding: 0 20px;">
            Initializing quantum optimization engine...
        </p>
    </div>
    
    <!-- Cyber Container -->
    <div class="cyber-container">
        <div class="grid-overlay"></div>
        <div class="scanlines"></div>
        
        <!-- Hacker App -->
        <div class="hacker-app">
            <!-- Status Bar -->
            <div class="status-bar">
                <div class="time" id="currentTime">12:00</div>
                <div class="signal-info">
                    <i class="fas fa-wifi" style="color: var(--primary);"></i>
                    <i class="fas fa-signal" style="color: var(--primary);"></i>
                    <span style="color: var(--primary);" id="batteryLevel">100%</span>
                    <i class="fas fa-battery-full" style="color: var(--primary);"></i>
                </div>
            </div>
            
            <!-- Header -->
            <div class="cyber-header">
                <h1 class="app-title">CYBER BOOSTER PRO</h1>
                <p class="app-subtitle">Professional Gaming Optimization Suite v5.0</p>
                <div style="margin-top: 15px; display: flex; justify-content: center; gap: 10px;">
                    <span style="background: rgba(0, 255, 65, 0.1); color: var(--primary); padding: 5px 15px; border-radius: 20px; font-size: 0.9rem;">
                        <i class="fas fa-shield-alt"></i> SECURE
                    </span>
                    <span style="background: rgba(0, 136, 255, 0.1); color: var(--secondary); padding: 5px 15px; border-radius: 20px; font-size: 0.9rem;">
                        <i class="fas fa-bolt"></i> ACTIVE
                    </span>
                </div>
            </div>
            
            <!-- Main Content -->
            <div class="main-content">
                <!-- Performance Dashboard -->
                <div class="dashboard-grid">
                    <div class="metric-card">
                        <div class="metric-value" id="currentFPS">60</div>
                        <div class="metric-label">FPS CURRENT</div>
                        <div class="metric-trend">+24%</div>
                    </div>
                    
                    <div class="metric-card">
                        <div class="metric-value" id="currentLatency">16ms</div>
                        <div class="metric-label">RESPONSE TIME</div>
                        <div class="metric-trend">-38%</div>
                    </div>
                    
                    <div class="metric-card">
                        <div class="metric-value" id="currentRAM">3.2GB</div>
                        <div class="metric-label">FREE MEMORY</div>
                        <div class="metric-trend">+1.8GB</div>
                    </div>
                    
                    <div class="metric-card">
                        <div class="metric-value" id="currentBattery">78%</div>
                        <div class="metric-label">BATTERY LIFE</div>
                        <div class="metric-trend">+45min</div>
                    </div>
                </div>
                
                <!-- Optimization Modules -->
                <div class="modules-section">
                    <div class="section-header">
                        <h2 class="section-title">
                            <i class="fas fa-microchip"></i> OPTIMIZATION MODULES
                        </h2>
                        <span style="color: var(--secondary); font-size: 0.9rem;">8/8 ACTIVE</span>
                    </div>
                    
                    <div class="modules-grid">
                        <!-- Module 1 -->
                        <div class="module-card">
                            <div class="module-icon">
                                <i class="fas fa-bolt"></i>
                            </div>
                            <div class="module-info">
                                <div class="module-name">ANIMATION REDUCTION</div>
                                <div class="module-desc">Increase FPS by 30%</div>
                            </div>
                            <label class="cyber-switch">
                                <input type="checkbox" checked data-module="1">
                                <span class="switch-slider"></span>
                            </label>
                        </div>
                        
                        <!-- Module 2 -->
                        <div class="module-card">
                            <div class="module-icon">
                                <i class="fas fa-tachometer-alt"></i>
                            </div>
                            <div class="module-info">
                                <div class="module-name">SENSITIVITY BOOST</div>
                                <div class="module-desc">+150% response speed</div>
                            </div>
                            <label class="cyber-switch">
                                <input type="checkbox" checked data-module="2">
                                <span class="switch-slider"></span>
                            </label>
                        </div>
                        
                        <!-- Module 3 -->
                        <div class="module-card">
                            <div class="module-icon">
                                <i class="fas fa-rocket"></i>
                            </div>
                            <div class="module-info">
                                <div class="module-name">FPS OVERCLOCK</div>
                                <div class="module-desc">Achieve 120+ FPS</div>
                            </div>
                            <label class="cyber-switch">
                                <input type="checkbox" checked data-module="3">
                                <span class="switch-slider"></span>
                            </label>
                        </div>
                        
                        <!-- Module 4 -->
                        <div class="module-card">
                            <div class="module-icon">
                                <i class="fas fa-shield-alt"></i>
                            </div>
                            <div class="module-info">
                                <div class="module-name">HEAVY GAME LAG FIX</div>
                                <div class="module-desc">Reduce lag by 90%</div>
                            </div>
                            <label class="cyber-switch">
                                <input type="checkbox" checked data-module="4">
                                <span class="switch-slider"></span>
                            </label>
                        </div>
                        
                        <!-- Module 5 -->
                        <div class="module-card">
                            <div class="module-icon">
                                <i class="fas fa-memory"></i>
                            </div>
                            <div class="module-info">
                                <div class="module-name">RAM MEMORY BOOST</div>
                                <div class="module-desc">Free up to 3GB+ RAM</div>
                            </div>
                            <label class="cyber-switch">
                                <input type="checkbox" checked data-module="5">
                                <span class="switch-slider"></span>
                            </label>
                        </div>
                        
                        <!-- Module 6 -->
                        <div class="module-card">
                            <div class="module-icon">
                                <i class="fas fa-hand-pointer"></i>
                            </div>
                            <div class="module-info">
                                <div class="module-name">TOUCH DELAY FIX</div>
                                <div class="module-desc">-80% touch latency</div>
                            </div>
                            <label class="cyber-switch">
                                <input type="checkbox" checked data-module="6">
                                <span class="switch-slider"></span>
                            </label>
                        </div>
                        
                        <!-- Module 7 -->
                        <div class="module-card">
                            <div class="module-icon">
                                <i class="fas fa-battery-full"></i>
                            </div>
                            <div class="module-info">
                                <div class="module-name">BATTERY SAVER</div>
                                <div class="module-desc">+60min play time</div>
                            </div>
                            <label class="cyber-switch">
                                <input type="checkbox" checked data-module="7">
                                <span class="switch-slider"></span>
                            </label>
                        </div>
                        
                        <!-- Module 8 -->
                        <div class="module-card">
                            <div class="module-icon">
                                <i class="fas fa-wifi"></i>
                            </div>
                            <div class="module-info">
                                <div class="module-name">INTERNET OPTIMIZATION</div>
                                <div class="module-desc">-70% network ping</div>
                            </div>
                            <label class="cyber-switch">
                                <input type="checkbox" checked data-module="8">
                                <span class="switch-slider"></span>
                            </label>
                        </div>
                    </div>
                </div>
                
                <!-- Progress Section -->
                <div class="progress-section">
                    <div class="section-header">
                        <h2 class="section-title">
                            <i class="fas fa-chart-line"></i> OPTIMIZATION PROGRESS
                        </h2>
                    </div>
                    
                    <div class="progress-item">
                        <div class="progress-header">
                            <span>FPS IMPROVEMENT</span>
                            <span id="fpsProgress">0%</span>
                        </div>
                        <div class="progress-bar">
                            <div class="progress-fill" id="fpsProgressBar"></div>
                        </div>
                    </div>
                    
                    <div class="progress-item">
                        <div class="progress-header">
                            <span>LATENCY REDUCTION</span>
                            <span id="latencyProgress">0%</span>
                        </div>
                        <div class="progress-bar">
                            <div class="progress-fill" id="latencyProgressBar"></div>
                        </div>
                    </div>
                    
                    <div class="progress-item">
                        <div class="progress-header">
                            <span>MEMORY OPTIMIZATION</span>
                            <span id="memoryProgress">0%</span>
                        </div>
                        <div class="progress-bar">
                            <div class="progress-fill" id="memoryProgressBar"></div>
                        </div>
                    </div>
                </div>
                
                <!-- Terminal Window -->
                <div class="terminal-window">
                    <div class="terminal-header">
                        <div style="color: var(--primary); font-weight: bold;">
                            <i class="fas fa-terminal"></i> SYSTEM TERMINAL
                        </div>
                        <div style="color: var(--secondary); font-size: 0.8rem;">
                            v5.0 | READY
                        </div>
                    </div>
                    <div id="terminalOutput">
                        <div class="terminal-line success">Cyber Booster Pro initialized</div>
                        <div class="terminal-line">Loading quantum optimization modules...</div>
                        <div class="terminal-line success">8/8 modules loaded successfully</div>
                        <div class="terminal-line">Device detected: Snapdragon 888 | 8GB RAM</div>
                        <div class="terminal-line">Current FPS: 60 | Target: 120+</div>
                        <div class="terminal-line">Network latency: 45ms | Target: &lt;20ms</div>
                        <div class="terminal-line warning">Optimization required for peak performance</div>
                        <div class="terminal-line">System ready. Awaiting commands...</div>
                    </div>
                </div>
            </div>
            
            <!-- Action Panel -->
            <div class="action-panel">
                <button class="cyber-button" id="scanBtn">
                    <i class="fas fa-search"></i>
                    <span>SCAN</span>
                </button>
                
                <button class="cyber-button" id="analyzeBtn">
                    <i class="fas fa-chart-bar"></i>
                    <span>ANALYZE</span>
                </button>
                
                <button class="cyber-button" id="settingsBtn">
                    <i class="fas fa-cog"></i>
                    <span>SETTINGS</span>
                </button>
                
                <button class="cyber-button primary" id="optimizeBtn">
                    <i class="fas fa-rocket"></i>
                    <span>LAUNCH OPTIMIZATION</span>
                </button>
            </div>
        </div>
    </div>
    
    <!-- Notification -->
    <div class="cyber-notification" id="notification">
        <div style="display: flex; align-items: center; gap: 15px; margin-bottom: 10px;">
            <i class="fas fa-check-circle" style="color: var(--primary); font-size: 1.5rem;"></i>
            <div>
                <div style="color: var(--primary); font-weight: bold; font-size: 1.1rem;" id="notifTitle">SUCCESS</div>
                <div style="color: var(--secondary); font-size: 0.9rem;" id="notifMessage">Operation completed</div>
            </div>
        </div>
        <div style="height: 3px; background: linear-gradient(90deg, var(--primary), transparent); border-radius: 2px; margin-top: 10px;"></div>
    </div>

    <script>
        // Khởi tạo biến
        let currentFPS = 60;
        let currentLatency = 16;
        let currentRAM = 2.4;
        let currentBattery = 78;
        let isOptimizing = false;
        let activeModules = 8;
        
        // DOM Elements
        const loadingScreen = document.getElementById('loadingScreen');
        const currentTimeElement = document.getElementById('currentTime');
        const batteryLevelElement = document.getElementById('batteryLevel');
        const currentFpsElement = document.getElementById('currentFPS');
        const currentLatencyElement = document.getElementById('currentLatency');
        const currentRamElement = document.getElementById('currentRAM');
        const currentBatteryElement = document.getElementById('currentBattery');
        const scanBtn = document.getElementById('scanBtn');
        const analyzeBtn = document.getElementById('analyzeBtn');
        const settingsBtn = document.getElementById('settingsBtn');
        const optimizeBtn = document.getElementById('optimizeBtn');
        const terminalOutput = document.getElementById('terminalOutput');
        const notification = document.getElementById('notification');
        const notifTitle = document.getElementById('notifTitle');
        const notifMessage = document.getElementById('notifMessage');
        
        // Progress elements
        const fpsProgress = document.getElementById('fpsProgress');
        const latencyProgress = document.getElementById('latencyProgress');
        const memoryProgress = document.getElementById('memoryProgress');
        const fpsProgressBar = document.getElementById('fpsProgressBar');
        const latencyProgressBar = document.getElementById('latencyProgressBar');
        const memoryProgressBar = document.getElementById('memoryProgressBar');
        
        // Module switches
        const moduleSwitches = document.querySelectorAll('.cyber-switch input');
        
        // Khởi tạo ứng dụng
        function initApp() {
            // Cập nhật thời gian
            updateTime();
            setInterval(updateTime, 60000);
            
            // Cập nhật pin
            updateBattery();
            setInterval(updateBattery, 30000);
            
            // Ẩn loading screen
            setTimeout(() => {
                loadingScreen.style.opacity = '0';
                setTimeout(() => {
                    loadingScreen.style.display = 'none';
                    showNotification('SYSTEM READY', 'Cyber Booster Pro initialized successfully');
                }, 500);
            }, 2000);
            
            // Khởi tạo sự kiện
            initEvents();
            
            // Tạo particle background
            initParticles();
        }
        
        // Cập nhật thời gian
        function updateTime() {
            const now = new Date();
            const hours = now.getHours().toString().padStart(2, '0');
            const minutes = now.getMinutes().toString().padStart(2, '0');
            currentTimeElement.textContent = `${hours}:${minutes}`;
        }
        
        // Cập nhật pin
        function updateBattery() {
            // Giả lập pin ngẫu nhiên
            let battery = parseInt(batteryLevelElement.textContent);
            if (battery > 20) {
                battery -= Math.random() > 0.8 ? 1 : 0;
            }
            batteryLevelElement.textContent = battery + '%';
            
            // Cập nhật icon pin
            const batteryIcon = document.querySelector('.fa-battery-full');
            if (battery > 70) {
                batteryIcon.className = 'fas fa-battery-full';
            } else if (battery > 40) {
                batteryIcon.className = 'fas fa-battery-three-quarters';
            } else if (battery > 20) {
                batteryIcon.className = 'fas fa-battery-half';
            } else {
                batteryIcon.className = 'fas fa-battery-quarter';
            }
        }
        
        // Khởi tạo sự kiện
        function initEvents() {
            // Module switch events
            moduleSwitches.forEach(switchEl => {
                switchEl.addEventListener('change', function() {
                    const moduleId = this.getAttribute('data-module');
                    const isActive = this.checked;
                    
                    // Cập nhật số module active
                    activeModules = document.querySelectorAll('.cyber-switch input:checked').length;
                    document.querySelector('.section-header span').textContent = `${activeModules}/8 ACTIVE`;
                    
                    // Hiệu ứng
                    const card = this.closest('.module-card');
                    card.classList.add('vibrate');
                    setTimeout(() => card.classList.remove('vibrate'), 300);
                    
                    // Thêm log terminal
                    const moduleName = card.querySelector('.module-name').textContent;
                    addTerminalLine(`${moduleName}: ${isActive ? 'ACTIVATED' : 'DEACTIVATED'}`, 
                        isActive ? 'success' : 'warning');
                    
                    // Hiệu ứng particle
                    const rect = card.getBoundingClientRect();
                    createParticles(rect.left + rect.width/2, rect.top + rect.height/2, 
                        isActive ? 'var(--primary)' : 'var(--danger)');
                });
            });
            
            // Scan button
            scanBtn.addEventListener('click', function() {
                if (isOptimizing) return;
                
                showNotification('SYSTEM SCAN', 'Analyzing hardware configuration...');
                
                // Hiệu ứng button
                this.classList.add('vibrate');
                setTimeout(() => this.classList.remove('vibrate'), 300);
                
                addTerminalLine('Initiating deep system scan...', 'warning');
                
                setTimeout(() => {
                    addTerminalLine('CPU: Qualcomm Snapdragon 888 detected', 'success');
                    setTimeout(() => {
                        addTerminalLine('GPU: Adreno 660 | 8GB RAM detected', 'success');
                        setTimeout(() => {
                            addTerminalLine('Storage: 256GB UFS 3.1 verified', 'success');
                            setTimeout(() => {
                                addTerminalLine('System scan complete. Ready for optimization.', 'success');
                                showNotification('SCAN COMPLETE', 'All hardware components verified');
                            }, 500);
                        }, 500);
                    }, 500);
                }, 500);
            });
            
            // Analyze button
            analyzeBtn.addEventListener('click', function() {
                showNotification('PERFORMANCE ANALYSIS', 'Calculating optimization potential...');
                
                // Hiệu ứng button
                this.classList.add('vibrate');
                setTimeout(() => this.classList.remove('vibrate'), 300);
                
                addTerminalLine('Analyzing performance metrics...', 'warning');
                
                // Tính toán potential
                const potential = Math.floor((activeModules / 8) * 100);
                const fpsPotential = Math.floor(potential * 0.8);
                const latencyPotential = Math.floor(potential * 0.6);
                const memoryPotential = Math.floor(potential * 0.5);
                
                // Cập nhật progress bars
                updateProgress(fpsPotential, latencyPotential, memoryPotential);
                
                setTimeout(() => {
                    addTerminalLine(`FPS improvement potential: ${fpsPotential}%`, 'success');
                    addTerminalLine(`Latency reduction potential: ${latencyPotential}%`, 'success');
                    addTerminalLine(`Memory optimization potential: ${memoryPotential}%`, 'success');
                    showNotification('ANALYSIS COMPLETE', `Optimization potential: ${potential}%`);
                }, 1500);
            });
            
            // Settings button
            settingsBtn.addEventListener('click', function() {
                showNotification('SETTINGS', 'Advanced configuration menu');
                
                // Hiệu ứng
                this.classList.add('vibrate');
                setTimeout(() => this.classList.remove('vibrate'), 300);
                
                addTerminalLine('Opening advanced configuration panel...', 'info');
                
                // Tạo modal settings
                createSettingsModal();
            });
            
            // Optimize button (MAIN)
            optimizeBtn.addEventListener('click', function() {
                if (isOptimizing) return;
                if (activeModules === 0) {
                    showNotification('ERROR', 'Please enable at least one optimization module');
                    return;
                }
                
                isOptimizing = true;
                showNotification('OPTIMIZATION INITIATED', 'Launching quantum optimization engine...');
                
                // Hiệu ứng button đặc biệt
                const originalHTML = this.innerHTML;
                this.innerHTML = '<i class="fas fa-cog fa-spin"></i><span>OPTIMIZING...</span>';
                this.classList.add('vibrate');
                
                // Thêm log terminal
                addTerminalLine('Launching full system optimization...', 'warning');
                addTerminalLine(`Active modules: ${activeModules}/8`, 'info');
                
                // Mô phỏng quá trình tối ưu hóa
                let step = 0;
                const steps = [
                    {name: 'ANIMATION REDUCTION', progress: 15},
                    {name: 'SENSITIVITY BOOST', progress: 30},
                    {name: 'FPS OVERCLOCK', progress: 45},
                    {name: 'HEAVY GAME LAG FIX', progress: 60},
                    {name: 'RAM MEMORY BOOST', progress: 75},
                    {name: 'TOUCH DELAY FIX', progress: 85},
                    {name: 'BATTERY SAVER', progress: 95},
                    {name: 'INTERNET OPTIMIZATION', progress: 100}
                ];
                
                // Chỉ thực hiện các bước tương ứng với module active
                const activeStepIndices = [];
                moduleSwitches.forEach((sw, idx) => {
                    if (sw.checked) activeStepIndices.push(idx);
                });
                
                const optimizeInterval = setInterval(() => {
                    if (step < activeStepIndices.length) {
                        const stepIdx = activeStepIndices[step];
                        const stepInfo = steps[stepIdx];
                        
                        // Cập nhật progress
                        updateProgress(stepInfo.progress, stepInfo.progress, stepInfo.progress);
                        
                        // Thêm log
                        addTerminalLine(`Applying ${stepInfo.name}...`, 'info');
                        
                        // Hiệu ứng particle
                        const moduleCard = document.querySelector(`[data-module="${stepIdx + 1}"]`).closest('.module-card');
                        const rect = moduleCard.getBoundingClientRect();
                        createParticles(rect.left + rect.width/2, rect.top + rect.height/2, 'var(--primary)');
                        
                        step++;
                    } else {
                        clearInterval(optimizeInterval);
                        
                        // Tính toán kết quả cuối cùng
                        const totalBoost = (activeModules / 8) * 100;
                        const newFPS = Math.min(120, 60 + totalBoost * 0.6);
                        const newLatency = Math.max(4, 16 - totalBoost * 0.12);
                        const newRAM = Math.min(8, 2.4 + totalBoost * 0.03);
                        const newBattery = Math.min(100, 78 + totalBoost * 0.2);
                        
                        // Cập nhật giá trị
                        currentFPS = newFPS;
                        currentLatency = newLatency;
                        currentRAM = newRAM;
                        currentBattery = newBattery;
                        
                        currentFpsElement.textContent = Math.round(newFPS);
                        currentLatencyElement.textContent = Math.round(newLatency) + 'ms';
                        currentRamElement.textContent = newRAM.toFixed(1) + 'GB';
                        currentBatteryElement.textContent = Math.round(newBattery) + '%';
                        
                        // Cập nhật progress hoàn thành
                        updateProgress(100, 100, 100);
                        
                        // Thêm log hoàn thành
                        addTerminalLine('OPTIMIZATION COMPLETE!', 'success');
                        addTerminalLine(`FPS: ${Math.round(newFPS)} | Latency: ${Math.round(newLatency)}ms | RAM: ${newRAM.toFixed(1)}GB`, 'success');
                        
                        // Khôi phục button
                        setTimeout(() => {
                            this.innerHTML = originalHTML;
                            this.classList.remove('vibrate');
                            isOptimizing = false;
                        }, 1000);
                        
                        // Hiệu ứng confetti
                        createConfetti();
                        
                        // Notification
                        showNotification('OPTIMIZATION SUCCESSFUL', 
                            `Performance improved by ${Math.round(totalBoost)}%`);
                    }
                }, 800);
            });
        }
        
        // Tạo particle system
        function initParticles() {
            // Tạo background particles
            for (let i = 0; i < 50; i++) {
                setTimeout(() => {
                    createBackgroundParticle();
                }, i * 100);
            }
        }
        
        function createBackgroundParticle() {
            const particle = document.createElement('div');
            particle.className = 'particle';
            particle.style.cssText = `
                width: 2px;
                height: 2px;
                background: var(--primary);
                border-radius: 50%;
                left: ${Math.random() * 100}%;
                top: ${Math.random() * 100}%;
                opacity: ${Math.random() * 0.3 + 0.1};
            `;
            
            document.querySelector('.cyber-container').appendChild(particle);
            
            // Animation
            const duration = Math.random() * 10000 + 5000;
            const animation = particle.animate([
                { transform: 'translate(0, 0)', opacity: 0.1 },
                { transform: `translate(${Math.random() * 100 - 50}px, ${Math.random() * 100 - 50}px)`, opacity: 0.4 },
                { transform: 'translate(0, 0)', opacity: 0.1 }
            ], {
                duration: duration,
                iterations: Infinity,
                easing: 'ease-in-out'
            });
        }
        
        function createParticles(x, y, color) {
            for (let i = 0; i < 20; i++) {
                const particle = document.createElement('div');
                particle.className = 'particle';
                particle.style.cssText = `
                    width: 4px;
                    height: 4px;
                    background: ${color};
                    border-radius: 50%;
                    left: ${x}px;
                    top: ${y}px;
                `;
                
                document.body.appendChild(particle);
                
                // Animation
                const animation = particle.animate([
                    { transform: 'scale(1) translate(0, 0)', opacity: 1 },
                    { transform: `scale(0) translate(${Math.random() * 100 - 50}px, ${Math.random() * 100 - 50}px)`, opacity: 0 }
                ], {
                    duration: Math.random() * 1000 + 500,
                    easing: 'cubic-bezier(0.2, 0, 0.8, 1)'
                });
                
                animation.onfinish = () => particle.remove();
            }
        }
        
        // Thêm dòng terminal
        function addTerminalLine(text, type = '') {
            const line = document.createElement('div');
            line.className = `terminal-line ${type}`;
            line.textContent = text;
            terminalOutput.appendChild(line);
            terminalOutput.scrollTop = terminalOutput.scrollHeight;
        }
        
        // Cập nhật progress
        function updateProgress(fpsVal, latencyVal, memoryVal) {
            fpsProgress.textContent = fpsVal + '%';
            latencyProgress.textContent = latencyVal + '%';
            memoryProgress.textContent = memoryVal + '%';
            
            fpsProgressBar.style.width = fpsVal + '%';
            latencyProgressBar.style.width = latencyVal + '%';
            memoryProgressBar.style.width = memoryVal + '%';
        }
        
        // Hiển thị notification
        function showNotification(title, message, duration = 3000) {
            notifTitle.textContent = title;
            notifMessage.textContent = message;
            
            notification.classList.add('show');
            
            setTimeout(() => {
                notification.classList.remove('show');
            }, duration);
        }
        
        // Tạo confetti effect
        function createConfetti() {
            const colors = ['var(--primary)', 'var(--secondary)', 'var(--accent)', 'var(--warning)'];
            
            for (let i = 0; i < 50; i++) {
                setTimeout(() => {
                    const confetti = document.createElement('div');
                    confetti.style.cssText = `
                        position: fixed;
                        width: 10px;
                        height: 10px;
                        background: ${colors[Math.floor(Math.random() * colors.length)]};
                        border-radius: 50%;
                        top: -20px;
                        left: ${Math.random() * 100}%;
                        z-index: 9999;
                        pointer-events: none;
                    `;
                    
                    document.body.appendChild(confetti);
                    
                    // Animation
                    const animation = confetti.animate([
                        { transform: 'translateY(0) rotate(0deg)', opacity: 1 },
                        { transform: `translateY(${window.innerHeight + 20}px) rotate(${Math.random() * 360}deg)`, opacity: 0 }
                    ], {
                        duration: Math.random() * 2000 + 1000,
                        easing: 'cubic-bezier(0.2, 0, 0.8, 1)'
                    });
                    
                    animation.onfinish = () => confetti.remove();
                }, i * 50);
            }
        }
        
        // Tạo settings modal
        function createSettingsModal() {
            const modal = document.createElement('div');
            modal.style.cssText = `
                position: fixed;
                top: 0;
                left: 0;
                right: 0;
                bottom: 0;
                background: rgba(0, 0, 0, 0.9);
                display: flex;
                align-items: center;
                justify-content: center;
                z-index: 10000;
                backdrop-filter: blur(10px);
            `;
            
            modal.innerHTML = `
                <div style="
                    background: rgba(10, 15, 25, 0.95);
                    border: 2px solid var(--primary);
                    border-radius: 20px;
                    padding: 30px;
                    max-width: 500px;
                    width: 90%;
                    max-height: 80vh;
                    overflow-y: auto;
                ">
                    <div style="display: flex; justify-content: space-between; align-items: center; margin-bottom: 30px;">
                        <h2 style="color: var(--primary); font-family: 'Orbitron';">ADVANCED SETTINGS</h2>
                        <button id="closeSettings" style="
                            background: none;
                            border: none;
                            color: var(--primary);
                            font-size: 1.5rem;
                            cursor: pointer;
                        ">&times;</button>
                    </div>
                    
                    <div style="margin-bottom: 25px;">
                        <h3 style="color: var(--secondary); margin-bottom: 15px;">Performance Mode</h3>
                        <div style="display: flex; gap: 10px;">
                            <button class="mode-btn" data-mode="balanced" style="
                                flex: 1;
                                padding: 15px;
                                background: rgba(0, 136, 255, 0.1);
                                border: 1px solid var(--secondary);
                                border-radius: 10px;
                                color: var(--secondary);
                                cursor: pointer;
                            ">Balanced</button>
                            <button class="mode-btn" data-mode="performance" style="
                                flex: 1;
                                padding: 15px;
                                background: rgba(0, 255, 65, 0.1);
                                border: 1px solid var(--primary);
                                border-radius: 10px;
                                color: var(--primary);
                                cursor: pointer;
                            ">Performance</button>
                            <button class="mode-btn" data-mode="extreme" style="
                                flex: 1;
                                padding: 15px;
                                background: rgba(255, 0, 255, 0.1);
                                border: 1px solid var(--accent);
                                border-radius: 10px;
                                color: var(--accent);
                                cursor: pointer;
                            ">Extreme</button>
                        </div>
                    </div>
                    
                    <div style="margin-bottom: 25px;">
                        <h3 style="color: var(--secondary); margin-bottom: 15px;">Game Profiles</h3>
                        <div style="display: grid; grid-template-columns: repeat(2, 1fr); gap: 10px;">
                            <button class="game-profile" data-game="pubg" style="
                                padding: 10px;
                                background: rgba(255, 255, 255, 0.05);
                                border: 1px solid rgba(255, 255, 255, 0.1);
                                border-radius: 8px;
                                color: var(--secondary);
                                cursor: pointer;
                                display: flex;
                                align-items: center;
                                gap: 10px;
                            "><span>🎮</span> PUBG</button>
                            <button class="game-profile" data-game="cod" style="
                                padding: 10px;
                                background: rgba(255, 255, 255, 0.05);
                                border: 1px solid rgba(255, 255, 255, 0.1);
                                border-radius: 8px;
                                color: var(--secondary);
                                cursor: pointer;
                                display: flex;
                                align-items: center;
                                gap: 10px;
                            "><span>🔫</span> COD</button>
                            <button class="game-profile" data-game="freefire" style="
                                padding: 10px;
                                background: rgba(255, 255, 255, 0.05);
                                border: 1px solid rgba(255, 255, 255, 0.1);
                                border-radius: 8px;
                                color: var(--secondary);
                                cursor: pointer;
                                display: flex;
                                align-items: center;
                                gap: 10px;
                            "><span>🔥</span> Free Fire</button>
                            <button class="game-profile" data-game="mlbb" style="
                                padding: 10px;
                                background: rgba(255, 255, 255, 0.05);
                                border: 1px solid rgba(255, 255, 255, 0.1);
                                border-radius: 8px;
                                color: var(--secondary);
                                cursor: pointer;
                                display: flex;
                                align-items: center;
                                gap: 10px;
                            "><span>⚔️</span> MLBB</button>
                        </div>
                    </div>
                    
                    <div style="margin-bottom: 25px;">
                        <h3 style="color: var(--secondary); margin-bottom: 15px;">Advanced Options</h3>
                        <div style="display: flex; flex-direction: column; gap: 15px;">
                            <label style="display: flex; justify-content: space-between; align-items: center;">
                                <span style="color: var(--secondary);">Auto-optimize on game launch</span>
                                <label class="cyber-switch">
                                    <input type="checkbox" id="autoOptimize">
                                    <span class="switch-slider"></span>
                                </label>
                            </label>
                            <label style="display: flex; justify-content: space-between; align-items: center;">
                                <span style="color: var(--secondary);">Background service</span>
                                <label class="cyber-switch">
                                    <input type="checkbox" id="backgroundService" checked>
                                    <span class="switch-slider"></span>
                                </label>
                            </label>
                            <label style="display: flex; justify-content: space-between; align-items: center;">
                                <span style="color: var(--secondary);">Performance monitoring</span>
                                <label class="cyber-switch">
                                    <input type="checkbox" id="performanceMonitor" checked>
                                    <span class="switch-slider"></span>
                                </label>
                            </label>
                        </div>
                    </div>
                    
                    <button id="saveSettings" style="
                        width: 100%;
                        padding: 15px;
                        background: linear-gradient(135deg, var(--primary), var(--secondary));
                        border: none;
                        border-radius: 12px;
                        color: #000;
                        font-family: 'Orbitron';
                        font-weight: bold;
                        font-size: 1.1rem;
                        cursor: pointer;
                        margin-top: 20px;
                    ">SAVE SETTINGS</button>
                </div>
            `;
            
            document.body.appendChild(modal);
            
            // Close button
            modal.querySelector('#closeSettings').addEventListener('click', () => {
                modal.remove();
            });
            
            // Mode buttons
            modal.querySelectorAll('.mode-btn').forEach(btn => {
                btn.addEventListener('click', function() {
                    modal.querySelectorAll('.mode-btn').forEach(b => {
                        b.style.background = 'rgba(0, 136, 255, 0.1)';
                        b.style.borderColor = 'var(--secondary)';
                        b.style.color = 'var(--secondary)';
                    });
                    
                    this.style.background = 'linear-gradient(135deg, var(--primary), var(--secondary))';
                    this.style.borderColor = 'var(--primary)';
                    this.style.color = '#000';
                    
                    addTerminalLine(`Performance mode changed to: ${this.dataset.mode.toUpperCase()}`, 'info');
                });
            });
            
            // Game profiles
            modal.querySelectorAll('.game-profile').forEach(btn => {
                btn.addEventListener('click', function() {
                    const game = this.dataset.game;
                    addTerminalLine(`Game profile loaded: ${game.toUpperCase()}`, 'success');
                    showNotification('PROFILE LOADED', `Optimized settings for ${game}`);
                });
            });
            
            // Save settings
            modal.querySelector('#saveSettings').addEventListener('click', () => {
                addTerminalLine('Settings saved successfully', 'success');
                showNotification('SETTINGS SAVED', 'Configuration updated');
                modal.remove();
            });
            
            // Click outside to close
            modal.addEventListener('click', (e) => {
                if (e.target === modal) {
                    modal.remove();
                }
            });
        }
        
        // Thêm CSS cho vibrate animation
        const style = document.createElement('style');
        style.textContent = `
            @keyframes vibrate {
                0% { transform: translateX(0); }
                25% { transform: translateX(-2px); }
                50% { transform: translateX(2px); }
                75% { transform: translateX(-2px); }
                100% { transform: translateX(0); }
            }
            
            .vibrate {
                animation: vibrate 0.3s linear;
            }
        `;
        document.head.appendChild(style);
        
        // Khởi chạy ứng dụng
        document.addEventListener('DOMContentLoaded', initApp);
        
        // PWA features
        window.addEventListener('beforeinstallprompt', (e) => {
            e.preventDefault();
            // Có thể lưu event để hiển thị nút cài đặt
        });
        
        // Ngăn pull-to-refresh trên mobile
        document.addEventListener('touchmove', function(e) {
            if (e.scale !== 1) {
                e.preventDefault();
            }
        }, { passive: false });
    </script>
</body>
</html># df
