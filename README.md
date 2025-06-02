## Hello world. My name is markRyan a computer science student. changing your perspective one line at a time. 👋

<!--
**macrya/macrya** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ryans Portfolio</title>
    <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;500;700&family=Exo+2:wght@300;400;600&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --primary: #00d2ff;
            --secondary: #3a7bd5;
            --accent: #ff00cc;
            --dark: #0a0f1e;
            --darker: #060914;
            --light: #a0f0ff;
            --card-bg: rgba(15, 20, 40, 0.7);
        }

        body {
            background: linear-gradient(135deg, var(--darker), var(--dark));
            color: #fff;
            font-family: 'Exo 2', sans-serif;
            line-height: 1.6;
            min-height: 100vh;
            overflow-x: hidden;
            position: relative;
        }

        body::before {
            content: "";
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: 
                radial-gradient(circle at 20% 30%, rgba(0, 210, 255, 0.1) 0%, transparent 40%),
                radial-gradient(circle at 80% 70%, rgba(255, 0, 204, 0.1) 0%, transparent 40%),
                radial-gradient(circle at 50% 20%, rgba(58, 123, 213, 0.1) 0%, transparent 40%);
            z-index: -1;
            pointer-events: none;
        }

        .grid-pattern {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: 
                linear-gradient(rgba(0, 210, 255, 0.05) 1px, transparent 1px),
                linear-gradient(90deg, rgba(0, 210, 255, 0.05) 1px, transparent 1px);
            background-size: 40px 40px;
            z-index: -1;
            pointer-events: none;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 2rem;
        }

        header {
            text-align: center;
            padding: 4rem 0 2rem;
            position: relative;
        }

        .glow-title {
            font-family: 'Orbitron', sans-serif;
            font-size: 3.5rem;
            margin-bottom: 0;
            background: linear-gradient(90deg, var(--primary), var(--secondary), var(--accent));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            text-shadow: 0 0 15px rgba(0, 210, 255, 0.5);
            letter-spacing: 2px;
            animation: glow-pulse 3s infinite alternate;
        }

        .divider {
            height: 4px;
            width: 300px;
            background: linear-gradient(90deg, var(--primary), var(--secondary), var(--accent));
            border-radius: 2px;
            margin: 10px auto 30px;
            animation: divider-glow 3s infinite alternate;
        }

        .profile-card {
            max-width: 800px;
            margin: 0 auto;
            padding: 2.5rem;
            border-radius: 20px;
            background: var(--card-bg);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(0, 210, 255, 0.3);
            box-shadow: 0 0 30px rgba(0, 210, 255, 0.2);
            position: relative;
            overflow: hidden;
            z-index: 1;
        }

        .profile-card::before {
            content: "";
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: radial-gradient(circle, rgba(0, 210, 255, 0.1) 0%, transparent 70%);
            z-index: -1;
            animation: rotate 20s linear infinite;
        }

        .avatar {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            border: 3px solid var(--primary);
            box-shadow: 0 0 30px rgba(0, 210, 255, 0.5);
            margin: 0 auto 20px;
            overflow: hidden;
            position: relative;
        }

        .avatar img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .avatar::after {
            content: "";
            position: absolute;
            top: -3px;
            left: -3px;
            right: -3px;
            bottom: -3px;
            border-radius: 50%;
            border: 2px solid transparent;
            border-top-color: var(--accent);
            animation: spin 5s linear infinite;
        }

        .name {
            font-family: 'Exo 2', sans-serif;
            font-size: 2.2rem;
            color: #fff;
            margin: 10px 0;
            text-shadow: 0 0 10px rgba(0, 210, 255, 0.7);
        }

        .tagline {
            color: var(--light);
            max-width: 600px;
            margin: 0 auto 30px;
            font-size: 1.2rem;
        }

        .social-icons {
            display: flex;
            justify-content: center;
            gap: 25px;
            margin: 30px 0;
        }

        .icon {
            width: 50px;
            height: 50px;
            display: flex;
            align-items: center;
            justify-content: center;
            border-radius: 50%;
            font-size: 1.5rem;
            color: white;
            position: relative;
            transition: all 0.3s ease;
            animation: float 6s ease-in-out infinite;
        }

        .icon:nth-child(1) {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            box-shadow: 0 0 15px rgba(0, 210, 255, 0.7);
            animation-delay: 0s;
        }

        .icon:nth-child(2) {
            background: linear-gradient(135deg, var(--secondary), #1e40af);
            box-shadow: 0 0 15px rgba(58, 123, 213, 0.7);
            animation-delay: 0.5s;
        }

        .icon:nth-child(3) {
            background: linear-gradient(135deg, var(--accent), #9d174d);
            box-shadow: 0 0 15px rgba(255, 0, 204, 0.7);
            animation-delay: 1s;
        }

        .icon:nth-child(4) {
            background: linear-gradient(135deg, #6366f1, #3b82f6);
            box-shadow: 0 0 15px rgba(99, 102, 241, 0.7);
            animation-delay: 1.5s;
        }

        .icon:hover {
            transform: translateY(-10px) scale(1.1);
            box-shadow: 0 0 25px currentColor;
        }

        .section-title {
            font-family: 'Orbitron', sans-serif;
            color: #fff;
            margin: 60px 0 30px;
            text-shadow: 0 0 10px rgba(0, 210, 255, 0.7);
            text-align: center;
            font-size: 2.2rem;
            letter-spacing: 2px;
            position: relative;
        }

        .section-title::after {
            content: "";
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 3px;
            background: linear-gradient(90deg, var(--primary), var(--accent));
            border-radius: 2px;
        }

        .tech-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
            gap: 25px;
            max-width: 900px;
            margin: 0 auto;
        }

        .tech-card {
            background: var(--card-bg);
            border-radius: 15px;
            padding: 1.5rem 1rem;
            border: 1px solid rgba(0, 210, 255, 0.3);
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
            text-align: center;
            z-index: 1;
        }

        .tech-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 25px rgba(0, 210, 255, 0.3);
            border-color: var(--primary);
        }

        .tech-icon {
            font-size: 2.5rem;
            margin-bottom: 15px;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            filter: drop-shadow(0 0 8px rgba(0, 210, 255, 0.7));
        }

        .tech-name {
            color: #fff;
            font-weight: 600;
            font-size: 1.1rem;
        }

        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            max-width: 1200px;
            margin: 0 auto;
        }

        .project-card {
            background: var(--card-bg);
            border-radius: 15px;
            padding: 1.8rem;
            border: 1px solid rgba(0, 210, 255, 0.3);
            position: relative;
            overflow: hidden;
            transition: all 0.3s ease;
        }

        .project-card:hover {
            transform: translateY(-8px);
            box-shadow: 0 10px 30px rgba(0, 210, 255, 0.2);
        }

        .project-card::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: linear-gradient(90deg, var(--primary), var(--secondary), var(--accent));
            animation: scanline 3s infinite linear;
        }

        .project-title {
            color: #fff;
            font-family: 'Exo 2', sans-serif;
            margin-top: 15px;
            font-size: 1.4rem;
            margin-bottom: 15px;
        }

        .project-description {
            color: var(--light);
            margin-bottom: 20px;
            min-height: 80px;
        }

        .tech-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }

        .tag {
            background: rgba(0, 210, 255, 0.2);
            color: var(--primary);
            padding: 5px 15px;
            border-radius: 20px;
            font-size: 0.85rem;
            font-weight: 500;
        }

        .contact-box {
            max-width: 600px;
            margin: 0 auto;
            background: var(--card-bg);
            padding: 2.5rem;
            border-radius: 20px;
            border: 1px solid rgba(0, 210, 255, 0.3);
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        .contact-text {
            color: var(--light);
            margin-bottom: 25px;
            font-size: 1.1rem;
        }

        .contact-btn {
            background: linear-gradient(90deg, var(--primary), var(--secondary));
            color: #fff;
            padding: 12px 35px;
            border: none;
            border-radius: 30px;
            font-family: 'Exo 2', sans-serif;
            font-weight: 600;
            font-size: 1.1rem;
            cursor: pointer;
            transition: all 0.3s ease;
            box-shadow: 0 0 20px rgba(0, 210, 255, 0.5);
            position: relative;
            overflow: hidden;
        }

        .contact-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 0 30px rgba(0, 210, 255, 0.7);
        }

        .contact-btn::after {
            content: "";
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: rgba(255, 255, 255, 0.1);
            transform: rotate(30deg);
            transition: all 0.5s ease;
        }

        .contact-btn:hover::after {
            transform: rotate(30deg) translate(100px, 100px);
        }

        footer {
            text-align: center;
            margin: 70px 0 30px;
            padding: 20px;
            position: relative;
        }

        .footer-divider {
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 2px;
            background: linear-gradient(90deg, transparent, var(--primary), var(--secondary), var(--accent), transparent);
        }

        .footer-text {
            color: var(--light);
            font-size: 1rem;
            margin-bottom: 15px;
        }

        .pulse-dots {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-top: 10px;
        }

        .dot {
            width: 10px;
            height: 10px;
            border-radius: 50%;
            animation: pulse 1.5s infinite;
        }

        .dot:nth-child(1) {
            background: var(--primary);
            animation-delay: 0s;
        }

        .dot:nth-child(2) {
            background: var(--secondary);
            animation-delay: 0.5s;
        }

        .dot:nth-child(3) {
            background: var(--accent);
            animation-delay: 1s;
        }

        /* Animations */
        @keyframes glow-pulse {
            0% { text-shadow: 0 0 15px rgba(0, 210, 255, 0.5); }
            100% { text-shadow: 0 0 25px rgba(255, 0, 204, 0.7); }
        }

        @keyframes divider-glow {
            0% { box-shadow: 0 0 10px rgba(0, 210, 255, 0.7); }
            100% { box-shadow: 0 0 20px rgba(255, 0, 204, 0.7); }
        }

        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-15px); }
            100% { transform: translateY(0px); }
        }

        @keyframes pulse {
            0% { opacity: 0.3; transform: scale(0.8); }
            50% { opacity: 1; transform: scale(1.2); box-shadow: 0 0 15px currentColor; }
            100% { opacity: 0.3; transform: scale(0.8); }
        }

        @keyframes scanline {
            0% { transform: translateX(-100%); }
            100% { transform: translateX(100%); }
        }

        @keyframes rotate {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }

        /* Responsive design */
        @media (max-width: 768px) {
            .glow-title {
                font-size: 2.5rem;
            }
            
            .profile-card {
                padding: 1.5rem;
            }
            
            .section-title {
                font-size: 1.8rem;
            }
            
            .tech-grid {
                grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
            }
        }

        @media (max-width: 480px) {
            .glow-title {
                font-size: 2rem;
            }
            
            .divider {
                width: 200px;
            }
            
            .avatar {
                width: 120px;
                height: 120px;
            }
            
            .name {
                font-size: 1.8rem;
            }
            
            .tagline {
                font-size: 1rem;
            }
            
            .social-icons {
                gap: 15px;
            }
            
            .icon {
                width: 45px;
                height: 45px;
                font-size: 1.3rem;
            }
        }
    </style>
