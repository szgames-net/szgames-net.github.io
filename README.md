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

Plain Text


    :root {
        --primary: #0a0e27;
        --secondary: #1a1f3a;
        --accent: #00d4ff;
        --highlight: #ff006e;
        --success: #00ff88;
        --text: #e8eef7;
        --text-muted: #a0a8c0;
        --border: #2a3050;
        --header-height: 180px;
        --nav-height: 80px;
        --filter-height: 160px;
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
        padding-top: calc(var(--header-height) + var(--nav-height) + var(--filter-height));
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

    /* Combined Header Container for easier hiding */
    .main-header-container {
        position: fixed;
        top: 0;
        left: 0;
        right: 0;
        z-index: 100;
        transition: transform 0.4s cubic-bezier(0.4, 0, 0.2, 1);
        will-change: transform;
    }

    .main-header-container.hide {
        transform: translateY(-100%);
    }

    .header {
        background: linear-gradient(135deg, rgba(10, 14, 39, 0.98) 0%, rgba(26, 31, 58, 0.98) 100%);
        backdrop-filter: blur(15px);
        border-bottom: 2px solid var(--accent);
        padding: 30px 20px;
        text-align: center;
        box-shadow: 0 8px 32px rgba(0, 212, 255, 0.15);
        height: var(--header-height);
        display: flex;
        flex-direction: column;
        justify-content: center;
    }

    .header-content {
        max-width: 1200px;
        margin: 0 auto;
        width: 100%;
    }

    .logo {
        font-size: 3em;
        font-weight: 900;
        background: linear-gradient(135deg, var(--accent) 0%, var(--highlight) 100%);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        background-clip: text;
        text-shadow: 0 0 30px rgba(0, 212, 255, 0.3);
        margin-bottom: 5px;
        letter-spacing: 2px;
        cursor: pointer;
        transition: all 0.3s ease;
        display: inline-block;
    }

    .logo:hover {
        transform: scale(1.05);
        text-shadow: 0 0 40px rgba(0, 212, 255, 0.5);
    }

    .tagline {
        color: var(--accent);
        font-size: 1em;
        text-shadow: 0 0 15px rgba(0, 212, 255, 0.2);
        font-weight: 500;
        opacity: 0.9;
    }

    .nav-wrapper {
        background: rgba(26, 31, 58, 0.95);
        backdrop-filter: blur(15px);
        border-bottom: 1px solid var(--border);
        height: var(--nav-height);
        display: flex;
        align-items: center;
    }

    .nav-container {
        max-width: 1200px;
        margin: 0 auto;
        display: flex;
        gap: 20px;
        width: 100%;
        justify-content: space-between;
        align-items: center;
        padding: 0 20px;
    }

    .nav-links {
        display: flex;
        gap: 12px;
    }

    .nav-btn {
        padding: 8px 18px;
        background: rgba(0, 212, 255, 0.05);
        border: 2px solid var(--accent);
        color: var(--accent);
        border-radius: 25px;
        cursor: pointer;
        font-weight: 600;
        transition: all 0.3s ease;
        font-size: 0.9em;
        text-decoration: none;
        display: flex;
        align-items: center;
        gap: 6px;
    }

    .nav-btn:hover, .nav-btn.active {
        background: var(--accent);
        color: var(--primary);
        box-shadow: 0 0 20px rgba(0, 212, 255, 0.4);
        transform: translateY(-2px);
    }

    .search-container {
        flex: 1;
        max-width: 350px;
    }

    .search-input {
        width: 100%;
        padding: 10px 20px;
        background: rgba(10, 14, 39, 0.6);
        border: 2px solid var(--accent);
        color: var(--text);
        border-radius: 25px;
        font-size: 0.95em;
        transition: all 0.3s;
    }

    .search-input:focus {
        outline: none;
        box-shadow: 0 0 20px rgba(0, 212, 255, 0.3);
        border-color: var(--highlight);
    }

    .filter-wrapper {
        background: rgba(26, 31, 58, 0.9);
        backdrop-filter: blur(15px);
        border-bottom: 1px solid var(--border);
        padding: 15px 0;
        display: flex;
        flex-direction: column;
        align-items: center;
        height: var(--filter-height);
        overflow: hidden;
    }

    .filter-container {
        max-width: 1200px;
        margin: 0 auto;
        display: flex;
        gap: 10px;
        flex-wrap: wrap;
        justify-content: center;
        padding: 0 20px;
    }

    .filter-btn {
        padding: 8px 16px;
        background: rgba(255, 0, 110, 0.1);
        border: 2px solid var(--highlight);
        color: var(--highlight);
        border-radius: 20px;
        cursor: pointer;
        font-weight: 600;
        transition: all 0.3s;
        font-size: 0.85em;
    }

    .filter-btn:hover, .filter-btn.active {
        background: var(--highlight);
        color: white;
        box-shadow: 0 0 15px rgba(255, 0, 110, 0.4);
        transform: scale(1.05);
    }

    .ad-container-header {
        text-align: center;
        padding: 10px 0;
        width: 100%;
        min-height: 100px;
        display: flex;
        justify-content: center;
        align-items: center;
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
    }

    .game-card-content {
        padding: 20px;
    }

    .game-card-title {
        font-size: 1.3em;
        font-weight: 700;
        margin-bottom: 8px;
        color: var(--text);
    }

    .game-card-category {
        display: inline-block;
        padding: 4px 12px;
        background: rgba(0, 212, 255, 0.1);
        border: 1px solid var(--accent);
        color: var(--accent);
        border-radius: 12px;
        font-size: 0.8em;
        font-weight: 600;
    }

    /* Modal Styles */
    .modal {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: rgba(10, 14, 39, 0.98);
        z-index: 2000;
        display: none;
        justify-content: center;
        align-items: center;
        backdrop-filter: blur(10px);
    }

    .modal.active {
        display: flex;
    }

    .modal-content {
        width: 95%;
        max-width: 1000px;
        height: 90vh;
        background: var(--secondary);
        border: 2px solid var(--accent);
        border-radius: 20px;
        position: relative;
        overflow: hidden;
        display: flex;
        flex-direction: column;
    }

    .modal-header {
        padding: 15px 25px;
        background: var(--primary);
        border-bottom: 1px solid var(--border);
        display: flex;
        justify-content: space-between;
        align-items: center;
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

    .game-container {
        flex: 1;
        background: #000;
    }

    .gamepix-responsive {
        width: 100%;
        height: 100%;
    }

    .gamepix-responsive iframe {
        width: 100%;
        height: 100%;
        border: none;
    }

    /* Content Pages */
    .content-page {
        background: rgba(26, 31, 58, 0.6);
        border: 2px solid var(--border);
        border-radius: 20px;
        padding: 40px;
        max-width: 900px;
        margin: 0 auto;
    }

    .content-page h2 {
        color: var(--accent);
        font-size: 2.2em;
        margin-bottom: 25px;
        text-align: center;
    }

    .content-page h3 {
        color: var(--highlight);
        font-size: 1.6em;
        margin: 30px 0 15px;
    }

    .content-page p {
        line-height: 1.8;
        margin-bottom: 15px;
        color: var(--text);
    }

    .footer {
        background: linear-gradient(135deg, rgba(10, 14, 39, 0.95) 0%, rgba(26, 31, 58, 0.95) 100%);
        border-top: 2px solid var(--accent);
        padding: 40px 20px;
        text-align: center;
        color: var(--text-muted);
        margin-top: 60px;
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
        font-weight: 600;
        transition: 0.3s;
    }

    .footer-links a:hover {
        color: var(--highlight);
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

    .side-ad-left { left: 10px; }
    .side-ad-right { right: 10px; }

    @media (max-width: 1024px) {
        .side-ad { display: none; }
    }

    @media (max-width: 768px) {
        :root {
            --header-height: 140px;
            --nav-height: 120px;
            --filter-height: 180px;
        }
        .logo { font-size: 2em; }
        .nav-container { flex-direction: column; padding: 10px; gap: 10px; }
        .nav-links { width: 100%; justify-content: center; }
        .search-container { width: 100%; max-width: 100%; }
        .content-page { padding: 20px; }
    }
</style>



</head>
<body>
    <div class="main-header-container" id="mainHeader">
        <!-- Header -->
        <div class="header">
            <div class="header-content">
                <div class="logo" onclick="showPage('home')">🎮 SZ GAMES 🎮</div>
                <div class="tagline">Play 100+ Free Online Games - No Downloads Required</div>
            </div>
        </div>

Plain Text


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
        <!-- Adsterra Ad Below Filter -->
        <div class="ad-container-header">
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
</div>

<!-- Main Container -->
<div class="container">
    <!-- Sidebar Ads -->
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
        </div>
    </div>

    <!-- Contact Page -->
    <div id="contact" class="page">
        <div class="content-page">
            <h2>Contact Us</h2>
            <p>Have questions, suggestions, or feedback? We'd love to hear from you! Our team is always looking for ways to improve SZ GAMES.</p>
            <div class="contact-form">
                <div class="form-group">
                    <label>Name</label>
                    <input type="text" id="name" placeholder="Your Name">
                </div>
                <div class="form-group">
                    <label>Email</label>
                    <input type="email" id="email" placeholder="Your Email">
                </div>
                <div class="form-group">
                    <label>Subject</label>
                    <input type="text" id="subject" placeholder="Subject">
                </div>
                <div class="form-group">
                    <label>Message</label>
                    <textarea id="message" placeholder="Your Message"></textarea>
                </div>
                <button class="submit-btn" onclick="submitForm( )">Send Message</button>
            </div>
        </div>
    </div>

    <!-- Privacy Page -->
    <div id="privacy" class="page">
        <div class="content-page">
            <h2>Privacy Policy</h2>
            <p>At SZ GAMES, we take your privacy seriously. This policy outlines how we collect, use, and protect your information when you use our website.</p>
            <h3>Information Collection</h3>
            <p>We do not require users to create accounts or provide personal information to play games. We may collect non-personal information such as browser type, device information, and usage patterns to improve our services.</p>
        </div>
    </div>
</div>

<!-- Game Modal -->
<div id="gameModal" class="modal">
    <div class="modal-content">
        <div class="modal-header">
            <h2 id="modalTitle" style="color: var(--accent); margin: 0;">Game Title</h2>
            <span class="close-modal" onclick="closeGame()">&times;</span>
        </div>
        <div id="gameContainer" class="game-container"></div>
    </div>
</div>

<!-- Footer -->
<footer class="footer">
    <div class="footer-content">
        <p>&copy; 2024 SZ GAMES. All rights reserved.</p>
        <div class="footer-links">
            <a onclick="showPage('home')">Home</a>
            <a onclick="showPage('about')">About Us</a>
            <a onclick="showPage('contact')">Contact Us</a>
            <a onclick="showPage('privacy')">Privacy Policy</a>
        </div>
    </div>
</footer>

<script>
    const games = [
        // ACTION GAMES (1-20)
        {id: 1, name: 'Cyber Hunter', category: 'Action', description: 'Fast-paced futuristic shooter', embedUrl: 'https://play.gamepix.com/cyber-hunter/embed?sid=1', emoji: '🔫'},
        {id: 2, name: 'Ninja Run', category: 'Action', description: 'Test your reflexes as a ninja', embedUrl: 'https://play.gamepix.com/ninja-run/embed?sid=1', emoji: '🥷'},
        {id: 3, name: 'Space Wars', category: 'Action', description: 'Epic space battles', embedUrl: 'https://play.gamepix.com/space-wars/embed?sid=1', emoji: '🚀'},
        {id: 4, name: 'Zombie Defense', category: 'Action', description: 'Survive the zombie apocalypse', embedUrl: 'https://play.gamepix.com/zombie-defense/embed?sid=1', emoji: '🧟'},
        {id: 5, name: 'Street Fighter', category: 'Action', description: 'Classic fighting game', embedUrl: 'https://play.gamepix.com/street-fighter/embed?sid=1', emoji: '🥊'},
        {id: 6, name: 'Tank Battle', category: 'Action', description: 'Intense tank warfare', embedUrl: 'https://play.gamepix.com/tank-battle/embed?sid=1', emoji: '🚜'},
        {id: 7, name: 'Robot Arena', category: 'Action', description: 'Battle with powerful robots', embedUrl: 'https://play.gamepix.com/robot-arena/embed?sid=1', emoji: '🤖'},
        {id: 8, name: 'Alien Invasion', category: 'Action', description: 'Defend Earth from aliens', embedUrl: 'https://play.gamepix.com/alien-invasion/embed?sid=1', emoji: '👽'},
        {id: 9, name: 'Sword Master', category: 'Action', description: 'Master the art of the sword', embedUrl: 'https://play.gamepix.com/sword-master/embed?sid=1', emoji: '⚔️'},
        {id: 10, name: 'Hero Quest', category: 'Action', description: 'Become a legendary hero', embedUrl: 'https://play.gamepix.com/hero-quest/embed?sid=1', emoji: '🛡️'},
        {id: 11, name: 'Shadow Assassin', category: 'Action', description: 'Stealth-based action', embedUrl: 'https://play.gamepix.com/shadow-assassin/embed?sid=1', emoji: '👤'},
        {id: 12, name: 'Dragon Slayer', category: 'Action', description: 'Hunt mythical dragons', embedUrl: 'https://play.gamepix.com/dragon-slayer/embed?sid=1', emoji: '🐉'},
        {id: 13, name: 'Super Soldier', category: 'Action', description: 'Elite military missions', embedUrl: 'https://play.gamepix.com/super-soldier/embed?sid=1', emoji: '🎖️'},
        {id: 14, name: 'Monster Hunter', category: 'Action', description: 'Battle giant monsters', embedUrl: 'https://play.gamepix.com/monster-hunter/embed?sid=1', emoji: '👹'},
        {id: 15, name: 'Galaxy Defender', category: 'Action', description: 'Protect the galaxy', embedUrl: 'https://play.gamepix.com/galaxy-defender/embed?sid=1', emoji: '🌌'},
        {id: 16, name: 'Pirate Adventure', category: 'Action', description: 'Sail the high seas', embedUrl: 'https://play.gamepix.com/pirate-adventure/embed?sid=1', emoji: '🏴‍☠️'},
        {id: 17, name: 'Viking War', category: 'Action', description: 'Lead Vikings to victory', embedUrl: 'https://play.gamepix.com/viking-war/embed?sid=1', emoji: '🪓'},
        {id: 18, name: 'Samurai Duel', category: 'Action', description: 'Honorable samurai combat', embedUrl: 'https://play.gamepix.com/samurai-duel/embed?sid=1', emoji: '🏮'},
        {id: 19, name: 'Commando Strike', category: 'Action', description: 'Tactical combat missions', embedUrl: 'https://play.gamepix.com/commando-strike/embed?sid=1', emoji: '🔫'},
        {id: 20, name: 'Mech Warrior', category: 'Action', description: 'Pilot giant mechs', embedUrl: 'https://play.gamepix.com/mech-warrior/embed?sid=1', emoji: '🦾'},

        // PUZZLE GAMES (21-40 )
        {id: 21, name: 'Jewel Match', category: 'Puzzle', description: 'Classic match-3 puzzle', embedUrl: 'https://play.gamepix.com/jewel-match/embed?sid=1', emoji: '💎'},
        {id: 22, name: 'Bubble Shooter', category: 'Puzzle', description: 'Pop bubbles and clear levels', embedUrl: 'https://play.gamepix.com/bubble-shooter/embed?sid=1', emoji: '🫧'},
        {id: 23, name: '2048', category: 'Puzzle', description: 'Combine numbers to reach 2048', embedUrl: 'https://play.gamepix.com/2048/embed?sid=1', emoji: '🔢'},
        {id: 24, name: 'Mahjong Solitaire', category: 'Puzzle', description: 'Classic tile-matching game', embedUrl: 'https://play.gamepix.com/mahjong/embed?sid=1', emoji: '🀄'},
        {id: 25, name: 'Maze Runner', category: 'Puzzle', description: 'Find your way through mazes', embedUrl: 'https://play.gamepix.com/maze-runner/embed?sid=1', emoji: '🌀'},
        {id: 26, name: 'Memory Match', category: 'Puzzle', description: 'Test your memory skills', embedUrl: 'https://play.gamepix.com/memory-match/embed?sid=1', emoji: '🧠'},
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

        // ADVENTURE GAMES (41-60 )
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

        // STRATEGY GAMES (61-80 )
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

        // SPORTS GAMES (81-100 )
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

    function showPage(pageName ) {
        currentPage = pageName;
        document.querySelectorAll('.page').forEach(page => page.classList.remove('active'));
        document.getElementById(pageName).classList.add('active');
        
        document.querySelectorAll('.nav-btn').forEach(btn => {
            btn.classList.remove('active');
            if (btn.getAttribute('onclick').includes(pageName)) btn.classList.add('active');
        });

        const filterWrapper = document.getElementById('filterWrapper');
        filterWrapper.style.display = pageName === 'home' ? 'flex' : 'none';
        
        // Update body padding based on visible elements
        const headerHeight = document.getElementById('mainHeader').offsetHeight;
        document.body.style.paddingTop = pageName === 'home' ? 'calc(var(--header-height) + var(--nav-height) + var(--filter-height))' : 'calc(var(--header-height) + var(--nav-height))';
        
        window.scrollTo(0, 0);
    }

    function filterCategory(category) {
        currentCategory = category;
        document.querySelectorAll('.filter-btn').forEach(btn => {
            btn.classList.toggle('active', btn.innerText.includes(category));
        });
        renderGames();
    }

    document.getElementById('searchInput').addEventListener('input', (e) => {
        currentSearch = e.target.value.toLowerCase();
        renderGames();
    });

    function renderGames() {
        const grid = document.getElementById('gamesGrid');
        const filteredGames = games.filter(game => {
            const matchesCategory = currentCategory === 'All' || game.category === currentCategory;
            const matchesSearch = game.name.toLowerCase().includes(currentSearch) || 
                                game.description.toLowerCase().includes(currentSearch);
            return matchesCategory && matchesSearch;
        });

        if (filteredGames.length === 0) {
            grid.innerHTML = '<div class="no-games">No games found matching your search.</div>';
            return;
        }

        grid.innerHTML = filteredGames.map(game => `
            <div class="game-card" onclick="playGame(${game.id}, '${game.name}', '${game.embedUrl}')">
                <div class="game-card-image">${game.emoji}</div>
                <div class="game-card-content">
                    <div class="game-card-title">${game.name}</div>
                    <div class="game-card-category">${game.category}</div>
                </div>
            </div>
        `).join('');
    }

    function playGame(id, name, embedUrl) {
        document.getElementById('modalTitle').innerText = name;
        document.getElementById('gameContainer').innerHTML = `
            <div class="gamepix-responsive">
                <iframe src="${embedUrl}" frameborder="0" scrolling="no" allowfullscreen></iframe>
            </div>
        `;
        document.getElementById('gameModal').classList.add('active');
    }

    function closeGame() {
        document.getElementById('gameModal').classList.remove('active');
        document.getElementById('gameContainer').innerHTML = '';
    }

    function submitForm() {
        const name = document.getElementById('name').value;
        const email = document.getElementById('email').value;
        if (name && email) {
            alert('Thank you for contacting us!');
            ['name', 'email', 'subject', 'message'].forEach(id => document.getElementById(id).value = '');
        } else {
            alert('Please fill all fields');
        }
    }

    // Improved Auto-hide logic
    let lastScrollTop = 0;
    const mainHeader = document.getElementById('mainHeader');
    const scrollThreshold = 10;

    window.addEventListener('scroll', () => {
        let currentScroll = window.pageYOffset || document.documentElement.scrollTop;
        
        if (Math.abs(lastScrollTop - currentScroll) <= scrollThreshold) return;

        if (currentScroll > lastScrollTop && currentScroll > 200) {
            // Scrolling DOWN
            mainHeader.classList.add('hide');
        } else {
            // Scrolling UP
            mainHeader.classList.remove('hide');
        }
        
        lastScrollTop = currentScroll <= 0 ? 0 : currentScroll;
    }, { passive: true });

    renderGames();
</script>



</body>
</html>

