<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Samarth Shendre - GitHub Profile</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: #fff;
            padding: 20px;
            line-height: 1.6;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 40px;
            box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.37);
            border: 1px solid rgba(255, 255, 255, 0.18);
        }

        .header-banner {
            width: 100%;
            border-radius: 15px;
            margin-bottom: 30px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
            animation: fadeIn 1s ease-in;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(-20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
        }

        @keyframes glow {
            0%, 100% { text-shadow: 0 0 20px rgba(255, 255, 255, 0.5); }
            50% { text-shadow: 0 0 40px rgba(255, 255, 255, 0.8); }
        }

        .title-section {
            text-align: center;
            margin-bottom: 40px;
            animation: fadeIn 1.5s ease-in;
        }

        h1 {
            font-size: 3.5em;
            margin: 20px 0;
            animation: glow 2s ease-in-out infinite;
            background: linear-gradient(45deg, #fff, #f0f0f0);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        h3 {
            font-size: 1.5em;
            opacity: 0.9;
            margin-bottom: 20px;
        }

        .content-wrapper {
            display: grid;
            grid-template-columns: 1fr 400px;
            gap: 40px;
            align-items: start;
        }

        .coding-gif {
            width: 100%;
            border-radius: 15px;
            animation: float 3s ease-in-out infinite;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
            position: sticky;
            top: 20px;
        }

        .profile-views {
            display: inline-block;
            margin: 20px 0;
            padding: 10px 20px;
            background: rgba(255, 255, 255, 0.2);
            border-radius: 10px;
            backdrop-filter: blur(5px);
        }

        .info-section {
            background: rgba(255, 255, 255, 0.1);
            padding: 30px;
            border-radius: 15px;
            margin: 30px 0;
            backdrop-filter: blur(5px);
            border: 1px solid rgba(255, 255, 255, 0.2);
            animation: slideIn 1s ease-out;
        }

        @keyframes slideIn {
            from { opacity: 0; transform: translateX(-50px); }
            to { opacity: 1; transform: translateX(0); }
        }

        .info-item {
            margin: 15px 0;
            font-size: 1.1em;
            padding: 10px;
            border-left: 4px solid rgba(255, 255, 255, 0.6);
            transition: all 0.3s ease;
        }

        .info-item:hover {
            background: rgba(255, 255, 255, 0.1);
            padding-left: 20px;
            border-left-color: #fff;
        }

        .info-item strong {
            margin-right: 10px;
        }

        .info-item a {
            color: #fff;
            text-decoration: none;
            border-bottom: 2px solid transparent;
            transition: border-color 0.3s ease;
        }

        .info-item a:hover {
            border-bottom-color: #fff;
        }

        .social-section {
            text-align: center;
            margin: 40px 0;
        }

        .social-section h3 {
            margin-bottom: 20px;
            font-size: 2em;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
        }

        .social-links a {
            display: inline-block;
            padding: 15px;
            background: rgba(255, 255, 255, 0.2);
            border-radius: 50%;
            transition: all 0.3s ease;
            animation: pulse 2s ease-in-out infinite;
        }

        @keyframes pulse {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.1); }
        }

        .social-links a:hover {
            background: rgba(255, 255, 255, 0.4);
            transform: translateY(-5px) scale(1.2);
            animation: none;
        }

        .social-links img {
            display: block;
        }

        .tech-section {
            margin: 40px 0;
        }

        .tech-section h3 {
            text-align: center;
            font-size: 2em;
            margin-bottom: 30px;
        }

        .tech-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(60px, 1fr));
            gap: 20px;
            padding: 20px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 15px;
        }

        .tech-item {
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 10px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 10px;
            transition: all 0.3s ease;
            cursor: pointer;
        }

        .tech-item:hover {
            background: rgba(255, 255, 255, 0.3);
            transform: scale(1.1) rotate(5deg);
        }

        .stats-section {
            margin: 40px 0;
        }

        .stats-section h3 {
            text-align: center;
            font-size: 2em;
            margin-bottom: 30px;
        }

        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
        }

        .stat-card {
            background: rgba(255, 255, 255, 0.1);
            border-radius: 15px;
            padding: 20px;
            text-align: center;
            transition: all 0.3s ease;
        }

        .stat-card:hover {
            background: rgba(255, 255, 255, 0.2);
            transform: translateY(-10px);
            box-shadow: 0 15px 40px rgba(0, 0, 0, 0.4);
        }

        .stat-card img {
            border-radius: 10px;
            width: 100%;
        }

        @media (max-width: 968px) {
            .content-wrapper {
                grid-template-columns: 1fr;
            }

            .coding-gif {
                position: relative;
                max-width: 400px;
                margin: 0 auto;
            }

            h1 {
                font-size: 2.5em;
            }
        }

        .wave {
            display: inline-block;
            animation: wave 2s ease-in-out infinite;
        }

        @keyframes wave {
            0%, 100% { transform: rotate(0deg); }
            25% { transform: rotate(20deg); }
            75% { transform: rotate(-20deg); }
        }
    </style>
