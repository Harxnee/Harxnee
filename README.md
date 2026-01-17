<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GitHub Profile Preview</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif;
            background: #0d1117;
            color: #c9d1d9;
            padding: 40px 20px;
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            background: #161b22;
            padding: 40px;
            border-radius: 12px;
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.4);
        }
        
        .header {
            text-align: center;
            margin-bottom: 40px;
            padding-bottom: 30px;
            border-bottom: 2px solid #30363d;
        }
        
        h1 {
            font-size: 2.5em;
            margin-bottom: 10px;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        
        h2 {
            font-size: 1.8em;
            margin: 30px 0 20px;
            color: #58a6ff;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        h3 {
            font-size: 1.3em;
            color: #8b949e;
            font-weight: 400;
            margin-bottom: 20px;
        }
        
        .badges {
            display: flex;
            gap: 15px;
            justify-content: center;
            flex-wrap: wrap;
            margin: 20px 0;
        }
        
        .badge {
            display: inline-block;
            padding: 8px 16px;
            border-radius: 6px;
            text-decoration: none;
            font-weight: 600;
            font-size: 0.9em;
            transition: transform 0.2s, box-shadow 0.2s;
        }
        
        .badge:hover {
            transform: translateY(-2px);
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.3);
        }
        
        .linkedin {
            background: #0077B5;
            color: white;
        }
        
        .email {
            background: #D14836;
            color: white;
        }
        
        .views {
            background: #8b5cf6;
            color: white;
        }
        
        .about {
            background: #0d1117;
            padding: 25px;
            border-radius: 8px;
            margin: 20px 0;
            border-left: 4px solid #58a6ff;
        }
        
        .about ul {
            list-style: none;
            padding-left: 0;
        }
        
        .about li {
            margin: 12px 0;
            padding-left: 25px;
            position: relative;
        }
        
        .about li:before {
            content: "▹";
            position: absolute;
            left: 0;
            color: #58a6ff;
            font-weight: bold;
        }
        
        .tech-section {
            margin: 30px 0;
        }
        
        .tech-category {
            margin-bottom: 25px;
        }
        
        .tech-category h4 {
            color: #8b949e;
            font-size: 1.1em;
            margin-bottom: 12px;
            text-transform: uppercase;
            letter-spacing: 1px;
        }
        
        .tech-badges {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }
        
        .tech-badge {
            padding: 6px 14px;
            border-radius: 6px;
            font-size: 0.85em;
            font-weight: 600;
            color: white;
            display: inline-flex;
            align-items: center;
            gap: 6px;
        }
        
        .python { background: #3776AB; }
        .java { background: #ED8B00; }
        .cpp { background: #00599C; }
        .c { background: #00599C; }
        .sql { background: #4479A1; }
        .tensorflow { background: #FF6F00; }
        .sklearn { background: #F7931E; }
        .pandas { background: #150458; }
        .opencv { background: #5C3EE8; }
        .numpy { background: #013243; }
        .git { background: #F05032; }
        .linux { background: #FCC624; color: black; }
        .mysql { background: #4479A1; }
        .matlab { background: #0076A8; }
        .arduino { background: #00979D; }
        
        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            margin: 30px 0;
        }
        
        .stat-card {
            background: #0d1117;
            padding: 20px;
            border-radius: 8px;
            border: 1px solid #30363d;
            text-align: center;
        }
        
        .stat-card img {
            max-width: 100%;
            height: auto;
            border-radius: 6px;
        }
        
        .divider {
            height: 2px;
            background: linear-gradient(90deg, transparent, #30363d, transparent);
            margin: 40px 0;
        }
        
        .connect {
            text-align: center;
            margin: 40px 0;
            padding: 30px;
            background: #0d1117;
            border-radius: 8px;
        }
        
        .connect p {
            margin-bottom: 20px;
            font-size: 1.1em;
        }
        
        @media (max-width: 768px) {
            .container {
                padding: 20px;
            }
            
            h1 {
                font-size: 2em;
            }
            
            .stats-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>Hi there, I'm Harinee! 👋</h1>
            <h3>Computer Science Student | Deep Learning Enthusiast | Full Stack Developer</h3>
            
            <div class="badges">
                <a href="https://www.linkedin.com/in/harinee-j-298529234/" class="badge linkedin">LinkedIn</a>
                <a href="mailto:harinee.j2021@vitstudent.ac.in" class="badge email">Email</a>
                <span class="badge views">Profile Views: 1,234</span>
            </div>
        </div>
        
        <h2>🚀 About Me</h2>
        <div class="about">
            <p style="margin-bottom: 15px;">I'm an undergraduate student at <strong>VIT Chennai</strong>, passionate about leveraging technology to solve real-world problems. My interests span across <strong>Deep Learning</strong>, <strong>Web Development</strong>, and <strong>Data Engineering</strong>.</p>
            
            <ul>
                <li>🔭 Currently mastering Data Structures & Algorithms and Full Stack Development</li>
                <li>🌱 Exploring cutting-edge Deep Learning architectures and frameworks</li>
                <li>👯 Open to collaborate on Data Analysis, Data Engineering, and Web Development projects</li>
                <li>🎯 2024 Goals: Build production-ready ML models and scalable web applications</li>
                <li>💡 Always learning new techniques and best practices to improve my craft</li>
            </ul>
        </div>
        
        <div class="divider"></div>
        
        <h2>🛠️ Tech Stack</h2>
        <div class="tech-section">
            <div class="tech-category">
                <h4>Languages</h4>
                <div class="tech-badges">
                    <span class="tech-badge python">Python</span>
                    <span class="tech-badge java">Java</span>
                    <span class="tech-badge cpp">C++</span>
                    <span class="tech-badge c">C</span>
                    <span class="tech-badge sql">SQL</span>
                </div>
            </div>
            
            <div class="tech-category">
                <h4>Machine Learning & Data Science</h4>
                <div class="tech-badges">
                    <span class="tech-badge tensorflow">TensorFlow</span>
                    <span class="tech-badge sklearn">Scikit-learn</span>
                    <span class="tech-badge pandas">Pandas</span>
                    <span class="tech-badge opencv">OpenCV</span>
                    <span class="tech-badge numpy">NumPy</span>
                </div>
            </div>
            
            <div class="tech-category">
                <h4>Tools & Technologies</h4>
                <div class="tech-badges">
                    <span class="tech-badge git">Git</span>
                    <span class="tech-badge linux">Linux</span>
                    <span class="tech-badge mysql">MySQL</span>
                    <span class="tech-badge matlab">MATLAB</span>
                    <span class="tech-badge arduino">Arduino</span>
                </div>
            </div>
        </div>
        
        <div class="divider"></div>
        
        <h2>📊 GitHub Stats</h2>
        <div class="stats-grid">
            <div class="stat-card">
                <img src="https://github-readme-stats.vercel.app/api?username=Harxnee&show_icons=true&theme=radical&include_all_commits=true&count_private=true" alt="GitHub Stats">
            </div>
            <div class="stat-card">
                <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Harxnee&layout=compact&theme=radical&langs_count=8" alt="Top Languages">
            </div>
        </div>
        <div class="stat-card" style="margin-top: 20px;">
            <img src="https://github-readme-streak-stats.herokuapp.com/?user=Harxnee&theme=radical" alt="GitHub Streak">
        </div>
        
        <div class="divider"></div>
        
        <div class="connect">
            <h2 style="margin-top: 0;">🤝 Let's Connect!</h2>
            <p>I'm always interested in collaborating on innovative projects and connecting with fellow developers and researchers. Feel free to reach out!</p>
            
            <div class="badges">
                <a href="https://www.linkedin.com/in/harinee-j-298529234/" class="badge linkedin">Let's Connect on LinkedIn</a>
                <a href="mailto:harinee.j2021@vitstudent.ac.in" class="badge email">Drop a Message</a>
            </div>
        </div>
    </div>
</body>
</html>
