<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
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
            padding-top: 280px;
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

        .header {
            background: linear-gradient(135deg, rgba(10, 14, 39, 0.95) 0%, rgba(26, 31, 58, 0.95) 100%);
            backdrop-filter: blur(10px);
            border-bottom: 2px solid var(--accent);
            padding: 40px 20px;
            text-align: center;
            box-shadow: 0 8px 32px rgba(0, 212, 255, 0.15);
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            z-index: 100;
            transition: transform 0.3s ease;
        }

        .header.hide {
            transform: translateY(-100%);
        }

        .header-content {
            max-width: 1200px;
            margin: 0 auto;
        }

        .logo {
            font-size: 3.5em;
            font-weight: 900;
            background: linear-gradient(135deg, var(--accent) 0%, var(--highlight) 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            text-shadow: 0 0 30px rgba(0, 212, 255, 0.3);
            margin-bottom: 10px;
            letter-spacing: 2px;
            cursor: pointer;
            transition: all 0.3s ease;
        }

        .logo:hover {
            transform: scale(1.05);
            text-shadow: 0 0 40px rgba(0, 212, 255, 0.5);
        }

        .tagline {
            color: var(--accent);
            font-size: 1.1em;
            text-shadow: 0 0 15px rgba(0, 212, 255, 0.2);
            font-weight: 500;
        }

        .nav-wrapper {
            background: rgba(26, 31, 58, 0.8);
            backdrop-filter: blur(10px);
            border-bottom: 1px solid var(--border);
            padding: 0;
            position: fixed;
            top: 180px;
            left: 0;
            right: 0;
            z-index: 99;
            transition: transform 0.3s ease;
        }

        .nav-wrapper.hide {
            transform: translateY(-100%);
        }

        body {
            padding-top: 280px;
        }
        }

        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            gap: 15px;
            flex-wrap: wrap;
            justify-content: center;
            align-items: center;
            padding: 15px 20px;
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
            background: rgba(26, 31, 58, 0.8);
            backdrop-filter: blur(10px);
            border-bottom: 1px solid var(--border);
            padding: 15px 0;
            margin-bottom: 30px;
            display: flex;
            flex-direction: column;
            align-items: center;
            position: fixed;
            top: 180px;
            left: 0;
            right: 0;
            z-index: 98;
            transition: transform 0.3s ease;
        }

        .filter-wrapper.hide {
            transform: translateY(-100%);
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
            color: var(--accent);
            font-size: 1.3em;
            margin-bottom: 8px;
            text-shadow: 0 2px 8px rgba(0, 212, 255, 0.2);
        }

        .game-card p {
            color: var(--text-muted);
            font-size: 0.9em;
            margin-bottom: 15px;
            line-height: 1.5;
        }

        .game-card-category {
            display: inline-block;
            background: rgba(255, 0, 110, 0.2);
            color: var(--highlight);
            padding: 6px 14px;
            border-radius: 15px;
            font-size: 0.8em;
            margin-bottom: 15px;
            border: 1px solid var(--highlight);
            font-weight: 600;
        }

        .play-button {
            width: 100%;
            padding: 12px;
            background: linear-gradient(135deg, var(--accent) 0%, var(--highlight) 100%);
            color: white;
            border: none;
            border-radius: 8px;
            font-weight: 700;
            cursor: pointer;
            font-size: 1em;
            transition: all 0.3s;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .play-button:hover {
            box-shadow: 0 8px 25px rgba(0, 212, 255, 0.4);
            transform: scale(1.02);
        }

        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.95);
            z-index: 2000;
            justify-content: center;
            align-items: center;
            padding: 20px;
        }

        .modal.active {
            display: flex;
        }

        .modal-content {
            background: linear-gradient(135deg, rgba(26, 31, 58, 0.95) 0%, rgba(15, 20, 40, 0.95) 100%);
            border: 2px solid var(--accent);
            border-radius: 15px;
            width: 100%;
            height: 90vh;
            max-width: 1200px;
            display: flex;
            flex-direction: column;
            box-shadow: 0 0 50px rgba(0, 212, 255, 0.4);
            position: relative;
        }

        .modal-header {
            background: linear-gradient(135deg, rgba(10, 14, 39, 0.95) 0%, rgba(26, 31, 58, 0.95) 100%);
            border-bottom: 2px solid var(--accent);
            padding: 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            border-radius: 13px 13px 0 0;
        }

        .modal-header h2 {
            color: var(--accent);
            font-size: 1.8em;
            text-shadow: 0 2px 8px rgba(0, 212, 255, 0.3);
        }

        .close-button {
            background: var(--highlight);
            color: white;
            border: none;
            width: 45px;
            height: 45px;
            border-radius: 50%;
            font-size: 1.5em;
            cursor: pointer;
            transition: all 0.3s;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
        }

        .close-button:hover {
            box-shadow: 0 0 25px rgba(255, 0, 110, 0.6);
            transform: scale(1.1);
        }

        .modal-body {
            flex: 1;
            overflow-y: auto;
            padding: 20px;
        }

        .gamepix-responsive {
            position: relative;
            width: 100%;
            padding-top: 56.25%;
            overflow: hidden;
            background: #000;
            border-radius: 10px;
            box-shadow: 0 8px 32px rgba(0, 212, 255, 0.2);
        }

        .gamepix-responsive iframe {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            border: 0;
            border-radius: 10px;
        }

        .content-page {
            background: linear-gradient(135deg, rgba(26, 31, 58, 0.8) 0%, rgba(15, 20, 40, 0.8) 100%);
            border: 2px solid var(--border);
            border-radius: 15px;
            padding: 50px;
            max-width: 900px;
            margin: 0 auto;
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.3);
        }

        .content-page h2 {
            color: var(--accent);
            font-size: 2.8em;
            margin-bottom: 25px;
            text-shadow: 0 2px 8px rgba(0, 212, 255, 0.2);
            border-bottom: 2px solid var(--highlight);
            padding-bottom: 15px;
        }

        .content-page h3 {
            color: var(--highlight);
            font-size: 1.6em;
            margin-top: 30px;
            margin-bottom: 15px;
        }

        .content-page p {
            line-height: 1.8;
            margin-bottom: 15px;
            color: var(--text);
            font-size: 1.05em;
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
            .logo {
                font-size: 2.2em;
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
    <!-- Header -->
    <div class="header">
        <div class="header-content">
            <div class="logo" onclick="navigateTo('home')" style="cursor: pointer;">🎮 SZ GAMES 🎮</div>
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
        <!-- Adsterra Ad Below Filter - 728x90 -->
        <div style="text-align: center; padding: 15px 0; background: rgba(26, 31, 58, 0.4); margin-top: 10px; border-radius: 8px;">
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
                <p>Welcome to SZ GAMES - your ultimate destination for free online gaming! We're a premier gaming platform dedicated to providing the best gaming experience to millions of players worldwide.</p>
                
                <h3>What We Offer</h3>
                <p>SZ GAMES brings you 100+ free games across multiple categories. Whether you're looking for action-packed adventures, mind-bending puzzles, strategic challenges, sports games, or thrilling explorations, we have something for everyone.</p>
                
                <h3>Why Choose Us?</h3>
                <ul>
                    <li><strong>100+ Free Games:</strong> Access to a vast library without any cost</li>
                    <li><strong>No Registration:</strong> Play instantly without creating an account</li>
                    <li><strong>No Downloads:</strong> All games are browser-based and play directly online</li>
                    <li><strong>Multiple Categories:</strong> Action, Puzzle, Adventure, Strategy, and Sports</li>
                    <li><strong>High Quality:</strong> Only the best and most popular games</li>
                    <li><strong>Regular Updates:</strong> New games added frequently</li>
                    <li><strong>Safe & Secure:</strong> Player safety and privacy are our priorities</li>
                    <li><strong>Mobile Friendly:</strong> Play on any device - desktop, tablet, or mobile</li>
                </ul>
                
                <h3>Our Mission</h3>
                <p>We believe everyone deserves access to quality entertainment without barriers. Our mission is to provide a safe, fun, and accessible gaming platform where players of all ages can enjoy premium games for free.</p>
                
                <h3>Why SZ GAMES?</h3>
                <ul>
                    <li>Instant Play - No waiting, no installations</li>
                    <li>Cross-Platform - Works on all devices</li>
                    <li>Regular Updates - New games added weekly</li>
                    <li>Community Driven - Your feedback shapes our platform</li>
                    <li>Fair Gameplay - No pay-to-win mechanics</li>
                    <li>Secure Platform - Your data is protected</li>
                </ul>
                
                <h3>Join Our Community</h3>
                <p>Join thousands of players who trust us for their daily gaming entertainment. Whether you're a casual gamer or a hardcore enthusiast, we offer the perfect gaming experience.</p>
            </div>
        </div>

        <!-- Contact Page -->
        <div id="contact" class="page">
            <div class="content-page">
                <h2>Contact Us</h2>
                <p>Have questions? Want to suggest a game? Need support? We'd love to hear from you. Fill out the form below and our team will get back to you within 24 hours.</p>
                
                <div class="contact-form">
                    <div class="form-group">
                        <label for="name">Your Name</label>
                        <input type="text" id="name" placeholder="Enter your full name">
                    </div>
                    <div class="form-group">
                        <label for="email">Email Address</label>
                        <input type="email" id="email" placeholder="your.email@example.com">
                    </div>
                    <div class="form-group">
                        <label for="subject">Subject</label>
                        <input type="text" id="subject" placeholder="What is this about?">
                    </div>
                    <div class="form-group">
                        <label for="message">Message</label>
                        <textarea id="message" placeholder="Tell us your message, feedback, or game suggestion..."></textarea>
                    </div>
                    <button class="submit-btn" onclick="submitForm()">Send Message</button>
                </div>

                <h3 style="margin-top: 50px;">Contact Information</h3>
                <p><strong>📧 Email:</strong> muhammadgullsher0786@gmail.com</p>
                <p><strong>⏱️ Response Time:</strong> We typically respond within 24 hours</p>
                <p><strong>💬 Support:</strong> For urgent matters, please mark "URGENT" in the subject line</p>
                
                <h3>Support Categories</h3>
                <ul>
                    <li><strong>Game Suggestions:</strong> Recommend games you'd like to see</li>
                    <li><strong>Technical Issues:</strong> Report problems with the platform</li>
                    <li><strong>Bug Reports:</strong> Help us improve by reporting bugs</li>
                    <li><strong>General Inquiries:</strong> Any other questions</li>
                </ul>
            </div>
        </div>

        <!-- Privacy Policy Page -->
        <div id="privacy" class="page">
            <div class="content-page">
                <h2>Privacy Policy</h2>
                <p><strong>Last Updated:</strong> 2024</p>
                
                <h3>1. Introduction</h3>
                <p>We are committed to protecting your privacy and ensuring you have a positive experience on our platform. This Privacy Policy explains how we collect, use, and safeguard your information.</p>
                
                <h3>2. Information We Collect</h3>
                <p>We may collect the following information:</p>
                <ul>
                    <li>Browser type and operating system</li>
                    <li>Pages visited and time spent on our platform</li>
                    <li>Date and time of visits</li>
                    <li>Referral source</li>
                    <li>IP address and device information</li>
                    <li>Game preferences and play history</li>
                    <li>Contact information (if you contact us)</li>
                </ul>
                
                <h3>3. How We Use Your Information</h3>
                <p>We use collected information to:</p>
                <ul>
                    <li>Improve our services and user experience</li>
                    <li>Analyze trends and usage patterns</li>
                    <li>Prevent fraud and enhance security</li>
                    <li>Personalize your experience</li>
                    <li>Respond to your inquiries and support requests</li>
                    <li>Send updates about our platform</li>
                    <li>Comply with legal obligations</li>
                </ul>
                
                <h3>4. Cookies and Tracking</h3>
                <p>We use cookies to enhance your experience. Cookies help us remember your preferences and understand how you use our platform. You can control cookies through your browser settings.</p>
                
                <h3>5. Third-Party Services</h3>
                <p>We use third-party game providers (like GamePix) to deliver games. Please review their privacy policies as we are not responsible for their practices.</p>
                
                <h3>6. Data Security</h3>
                <p>We implement industry-standard security measures to protect your information. However, no method of transmission over the internet is 100% secure.</p>
                
                <h3>7. Your Rights</h3>
                <p>You have the right to:</p>
                <ul>
                    <li>Access your information</li>
                    <li>Modify or update your information</li>
                    <li>Delete your information</li>
                    <li>Opt-out of communications</li>
                    <li>Request a copy of your data</li>
                </ul>
                <p>To exercise these rights, contact us at muhammadgullsher0786@gmail.com</p>
                
                <h3>8. Children's Privacy</h3>
                <p>Our platform is designed for users of all ages. However, we do not knowingly collect personal information from children under 13. If we become aware of such collection, we will delete the information immediately.</p>
                
                <h3>9. Changes to This Policy</h3>
                <p>We may update this Privacy Policy periodically. We will notify users of significant changes through email or prominent notice on our website.</p>
                
                <h3>10. Contact Us</h3>
                <p>If you have questions about our privacy practices, please contact us:</p>
                <ul>
                    <li><strong>Email:</strong> muhammadgullsher0786@gmail.com</li>
                    <li><strong>Subject:</strong> "Privacy Inquiry"</li>
                    <li><strong>Response Time:</strong> 24-48 hours</li>
                </ul>
                
                <h3>11. Legal Compliance</h3>
                <p>We comply with applicable privacy laws and regulations including GDPR, CCPA, and other international privacy standards.</p>
                
                <h3>12. Third-Party Links</h3>
                <p>Our platform may contain links to third-party websites. We are not responsible for their privacy practices. We recommend reviewing their privacy policies before providing information.</p>
            </div>
        </div>
    </div>

    <!-- Right Sidebar Ad - 160x600 Fixed -->
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

    <!-- Game Modal -->
    <div class="modal" id="gameModal">
        <div class="modal-content">
            <div class="modal-header">
                <h2 id="modalTitle">Game</h2>
                <button class="close-button" onclick="closeGame()">✕</button>
            </div>
            <div class="modal-body">
                <div id="gameContainer"></div>
            </div>
        </div>
    </div>

    <!-- Footer -->
    <div class="footer">
        <div class="footer-content">
            <p>© 2024 SZ GAMES - All Rights Reserved</p>
            <p>Play Free Games Online - No Registration Required</p>
            <div class="footer-links">
                <a onclick="showPage('home')">🏠 Home</a>
                <a onclick="showPage('about')">ℹ️ About</a>
                <a onclick="showPage('contact')">📧 Contact</a>
                <a onclick="showPage('privacy')">🔒 Privacy</a>
            </div>
        </div>
    </div>

    <script>
        // 100+ Games Database
        const games = [
            // ACTION GAMES (1-20)
            {id: 1, name: 'Minecraft-ish MMO', category: 'Action', description: 'Build and explore in this Minecraft-inspired world', embedUrl: 'https://play.gamepix.com/minecraft-ish-mmo/embed?sid=1', emoji: '⛏️'},
            {id: 2, name: 'Subway Surfers', category: 'Action', description: 'Run and dodge obstacles in this endless runner', embedUrl: 'https://play.gamepix.com/subway-surfers/embed?sid=1', emoji: '🚇'},
            {id: 3, name: 'Flappy Bird', category: 'Action', description: 'Tap to fly through the pipes', embedUrl: 'https://play.gamepix.com/flappy-bird/embed?sid=1', emoji: '🐦'},
            {id: 4, name: 'Dino Runner', category: 'Action', description: 'Jump over obstacles with the dinosaur', embedUrl: 'https://play.gamepix.com/dino-runner/embed?sid=1', emoji: '🦖'},
            {id: 5, name: 'Space Invaders', category: 'Action', description: 'Defend against alien invaders', embedUrl: 'https://play.gamepix.com/space-invaders/embed?sid=1', emoji: '👽'},
            {id: 6, name: 'Snake Game', category: 'Action', description: 'Grow your snake and eat food', embedUrl: 'https://play.gamepix.com/snake/embed?sid=1', emoji: '🐍'},
            {id: 7, name: 'Pac-Man', category: 'Action', description: 'Eat dots and avoid ghosts', embedUrl: 'https://play.gamepix.com/pacman/embed?sid=1', emoji: '👾'},
            {id: 8, name: 'Zombie Runner', category: 'Action', description: 'Escape from zombies', embedUrl: 'https://play.gamepix.com/zombie-runner/embed?sid=1', emoji: '🧟'},
            {id: 9, name: 'Ninja Quest', category: 'Action', description: 'Complete ninja missions', embedUrl: 'https://play.gamepix.com/ninja-quest/embed?sid=1', emoji: '🥷'},
            {id: 10, name: 'Pirate Adventure', category: 'Action', description: 'Sail the seas and find treasure', embedUrl: 'https://play.gamepix.com/pirate-adventure/embed?sid=1', emoji: '🏴‍☠️'},
            {id: 11, name: 'Police Chase', category: 'Action', description: 'Chase criminals through the city', embedUrl: 'https://play.gamepix.com/police-chase/embed?sid=1', emoji: '🚓'},
            {id: 12, name: 'Superhero Flight', category: 'Action', description: 'Fly as a superhero', embedUrl: 'https://play.gamepix.com/superhero-flight/embed?sid=1', emoji: '🦸'},
            {id: 13, name: 'Alien Shooter', category: 'Action', description: 'Shoot down alien spaceships', embedUrl: 'https://play.gamepix.com/alien-shooter/embed?sid=1', emoji: '🛸'},
            {id: 14, name: 'Dragon Slayer', category: 'Action', description: 'Slay dragons and save the kingdom', embedUrl: 'https://play.gamepix.com/dragon-slayer/embed?sid=1', emoji: '🐉'},
            {id: 15, name: 'Zombie Apocalypse', category: 'Action', description: 'Survive the zombie apocalypse', embedUrl: 'https://play.gamepix.com/zombie-apocalypse/embed?sid=1', emoji: '🧛'},
            {id: 16, name: 'Neon Runner', category: 'Action', description: 'Run through neon-lit streets', embedUrl: 'https://play.gamepix.com/neon-runner/embed?sid=1', emoji: '⚡'},
            {id: 17, name: 'Sword Master', category: 'Action', description: 'Master the sword and defeat enemies', embedUrl: 'https://play.gamepix.com/sword-master/embed?sid=1', emoji: '⚔️'},
            {id: 18, name: 'Bomb Defuser', category: 'Action', description: 'Defuse bombs before they explode', embedUrl: 'https://play.gamepix.com/bomb-defuser/embed?sid=1', emoji: '💣'},
            {id: 19, name: 'Ninja Warrior', category: 'Action', description: 'Complete ninja obstacle courses', embedUrl: 'https://play.gamepix.com/ninja-warrior/embed?sid=1', emoji: '🗡️'},
            {id: 20, name: 'Cyber Runner', category: 'Action', description: 'Run through cyberspace', embedUrl: 'https://play.gamepix.com/cyber-runner/embed?sid=1', emoji: '🤖'},

            // PUZZLE GAMES (21-40)
            {id: 21, name: 'Candy Crush', category: 'Puzzle', description: 'Match candies and complete levels', embedUrl: 'https://play.gamepix.com/candy-crush-saga/embed?sid=1', emoji: '🍬'},
            {id: 22, name: 'Tetris', category: 'Puzzle', description: 'Stack blocks and clear lines', embedUrl: 'https://play.gamepix.com/tetris/embed?sid=1', emoji: '🧱'},
            {id: 23, name: '2048', category: 'Puzzle', description: 'Combine tiles to reach 2048', embedUrl: 'https://play.gamepix.com/2048/embed?sid=1', emoji: '🔢'},
            {id: 24, name: 'Bubble Shooter', category: 'Puzzle', description: 'Shoot and pop bubbles', embedUrl: 'https://play.gamepix.com/bubble-shooter/embed?sid=1', emoji: '🫧'},
            {id: 25, name: 'Memory Game', category: 'Puzzle', description: 'Match pairs and test your memory', embedUrl: 'https://play.gamepix.com/memory-game/embed?sid=1', emoji: '🧠'},
            {id: 26, name: 'Mahjong', category: 'Puzzle', description: 'Match tiles in this classic game', embedUrl: 'https://play.gamepix.com/mahjong/embed?sid=1', emoji: '🀄'},
            {id: 27, name: 'Sudoku', category: 'Puzzle', description: 'Solve number puzzles', embedUrl: 'https://play.gamepix.com/sudoku/embed?sid=1', emoji: '🔤'},
            {id: 28, name: 'Jigsaw Puzzle', category: 'Puzzle', description: 'Complete jigsaw puzzles', embedUrl: 'https://play.gamepix.com/jigsaw/embed?sid=1', emoji: '🧩'},
            {id: 29, name: 'Block Blast', category: 'Puzzle', description: 'Blast blocks and clear the board', embedUrl: 'https://play.gamepix.com/block-blast/embed?sid=1', emoji: '💥'},
            {id: 30, name: 'Connect Dots', category: 'Puzzle', description: 'Connect dots to create patterns', embedUrl: 'https://play.gamepix.com/connect-dots/embed?sid=1', emoji: '⚫'},
            {id: 31, name: 'Pipe Master', category: 'Puzzle', description: 'Connect pipes to complete the circuit', embedUrl: 'https://play.gamepix.com/pipe-master/embed?sid=1', emoji: '🔧'},
            {id: 32, name: 'Color Match', category: 'Puzzle', description: 'Match colors and complete levels', embedUrl: 'https://play.gamepix.com/color-match/embed?sid=1', emoji: '🎨'},
            {id: 33, name: 'Shape Fit', category: 'Puzzle', description: 'Fit shapes into the grid', embedUrl: 'https://play.gamepix.com/shape-fit/embed?sid=1', emoji: '⬜'},
            {id: 34, name: 'Word Search', category: 'Puzzle', description: 'Find hidden words in the grid', embedUrl: 'https://play.gamepix.com/word-search/embed?sid=1', emoji: '📝'},
            {id: 35, name: 'Crossword', category: 'Puzzle', description: 'Solve crossword puzzles', embedUrl: 'https://play.gamepix.com/crossword/embed?sid=1', emoji: '✏️'},
            {id: 36, name: 'Sliding Puzzle', category: 'Puzzle', description: 'Slide tiles to complete the picture', embedUrl: 'https://play.gamepix.com/sliding-puzzle/embed?sid=1', emoji: '🖼️'},
            {id: 37, name: 'Ice Cream Match', category: 'Puzzle', description: 'Match ice cream flavors', embedUrl: 'https://play.gamepix.com/ice-cream-match/embed?sid=1', emoji: '🍦'},
            {id: 38, name: 'Gem Swap', category: 'Puzzle', description: 'Swap gems to make matches', embedUrl: 'https://play.gamepix.com/gem-swap/embed?sid=1', emoji: '💎'},
            {id: 39, name: 'Number Puzzle', category: 'Puzzle', description: 'Solve number-based puzzles', embedUrl: 'https://play.gamepix.com/number-puzzle/embed?sid=1', emoji: '🔢'},
            {id: 40, name: 'Brain Teaser', category: 'Puzzle', description: 'Challenge your brain with teasers', embedUrl: 'https://play.gamepix.com/brain-teaser/embed?sid=1', emoji: '🧩'},

            // ADVENTURE GAMES (41-60)
            {id: 41, name: 'Quest Adventure', category: 'Adventure', description: 'Epic quests and adventures await', embedUrl: 'https://play.gamepix.com/quest-adventure/embed?sid=1', emoji: '⚔️'},
            {id: 42, name: 'Lost Temple', category: 'Adventure', description: 'Explore ancient temples', embedUrl: 'https://play.gamepix.com/lost-temple/embed?sid=1', emoji: '🏛️'},
            {id: 43, name: 'Treasure Hunt', category: 'Adventure', description: 'Hunt for hidden treasures', embedUrl: 'https://play.gamepix.com/treasure-hunt/embed?sid=1', emoji: '💰'},
            {id: 44, name: 'Jungle Explorer', category: 'Adventure', description: 'Explore mysterious jungles', embedUrl: 'https://play.gamepix.com/jungle-explorer/embed?sid=1', emoji: '🌴'},
            {id: 45, name: 'Mountain Climb', category: 'Adventure', description: 'Climb treacherous mountains', embedUrl: 'https://play.gamepix.com/mountain-climb/embed?sid=1', emoji: '⛰️'},
            {id: 46, name: 'Ocean Quest', category: 'Adventure', description: 'Dive deep into the ocean', embedUrl: 'https://play.gamepix.com/ocean-quest/embed?sid=1', emoji: '🌊'},
            {id: 47, name: 'Sky Rider', category: 'Adventure', description: 'Fly through the skies', embedUrl: 'https://play.gamepix.com/sky-rider/embed?sid=1', emoji: '✈️'},
            {id: 48, name: 'Desert Quest', category: 'Adventure', description: 'Cross the vast desert', embedUrl: 'https://play.gamepix.com/desert-quest/embed?sid=1', emoji: '🏜️'},
            {id: 49, name: 'Frozen Lands', category: 'Adventure', description: 'Survive in frozen wastelands', embedUrl: 'https://play.gamepix.com/frozen-lands/embed?sid=1', emoji: '❄️'},
            {id: 50, name: 'Volcano Quest', category: 'Adventure', description: 'Escape from an active volcano', embedUrl: 'https://play.gamepix.com/volcano-quest/embed?sid=1', emoji: '🌋'},
            {id: 51, name: 'Cave Explorer', category: 'Adventure', description: 'Explore dark caves', embedUrl: 'https://play.gamepix.com/cave-explorer/embed?sid=1', emoji: '🕳️'},
            {id: 52, name: 'Forest Adventure', category: 'Adventure', description: 'Adventure through enchanted forests', embedUrl: 'https://play.gamepix.com/forest-adventure/embed?sid=1', emoji: '🌲'},
            {id: 53, name: 'Castle Quest', category: 'Adventure', description: 'Explore ancient castles', embedUrl: 'https://play.gamepix.com/castle-quest/embed?sid=1', emoji: '🏰'},
            {id: 54, name: 'Underwater Adventure', category: 'Adventure', description: 'Explore underwater worlds', embedUrl: 'https://play.gamepix.com/underwater-adventure/embed?sid=1', emoji: '🐠'},
            {id: 55, name: 'Space Explorer', category: 'Adventure', description: 'Explore outer space', embedUrl: 'https://play.gamepix.com/space-explorer/embed?sid=1', emoji: '🚀'},
            {id: 56, name: 'Time Travel', category: 'Adventure', description: 'Travel through time', embedUrl: 'https://play.gamepix.com/time-travel/embed?sid=1', emoji: '⏰'},
            {id: 57, name: 'Lost City', category: 'Adventure', description: 'Find the lost city', embedUrl: 'https://play.gamepix.com/lost-city/embed?sid=1', emoji: '🏛️'},
            {id: 58, name: 'Island Adventure', category: 'Adventure', description: 'Survive on a mysterious island', embedUrl: 'https://play.gamepix.com/island-adventure/embed?sid=1', emoji: '🏝️'},
            {id: 59, name: 'Dungeon Crawler', category: 'Adventure', description: 'Crawl through dark dungeons', embedUrl: 'https://play.gamepix.com/dungeon-crawler/embed?sid=1', emoji: '🗝️'},
            {id: 60, name: 'Portal Quest', category: 'Adventure', description: 'Travel through magical portals', embedUrl: 'https://play.gamepix.com/portal-quest/embed?sid=1', emoji: '🌀'},

            // STRATEGY GAMES (61-80)
            {id: 61, name: 'Chess Master', category: 'Strategy', description: 'Play chess against AI', embedUrl: 'https://play.gamepix.com/chess/embed?sid=1', emoji: '♟️'},
            {id: 62, name: 'Tower Defense', category: 'Strategy', description: 'Defend your tower from enemies', embedUrl: 'https://play.gamepix.com/tower-defense/embed?sid=1', emoji: '🏰'},
            {id: 63, name: 'Strategy War', category: 'Strategy', description: 'Wage strategic wars', embedUrl: 'https://play.gamepix.com/strategy-war/embed?sid=1', emoji: '🎖️'},
            {id: 64, name: 'Checkers', category: 'Strategy', description: 'Play classic checkers', embedUrl: 'https://play.gamepix.com/checkers/embed?sid=1', emoji: '🔴'},
            {id: 65, name: 'Solitaire', category: 'Strategy', description: 'Play classic solitaire', embedUrl: 'https://play.gamepix.com/solitaire/embed?sid=1', emoji: '🃏'},
            {id: 66, name: 'Dominoes', category: 'Strategy', description: 'Play dominoes', embedUrl: 'https://play.gamepix.com/dominoes/embed?sid=1', emoji: '🎲'},
            {id: 67, name: 'Connect Four', category: 'Strategy', description: 'Connect four pieces to win', embedUrl: 'https://play.gamepix.com/connect-four/embed?sid=1', emoji: '🟡'},
            {id: 68, name: 'Tic Tac Toe', category: 'Strategy', description: 'Play tic tac toe', embedUrl: 'https://play.gamepix.com/tic-tac-toe/embed?sid=1', emoji: '⭕'},
            {id: 69, name: 'Ludo', category: 'Strategy', description: 'Play the classic board game', embedUrl: 'https://play.gamepix.com/ludo/embed?sid=1', emoji: '🎯'},
            {id: 70, name: 'Carrom', category: 'Strategy', description: 'Play carrom board game', embedUrl: 'https://play.gamepix.com/carrom/embed?sid=1', emoji: '🎱'},
            {id: 71, name: 'City Builder', category: 'Strategy', description: 'Build and manage cities', embedUrl: 'https://play.gamepix.com/city-builder/embed?sid=1', emoji: '🏙️'},
            {id: 72, name: 'Farm Tycoon', category: 'Strategy', description: 'Build and manage farms', embedUrl: 'https://play.gamepix.com/farm-tycoon/embed?sid=1', emoji: '🌾'},
            {id: 73, name: 'Zoo Builder', category: 'Strategy', description: 'Build and manage zoos', embedUrl: 'https://play.gamepix.com/zoo-builder/embed?sid=1', emoji: '🦁'},
            {id: 74, name: 'Restaurant Manager', category: 'Strategy', description: 'Manage restaurants', embedUrl: 'https://play.gamepix.com/restaurant-manager/embed?sid=1', emoji: '🍽️'},
            {id: 75, name: 'Hospital Manager', category: 'Strategy', description: 'Manage hospitals', embedUrl: 'https://play.gamepix.com/hospital-manager/embed?sid=1', emoji: '🏥'},
            {id: 76, name: 'Hotel Manager', category: 'Strategy', description: 'Manage hotels', embedUrl: 'https://play.gamepix.com/hotel-manager/embed?sid=1', emoji: '🏨'},
            {id: 77, name: 'Business Tycoon', category: 'Strategy', description: 'Build a business empire', embedUrl: 'https://play.gamepix.com/business-tycoon/embed?sid=1', emoji: '💼'},
            {id: 78, name: 'Mining Tycoon', category: 'Strategy', description: 'Mine resources and build wealth', embedUrl: 'https://play.gamepix.com/mining-tycoon/embed?sid=1', emoji: '⛏️'},
            {id: 79, name: 'Trading Game', category: 'Strategy', description: 'Trade goods and make profits', embedUrl: 'https://play.gamepix.com/trading-game/embed?sid=1', emoji: '📊'},
            {id: 80, name: 'Empire Builder', category: 'Strategy', description: 'Build an empire', embedUrl: 'https://play.gamepix.com/empire-builder/embed?sid=1', emoji: '👑'},

            // SPORTS GAMES (81-100)
            {id: 81, name: 'Basketball', category: 'Sports', description: 'Play basketball', embedUrl: 'https://play.gamepix.com/basketball/embed?sid=1', emoji: '🏀'},
            {id: 82, name: 'Soccer', category: 'Sports', description: 'Play soccer/football', embedUrl: 'https://play.gamepix.com/soccer/embed?sid=1', emoji: '⚽'},
            {id: 83, name: 'Tennis', category: 'Sports', description: 'Play tennis', embedUrl: 'https://play.gamepix.com/tennis/embed?sid=1', emoji: '🎾'},
            {id: 84, name: 'Golf', category: 'Sports', description: 'Play golf', embedUrl: 'https://play.gamepix.com/golf/embed?sid=1', emoji: '⛳'},
            {id: 85, name: 'Bowling', category: 'Sports', description: 'Play bowling', embedUrl: 'https://play.gamepix.com/bowling/embed?sid=1', emoji: '🎳'},
            {id: 86, name: 'Racing', category: 'Sports', description: 'Race cars', embedUrl: 'https://play.gamepix.com/racing/embed?sid=1', emoji: '🏎️'},
            {id: 87, name: 'Bike Racing', category: 'Sports', description: 'Race bikes', embedUrl: 'https://play.gamepix.com/bike-racing/embed?sid=1', emoji: '🏍️'},
            {id: 88, name: 'Skateboard', category: 'Sports', description: 'Skateboard tricks', embedUrl: 'https://play.gamepix.com/skateboard/embed?sid=1', emoji: '🛹'},
            {id: 89, name: 'Surfing', category: 'Sports', description: 'Surf waves', embedUrl: 'https://play.gamepix.com/surfing/embed?sid=1', emoji: '🏄'},
            {id: 90, name: 'Skiing', category: 'Sports', description: 'Ski down slopes', embedUrl: 'https://play.gamepix.com/skiing/embed?sid=1', emoji: '⛷️'},
            {id: 91, name: 'Archery', category: 'Sports', description: 'Practice archery', embedUrl: 'https://play.gamepix.com/archery/embed?sid=1', emoji: '🏹'},
            {id: 92, name: 'Boxing', category: 'Sports', description: 'Box opponents', embedUrl: 'https://play.gamepix.com/boxing/embed?sid=1', emoji: '🥊'},
            {id: 93, name: 'Wrestling', category: 'Sports', description: 'Wrestling matches', embedUrl: 'https://play.gamepix.com/wrestling/embed?sid=1', emoji: '🤼'},
            {id: 94, name: 'Volleyball', category: 'Sports', description: 'Play volleyball', embedUrl: 'https://play.gamepix.com/volleyball/embed?sid=1', emoji: '🏐'},
            {id: 95, name: 'Badminton', category: 'Sports', description: 'Play badminton', embedUrl: 'https://play.gamepix.com/badminton/embed?sid=1', emoji: '🏸'},
            {id: 96, name: 'Table Tennis', category: 'Sports', description: 'Play table tennis', embedUrl: 'https://play.gamepix.com/table-tennis/embed?sid=1', emoji: '🏓'},
            {id: 97, name: 'Cricket', category: 'Sports', description: 'Play cricket', embedUrl: 'https://play.gamepix.com/cricket/embed?sid=1', emoji: '🏏'},
            {id: 98, name: 'Baseball', category: 'Sports', description: 'Play baseball', embedUrl: 'https://play.gamepix.com/baseball/embed?sid=1', emoji: '⚾'},
            {id: 99, name: 'Horse Racing', category: 'Sports', description: 'Race horses', embedUrl: 'https://play.gamepix.com/horse-racing/embed?sid=1', emoji: '🐎'},
            {id: 100, name: 'Swimming', category: 'Sports', description: 'Competitive swimming', embedUrl: 'https://play.gamepix.com/swimming/embed?sid=1', emoji: '🏊'}
        ];

        let currentCategory = 'All';
        let currentSearch = '';
        let currentPage = 'home';

        function showPage(pageName) {
            document.querySelectorAll('.page').forEach(page => page.classList.remove('active'));
            document.getElementById(pageName).classList.add('active');
            
            const filterWrapper = document.getElementById('filterWrapper');
            filterWrapper.style.display = pageName === 'home' ? 'block' : 'none';
            
            document.querySelectorAll('.nav-btn').forEach(btn => btn.classList.remove('active'));
            event.target.classList.add('active');
            
            currentPage = pageName;
            window.scrollTo(0, 0);
        }

        function renderGames() {
            const grid = document.getElementById('gamesGrid');
            grid.innerHTML = '';

            const filtered = games.filter(game => {
                const matchCategory = currentCategory === 'All' || game.category === currentCategory;
                const matchSearch = game.name.toLowerCase().includes(currentSearch.toLowerCase());
                return matchCategory && matchSearch;
            });

            if (filtered.length === 0) {
                grid.innerHTML = '<div class="no-games">No games found. Try a different search!</div>';
                return;
            }

            filtered.forEach(game => {
                const card = document.createElement('div');
                card.className = 'game-card';
                card.innerHTML = `
                    <div class="game-card-image">${game.emoji}</div>
                    <div class="game-card-content">
                        <h3>${game.name}</h3>
                        <p>${game.description}</p>
                        <span class="game-card-category">${game.category}</span>
                        <button class="play-button" onclick="playGame(${game.id}, '${game.name}', '${game.embedUrl}')">
                            Play Now
                        </button>
                    </div>
                `;
                grid.appendChild(card);
            });
        }

        function filterCategory(category) {
            currentCategory = category;
            document.querySelectorAll('.filter-btn').forEach(btn => btn.classList.remove('active'));
            event.target.classList.add('active');
            renderGames();
            window.history.pushState({}, '', `?category=${category}`);
        }

        document.getElementById('searchInput').addEventListener('input', (e) => {
            currentSearch = e.target.value;
            renderGames();
        });

        function playGame(id, name, embedUrl) {
            document.getElementById('modalTitle').textContent = name;
            const container = document.getElementById('gameContainer');
            container.innerHTML = `
                <div class="gamepix-responsive">
                    <iframe 
                        src="${embedUrl}"
                        frameborder="0"
                        scrolling="no"
                        allowfullscreen>
                    </iframe>
                </div>
            `;
            document.getElementById('gameModal').classList.add('active');
            window.history.pushState({}, '', `?game=${id}`);
        }

        function closeGame() {
            document.getElementById('gameModal').classList.remove('active');
            document.getElementById('gameContainer').innerHTML = '';
            window.history.pushState({}, '', '?');
        }

        document.getElementById('gameModal').addEventListener('click', (e) => {
            if (e.target.id === 'gameModal') {
                closeGame();
            }
        });

        function submitForm() {
            const name = document.getElementById('name').value;
            const email = document.getElementById('email').value;
            const subject = document.getElementById('subject').value;
            const message = document.getElementById('message').value;
            
            if (name && email && subject && message) {
                alert('Thank you for contacting us! We will get back to you soon at ' + email);
                document.getElementById('name').value = '';
                document.getElementById('email').value = '';
                document.getElementById('subject').value = '';
                document.getElementById('message').value = '';
            } else {
                alert('Please fill all fields');
            }
        }

        window.addEventListener('popstate', () => {
            const params = new URLSearchParams(window.location.search);
            const gameId = params.get('game');
            const category = params.get('category');
            
            if (gameId) {
                const game = games.find(g => g.id == gameId);
                if (game) {
                    playGame(game.id, game.name, game.embedUrl);
                }
            } else {
                closeGame();
            }
            
            if (category) {
                filterCategory(category);
            }
        });

        // Auto-hide header on scroll
        let lastScrollTop = 0;
        const header = document.querySelector('.header');
        const navWrapper = document.querySelector('.nav-wrapper');
        const filterWrapper = document.querySelector('.filter-wrapper');

        window.addEventListener('scroll', () => {
            let currentScroll = window.pageYOffset || document.documentElement.scrollTop;
            
            if (currentScroll > lastScrollTop) {
                // Scrolling DOWN - hide header
                header.classList.add('hide');
                navWrapper.classList.add('hide');
                filterWrapper.classList.add('hide');
            } else {
                // Scrolling UP - show header
                header.classList.remove('hide');
                navWrapper.classList.remove('hide');
                filterWrapper.classList.remove('hide');
            }
            
            lastScrollTop = currentScroll <= 0 ? 0 : currentScroll;
        });

        renderGames();
    </script>
</body>
</html>