</head>
<body>
    <div class="container">
        <img class="header-banner" src="https://www.mywebworld.in/wp-content/uploads/2018/05/web-design-kerala.gif" alt="Header Banner">
        
        <div class="title-section">
            <h1>Hi <span class="wave">👋</span>, I'm Samarth Shendre</h1>
            <h3>A passionate cyber security enthusiast from India</h3>
            <div class="profile-views">
                <img src="https://komarev.com/ghpvc/?username=i-m-samarth-cs&label=Profile%20views&color=0e75b6&style=flat" alt="Profile views">
            </div>
        </div>

        <div class="content-wrapper">
            <div class="main-content">
                <div class="info-section">
                    <div class="info-item">
                        🔭 I'm currently working on <a href="https://www.coursera.org/account/accomplishments/specialization/3DCZ9BZW9N2L" target="_blank">Cyber Security</a>
                    </div>
                    <div class="info-item">
                        🌱 I'm currently learning <strong>Web 3.0, Ethereum, Cyber Security, Machine Learning</strong>
                    </div>
                    <div class="info-item">
                        👯 I'm looking to collaborate on <strong>Machine Learning Projects</strong>
                    </div>
                    <div class="info-item">
                        🤝 I'm looking for help with <strong>Web Development / MERN</strong>
                    </div>
                    <div class="info-item">
                        👨‍💻 All of my projects are available at <a href="https://www.linkedin.com/in/samarth-shendre-b3b039297" target="_blank">LinkedIn</a>
                    </div>
                    <div class="info-item">
                        📫 How to reach me: <a href="mailto:samarthscoe@gmail.com">samarthscoe@gmail.com</a>
                    </div>
                    <div class="info-item">
                        📄 Know about my experiences: <a href="https://drive.google.com/file/d/1BHooFaerZkXOojpKfl_NRtjup0OfQz3h/view?usp=sharing" target="_blank">View Resume</a>
                    </div>
                    <div class="info-item">
                        ⚡ Fun fact: <strong>Programming is Easy</strong>
                    </div>
                </div>
            </div>
            
            <div class="side-content">
                <img class="coding-gif" src="https://ecard.link/content/card/animated_gif1780.gif" alt="Coding Animation">
            </div>
        </div>

        <div class="social-section">
            <h3>🌐 Connect with me</h3>
            <div class="social-links">
                <a href="https://twitter.com/i_m_samarth004" target="_blank">
                    <img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/twitter.svg" alt="Twitter" height="30" width="40">
                </a>
                <a href="https://linkedin.com/in/https://www.linkedin.com/in/samarth-shendre-b3b039297" target="_blank">
                    <img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="LinkedIn" height="30" width="40">
                </a>
                <a href="https://fb.com/samarth shendre" target="_blank">
                    <img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/facebook.svg" alt="Facebook" height="30" width="40">
                </a>
                <a href="https://instagram.com/iam_samarth004" target="_blank">
                    <img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/instagram.svg" alt="Instagram" height="30" width="40">
                </a>
                <a href="https://auth.geeksforgeeks.org/user/samartj6ps" target="_blank">
                    <img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/geeks-for-geeks.svg" alt="GeeksforGeeks" height="30" width="40">
                </a>
            </div>
        </div>

        <div class="tech-section">
            <h3>🛠️ Languages and Tools</h3>
            <div class="tech-grid">
                <div class="tech-item"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/android/android-original-wordmark.svg" alt="android" width="40" height="40"></div>
                <div class="tech-item"><img src="https://cdn.worldvectorlogo.com/logos/arduino-1.svg" alt="arduino" width="40" height="40"></div>
                <div class="tech-item"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/amazonwebservices/amazonwebservices-original-wordmark.svg" alt="aws" width="40" height="40"></div>
                <div class="tech-item"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/bootstrap/bootstrap-plain-wordmark.svg" alt="bootstrap" width="40" height="40"></div>
                <div class="tech-item"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/c/c-original.svg" alt="c" width="40" height="40"></div>
                <div class="tech-item"><img src="https://raw.githubusercontent.com/Hardik0307/Hardik0307/master/assets/canvasjs-charts.svg" alt="canvasjs" width="40" height="40"></div>
                <div class="tech-item"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/cplusplus/cplusplus-original.svg" alt="cplusplus" width="40" height="40"></div>
                <div class="tech-item"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/csharp/csharp-original.svg" alt="csharp" width="40" height="40"></div>
                <div class="tech-item"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="40" height="40"></div>
                <div class="tech-item"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/d3js/d3js-original.svg" alt="d3js" width="40" height="40"></div>
                <div class="tech-item"><img src="https://cdn.worldvectorlogo.com/logos/django.svg" alt="django" width="40" height="40"></div>
                <div class="tech-item"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/docker/docker-original-wordmark.svg" alt="docker" width="40" height="40"></div>
                <div class="tech-item"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/express/express-original-wordmark.svg" alt="express" width="40" height="40"></div>
                <div class="tech-item"><img src="https://www.vectorlogo.zone/logos/flutterio/flutterio-icon.svg" alt="flutter" width="40" height="40"></div>
                <div class="tech-item"><img src="https://www.vectorlogo.zone/logos/google_cloud/google_cloud-icon.svg" alt="gcp" width="40" height="40"></div>
                <div class="tech-item"><img src="https://www.vectorlogo.zone/logos/git-scm/git-scm-icon.svg" alt="git" width="40" height="40"></div>
                <div class="tech-item"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40"></div>
                <div class="tech-item"><img src="https://www.vectorlogo.zone/logos/adobe_illustrator/adobe_illustrator-icon.svg" alt="illustrator" width="40" height="40"></div>
                <div class="tech-item"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg" alt="java" width="40" height="40"></div>
                <div class="tech-item"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"></div>
                <div class="tech-item"><img src="https://www.vectorlogo.zone/logos/kubernetes/kubernetes-icon.svg" alt="kubernetes" width="40" height="40"></div>
                <div class="tech-item"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/linux/linux-original.svg" alt="linux" width="40" height="40"></div>
                <div class="tech-item"><img src="https://www.vectorlogo.zone/logos/mariadb/mariadb-icon.svg" alt="mariadb" width="40" height="40"></div>
                <div class="tech-item"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mongodb/mongodb-original-wordmark.svg" alt="mongodb" width="40" height="40"></div>
                <div class="tech-item"><img src="https://www.svgrepo.com/show/303229/microsoft-sql-server-logo.svg" alt="mssql" width="40" height="40"></div>
                <div class="tech-item"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg" alt="mysql" width="40" height="40"></div>
                <div class="tech-item"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nodejs/nodejs-original-wordmark.svg" alt="nodejs" width="40" height="40"></div>
                <div class="tech-item"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/oracle/oracle-original.svg" alt="oracle" width="40" height="40"></div>
                <div class="tech-item"><img src="https://raw.githubusercontent.com/devicons/devicon/2ae2a900d2f041da66e950e4d48052658d850630/icons/pandas/pandas-original.svg" alt="pandas" width="40" height="40"></div>
                <div class="tech-item"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/photoshop/photoshop-line.svg" alt="photoshop" width="40" height="40"></div>
                <div class="tech-item"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/php/php-original.svg" alt="php" width="40" height="40"></div>
                <div class="tech-item"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/postgresql/postgresql-original-wordmark.svg" alt="postgresql" width="40" height="40"></div>
                <div class="tech-item"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"></div>
                <div class="tech-item"><img src="https://www.vectorlogo.zone/logos/pytorch/pytorch-icon.svg" alt="pytorch" width="40" height="40"></div>
                <div class="tech-item"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original-wordmark.svg" alt="react" width="40" height="40"></div>
                <div class="tech-item"><img src="https://raw.githubusercontent.com/detain/svg-logos/780f25886640cef088af994181646db2f6b1a3f8/svg/selenium-logo.svg" alt="selenium" width="40" height="40"></div>
                <div class="tech-item"><img src="https://www.vectorlogo.zone/logos/springio/springio-icon.svg" alt="spring" width="40" height="40"></div>
                <div class="tech-item"><img src="https://www.vectorlogo.zone/logos/tensorflow/tensorflow-icon.svg" alt="tensorflow" width="40" height="40"></div>
                <div class="tech-item"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/vuejs/vuejs-original-wordmark.svg" alt="vuejs" width="40" height="40"></div>
            </div>
        </div>

        <div class="stats-section">
            <h3>📊 GitHub Statistics</h3>
            <div class="stats-grid">
                <div class="stat-card">
                    <img src="https://github-readme-stats.vercel.app/api/top-langs?username=i-m-samarth-cs&show_icons=true&locale=en&layout=compact&theme=radical" alt="Top Languages">
                </div>
                <div class="stat-card">
                    <img src="https://github-readme-stats.vercel.app/api?username=i-m-samarth-cs&show_icons=true&locale=en&theme=radical" alt="GitHub Stats">
                </div>
                <div class="stat-card">
                    <img src="https://github-readme-streak-stats.herokuapp.com/?user=i-m-samarth-cs&theme=radical" alt="GitHub Streak">
                </div>
            </div>
        </div>
    </div>
</body>
</html>
