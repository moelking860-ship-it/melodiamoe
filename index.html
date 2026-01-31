<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Melodia - Plateforme Musicale Créée par Moe L'king</title>
    <meta name="author" content="Moe L'king">
    <meta name="description" content="Melodia - La plateforme musicale complète créée par Moe L'king pour distribuer, streamer et gérer votre musique">
    
    <!-- AJOUT : Bibliothèque Supabase -->
    <script src="https://cdn.jsdelivr.net/npm/@supabase/supabase-js@2"></script>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --primary: #6366f1;
            --primary-dark: #4f46e5;
            --secondary: #ec4899;
            --dark: #0f172a;
            --dark-light: #1e293b;
            --gray: #64748b;
            --light: #f1f5f9;
            --success: #10b981;
            --danger: #ef4444;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
            background: var(--dark);
            color: #fff;
            line-height: 1.6;
            overflow-x: hidden;
        }

        /* Header & Navigation */
        header {
            background: rgba(15, 23, 42, 0.95);
            backdrop-filter: blur(10px);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 5%;
            max-width: 1400px;
            margin: 0 auto;
            width: 100%;
        }

        .logo {
            font-size: 1.8rem;
            font-weight: 800;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            cursor: pointer;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

        .logo-subtext {
            font-size: 0.7rem;
            color: var(--gray);
            margin-left: 0.5rem;
            font-weight: 500;
        }

        .nav-links {
            display: flex;
            gap: 2rem;
            list-style: none;
        }

        .nav-links a {
            color: #fff;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
            cursor: pointer;
        }

        .nav-links a:hover {
            color: var(--primary);
        }

        .user-menu {
            position: relative;
        }

        .user-avatar {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            font-weight: 600;
            font-size: 1.1rem;
        }

        .dropdown {
            position: absolute;
            top: 60px;
            right: 0;
            background: var(--dark-light);
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 12px;
            padding: 1rem;
            min-width: 200px;
            display: none;
            box-shadow: 0 10px 40px rgba(0, 0, 0, 0.5);
        }

        .dropdown.active {
            display: block;
        }

        .dropdown-item {
            padding: 0.8rem;
            border-radius: 8px;
            cursor: pointer;
            transition: background 0.3s;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

        .dropdown-item:hover {
            background: rgba(99, 102, 241, 0.1);
        }

        .btn {
            padding: 0.7rem 1.5rem;
            border-radius: 8px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s;
            border: none;
            font-size: 0.95rem;
        }

        .btn-primary {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
        }

        .btn-primary:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 25px rgba(99, 102, 241, 0.3);
        }

        .btn-secondary {
            background: transparent;
            color: white;
            border: 2px solid var(--primary);
        }

        .btn-secondary:hover {
            background: var(--primary);
        }

        .btn-danger {
            background: var(--danger);
            color: white;
        }

        /* Modal System */
        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.8);
            z-index: 2000;
            align-items: center;
            justify-content: center;
        }

        .modal.active {
            display: flex;
        }

        .modal-content {
            background: var(--dark-light);
            border-radius: 20px;
            padding: 2.5rem;
            max-width: 500px;
            width: 90%;
            max-height: 90vh;
            overflow-y: auto;
            position: relative;
            border: 1px solid rgba(255, 255, 255, 0.1);
        }

        .modal-close {
            position: absolute;
            top: 1.5rem;
            right: 1.5rem;
            font-size: 1.5rem;
            cursor: pointer;
            color: var(--gray);
            transition: color 0.3s;
        }

        .modal-close:hover {
            color: white;
        }

        .modal-title {
            font-size: 2rem;
            margin-bottom: 2rem;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .form-group {
            margin-bottom: 1.5rem;
        }

        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 600;
        }

        .form-group input,
        .form-group textarea,
        .form-group select {
            width: 100%;
            padding: 0.8rem;
            background: var(--dark);
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 8px;
            color: white;
            font-size: 1rem;
            transition: border-color 0.3s;
        }

        .form-group input:focus,
        .form-group textarea:focus,
        .form-group select:focus {
            outline: none;
            border-color: var(--primary);
        }

        .form-group textarea {
            resize: vertical;
            min-height: 100px;
        }

        .file-upload {
            border: 2px dashed rgba(99, 102, 241, 0.3);
            padding: 2rem;
            text-align: center;
            border-radius: 12px;
            cursor: pointer;
            transition: all 0.3s;
        }

        .file-upload:hover {
            border-color: var(--primary);
            background: rgba(99, 102, 241, 0.05);
        }

        .file-upload input {
            display: none;
        }

        .preview-image {
            max-width: 100%;
            max-height: 200px;
            border-radius: 12px;
            margin-top: 1rem;
        }

        /* Pages */
        .page {
            display: none;
            padding: 6rem 5% 3rem;
            min-height: 100vh;
        }

        .page.active {
            display: block;
        }

        .container {
            max-width: 1400px;
            margin: 0 auto;
        }

        /* Dashboard */
        .dashboard-grid {
            display: grid;
            grid-template-columns: 250px 1fr;
            gap: 2rem;
            margin-top: 2rem;
        }

        .sidebar {
            background: var(--dark-light);
            border-radius: 15px;
            padding: 1.5rem;
            height: fit-content;
            position: sticky;
            top: 100px;
        }

        .sidebar-item {
            padding: 1rem;
            border-radius: 8px;
            cursor: pointer;
            transition: all 0.3s;
            margin-bottom: 0.5rem;
            display: flex;
            align-items: center;
            gap: 0.8rem;
        }

        .sidebar-item:hover,
        .sidebar-item.active {
            background: rgba(99, 102, 241, 0.1);
            color: var(--primary);
        }

        .dashboard-content {
            background: var(--dark-light);
            border-radius: 15px;
            padding: 2rem;
        }

        /* Music Grid */
        .music-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 1.5rem;
            margin-top: 2rem;
        }

        .music-card {
            background: rgba(30, 41, 59, 0.6);
            border-radius: 12px;
            overflow: hidden;
            cursor: pointer;
            transition: all 0.3s;
            border: 1px solid rgba(255, 255, 255, 0.05);
        }

        .music-card:hover {
            transform: translateY(-5px);
            border-color: var(--primary);
        }

        .music-cover {
            width: 100%;
            height: 250px;
            object-fit: cover;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
        }

        .music-info {
            padding: 1rem;
        }

        .music-title {
            font-weight: 600;
            margin-bottom: 0.3rem;
            font-size: 1.1rem;
        }

        .music-artist {
            color: var(--gray);
            font-size: 0.9rem;
            margin-bottom: 0.5rem;
        }

        .music-metadata {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
            margin-top: 0.8rem;
        }

        .metadata-tag {
            background: rgba(99, 102, 241, 0.1);
            padding: 0.3rem 0.8rem;
            border-radius: 20px;
            font-size: 0.8rem;
            color: var(--primary);
        }

        .music-actions {
            display: flex;
            gap: 1rem;
            margin-top: 1rem;
            padding-top: 1rem;
            border-top: 1px solid rgba(255, 255, 255, 0.05);
        }

        .action-btn {
            flex: 1;
            padding: 0.6rem;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            font-weight: 600;
            transition: all 0.3s;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 0.5rem;
        }

        .play-btn-card {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
        }

        .like-btn {
            background: rgba(236, 72, 153, 0.1);
            color: var(--secondary);
        }

        .like-btn.liked {
            background: var(--secondary);
            color: white;
        }

        /* Audio Player */
        .audio-player {
            position: fixed;
            bottom: 0;
            left: 0;
            right: 0;
            background: rgba(30, 41, 59, 0.98);
            backdrop-filter: blur(20px);
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            padding: 1.5rem 5%;
            z-index: 999;
            display: none;
        }

        .audio-player.active {
            display: block;
        }

        .player-container {
            max-width: 1400px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: auto 1fr auto;
            gap: 2rem;
            align-items: center;
        }

        .player-info {
            display: flex;
            align-items: center;
            gap: 1rem;
        }

        .player-cover {
            width: 60px;
            height: 60px;
            border-radius: 8px;
            object-fit: cover;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
        }

        .player-controls {
            display: flex;
            flex-direction: column;
            gap: 0.8rem;
        }

        .controls-buttons {
            display: flex;
            justify-content: center;
            gap: 1rem;
        }

        .control-btn {
            background: transparent;
            border: none;
            color: white;
            font-size: 1.5rem;
            cursor: pointer;
            transition: all 0.3s;
            width: 40px;
            height: 40px;
            display: flex;
            align-items: center;
            justify-content: center;
            border-radius: 50%;
        }

        .control-btn:hover {
            background: rgba(255, 255, 255, 0.1);
        }

        .play-btn-main {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            width: 50px;
            height: 50px;
            font-size: 1.8rem;
        }

        .progress-container {
            display: flex;
            align-items: center;
            gap: 1rem;
        }

        .progress-bar {
            flex: 1;
            height: 6px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 3px;
            cursor: pointer;
            position: relative;
        }

        .progress-fill {
            height: 100%;
            background: linear-gradient(90deg, var(--primary), var(--secondary));
            border-radius: 3px;
            width: 0%;
            position: relative;
        }

        .progress-fill::after {
            content: '';
            position: absolute;
            right: 0;
            top: 50%;
            transform: translateY(-50%);
            width: 12px;
            height: 12px;
            background: white;
            border-radius: 50%;
        }

        .time-display {
            font-size: 0.85rem;
            color: var(--gray);
            min-width: 100px;
            text-align: center;
        }

        .volume-control {
            display: flex;
            align-items: center;
            gap: 1rem;
        }

        .volume-bar {
            width: 100px;
            height: 4px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 2px;
            cursor: pointer;
            position: relative;
        }

        .volume-fill {
            height: 100%;
            background: var(--primary);
            border-radius: 2px;
            width: 70%;
        }

        /* Comments Section */
        .comments-section {
            margin-top: 2rem;
            background: var(--dark);
            border-radius: 12px;
            padding: 1.5rem;
        }

        .comment-form {
            display: flex;
            gap: 1rem;
            margin-bottom: 2rem;
        }

        .comment-input {
            flex: 1;
            padding: 0.8rem;
            background: var(--dark-light);
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 8px;
            color: white;
        }

        .comment {
            display: flex;
            gap: 1rem;
            padding: 1rem;
            border-bottom: 1px solid rgba(255, 255, 255, 0.05);
        }

        .comment-avatar {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: 600;
        }

        .comment-content {
            flex: 1;
        }

        .comment-author {
            font-weight: 600;
            margin-bottom: 0.3rem;
        }

        .comment-time {
            font-size: 0.8rem;
            color: var(--gray);
            margin-bottom: 0.5rem;
        }

        /* Profile Page */
        .profile-header {
            background: var(--dark-light);
            border-radius: 15px;
            padding: 2rem;
            display: flex;
            gap: 2rem;
            align-items: center;
            margin-bottom: 2rem;
        }

        .profile-avatar-large {
            width: 120px;
            height: 120px;
            border-radius: 50%;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 3rem;
            font-weight: 600;
        }

        .profile-stats {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 2rem;
            margin-top: 2rem;
        }

        .stat-card {
            background: var(--dark);
            border-radius: 12px;
            padding: 1.5rem;
            text-align: center;
        }

        .stat-value {
            font-size: 2rem;
            font-weight: 700;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .stat-label {
            color: var(--gray);
            margin-top: 0.5rem;
        }

        /* Hero Section */
        .hero {
            margin-top: 80px;
            padding: 4rem 5% 2rem;
            background: linear-gradient(135deg, #1e293b 0%, #0f172a 100%);
            text-align: center;
        }

        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 1.5rem;
            background: linear-gradient(135deg, #fff 0%, #cbd5e1 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .hero-subtitle {
            font-size: 1rem;
            color: var(--gray);
            margin-bottom: 1rem;
            font-style: italic;
        }

        .hero p {
            font-size: 1.3rem;
            color: var(--gray);
            margin-bottom: 2rem;
        }

        /* Stats */
        .stats {
            padding: 3rem 5%;
            background: var(--dark-light);
        }

        .stats-grid {
            max-width: 1400px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 2rem;
            text-align: center;
        }

        .stat-item h3 {
            font-size: 2.5rem;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        /* Footer */
        .footer {
            background: rgba(15, 23, 42, 0.95);
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            padding: 2rem 5%;
            text-align: center;
            color: var(--gray);
            font-size: 0.9rem;
            margin-top: 2rem;
        }

        .footer-creator {
            color: var(--primary);
            font-weight: 600;
        }

        /* Alert */
        .alert {
            position: fixed;
            top: 100px;
            right: 20px;
            padding: 1rem 1.5rem;
            border-radius: 12px;
            background: var(--dark-light);
            border: 1px solid rgba(255, 255, 255, 0.1);
            z-index: 3000;
            animation: slideIn 0.3s ease-out;
            display: none;
        }

        .alert.active {
            display: block;
        }

        .alert.success {
            border-color: var(--success);
            background: rgba(16, 185, 129, 0.1);
        }

        .alert.error {
            border-color: var(--danger);
            background: rgba(239, 68, 68, 0.1);
        }

        @keyframes slideIn {
            from {
                transform: translateX(400px);
                opacity: 0;
            }
            to {
                transform: translateX(0);
                opacity: 1;
            }
        }

        /* Responsive */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }

            .dashboard-grid {
                grid-template-columns: 1fr;
            }

            .sidebar {
                position: static;
            }

            .player-container {
                grid-template-columns: 1fr;
            }

            .stats-grid {
                grid-template-columns: repeat(2, 1fr);
            }

            .profile-stats {
                grid-template-columns: repeat(2, 1fr);
            }

            .hero h1 {
                font-size: 2.5rem;
            }
        }

        /* Scrollbar */
        ::-webkit-scrollbar {
            width: 10px;
        }

        ::-webkit-scrollbar-track {
            background: var(--dark);
        }

        ::-webkit-scrollbar-thumb {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            border-radius: 5px;
        }
    </style>
</head>
<body>
    <!-- Alert System -->
    <div id="alert" class="alert"></div>

    <!-- Header -->
    <header>
        <nav>
            <div class="logo" onclick="showPage('home')">
                🎵 Melodia
                <span class="logo-subtext">Par Moe L'king</span>
            </div>
            <ul class="nav-links" id="navLinks">
                <li><a onclick="showPage('home')">Accueil</a></li>
                <li><a onclick="showPage('explore')">Explorer</a></li>
                <li><a onclick="showPage('dashboard')" id="dashboardLink" style="display: none;">Dashboard</a></li>
            </ul>
            <div id="authButtons">
                <button class="btn btn-secondary" onclick="showModal('login')">Connexion</button>
                <button class="btn btn-primary" onclick="showModal('register')">Inscription</button>
            </div>
            <div id="userMenu" class="user-menu" style="display: none;">
                <div class="user-avatar" onclick="toggleDropdown()">
                    <span id="userInitials"></span>
                </div>
                <div id="userDropdown" class="dropdown">
                    <div class="dropdown-item" onclick="showPage('profile')">
                        👤 Mon Profil
                    </div>
                    <div class="dropdown-item" onclick="showPage('dashboard')">
                        📊 Dashboard
                    </div>
                    <div class="dropdown-item" onclick="showModal('upload')">
                        ⬆️ Upload Musique
                    </div>
                    <div class="dropdown-item" onclick="logout()">
                        🚪 Déconnexion
                    </div>
                </div>
            </div>
        </nav>
    </header>

    <!-- Login Modal -->
    <div id="loginModal" class="modal">
        <div class="modal-content">
            <span class="modal-close" onclick="closeModal('login')">&times;</span>
            <h2 class="modal-title">Connexion à Melodia</h2>
            <form onsubmit="login(event)">
                <div class="form-group">
                    <label>Email</label>
                    <input type="email" id="loginEmail" required>
                </div>
                <div class="form-group">
                    <label>Mot de passe</label>
                    <input type="password" id="loginPassword" required>
                </div>
                <button type="submit" class="btn btn-primary" style="width: 100%;">Se connecter</button>
                <p style="text-align: center; margin-top: 1rem; color: var(--gray);">
                    Pas de compte ? <a onclick="closeModal('login'); showModal('register')" style="color: var(--primary); cursor: pointer;">Inscrivez-vous</a>
                </p>
            </form>
        </div>
    </div>

    <!-- Register Modal -->
    <div id="registerModal" class="modal">
        <div class="modal-content">
            <span class="modal-close" onclick="closeModal('register')">&times;</span>
            <h2 class="modal-title">Rejoindre Melodia</h2>
            <form onsubmit="register(event)">
                <div class="form-group">
                    <label>Nom d'artiste</label>
                    <input type="text" id="registerName" required>
                </div>
                <div class="form-group">
                    <label>Email</label>
                    <input type="email" id="registerEmail" required>
                </div>
                <div class="form-group">
                    <label>Mot de passe</label>
                    <input type="password" id="registerPassword" required minlength="6">
                </div>
                <div class="form-group">
                    <label>Bio (optionnel)</label>
                    <textarea id="registerBio" rows="3"></textarea>
                </div>
                <button type="submit" class="btn btn-primary" style="width: 100%;">Créer mon compte</button>
                <p style="text-align: center; margin-top: 1rem; color: var(--gray);">
                    Déjà un compte ? <a onclick="closeModal('register'); showModal('login')" style="color: var(--primary); pointer; cursor: pointer;">Connectez-vous</a>
                </p>
            </form>
        </div>
    </div>

    <!-- Upload Modal -->
    <div id="uploadModal" class="modal">
        <div class="modal-content" style="max-width: 600px;">
            <span class="modal-close" onclick="closeModal('upload')">&times;</span>
            <h2 class="modal-title">Upload sur Melodia</h2>
            <form onsubmit="uploadMusic(event)">
                <div class="form-group">
                    <label>Fichier Audio *</label>
                    <div class="file-upload" onclick="document.getElementById('audioFile').click()">
                        <input type="file" id="audioFile" accept="audio/*" required onchange="previewAudio(this)">
                        <p>📁 Cliquez pour sélectionner un fichier audio</p>
                        <p style="font-size: 0.9rem; color: var(--gray);">MP3, WAV, FLAC (max 50MB)</p>
                        <div id="audioPreview"></div>
                    </div>
                </div>
                <div class="form-group">
                    <label>Cover Art *</label>
                    <div class="file-upload" onclick="document.getElementById('coverFile').click()">
                        <input type="file" id="coverFile" accept="image/*" required onchange="previewCover(this)">
                        <p>🖼️ Cliquez pour sélectionner une image</p>
                        <p style="font-size: 0.9rem; color: var(--gray);">JPG, PNG (min 1000x1000px)</p>
                        <img id="coverPreview" class="preview-image" style="display: none;">
                    </div>
                </div>
                <div class="form-group">
                    <label>Titre de la chanson *</label>
                    <input type="text" id="songTitle" required>
                </div>
                <div class="form-group">
                    <label>Genre *</label>
                    <select id="songGenre" required>
                        <option value="">Sélectionnez un genre</option>
                        <option value="Pop">Pop</option>
                        <option value="Hip-Hop">Hip-Hop/Rap</option>
                        <option value="Rock">Rock</option>
                        <option value="Électronique">Électronique</option>
                        <option value="R&B">R&B</option>
                        <option value="Jazz">Jazz</option>
                        <option value="Classique">Classique</option>
                        <option value="Country">Country</option>
                        <option value="Reggae">Reggae</option>
                        <option value="Metal">Metal</option>
                    </select>
                </div>
                <div class="form-group">
                    <label>Producteur(s)</label>
                    <input type="text" id="songProducer" placeholder="Nom du/des producteur(s)">
                </div>
                <div class="form-group">
                    <label>Mixage par</label>
                    <input type="text" id="songMixing" placeholder="Ingénieur de mixage">
                </div>
                <div class="form-group">
                    <label>Mastering par</label>
                    <input type="text" id="songMastering" placeholder="Ingénieur de mastering">
                </div>
                <div class="form-group">
                    <label>Featuring (optionnel)</label>
                    <input type="text" id="songFeaturing" placeholder="Artistes en featuring">
                </div>
                <div class="form-group">
                    <label>Année de sortie</label>
                    <input type="number" id="songYear" min="1900" max="2030" value="2026">
                </div>
                <div class="form-group">
                    <label>Description / Paroles</label>
                    <textarea id="songDescription" rows="4"></textarea>
                </div>
                <button type="submit" class="btn btn-primary" style="width: 100%;">
                    📤 Uploader et Distribuer
                </button>
            </form>
        </div>
    </div>

    <!-- Edit Profile Modal -->
    <div id="editProfileModal" class="modal">
        <div class="modal-content">
            <span class="modal-close" onclick="closeModal('editProfile')">&times;</span>
            <h2 class="modal-title">Modifier votre Profil</h2>
            <form onsubmit="updateProfile(event)">
                <div class="form-group">
                    <label>Nom d'artiste</label>
                    <input type="text" id="editName" required>
                </div>
                <div class="form-group">
                    <label>Email</label>
                    <input type="email" id="editEmail" required>
                </div>
                <div class="form-group">
                    <label>Bio</label>
                    <textarea id="editBio" rows="4"></textarea>
                </div>
                <div class="form-group">
                    <label>Localisation</label>
                    <input type="text" id="editLocation" placeholder="Ville, Pays">
                </div>
                <button type="submit" class="btn btn-primary" style="width: 100%;">Sauvegarder</button>
            </form>
        </div>
    </div>

    <!-- Edit Music Modal -->
    <div id="editMusicModal" class="modal">
        <div class="modal-content" style="max-width: 600px;">
            <span class="modal-close" onclick="closeModal('editMusic')">&times;</span>
            <h2 class="modal-title">Modifier votre Musique</h2>
            <form onsubmit="updateMusic(event)">
                <input type="hidden" id="editMusicId">
                <div class="form-group">
                    <label>Nouvelle Cover (optionnel)</label>
                    <div class="file-upload" onclick="document.getElementById('editCoverFile').click()">
                        <input type="file" id="editCoverFile" accept="image/*" onchange="previewEditCover(this)">
                        <img id="editCoverPreview" class="preview-image">
                    </div>
                </div>
                <div class="form-group">
                    <label>Titre</label>
                    <input type="text" id="editSongTitle" required>
                </div>
                <div class="form-group">
                    <label>Genre</label>
                    <select id="editSongGenre" required>
                        <option value="Pop">Pop</option>
                        <option value="Hip-Hop">Hip-Hop/Rap</option>
                        <option value="Rock">Rock</option>
                        <option value="Électronique">Électronique</option>
                        <option value="R&B">R&B</option>
                        <option value="Jazz">Jazz</option>
                        <option value="Classique">Classique</option>
                        <option value="Country">Country</option>
                    </select>
                </div>
                <div class="form-group">
                    <label>Producteur(s)</label>
                    <input type="text" id="editSongProducer">
                </div>
                <div class="form-group">
                    <label>Mixage</label>
                    <input type="text" id="editSongMixing">
                </div>
                <div class="form-group">
                    <label>Mastering</label>
                    <input type="text" id="editSongMastering">
                </div>
                <div class="form-group">
                    <label>Description</label>
                    <textarea id="editSongDescription" rows="4"></textarea>
                </div>
                <button type="submit" class="btn btn-primary" style="width: 100%;">Sauvegarder</button>
                <button type="button" class="btn btn-danger" style="width: 100%; margin-top: 1rem;" onclick="deleteMusic()">
                    🗑️ Supprimer cette musique
                </button>
            </form>
        </div>
    </div>

    <!-- Home Page -->
    <div id="homePage" class="page active">
        <section class="hero">
            <div class="container">
                <h1>Bienvenue sur Melodia</h1>
                <p class="hero-subtitle">Créée par Moe L'king</p>
                <p>La plateforme complète pour distribuer, streamer et gérer votre musique</p>
                <button class="btn btn-primary" onclick="showModal('register')" style="font-size: 1.1rem; padding: 1rem 2rem;">
                    Commencer Gratuitement
                </button>
            </div>
        </section>

        <section class="stats">
            <div class="stats-grid">
                <div class="stat-item">
                    <h3 id="totalUsers">0</h3>
                    <p>Artistes actifs</p>
                </div>
                <div class="stat-item">
                    <h3 id="totalTracks">0</h3>
                    <p>Titres distribués</p>
                </div>
                <div class="stat-item">
                    <h3 id="totalPlays">0</h3>
                    <p>Lectures totales</p>
                </div>
                <div class="stat-item">
                    <h3 id="totalLikes">0</h3>
                    <p>J'aime</p>
                </div>
            </div>
        </section>
    </div>

    <!-- Explore Page -->
    <div id="explorePage" class="page">
        <div class="container">
            <h1 style="margin-bottom: 2rem;">Explorer la Musique sur Melodia</h1>
            <div id="exploreGrid" class="music-grid"></div>
        </div>
    </div>

    <!-- Dashboard Page -->
    <div id="dashboardPage" class="page">
        <div class="container">
            <h1 style="margin-bottom: 2rem;">Votre Dashboard Melodia</h1>
            <div class="dashboard-grid">
                <div class="sidebar">
                    <div class="sidebar-item active" onclick="showDashboardSection('mymusic')">
                        🎵 Ma Musique
                    </div>
                    <div class="sidebar-item" onclick="showDashboardSection('analytics')">
                        📊 Analytics
                    </div>
                    <div class="sidebar-item" onclick="showModal('upload')">
                        ⬆️ Upload
                    </div>
                </div>
                <div class="dashboard-content">
                    <div id="myMusicSection">
                        <div style="display: flex; justify-content: space-between; align-items: center; margin-bottom: 2rem;">
                            <h2>Ma Musique sur Melodia</h2>
                            <button class="btn btn-primary" onclick="showModal('upload')">
                                ⬆️ Upload Nouvelle Musique
                            </button>
                        </div>
                        <div id="myMusicGrid" class="music-grid"></div>
                    </div>
                    <div id="analyticsSection" style="display: none;">
                        <h2 style="margin-bottom: 2rem;">Mes Analytics Melodia</h2>
                        <div class="profile-stats">
                            <div class="stat-card">
                                <div class="stat-value" id="userTotalPlays">0</div>
                                <div class="stat-label">Lectures totales</div>
                            </div>
                            <div class="stat-card">
                                <div class="stat-value" id="userTotalLikes">0</div>
                                <div class="stat-label">J'aime</div>
                            </div>
                            <div class="stat-card">
                                <div class="stat-value" id="userTotalTracks">0</div>
                                <div class="stat-label">Titres</div>
                            </div>
                            <div class="stat-card">
                                <div class="stat-value" id="userTotalComments">0</div>
                                <div class="stat-label">Commentaires</div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Profile Page -->
    <div id="profilePage" class="page">
        <div class="container">
            <div class="profile-header">
                <div class="profile-avatar-large" id="profileAvatar"></div>
                <div style="flex: 1;">
                    <div style="display: flex; justify-content: space-between; align-items: center;">
                        <div>
                            <h1 id="profileName"></h1>
                            <p style="color: var(--gray); margin-top: 0.5rem;" id="profileEmail"></p>
                        </div>
                        <button class="btn btn-primary" onclick="openEditProfile()">
                            ✏️ Modifier le profil
                        </button>
                    </div>
                    <p style="margin-top: 1rem;" id="profileBio"></p>
                    <p style="color: var(--gray); margin-top: 0.5rem;" id="profileLocation"></p>
                </div>
            </div>
            <div class="profile-stats">
                <div class="stat-card">
                    <div class="stat-value" id="profileTotalPlays">0</div>
                    <div class="stat-label">Lectures</div>
                </div>
                <div class="stat-card">
                    <div class="stat-value" id="profileTotalLikes">0</div>
                    <div class="stat-label">J'aime</div>
                </div>
                <div class="stat-card">
                    <div class="stat-value" id="profileTotalTracks">0</div>
                    <div class="stat-label">Titres</div>
                </div>
                <div class="stat-card">
                    <div class="stat-value" id="profileFollowers">0</div>
                    <div class="stat-label">Followers</div>
                </div>
            </div>
            <h2 style="margin: 2rem 0;">Mes Musiques</h2>
            <div id="profileMusicGrid" class="music-grid"></div>
        </div>
    </div>

    <!-- Audio Player -->
    <div id="audioPlayer" class="audio-player">
        <audio id="audioElement"></audio>
        <div class="player-container">
            <div class="player-info">
                <img id="currentCover" class="player-cover">
                <div>
                    <div style="font-weight: 600;" id="currentTitle">Titre</div>
                    <div style="color: var(--gray); font-size: 0.9rem;" id="currentArtist">Artiste</div>
                </div>
            </div>
            <div class="player-controls">
                <div class="controls-buttons">
                    <button class="control-btn" onclick="previousTrack()">⏮</button>
                    <button class="control-btn play-btn-main" id="playPauseBtn" onclick="togglePlay()">▶</button>
                    <button class="control-btn" onclick="nextTrack()">⏭</button>
                </div>
                <div class="progress-container">
                    <span class="time-display" id="currentTime">0:00</span>
                    <div class="progress-bar" id="progressBar" onclick="seekTrack(event)">
                        <div class="progress-fill" id="progressFill"></div>
                    </div>
                    <span class="time-display" id="totalTime">0:00</span>
                </div>
            </div>
            <div class="volume-control">
                <span style="cursor: pointer;" onclick="toggleMute()">🔊</span>
                <div class="volume-bar" onclick="changeVolume(event)">
                    <div class="volume-fill" id="volumeFill"></div>
                </div>
            </div>
        </div>
    </div>

    <!-- Footer -->
    <footer class="footer">
        <p>🎵 <span class="footer-creator">Melodia</span> - Plateforme Musicale Créée par <span class="footer-creator">Moe L'king</span></p>
        <p style="margin-top: 0.5rem; font-size: 0.85rem;">© 2024-2026 Melodia. Tous droits réservés. | Distribuer, Streamer, Gérer votre Musique</p>
    </footer>

    <script>
        // -----------------------------------------------------------------
        // CONFIGURATION SUPABASE : INSÉREZ VOS CLÉS ICI
        // -----------------------------------------------------------------
        const SUPABASE_URL = 'https://bqxpohaaqnzpeotgsaxc.supabase.co'; 
        const SUPABASE_ANON_KEY = 'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6ImJxeHBvaGFhcW56cGVvdGdzYXhjIiwicm9sZSI6ImFub24iLCJpYXQiOjE3Njk4ODEyOTMsImV4cCI6MjA4NTQ1NzI5M30.oCBS8aVGUr6KjSTX2zAMZstKTQcpvWETyGW7pI19qbo';
        
        // Initialisation du client Supabase
        const supabaseClient = supabase.createClient(SUPABASE_URL, SUPABASE_ANON_KEY);
        // -----------------------------------------------------------------

        // Data Storage
        let users = JSON.parse(localStorage.getItem('melodia_users')) || [];
        let tracks = JSON.parse(localStorage.getItem('melodia_tracks')) || [];
        let comments = JSON.parse(localStorage.getItem('melodia_comments')) || [];
        let currentUser = JSON.parse(localStorage.getItem('melodia_currentUser')) || null;
        
        let currentTrackIndex = 0;
        let playlist = [];
        let audioElement = document.getElementById('audioElement');

        // Initialize
        window.onload = function() {
            if (currentUser) {
                showUserMenu();
            }
            updateStats();
            loadExplorePage();
            
            // Audio events
            audioElement.addEventListener('timeupdate', updateProgress);
            audioElement.addEventListener('ended', nextTrack);
            audioElement.addEventListener('loadedmetadata', function() {
                document.getElementById('totalTime').textContent = formatTime(audioElement.duration);
            });
        };

        // Authentication
        function register(e) {
            e.preventDefault();
            const name = document.getElementById('registerName').value;
            const email = document.getElementById('registerEmail').value;
            const password = document.getElementById('registerPassword').value;
            const bio = document.getElementById('registerBio').value;

            if (users.find(u => u.email === email)) {
                showAlert('Cet email est déjà utilisé sur Melodia', 'error');
                return;
            }

            const user = {
                id: Date.now(),
                name,
                email,
                password,
                bio,
                location: '',
                joined: new Date().toISOString(),
                followers: 0
            };

            users.push(user);
            localStorage.setItem('melodia_users', JSON.stringify(users));
            
            currentUser = { ...user };
            delete currentUser.password;
            localStorage.setItem('melodia_currentUser', JSON.stringify(currentUser));
            
            closeModal('register');
            showUserMenu();
            showAlert('✅ Compte créé avec succès ! Bienvenue sur Melodia ' + name, 'success');
            showPage('dashboard');
        }

        function login(e) {
            e.preventDefault();
            const email = document.getElementById('loginEmail').value;
            const password = document.getElementById('loginPassword').value;

            const user = users.find(u => u.email === email && u.password === password);
            
            if (user) {
                currentUser = { ...user };
                delete currentUser.password;
                localStorage.setItem('melodia_currentUser', JSON.stringify(currentUser));
                
                closeModal('login');
                showUserMenu();
                showAlert('✅ Bienvenue sur Melodia ' + user.name + ' !', 'success');
                showPage('dashboard');
            } else {
                showAlert('❌ Email ou mot de passe incorrect', 'error');
            }
        }

        function logout() {
            currentUser = null;
            localStorage.removeItem('melodia_currentUser');
            document.getElementById('userMenu').style.display = 'none';
            document.getElementById('authButtons').style.display = 'flex';
            document.getElementById('dashboardLink').style.display = 'none';
            showAlert('✅ Déconnexion réussie', 'success');
            showPage('home');
        }

        function showUserMenu() {
            document.getElementById('authButtons').style.display = 'none';
            document.getElementById('userMenu').style.display = 'block';
            document.getElementById('dashboardLink').style.display = 'block';
            document.getElementById('userInitials').textContent = currentUser.name.charAt(0).toUpperCase();
        }

        // Upload Music
        function uploadMusic(e) {
            e.preventDefault();
            
            if (!currentUser) {
                showAlert('❌ Vous devez être connecté à Melodia', 'error');
                return;
            }

            const audioFile = document.getElementById('audioFile').files[0];
            const coverFile = document.getElementById('coverFile').files[0];
            
            if (!audioFile || !coverFile) {
                showAlert('❌ Veuillez sélectionner tous les fichiers requis', 'error');
                return;
            }

            const reader1 = new FileReader();
            const reader2 = new FileReader();

            reader1.onload = function(e1) {
                reader2.onload = function(e2) {
                    const track = {
                        id: Date.now(),
                        title: document.getElementById('songTitle').value,
                        artist: currentUser.name,
                        artistId: currentUser.id,
                        genre: document.getElementById('songGenre').value,
                        producer: document.getElementById('songProducer').value,
                        mixing: document.getElementById('songMixing').value,
                        mastering: document.getElementById('songMastering').value,
                        featuring: document.getElementById('songFeaturing').value,
                        year: document.getElementById('songYear').value,
                        description: document.getElementById('songDescription').value,
                        audioUrl: e1.target.result,
                        coverUrl: e2.target.result,
                        uploadDate: new Date().toISOString(),
                        plays: 0,
                        likes: 0,
                        likedBy: []
                    };

                    tracks.push(track);
                    localStorage.setItem('melodia_tracks', JSON.stringify(tracks));
                    
                    closeModal('upload');
                    showAlert('✅ Musique uploadée avec succès sur Melodia !', 'success');
                    updateStats();
                    loadExplorePage();
                    loadMyMusic();
                    
                    // Reset form
                    document.querySelector('#uploadModal form').reset();
                    document.getElementById('coverPreview').style.display = 'none';
                    document.getElementById('audioPreview').innerHTML = '';
                };
                reader2.readAsDataURL(coverFile);
            };
            reader1.readAsDataURL(audioFile);
        }

        function previewCover(input) {
            if (input.files && input.files[0]) {
                const reader = new FileReader();
                reader.onload = function(e) {
                    const preview = document.getElementById('coverPreview');
                    preview.src = e.target.result;
                    preview.style.display = 'block';
                };
                reader.readAsDataURL(input.files[0]);
            }
        }

        function previewAudio(input) {
            if (input.files && input.files[0]) {
                const preview = document.getElementById('audioPreview');
                preview.innerHTML = `<p style="color: var(--success); margin-top: 1rem;">✓ ${input.files[0].name}</p>`;
            }
        }

        function previewEditCover(input) {
            if (input.files && input.files[0]) {
                const reader = new FileReader();
                reader.onload = function(e) {
                    document.getElementById('editCoverPreview').src = e.target.result;
                };
                reader.readAsDataURL(input.files[0]);
            }
        }

        // Music Player
        function playTrack(trackId) {
            const track = tracks.find(t => t.id === trackId);
            if (!track) return;

            // Increment plays
            track.plays++;
            localStorage.setItem('melodia_tracks', JSON.stringify(tracks));
            updateStats();

            // Setup player
            audioElement.src = track.audioUrl;
            document.getElementById('currentCover').src = track.coverUrl;
            document.getElementById('currentTitle').textContent = track.title;
            document.getElementById('currentArtist').textContent = track.artist;
            document.getElementById('audioPlayer').classList.add('active');
            
            audioElement.play();
            document.getElementById('playPauseBtn').textContent = '⏸';

            // Setup playlist
            playlist = tracks.map(t => t.id);
            currentTrackIndex = playlist.indexOf(trackId);
        }

        function togglePlay() {
            if (audioElement.paused) {
                audioElement.play();
                document.getElementById('playPauseBtn').textContent = '⏸';
            } else {
                audioElement.pause();
                document.getElementById('playPauseBtn').textContent = '▶';
            }
        }

        function nextTrack() {
            if (playlist.length === 0) return;
            currentTrackIndex = (currentTrackIndex + 1) % playlist.length;
            playTrack(playlist[currentTrackIndex]);
        }

        function previousTrack() {
            if (playlist.length === 0) return;
            currentTrackIndex = (currentTrackIndex - 1 + playlist.length) % playlist.length;
            playTrack(playlist[currentTrackIndex]);
        }

        function updateProgress() {
            if (audioElement.duration) {
                const progress = (audioElement.currentTime / audioElement.duration) * 100;
                document.getElementById('progressFill').style.width = progress + '%';
                document.getElementById('currentTime').textContent = formatTime(audioElement.currentTime);
            }
        }

        function seekTrack(e) {
            const bar = document.getElementById('progressBar');
            const percent = e.offsetX / bar.offsetWidth;
            audioElement.currentTime = percent * audioElement.duration;
        }

        function changeVolume(e) {
            const bar = e.currentTarget;
            const percent = e.offsetX / bar.offsetWidth;
            audioElement.volume = percent;
            document.getElementById('volumeFill').style.width = (percent * 100) + '%';
        }

        function toggleMute() {
            audioElement.muted = !audioElement.muted;
        }

        function formatTime(seconds) {
            if (isNaN(seconds)) return '0:00';
            const mins = Math.floor(seconds / 60);
            const secs = Math.floor(seconds % 60);
            return `${mins}:${secs < 10 ? '0' : ''}${secs}`;
        }

        // Like System
        function toggleLike(trackId) {
            if (!currentUser) {
                showAlert('❌ Vous devez être connecté pour liker', 'error');
                return;
            }

            const track = tracks.find(t => t.id === trackId);
            if (!track) return;

            const likedIndex = track.likedBy.indexOf(currentUser.id);
            if (likedIndex > -1) {
                track.likedBy.splice(likedIndex, 1);
                track.likes--;
            } else {
                track.likedBy.push(currentUser.id);
                track.likes++;
            }

            localStorage.setItem('melodia_tracks', JSON.stringify(tracks));
            updateStats();
            loadExplorePage();
            loadMyMusic();
        }

        // Edit Music
        function openEditMusic(trackId) {
            const track = tracks.find(t => t.id === trackId);
            if (!track || track.artistId !== currentUser.id) return;

            document.getElementById('editMusicId').value = track.id;
            document.getElementById('editSongTitle').value = track.title;
            document.getElementById('editSongGenre').value = track.genre;
            document.getElementById('editSongProducer').value = track.producer || '';
            document.getElementById('editSongMixing').value = track.mixing || '';
            document.getElementById('editSongMastering').value = track.mastering || '';
            document.getElementById('editSongDescription').value = track.description || '';
            document.getElementById('editCoverPreview').src = track.coverUrl;
            
            showModal('editMusic');
        }

        function updateMusic(e) {
            e.preventDefault();
            const trackId = parseInt(document.getElementById('editMusicId').value);
            const track = tracks.find(t => t.id === trackId);
            
            if (!track) return;

            track.title = document.getElementById('editSongTitle').value;
            track.genre = document.getElementById('editSongGenre').value;
            track.producer = document.getElementById('editSongProducer').value;
            track.mixing = document.getElementById('editSongMixing').value;
            track.mastering = document.getElementById('editSongMastering').value;
            track.description = document.getElementById('editSongDescription').value;

            const newCover = document.getElementById('editCoverFile').files[0];
            if (newCover) {
                const reader = new FileReader();
                reader.onload = function(e) {
                    track.coverUrl = e.target.result;
                    localStorage.setItem('melodia_tracks', JSON.stringify(tracks));
                    closeModal('editMusic');
                    showAlert('✅ Musique mise à jour sur Melodia !', 'success');
                    loadMyMusic();
                    loadExplorePage();
                };
                reader.readAsDataURL(newCover);
            } else {
                localStorage.setItem('melodia_tracks', JSON.stringify(tracks));
                closeModal('editMusic');
                showAlert('✅ Musique mise à jour sur Melodia !', 'success');
                loadMyMusic();
                loadExplorePage();
            }
        }

        function deleteMusic() {
            if (!confirm('Êtes-vous sûr de vouloir supprimer cette musique de Melodia ?')) return;

            const trackId = parseInt(document.getElementById('editMusicId').value);
            tracks = tracks.filter(t => t.id !== trackId);
            localStorage.setItem('melodia_tracks', JSON.stringify(tracks));
            
            closeModal('editMusic');
            showAlert('✅ Musique supprimée de Melodia', 'success');
            updateStats();
            loadMyMusic();
            loadExplorePage();
        }

        // Profile
        function openEditProfile() {
            document.getElementById('editName').value = currentUser.name;
            document.getElementById('editEmail').value = currentUser.email;
            document.getElementById('editBio').value = currentUser.bio || '';
            document.getElementById('editLocation').value = currentUser.location || '';
            showModal('editProfile');
        }

        function updateProfile(e) {
            e.preventDefault();
            
            currentUser.name = document.getElementById('editName').value;
            currentUser.email = document.getElementById('editEmail').value;
            currentUser.bio = document.getElementById('editBio').value;
            currentUser.location = document.getElementById('editLocation').value;

            // Update in users array
            const userIndex = users.findIndex(u => u.id === currentUser.id);
            if (userIndex > -1) {
                users[userIndex] = { ...users[userIndex], ...currentUser };
                localStorage.setItem('melodia_users', JSON.stringify(users));
            }

            localStorage.setItem('melodia_currentUser', JSON.stringify(currentUser));
            
            closeModal('editProfile');
            showAlert('✅ Profil mis à jour sur Melodia !', 'success');
            loadProfilePage();
        }

        // Load Pages
        function loadExplorePage() {
            const grid = document.getElementById('exploreGrid');
            grid.innerHTML = '';

            if (tracks.length === 0) {
                grid.innerHTML = '<p style="text-align: center; color: var(--gray); grid-column: 1 / -1;">Aucune musique disponible sur Melodia pour le moment...</p>';
                return;
            }

            tracks.slice().reverse().forEach(track => {
                const isLiked = currentUser && track.likedBy.includes(currentUser.id);
                grid.innerHTML += `
                    <div class="music-card">
                        <img src="${track.coverUrl}" class="music-cover" onclick="playTrack(${track.id})">
                        <div class="music-info">
                            <div class="music-title">${track.title}</div>
                            <div class="music-artist">${track.artist}</div>
                            <div class="music-metadata">
                                <span class="metadata-tag">${track.genre}</span>
                                ${track.producer ? `<span class="metadata-tag">🎛️ ${track.producer}</span>` : ''}
                            </div>
                            <div style="display: flex; justify-content: space-between; margin-top: 1rem; color: var(--gray); font-size: 0.9rem;">
                                <span>🎵 ${track.plays} plays</span>
                                <span>❤️ ${track.likes} likes</span>
                            </div>
                            <div class="music-actions">
                                <button class="action-btn play-btn-card" onclick="playTrack(${track.id})">
                                    ▶ Écouter
                                </button>
                                <button class="action-btn like-btn ${isLiked ? 'liked' : ''}" onclick="toggleLike(${track.id})">
                                    ${isLiked ? '❤️' : '🤍'}
                                </button>
                            </div>
                        </div>
                    </div>
                `;
            });
        }

        function loadMyMusic() {
            if (!currentUser) return;
            
            const grid = document.getElementById('myMusicGrid');
            const myTracks = tracks.filter(t => t.artistId === currentUser.id);
            
            grid.innerHTML = '';
            if (myTracks.length === 0) {
                grid.innerHTML = '<p style="color: var(--gray); grid-column: 1 / -1;">Vous n\'avez pas encore uploadé de musique sur Melodia...</p>';
                return;
            }

            myTracks.reverse().forEach(track => {
                grid.innerHTML += `
                    <div class="music-card">
                        <img src="${track.coverUrl}" class="music-cover" onclick="playTrack(${track.id})">
                        <div class="music-info">
                            <div class="music-title">${track.title}</div>
                            <div class="music-artist">${track.artist}</div>
                            <div class="music-metadata">
                                <span class="metadata-tag">${track.genre}</span>
                                ${track.year ? `<span class="metadata-tag">${track.year}</span>` : ''}
                            </div>
                            <div style="display: flex; justify-content: space-between; margin-top: 1rem; color: var(--gray); font-size: 0.9rem;">
                                <span>🎵 ${track.plays} plays</span>
                                <span>❤️ ${track.likes} likes</span>
                            </div>
                            <div class="music-actions">
                                <button class="action-btn play-btn-card" onclick="playTrack(${track.id})">
                                    ▶ Écouter
                                </button>
                                <button class="action-btn" style="background: rgba(99, 102, 241, 0.1); color: var(--primary);" onclick="openEditMusic(${track.id})">
                                    ✏️ Modifier
                                </button>
                            </div>
                        </div>
                    </div>
                `;
            });

            // Update analytics
            const totalPlays = myTracks.reduce((sum, t) => sum + t.plays, 0);
            const totalLikes = myTracks.reduce((sum, t) => sum + t.likes, 0);
            document.getElementById('userTotalPlays').textContent = totalPlays;
            document.getElementById('userTotalLikes').textContent = totalLikes;
            document.getElementById('userTotalTracks').textContent = myTracks.length;
            document.getElementById('userTotalComments').textContent = '0';
        }

        function loadProfilePage() {
            if (!currentUser) return;

            const myTracks = tracks.filter(t => t.artistId === currentUser.id);
            const totalPlays = myTracks.reduce((sum, t) => sum + t.plays, 0);
            const totalLikes = myTracks.reduce((sum, t) => sum + t.likes, 0);

            document.getElementById('profileAvatar').textContent = currentUser.name.charAt(0).toUpperCase();
            document.getElementById('profileName').textContent = currentUser.name;
            document.getElementById('profileEmail').textContent = currentUser.email;
            document.getElementById('profileBio').textContent = currentUser.bio || 'Aucune bio';
            document.getElementById('profileLocation').textContent = currentUser.location || '';
            document.getElementById('profileTotalPlays').textContent = totalPlays;
            document.getElementById('profileTotalLikes').textContent = totalLikes;
            document.getElementById('profileTotalTracks').textContent = myTracks.length;
            document.getElementById('profileFollowers').textContent = currentUser.followers || 0;

            const grid = document.getElementById('profileMusicGrid');
            grid.innerHTML = '';
            
            if (myTracks.length === 0) {
                grid.innerHTML = '<p style="color: var(--gray);">Aucune musique uploadée sur Melodia.</p>';
                return;
            }

            myTracks.reverse().forEach(track => {
                grid.innerHTML += `
                    <div class="music-card">
                        <img src="${track.coverUrl}" class="music-cover" onclick="playTrack(${track.id})">
                        <div class="music-info">
                            <div class="music-title">${track.title}</div>
                            <div class="music-metadata">
                                <span class="metadata-tag">${track.genre}</span>
                            </div>
                            <div style="display: flex; justify-content: space-between; margin-top: 1rem; color: var(--gray); font-size: 0.9rem;">
                                <span>🎵 ${track.plays}</span>
                                <span>❤️ ${track.likes}</span>
                            </div>
                        </div>
                    </div>
                `;
            });
        }

        // Stats
        function updateStats() {
            const totalPlays = tracks.reduce((sum, t) => sum + t.plays, 0);
            const totalLikes = tracks.reduce((sum, t) => sum + t.likes, 0);
            
            document.getElementById('totalUsers').textContent = users.length;
            document.getElementById('totalTracks').textContent = tracks.length;
            document.getElementById('totalPlays').textContent = totalPlays;
            document.getElementById('totalLikes').textContent = totalLikes;
        }

        // UI Functions
        function showPage(pageName) {
            document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
            document.getElementById(pageName + 'Page').classList.add('active');
            
            if (pageName === 'dashboard') {
                loadMyMusic();
            } else if (pageName === 'explore') {
                loadExplorePage();
            } else if (pageName === 'profile') {
                loadProfilePage();
            }
        }

        function showModal(modalName) {
            document.getElementById(modalName + 'Modal').classList.add('active');
        }

        function closeModal(modalName) {
            document.getElementById(modalName + 'Modal').classList.remove('active');
        }

        function showDashboardSection(section) {
            document.querySelectorAll('.sidebar-item').forEach(i => i.classList.remove('active'));
            if(event) event.target.classList.add('active');
            
            document.getElementById('myMusicSection').style.display = section === 'mymusic' ? 'block' : 'none';
            document.getElementById('analyticsSection').style.display = section === 'analytics' ? 'block' : 'none';
        }

        function toggleDropdown() {
            document.getElementById('userDropdown').classList.toggle('active');
        }

        function showAlert(message, type) {
            const alert = document.getElementById('alert');
            alert.textContent = message;
            alert.className = 'alert active ' + type;
            setTimeout(() => {
                alert.classList.remove('active');
            }, 3000);
        }

        // Close dropdowns when clicking outside
        document.addEventListener('click', function(e) {
            if (!e.target.closest('.user-menu')) {
                document.getElementById('userDropdown').classList.remove('active');
            }
        });
    </script>
</body>
</html>