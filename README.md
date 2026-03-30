<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="google-site-verification" content="iNLP5cp2ovjMTi5QvEe5JaMz7EpHTZwCIPSk6s-Yjnw" />
    <meta name="description" content="SZ GAMES - Play 100+ free online games including action, puzzle, adventure, strategy and sports games. No downloads required!">
    <meta name="keywords" content="free games, online games, play games, SZ GAMES, game portal">
    <meta name="author" content="SZ GAMES">
    <meta property="og:title" content="SZ GAMES - 100+ Free Online Games">
    <meta property="og:description" content="Play 100+ free games on SZ GAMES. Action, puzzle, adventure, strategy and sports games available.">
    <meta property="og:type" content="website">
    <title>SZ GAMES - Play 100+ Free Online Games</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --primary: #0a0e27;
            --secondary: #1a1f3a;
            --accent: #00d4ff;
            --highlight: #ff006e;
            --success: #00ff88;
            --text: #e8eef7;
            --text-muted: #a0a8c0;
            --border: #2a3050;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            background: linear-gradient(135deg, #0a0e27 0%, #1a1f3a 50%, #0f1428 100%);
            background-attachment: fixed;
            color: var(--text);
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            min-height: 100vh;
            overflow-x: hidden;
            /* Adjusted padding to match the new fixed container height */
            padding-top: 450px;
        }

        body::before {
            content: '';
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: radial-gradient(circle at 20% 50%, rgba(0, 212, 255, 0.05) 0%, transparent 50%),
                        radial-gradient(circle at 80% 80%, rgba(255, 0, 110, 0.05) 0%, transparent 50%);
            pointer-events: none;
            z-index: 0;
        }

        /* Combined Fixed Container */
        .fixed-header-container {
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            z-index: 100;
            transition: transform 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            background: linear-gradient(135deg, rgba(10, 14, 39, 0.98) 0%, rgba(26, 31, 58, 0.98) 100%);
            backdrop-filter: blur(15px);
            border-bottom: 2px solid var(--accent);
            box-shadow: 0 8px 32px rgba(0, 212, 255, 0.15);
        }

        .fixed-header-container.hide {
            transform: translateY(-100%);
        }

        .header {
            padding: 20px 20px;
            text-align: center;
        }

        .header-content {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .logo-container {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 15px;
            cursor: pointer;
            transition: all 0.3s ease;
            margin-bottom: 10px;
        }

        .logo-container:hover {
            transform: scale(1.05);
        }

        .logo-icon {
            width: 60px;
            height: 60px;
            fill: url(#logo-gradient);
            filter: drop-shadow(0 0 15px rgba(0, 212, 255, 0.5));
        }

        .logo {
            font-size: 3.5em;
            font-weight: 900;
            background: linear-gradient(135deg, var(--accent) 0%, var(--highlight) 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            text-shadow: 0 0 30px rgba(0, 212, 255, 0.3);
            letter-spacing: 2px;
        }

        .tagline {
            color: var(--accent);
            font-size: 1.1em;
            text-shadow: 0 0 15px rgba(0, 212, 255, 0.2);
            font-weight: 500;
        }

        .nav-wrapper {
            border-top: 1px solid var(--border);
            border-bottom: 1px solid var(--border);
            padding: 10px 0;
        }

        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            gap: 15px;
            flex-wrap: wrap;
            justify-content: center;
            align-items: center;
            padding: 5px 20px;
        }

        .nav-links {
            display: flex;
            gap: 10px;
            flex-wrap: wrap;
            justify-content: center;
        }

        .nav-links button, .nav-links a {
            padding: 10px 20px;
            background: rgba(0, 212, 255, 0.1);
            border: 2px solid var(--accent);
            color: var(--accent);
            border-radius: 25px;
            cursor: pointer;
            font-weight: 600;
            transition: all 0.3s ease;
            font-size: 0.95em;
            text-decoration: none;
        }

        .nav-links button:hover, .nav-links a:hover,
        .nav-links button.active, .nav-links a.active {
            background: var(--accent);
            color: var(--primary);
            box-shadow: 0 0 20px rgba(0, 212, 255, 0.5);
            transform: translateY(-2px);
        }

        .search-container {
            flex: 1;
            min-width: 250px;
            max-width: 400px;
        }

        .search-input {
            width: 100%;
            padding: 12px 20px;
            background: rgba(10, 14, 39, 0.8);
            border: 2px solid var(--accent);
            color: var(--text);
            border-radius: 25px;
            font-size: 1em;
            transition: all 0.3s;
        }

        .search-input:focus {
            outline: none;
            box-shadow: 0 0 20px rgba(0, 212, 255, 0.4);
            border-color: var(--highlight);
        }

        .search-input::placeholder {
            color: var(--text-muted);
        }

        .filter-wrapper {
            padding: 15px 0;
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .filter-container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            gap: 10px;
            flex-wrap: wrap;
            justify-content: center;
        }

        .filter-btn {
            padding: 10px 20px;
            background: rgba(255, 0, 110, 0.15);
            border: 2px solid var(--highlight);
            color: var(--highlight);
            border-radius: 20px;
            cursor: pointer;
            font-weight: 600;
            transition: all 0.3s;
            font-size: 0.9em;
        }

        .filter-btn:hover,
        .filter-btn.active {
            background: var(--highlight);
            color: white;
            box-shadow: 0 0 20px rgba(255, 0, 110, 0.5);
            transform: scale(1.05);
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 40px 20px;
            position: relative;
            z-index: 1;
        }

        .page {
            display: none;
            animation: fadeIn 0.5s ease;
        }

        .page.active {
            display: block;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .games-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(260px, 1fr));
            gap: 25px;
            margin-bottom: 50px;
        }

        .game-card {
            background: linear-gradient(135deg, rgba(26, 31, 58, 0.8) 0%, rgba(15, 20, 40, 0.8) 100%);
            border: 2px solid var(--border);
            border-radius: 15px;
            overflow: hidden;
            cursor: pointer;
            transition: all 0.3s ease;
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.3);
            position: relative;
        }

        .game-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(0, 212, 255, 0.2), transparent);
            transition: left 0.5s;
            z-index: 1;
        }

        .game-card:hover::before {
            left: 100%;
        }

        .game-card:hover {
            transform: translateY(-10px);
            border-color: var(--accent);
            box-shadow: 0 15px 40px rgba(0, 212, 255, 0.3);
        }

        .game-card-image {
            width: 100%;
            height: 180px;
            background: linear-gradient(135deg, rgba(0, 212, 255, 0.1) 0%, rgba(255, 0, 110, 0.1) 100%);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 4em;
            position: relative;
            overflow: hidden;
        }

        .game-card-image::after {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: linear-gradient(45deg, transparent 30%, rgba(0, 212, 255, 0.1) 50%, transparent 70%);
            animation: shimmer 3s infinite;
        }

        @keyframes shimmer {
            0% { transform: translateX(-100%); }
            100% { transform: translateX(100%); }
        }

        .game-card-content {
            padding: 20px;
            position: relative;
            z-index: 2;
        }

        .game-card h3 {
            font-size: 1.4em;
            margin-bottom: 10px;
            color: var(--accent);
        }

        .game-card p {
            color: var(--text-muted);
            font-size: 0.95em;
            line-height: 1.5;
            margin-bottom: 15px;
        }

        .game-card-footer {
            display: flex;
            justify-content: space-between;
            align-items: center;
            border-top: 1px solid var(--border);
            padding-top: 15px;
        }

        .game-category {
            font-size: 0.8em;
            color: var(--highlight);
            font-weight: 700;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .play-btn {
            padding: 8px 16px;
            background: var(--accent);
            color: var(--primary);
            border-radius: 20px;
            font-weight: 700;
            font-size: 0.85em;
            transition: all 0.3s;
        }

        /* Modal / Game Player */
        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(10, 14, 39, 0.98);
            z-index: 1000;
            backdrop-filter: blur(10px);
        }

        .modal-content {
            position: relative;
            width: 95%;
            max-width: 1200px;
            height: 85vh;
            margin: 2.5vh auto;
            background: var(--secondary);
            border: 2px solid var(--accent);
            border-radius: 20px;
            overflow: hidden;
            box-shadow: 0 0 50px rgba(0, 212, 255, 0.3);
            display: flex;
            flex-direction: column;
        }

        .modal-header {
            padding: 15px 25px;
            background: var(--primary);
            display: flex;
            justify-content: space-between;
            align-items: center;
            border-bottom: 2px solid var(--border);
        }

        .modal-title {
            font-size: 1.5em;
            font-weight: 700;
            color: var(--accent);
        }

        .close-modal {
            font-size: 2em;
            color: var(--text-muted);
            cursor: pointer;
            transition: color 0.3s;
        }

        .close-modal:hover {
            color: var(--highlight);
        }

        .game-frame-container {
            flex: 1;
            position: relative;
            background: #000;
        }

        iframe {
            width: 100%;
            height: 100%;
            border: none;
        }

        .game-info-bar {
            padding: 15px 25px;
            background: var(--primary);
            border-top: 2px solid var(--border);
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        /* Content Pages */
        .content-page {
            background: rgba(26, 31, 58, 0.8);
            border: 2px solid var(--border);
            border-radius: 20px;
            padding: 40px;
            margin-top: 20px;
        }

        .content-page h2 {
            color: var(--accent);
            font-size: 2.5em;
            margin-bottom: 25px;
            border-bottom: 2px solid var(--accent);
            padding-bottom: 15px;
            display: inline-block;
        }

        .content-page p {
            line-height: 1.8;
            margin-bottom: 20px;
            font-size: 1.1em;
            color: var(--text);
        }

        .content-page h3 {
            color: var(--highlight);
            font-size: 1.5em;
            margin: 30px 0 15px 0;
        }

        .content-page ul {
            margin-left: 25px;
            margin-bottom: 15px;
        }

        .content-page li {
            margin-bottom: 12px;
            color: var(--text);
            line-height: 1.6;
        }

        .contact-form {
            margin-top: 30px;
        }

        .form-group {
            margin-bottom: 25px;
        }

        .form-group label {
            display: block;
            margin-bottom: 10px;
            color: var(--accent);
            font-weight: 700;
            font-size: 1.05em;
        }

        .form-group input,
        .form-group textarea {
            width: 100%;
            padding: 15px;
            background: rgba(10, 14, 39, 0.8);
            border: 2px solid var(--border);
            color: var(--text);
            border-radius: 8px;
            font-family: inherit;
            font-size: 1em;
            transition: all 0.3s;
        }

        .form-group input:focus,
        .form-group textarea:focus {
            outline: none;
            box-shadow: 0 0 20px rgba(0, 212, 255, 0.3);
            border-color: var(--accent);
        }

        .form-group textarea {
            resize: vertical;
            min-height: 150px;
        }

        .submit-btn {
            width: 100%;
            padding: 15px;
            background: linear-gradient(135deg, var(--accent) 0%, var(--highlight) 100%);
            color: white;
            border: none;
            border-radius: 8px;
            font-weight: 700;
            cursor: pointer;
            font-size: 1.1em;
            transition: all 0.3s;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .submit-btn:hover {
            box-shadow: 0 8px 25px rgba(0, 212, 255, 0.4);
            transform: scale(1.02);
        }

        .footer {
            background: linear-gradient(135deg, rgba(10, 14, 39, 0.95) 0%, rgba(26, 31, 58, 0.95) 100%);
            border-top: 2px solid var(--accent);
            padding: 40px 20px;
            text-align: center;
            color: var(--text-muted);
            margin-top: 60px;
        }

        .footer-content {
            max-width: 1200px;
            margin: 0 auto;
        }

        .footer p {
            margin-bottom: 12px;
            font-size: 1.05em;
        }

        .footer-links {
            display: flex;
            justify-content: center;
            gap: 25px;
            margin-top: 20px;
            flex-wrap: wrap;
        }

        .footer-links a {
            color: var(--accent);
            text-decoration: none;
            transition: all 0.3s;
            cursor: pointer;
            font-weight: 600;
        }

        .footer-links a:hover {
            color: var(--highlight);
            text-shadow: 0 0 15px rgba(0, 212, 255, 0.4);
        }

        .no-games {
            text-align: center;
            padding: 60px 20px;
            color: var(--text-muted);
            font-size: 1.3em;
        }

        .sidebar-ads {
            display: none;
        }

        .sidebar-ad {
            display: none;
        }

        .side-ad {
            position: fixed;
            top: 200px;
            z-index: 50;
            background: rgba(26, 31, 58, 0.9);
            border: 2px solid var(--border);
            border-radius: 10px;
            padding: 10px;
        }

        .side-ad-left {
            left: 10px;
        }

        .side-ad-right {
            right: 10px;
        }

        @media (max-width: 1024px) {
            .side-ad {
                display: none;
            }
        }

        @media (max-width: 768px) {
            body {
                padding-top: 550px; /* More padding for mobile as items stack */
            }

            .logo {
                font-size: 2.2em;
            }

            .logo-icon {
                width: 40px;
                height: 40px;
            }

            .games-grid {
                grid-template-columns: repeat(auto-fill, minmax(180px, 1fr));
                gap: 15px;
            }

            .nav-container {
                flex-direction: column;
            }

            .search-container {
                max-width: 100%;
            }

            .modal-content {
                height: 95vh;
            }

            .content-page {
                padding: 25px;
            }

            .content-page h2 {
                font-size: 1.8em;
            }

            .filter-container {
                overflow-x: auto;
                padding-bottom: 10px;
            }
        }
    </style>
</head>
<body>
    <!-- SVG Gradient Definition -->
    <svg style="width:0;height:0;position:absolute;" aria-hidden="true" focusable="false">
        <linearGradient id="logo-gradient" x1="0%" y1="0%" x2="100%" y2="100%">
            <stop offset="0%" stop-color="#00d4ff" />
            <stop offset="100%" stop-color="#ff006e" />
        </linearGradient>
    </svg>

    <!-- Combined Fixed Container -->
    <div class="fixed-header-container" id="mainHeader">
        <!-- Adsterra Ad at the very top -->
        <div style="text-align: center; padding: 10px 0; background: rgba(26, 31, 58, 0.4); border-bottom: 1px solid var(--border);">
            <script>
              atOptions = {
                'key' : '6d5fc2bb86a2405e48f209077365fea6',
                'format' : 'iframe',
                'height' : 90,
                'width' : 728,
                'params' : {}
              };
            </script>
            <script src="https://www.highperformanceformat.com/6d5fc2bb86a2405e48f209077365fea6/invoke.js"></script>
        </div>

        <!-- Header -->
        <div class="header">
            <div class="header-content">
                <div class="logo-container" onclick="showPage('home')">
                    <svg class="logo-icon" viewBox="0 0 24 24">
                        <path d="M21,6H3C1.9,6,1,6.9,1,8v8c0,1.1,0.9,2,2,2h18c1.1,0,2-0.9,2-2V8C23,6.9,22.1,6,21,6z M11,15H9v-2H7v-2h2V9h2v2h2v2h-2V15z M16.5,15c-0.8,0-1.5-0.7-1.5-1.5s0.7-1.5,1.5-1.5s1.5,0.7,1.5,1.5S17.3,15,16.5,15z M19.5,12c-0.8,0-1.5-0.7-1.5-1.5 s0.7-1.5,1.5-1.5s1.5,0.7,1.5,1.5S20.3,12,19.5,12z"/>
                    </svg>
                    <div class="logo">SZ GAMES</div>
                </div>
                <div class="tagline">Play 100+ Free Online Games - No Downloads Required</div>
            </div>
        </div>

        <!-- Navigation -->
        <div class="nav-wrapper">
            <div class="nav-container">
                <div class="nav-links">
                    <button class="nav-btn active" onclick="showPage('home')">🏠 Home</button>
                    <button class="nav-btn" onclick="showPage('about')">ℹ️ About</button>
                    <button class="nav-btn" onclick="showPage('contact')">📧 Contact</button>
                    <button class="nav-btn" onclick="showPage('privacy')">🔒 Privacy</button>
                </div>
                <div class="search-container">
                    <input type="text" id="searchInput" class="search-input" placeholder="Search games...">
                </div>
            </div>
        </div>

        <!-- Filter Container -->
        <div id="filterWrapper" class="filter-wrapper">
            <div class="filter-container">
                <button class="filter-btn active" onclick="filterCategory('All')">All Games</button>
                <button class="filter-btn" onclick="filterCategory('Action')">⚡ Action</button>
                <button class="filter-btn" onclick="filterCategory('Puzzle')">🧩 Puzzle</button>
                <button class="filter-btn" onclick="filterCategory('Adventure')">🗺️ Adventure</button>
                <button class="filter-btn" onclick="filterCategory('Strategy')">♟️ Strategy</button>
                <button class="filter-btn" onclick="filterCategory('Sports')">⚽ Sports</button>
            </div>
        </div>
    </div>

    <!-- Main Container -->
    <div class="container">
        <!-- Sidebar Ads - Left 160x600 -->
        <div class="side-ad side-ad-left">
            <script>
              atOptions = {
                'key' : '6f5634b1298ddda613ff864793ada29e',
                'format' : 'iframe',
                'height' : 600,
                'width' : 160,
                'params' : {}
              };
            </script>
            <script src="https://www.highperformanceformat.com/6f5634b1298ddda613ff864793ada29e/invoke.js"></script>
        </div>

        <!-- Home Page -->
        <div id="home" class="page active">
            <div class="games-grid" id="gamesGrid"></div>
        </div>

        <!-- About Page -->
        <div id="about" class="page">
            <div class="content-page">
                <h2>About SZ GAMES</h2>
                <p>Welcome to SZ GAMES - your ultimate destination for free online gaming! We're a premier game portal dedicated to bringing you the best HTML5 games from across the web, all playable directly in your browser with no downloads or registrations required.</p>
                <p>Our mission is to provide high-quality entertainment for everyone, whether you're looking for a quick 5-minute break or an immersive gaming session. We carefully curate our collection to ensure every game meets our standards for fun and quality.</p>
                <h3>Why Play at SZ GAMES?</h3>
                <ul>
                    <li><strong>100% Free:</strong> All our games are completely free to play.</li>
                    <li><strong>No Downloads:</strong> Play instantly in your browser on any device.</li>
                    <li><strong>Diverse Categories:</strong> From high-octane action to brain-teasing puzzles.</li>
                    <li><strong>Safe Gaming:</strong> A family-friendly environment for players of all ages.</li>
                </ul>
            </div>
        </div>

        <!-- Contact Page -->
        <div id="contact" class="page">
            <div class="content-page">
                <h2>Contact Us</h2>
                <p>Have questions, feedback, or game suggestions? We'd love to hear from you! Reach out to the SZ GAMES team using the form below.</p>
                <div class="contact-form">
                    <div class="form-group">
                        <label for="name">Name</label>
                        <input type="text" id="name" placeholder="Your Name">
                    </div>
                    <div class="form-group">
                        <label for="email">Email</label>
                        <input type="email" id="email" placeholder="Your Email">
                    </div>
                    <div class="form-group">
                        <label for="message">Message</label>
                        <textarea id="message" placeholder="How can we help you?"></textarea>
                    </div>
                    <button class="submit-btn" onclick="alert('Thank you for your message! This is a demo form.')">Send Message</button>
                </div>
            </div>
        </div>

        <!-- Privacy Page -->
        <div id="privacy" class="page">
            <div class="content-page">
                <h2>Privacy Policy</h2>
                <p>At SZ GAMES, we take your privacy seriously. This policy explains how we handle information when you use our website.</p>
                <h3>Information Collection</h3>
                <p>We do not require users to create accounts or provide personal information to play our games. We may collect non-personal data such as browser type and device information to improve our services.</p>
                <h3>Cookies</h3>
                <p>We use cookies to remember your preferences and analyze our traffic. Third-party advertisers on our site may also use cookies to serve personalized ads.</p>
                <h3>Third-Party Links</h3>
                <p>Our site contains links to other websites. We are not responsible for the privacy practices or content of these external sites.</p>
                <h3>Updates</h3>
                <p>We may update this policy from time to time. Any changes will be posted on this page.</p>
            </div>
        </div>

        <!-- Sidebar Ads - Right 160x600 -->
        <div class="side-ad side-ad-right">
            <script>
              atOptions = {
                'key' : '6f5634b1298ddda613ff864793ada29e',
                'format' : 'iframe',
                'height' : 600,
                'width' : 160,
                'params' : {}
              };
            </script>
            <script src="https://www.highperformanceformat.com/6f5634b1298ddda613ff864793ada29e/invoke.js"></script>
        </div>
    </div>

    <!-- Game Modal -->
    <div id="gameModal" class="modal">
        <div class="modal-content">
            <div class="modal-header">
                <div class="modal-title" id="modalTitle">Game Title</div>
                <div class="close-modal" onclick="closeGame()">&times;</div>
            </div>
            <div class="game-frame-container">
                <iframe id="gameFrame" src="" allowfullscreen></iframe>
            </div>
            <div class="game-info-bar">
                <div id="modalCategory" class="game-category">CATEGORY</div>
                <button class="play-btn" onclick="toggleFullScreen()">Full Screen</button>
            </div>
        </div>
    </div>

    <!-- Footer -->
    <footer class="footer">
        <div class="footer-content">
            <p>&copy; 2024 SZ GAMES. All rights reserved.</p>
            <p>Providing the best free online gaming experience since 2024.</p>
            <div class="footer-links">
                <a onclick="showPage('home')">Home</a>
                <a onclick="showPage('about')">About</a>
                <a onclick="showPage('contact')">Contact</a>
                <a onclick="showPage('privacy')">Privacy Policy</a>
            </div>
        </div>
    </footer>

    <script>
        // Game Data
        const games = [
            { id: 1, title: "Cyber Racer", category: "Action", icon: "🏎️", url: "https://www.gamezhero.com/get-game-code/29241" },
            { id: 2, title: "Neon Blocks", category: "Puzzle", icon: "🧩", url: "https://www.gamezhero.com/get-game-code/29235" },
            { id: 3, title: "Star Fighter", category: "Action", icon: "🚀", url: "https://www.gamezhero.com/get-game-code/29220" },
            { id: 4, title: "Forest Quest", category: "Adventure", icon: "🌳", url: "https://www.gamezhero.com/get-game-code/29215" },
            { id: 5, title: "Mind Master", category: "Strategy", icon: "🧠", url: "https://www.gamezhero.com/get-game-code/29200" },
            { id: 6, title: "Turbo Soccer", category: "Sports", icon: "⚽", url: "https://www.gamezhero.com/get-game-code/29190" },
            { id: 7, title: "Dungeon Run", category: "Adventure", icon: "⚔️", url: "https://www.gamezhero.com/get-game-code/29180" },
            { id: 8, title: "Word Spark", category: "Puzzle", icon: "📝", url: "https://www.gamezhero.com/get-game-code/29170" },
            { id: 9, title: "Pixel Jump", category: "Action", icon: "👾", url: "https://www.gamezhero.com/get-game-code/29160" },
            { id: 10, title: "Hex King", category: "Strategy", icon: "👑", url: "https://www.gamezhero.com/get-game-code/29150" },
            { id: 11, title: "Gravity Ball", category: "Puzzle", icon: "🏀", url: "https://www.gamezhero.com/get-game-code/29140" },
            { id: 12, title: "Shadow Ninja", category: "Action", icon: "🥷", url: "https://www.gamezhero.com/get-game-code/29130" }
        ];

        // State Management
        let currentCategory = 'All';
        let searchQuery = '';

        // DOM Elements
        const gamesGrid = document.getElementById('gamesGrid');
        const searchInput = document.getElementById('searchInput');
        const gameModal = document.getElementById('gameModal');
        const gameFrame = document.getElementById('gameFrame');
        const modalTitle = document.getElementById('modalTitle');
        const modalCategory = document.getElementById('modalCategory');
        const mainHeader = document.getElementById('mainHeader');

        // Header scroll behavior
        let lastScroll = 0;
        window.addEventListener('scroll', () => {
            const currentScroll = window.pageYOffset;
            if (currentScroll <= 0) {
                mainHeader.classList.remove('hide');
                return;
            }
            if (currentScroll > lastScroll && !mainHeader.classList.contains('hide')) {
                mainHeader.classList.add('hide');
            } else if (currentScroll < lastScroll && mainHeader.classList.contains('hide')) {
                mainHeader.classList.remove('hide');
            }
            lastScroll = currentScroll;
        });

        // Initialize Games
        function renderGames() {
            const filteredGames = games.filter(game => {
                const matchesCategory = currentCategory === 'All' || game.category === currentCategory;
                const matchesSearch = game.title.toLowerCase().includes(searchQuery.toLowerCase());
                return matchesCategory && matchesSearch;
            });

            gamesGrid.innerHTML = '';

            if (filteredGames.length === 0) {
                gamesGrid.innerHTML = '<div class="no-games">No games found matching your search.</div>';
                return;
            }

            filteredGames.forEach(game => {
                const card = document.createElement('div');
                card.className = 'game-card';
                card.onclick = () => openGame(game);
                card.innerHTML = `
                    <div class="game-card-image">${game.icon}</div>
                    <div class="game-card-content">
                        <h3>${game.title}</h3>
                        <p>Experience the thrill of ${game.title}! A fantastic ${game.category.toLowerCase()} game that will keep you entertained for hours.</p>
                        <div class="game-card-footer">
                            <span class="game-category">${game.category}</span>
                            <span class="play-btn">Play Now</span>
                        </div>
                    </div>
                `;
                gamesGrid.appendChild(card);
            });
        }

        // Search Handling
        searchInput.addEventListener('input', (e) => {
            searchQuery = e.target.value;
            renderGames();
        });

        // Category Filtering
        function filterCategory(category) {
            currentCategory = category;
            document.querySelectorAll('.filter-btn').forEach(btn => {
                btn.classList.toggle('active', btn.innerText.includes(category));
            });
            renderGames();
        }

        // Navigation
        function showPage(pageId) {
            document.querySelectorAll('.page').forEach(page => {
                page.classList.toggle('active', page.id === pageId);
            });
            document.querySelectorAll('.nav-btn').forEach(btn => {
                btn.classList.toggle('active', btn.innerText.toLowerCase().includes(pageId));
            });
            
            // Hide filter wrapper if not on home page
            const filterWrapper = document.getElementById('filterWrapper');
            filterWrapper.style.display = pageId === 'home' ? 'flex' : 'none';
            
            // Adjust body padding based on header content
            document.body.style.paddingTop = pageId === 'home' ? '450px' : '350px';
            
            window.scrollTo(0, 0);
        }

        // Modal Functions
        function openGame(game) {
            modalTitle.innerText = game.title;
            modalCategory.innerText = game.category;
            gameFrame.src = game.url;
            gameModal.style.display = 'block';
            document.body.style.overflow = 'hidden';
        }

        function closeGame() {
            gameModal.style.display = 'none';
            gameFrame.src = '';
            document.body.style.overflow = 'auto';
        }

        function toggleFullScreen() {
            if (gameFrame.requestFullscreen) {
                gameFrame.requestFullscreen();
            } else if (gameFrame.webkitRequestFullscreen) {
                gameFrame.webkitRequestFullscreen();
            } else if (gameFrame.msRequestFullscreen) {
                gameFrame.msRequestFullscreen();
            }
        }

        // Close modal on outside click
        window.onclick = (event) => {
            if (event.target === gameModal) {
                closeGame();
            }
        };

        // Initial Render
        renderGames();
    </script>
</body>
</html>