</head>
<body>
    <div class="grid-pattern"></div>
    
    <div class="container">
        <header>
            <h1 class="glow-title">TECH INNOVATOR</h1>
            <div class="divider"></div>
        </header>
        
        <div class="profile-card">
            <div class="avatar">
                <img src="https://images.unsplash.com/photo-1534030347209-467a5b0ad3e6?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1887&q=80" alt="Profile">
            </div>
            
            <h2 class="name">ALEX JOHNSON</h2>
            <p class="tagline">Full Stack Developer | Learning AI Specialist | Tech Innovator<br>
            Transforming ideas into digital realities with cutting-edge technology</p>
            
            <div class="social-icons">
                <a href="#" class="icon">
                    <i class="fab fa-github">Albus miles</i>
                </a>
               
                <a href="#" class="icon">
                    <i class="fab fa-discord">mr_ryan05</i>
                </a>
            </div>
        </div>
        
        <h2 class="section-title">TECH STACK</h2>
        
        <div class="tech-grid">
            <div class="tech-card">
                <div class="tech-icon">
                    <i class="fab fa-C++"></i>
                </div>
                <div class="tech-name">c++</div>
            </div>
            
            <div class="tech-card">
                <div class="tech-icon">
                    <i class="fab fa-Html"></i>
                </div>
                <div class="tech-name">Html</div>
            </div>
            
            <div class="tech-card">
                <div class="tech-icon">
                    <i class="fab fa-python"></i>
                </div>
                <div class="tech-name">Python</div>
            </div>
            
            <div class="tech-card">
                <div class="tech-icon">
                    <i class="fas fa-robot"></i>
                </div>
                <div class="tech-name">AI/ML</div>
            </div>
            
           
            
            <div class="tech-card">
                <div class="tech-icon">
                    <i class="fab fa-git-alt"></i>
                </div>
                <div class="Albus miles">Git</div>
            </div>
        </div>
        
        <h2 class="section-title">Ongoing projects and research areas</h2>
        
        <div class="projects-grid">
            <div class="project-card">
                <h3 class="project-title">Neural Network Framework</h3>
                <p class="project-description">Custom deep learning framework with GPU acceleration and visualization tools for neural network development.</p>
                <div class="tech-tags">
                    <span class="tag">Python</span>
                    <span class="tag">TensorFlow</span>
                    <span class="tag">CUDA</span>
                </div>
            </div>
            
            <div class="project-card">
                <h3 class="project-title">Quantum Computing Simulator</h3>
                <p class="project-description">Web-based quantum circuit simulator with educational resources and interactive visualization.</p>
                <div class="tech-tags">
                    <span class="tag">JavaScript</span>
                    <span class="tag">React</span>
                    <span class="tag">WebGL</span>
                </div>
            </div>
            
            <div class="project-card">
                <h3 class="project-title">AR Navigation System</h3>
                <p class="project-description">Augmented reality navigation for indoor spaces using smartphone sensors and computer vision.</p>
                <div class="tech-tags">
                    <span class="tag">Swift</span>
                    <span class="tag">ARKit</span>
                    <span class="tag">CoreML</span>
                </div>
            </div>
        </div>
        
        <h2 class="section-title">CONNECT WITH ME</h2>
        
        <div class="contact-box">
            <p class="contact-text">I'm always open to discussing new projects, creative ideas, or opportunities to be part of your vision. Let's build the future together!</p>
            <button class="contact-btn">
                <i class="fas fa-paper-plane"></i> Send Message
            </button>
        </div>
    </div>
    
    <footer>
        <div class="footer-divider"></div>
        <p class="footer-text">Designed with ❤️ using HTML & CSS | © 2023 Tech Innovator</p>
        <div class="pulse-dots">
            <div class="dot"></div>
            <div class="dot"></div>
            <div class="dot"></div>
        </div>
    </footer>
</body>
</html>
