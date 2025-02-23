<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ibrahim Khalilullah - Digital Marketing Expert</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(135deg, #ffffff 0%, #f8e1d9 100%);
            color: #2d2d2d;
            min-height: 100vh;
            overflow-x: hidden;
            line-height: 1.7;
        }

        .container {
            max-width: 1100px;
            margin: 50px auto;
            background: #fff;
            border-radius: 25px;
            box-shadow: 0 15px 50px rgba(0, 0, 0, 0.1);
            padding: 50px;
            position: relative;
        }

        .header {
            text-align: center;
            padding: 20px 0 40px;
            border-bottom: 4px solid #ff7043;
            position: relative;
        }

        .profile-img {
            width: 200px;
            height: 200px;
            border-radius: 50%;
            object-fit: cover;
            margin-bottom: 20px;
            border: 6px solid #ff7043;
            transition: transform 0.5s ease, box-shadow 0.5s ease;
        }

        .profile-img:hover {
            transform: scale(1.1) rotate(5deg);
            box-shadow: 0 0 30px rgba(255, 112, 67, 0.5);
        }

        h1 {
            color: #ff7043;
            font-size: 3em;
            font-weight: 700;
            letter-spacing: 1px;
            margin-bottom: 10px;
            animation: fadeInDown 1s ease-out;
        }

        .subtitle {
            color: #5c4033;
            font-size: 1.4em;
            font-weight: 500;
        }

        .section {
            margin: 40px 0;
            padding: 30px;
            background: #fef9f6;
            border-radius: 15px;
            position: relative;
            overflow: hidden;
            transition: all 0.4s ease;
        }

        .section:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.08);
        }

        h2 {
            color: #5c4033;
            font-size: 2em;
            margin-bottom: 20px;
            font-weight: 600;
            position: relative;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        h2::before {
            content: '';
            width: 10px;
            height: 10px;
            background: #ff7043;
            border-radius: 50%;
            transition: transform 0.3s ease;
        }

        h2:hover::before {
            transform: scale(1.5);
        }

        .section p, .section li {
            color: #2d2d2d;
            font-size: 1.2em;
        }

        ul {
            list-style: none;
            padding-left: 0;
        }

        ul li {
            margin: 15px 0;
            position: relative;
            padding-left: 30px;
            transition: color 0.3s ease;
        }

        ul li::before {
            content: "✔";
            color: #ff7043;
            position: absolute;
            left: 0;
            font-size: 1.2em;
            animation: bounce 1.5s infinite;
        }

        ul li:hover {
            color: #ff7043;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
            margin-top: 25px;
        }

        .social-links a {
            color: #fff;
            background: #5c4033;
            text-decoration: none;
            font-size: 1.2em;
            padding: 12px 30px;
            border-radius: 50px;
            transition: all 0.4s ease;
            font-weight: 500;
            box-shadow: 0 5px 15px rgba(92, 64, 51, 0.2);
        }

        .social-links a:hover {
            background: #ff7043;
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(255, 112, 67, 0.3);
        }

        .cta-button {
            display: inline-block;
            margin-top: 20px;
            padding: 15px 40px;
            background: #ff7043;
            color: #fff;
            text-decoration: none;
            border-radius: 50px;
            font-size: 1.3em;
            font-weight: 600;
            transition: all 0.4s ease;
        }

        .cta-button:hover {
            background: #5c4033;
            transform: scale(1.05);
            box-shadow: 0 10px 20px rgba(92, 64, 51, 0.3);
        }

        .footer {
            text-align: center;
            padding-top: 40px;
            color: #5c4033;
            font-size: 1em;
            font-style: italic;
        }

        /* Animations */
        @keyframes fadeInDown {
            from { opacity: 0; transform: translateY(-20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-5px); }
        }

        @keyframes slideUp {
            from { opacity: 0; transform: translateY(30px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .container {
            animation: fadeInDown 1s ease-out;
        }

        .section {
            opacity: 0;
            animation: slideUp 0.8s ease-out forwards;
        }

        .section:nth-child(2) { animation-delay: 0.2s; }
        .section:nth-child(3) { animation-delay: 0.4s; }
        .section:nth-child(4) { animation-delay: 0.6s; }
        .section:nth-child(5) { animation-delay: 0.8s; }
        .section:nth-child(6) { animation-delay: 1s; }
        .section:nth-child(7) { animation-delay: 1.2s; }
        .section:nth-child(8) { animation-delay: 1.4s; }
        .section:nth-child(9) { animation-delay: 1.6s; }

        /* Responsive Design */
        @media (max-width: 768px) {
            .container {
                margin: 20px;
                padding: 30px;
            }
            h1 { font-size: 2.2em; }
            .subtitle { font-size: 1.2em; }
            h2 { font-size: 1.6em; }
            .profile-img { width: 150px; height: 150px; }
            .section { padding: 20px; }
            .social-links a { font-size: 1em; padding: 10px 20px; }
            .cta-button { font-size: 1.1em; padding: 12px 30px; }
        }
    </style>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700&display=swap" rel="stylesheet">
</head>
<body>
    <div class="container">
        <div class="header">
            <img src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEj97gPJNUoMnspPsULNIkB4XvsDWUN6KG2j4oMaR02_PhGC98nu6OL8nVTaD_dXMvgmGMpMcsc2yIl12lld1NbjhQWv8dJ55MW1rv_yCoPMtx-BbO8POTMgFmxYOEhTRWl1mJVrhyphenhyphen0nRvsayeudeC8R73DypH6tqvmRs3WnnIm7XeslI3uYJhlfaNc25hyphenhyphenm/s1600/BG.webp" 
                 alt="Ibrahim Khalilullah" class="profile-img">
            <h1>Ibrahim Khalilullah</h1>
            <p class="subtitle">Digital Marketing Expert | Motion Designer</p>
        </div>

        <div class="section">
            <h2>About Me</h2>
            <p>I’m Ibrahim, a passionate digital marketer and motion designer based in Noapara, Ghoraghat, Dinajpur, Bangladesh. I specialize in turning ideas into results.</p>
            <p>Email: <a href="mailto:ibrahim3.uk@gmail.com">ibrahim3.uk@gmail.com</a></p>
            <p>Phone: +88 01760792853</p>
        </div>

        <div class="section">
            <h2>My Experience</h2>
            <ul>
                <li><strong>Trainer (Marketing), 2017 - 2018</strong>: Trained students in Digital Marketing under LEDP across Dinajpur, Panchagarh, and Thakurgaon.</li>
                <li><strong>Assistant Director, 2018 - 2025</strong>: Leading freelancing training at Plan Explorer, Dinajpur.</li>
                <li><strong>Assistant Instructor, 2023 - 2024</strong>: Managed ad campaigns and email marketing at Bogura All IT BD.</li>
                <li><strong>Assistant Instructor, 2024 - 2025</strong>: Teaching digital marketing online at Dhaka Web Institute.</li>
            </ul>
        </div>

        <div class="section">
            <h2>My Skills</h2>
            <p><strong>Software:</strong> MS Office, Excel, Motion, After Effects, Photoshop, Illustrator</p>
            <p><strong>Expertise:</strong> Analytical Thinking, Creativity, Motivation, Positivity, Resilience</p>
            <p><strong>Languages:</strong> English, Bangla, Hindi</p>
        </div>

        <div class="section">
            <h2>My Achievements</h2>
            <p>Over 5 years of delivering measurable success:</p>
            <ul>
                <li>Team Members: 15+</li>
                <li>Awards Won: 11+</li>
                <li>Projects Completed: 662+</li>
                <li>Client Reviews: 483+</li>
            </ul>
        </div>

        <div class="section">
            <h2>Services I Offer</h2>
            <p>Grow your business with my expertise:</p>
            <ul>
                <li>Lead Generation - Attract potential customers effortlessly.</li>
                <li>SEO - Boost your website’s visibility on search engines.</li>
                <li>Social Media Marketing - Engage and grow your audience.</li>
                <li>Video Marketing - Tell your story with stunning visuals.</li>
                <li>Email Marketing - Connect directly with your clients.</li>
                <li>Ads Campaign - Targeted ads for maximum ROI.</li>
            </ul>
            <a href="mailto:ibrahim3.uk@gmail.com" class="cta-button">Hire Me Now</a>
        </div>

        <div class="section">
            <h2>Global Reach</h2>
            <p>Trusted by clients in 15+ countries, including Europe, USA, Canada, Australia, and Singapore.</p>
        </div>

        <div class="section">
            <h2>My Platforms</h2>
            <ul>
                <li>Fiverr - Top-rated services.</li>
                <li>Upwork - Proven track record.</li>
                <li>Freelancer - Reliable solutions.</li>
            </ul>
        </div>

        <div class="section">
            <h2>Certifications</h2>
            <ul>
                <li>Reward Certificate</li>
                <li>LEDP Certificate</li>
                <li>BTEB Certificate</li>
                <li>Moz Academy</li>
                <li>Google Analytics</li>
                <li>HubSpot Academy</li>
            </ul>
        </div>

        <div class="section">
            <h2>Let’s Connect</h2>
            <p>Ready to collaborate? Reach out!</p>
            <div class="social-links">
                <a href="https://www.youtube.com/@PlanExplorerOrg" target="_blank">YouTube</a>
                <a href="https://www.linkedin.com/in/ibrahim1BD" target="_blank">LinkedIn</a>
                <a href="https://www.facebook.com/bd.ibrahim.2" target="_blank">Facebook</a>
                <a href="https://twitter.com/meibrahimbd" target="_blank">Twitter</a>
                <a href="https://wa.me/+8801760792853" target="_blank">WhatsApp</a>
            </div>
        </div>

        <div class="footer">
            Designed for Success by Grok | February 22, 2025
        </div>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const container = document.querySelector('.container');
            container.style.opacity = '0';
            setTimeout(() => {
                container.style.opacity = '1';
            }, 100);

            // Scroll animation for sections
            const sections = document.querySelectorAll('.section');
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.style.opacity = '1';
                        entry.target.style.transform = 'translateY(0)';
                    }
                });
            }, { threshold: 0.1 });

            sections.forEach(section => {
                section.style.opacity = '0';
                section.style.transform = 'translateY(30px)';
                observer.observe(section);
            });
        });
    </script>
</body>
</html>
