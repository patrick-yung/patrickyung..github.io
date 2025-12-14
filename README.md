# patrickyung..github.io
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Patrick Yung Pak Hong - Resume</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
            background-color: #f8f9fa;
            color: #1a1a1a;
            line-height: 1.5;
            padding: 30px 20px;
        }
        
        .resume-container {
            max-width: 800px;
            margin: 0 auto;
            background: white;
            box-shadow: 0 2px 12px rgba(0, 0, 0, 0.06);
            border-radius: 8px;
            overflow: hidden;
        }
        
        /* Header - Clean Design */
        .header {
            background: #ffffff;
            padding: 40px 40px 30px;
            border-bottom: 1px solid #eaeaea;
        }
        
        .name-title h1 {
            font-size: 2.2rem;
            font-weight: 700;
            color: #1a1a1a;
            margin-bottom: 6px;
            letter-spacing: -0.3px;
        }
        
        .name-title h2 {
            font-size: 1.1rem;
            font-weight: 400;
            color: #666;
        }
        
        .contact-info {
            margin-top: 20px;
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
        }
        
        .contact-item {
            display: flex;
            align-items: center;
            gap: 8px;
            color: #555;
            font-size: 0.9rem;
        }
        
        .links {
            display: flex;
            gap: 15px;
            margin-top: 15px;
        }
        
        .links a {
            color: #2563eb;
            text-decoration: none;
            font-size: 0.9rem;
            font-weight: 500;
        }
        
        /* Main Content */
        .main-content {
            padding: 40px;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
        }
        
        /* Section Headers */
        .section-title {
            font-size: 1rem;
            font-weight: 600;
            color: #1a1a1a;
            margin-bottom: 20px;
            padding-bottom: 8px;
            border-bottom: 1px solid #eaeaea;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }
        
        /* Summary */
        .summary {
            margin-bottom: 30px;
            line-height: 1.6;
            color: #444;
            font-size: 0.95rem;
        }
        
        /* Experience & Education Items */
        .timeline-item {
            margin-bottom: 24px;
        }
        
        .item-header {
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
            margin-bottom: 6px;
        }
        
        .item-title {
            font-weight: 600;
            color: #1a1a1a;
            font-size: 1rem;
        }
        
        .item-date {
            color: #888;
            font-size: 0.85rem;
            font-weight: 500;
        }
        
        .item-company {
            color: #2563eb;
            font-size: 0.95rem;
            margin-bottom: 8px;
        }
        
        .item-description {
            color: #555;
            font-size: 0.9rem;
            line-height: 1.5;
        }
        
        .item-description ul {
            padding-left: 18px;
        }
        
        .item-description li {
            margin-bottom: 4px;
        }
        
        /* Skills */
        .skill-category {
            margin-bottom: 20px;
        }
        
        .skill-category h4 {
            font-size: 0.95rem;
            font-weight: 600;
            color: #1a1a1a;
            margin-bottom: 8px;
        }
        
        .skill-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 6px;
        }
        
        .skill-tag {
            background: #f0f4f8;
            color: #374151;
            padding: 4px 10px;
            border-radius: 4px;
            font-size: 0.85rem;
        }
        
        /* Languages */
        .language-item {
            display: flex;
            justify-content: space-between;
            margin-bottom: 10px;
        }
        
        .language-name {
            font-weight: 500;
            font-size: 0.9rem;
        }
        
        .language-level {
            color: #888;
            font-size: 0.85rem;
        }
        
        /* Projects */
        .project-item {
            margin-bottom: 20px;
            padding-bottom: 20px;
            border-bottom: 1px solid #f0f0f0;
        }
        
        .project-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 8px;
        }
        
        .project-title {
            font-weight: 600;
            color: #1a1a1a;
            font-size: 0.95rem;
        }
        
        .project-status {
            color: #ea580c;
            font-size: 0.8rem;
            font-weight: 500;
        }
        
        .project-desc {
            color: #555;
            font-size: 0.9rem;
            margin-bottom: 10px;
        }
        
        .project-tech {
            display: flex;
            flex-wrap: wrap;
            gap: 6px;
        }
        
        .tech-tag {
            background: #e0f2fe;
            color: #0369a1;
            padding: 3px 8px;
            border-radius: 4px;
            font-size: 0.8rem;
        }
        
        /* Additional Info */
        .additional-info {
            margin-top: 20px;
            padding: 20px;
            background: #f8fafc;
            border-radius: 6px;
        }
        
        .info-list li {
            margin-bottom: 8px;
            color: #555;
            font-size: 0.9rem;
            line-height: 1.5;
        }
        
        /* Footer */
        .footer {
            text-align: center;
            padding: 20px;
            border-top: 1px solid #eaeaea;
            color: #888;
            font-size: 0.85rem;
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            .main-content {
                grid-template-columns: 1fr;
                padding: 30px 20px;
                gap: 30px;
            }
        }
        
        @media print {
            body {
                background: white;
                padding: 0;
            }
            
            .resume-container {
                box-shadow: none;
                max-width: 100%;
            }
        }
    </style>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body>
    <div class="resume-container">
        <!-- Clean Header -->
        <header class="header">
            <div class="name-title">
                <h1>Patrick Yung Pak Hong</h1>
                <h2>Computer Engineer & Mobile Developer</h2>
            </div>
            <div class="contact-info">
                <div class="contact-item">📍 Toronto, ON</div>
                <div class="contact-item">📧 patrickyyung@gmail.com</div>
                <div class="contact-item">📱 9677-0137</div>
            </div>
            <div class="links">
                <a href="https://github.com/patrick-yung">GitHub</a>
                <a href="https://www.linkedin.com/in/pak-hong-patrick-yung-159726214/">LinkedIn</a>
            </div>
        </header>

        <!-- Main Content -->
        <div class="main-content">
            <!-- Left Column -->
            <div class="left-column">
                <!-- Summary -->
                <section class="summary">
                    <h3 class="section-title">Summary</h3>
                    <p>Computer Engineering graduate from CUHK with 2+ years of FPGA hardware/software experience. Currently advancing mobile development skills at Centennial College. International background with strong technical versatility from hardware to full-stack development.</p>
                </section>

                <!-- Experience -->
                <section class="experience">
                    <h3 class="section-title">Experience</h3>
                    <div class="timeline-item">
                        <div class="item-header">
                            <div class="item-title">Application/Software Engineer</div>
                            <div class="item-date">Jun 2022 – Dec 2024</div>
                        </div>
                        <div class="item-company">Efinix – FPGA Company</div>
                        <div class="item-description">
                            <ul>
                                <li>Designed IP AXI4 and I2C memory controllers</li>
                                <li>Tested FPGA devices for power efficiency</li>
                                <li>Bug fixing and feature development in Efinity software</li>
                                <li>FPGA design using Verilog, VHDL, and AutoCAD</li>
                            </ul>
                        </div>
                    </div>
                    
                    <div class="timeline-item">
                        <div class="item-header">
                            <div class="item-title">High School Work Experience</div>
                            <div class="item-date">Nov 2016</div>
                        </div>
                        <div class="item-company">China Light and Power Co Ltd (CLP)</div>
                        <div class="item-description">
                            Observed power plant operations and designed control system improvements.
                        </div>
                    </div>
                </section>

                <!-- Education -->
                <section class="education">
                    <h3 class="section-title">Education</h3>
                    <div class="timeline-item">
                        <div class="item-header">
                            <div class="item-title">Centennial College</div>
                            <div class="item-date">2025 – Present</div>
                        </div>
                        <div class="item-company">Mobile Application Development</div>
                    </div>
                    
                    <div class="timeline-item">
                        <div class="item-header">
                            <div class="item-title">The Chinese University of Hong Kong</div>
                            <div class="item-date">2019 – 2023</div>
                        </div>
                        <div class="item-company">B.Eng Computer Engineering • GPA: 3.34/4.0</div>
                    </div>
                    
                    <div class="timeline-item">
                        <div class="item-header">
                            <div class="item-title">Renaissance College Hong Kong</div>
                            <div class="item-date">2012 – 2019</div>
                        </div>
                        <div class="item-company">International Baccalaureate Diploma</div>
                    </div>
                </section>
            </div>

            <!-- Right Column -->
            <div class="right-column">
                <!-- Skills -->
                <section class="skills">
                    <h3 class="section-title">Skills</h3>
                    <div class="skill-category">
                        <h4>Mobile & Web</h4>
                        <div class="skill-tags">
                            <span class="skill-tag">Kotlin</span>
                            <span class="skill-tag">SwiftUI</span>
                            <span class="skill-tag">JavaScript</span>
                            <span class="skill-tag">Node.js</span>
                            <span class="skill-tag">MongoDB</span>
                        </div>
                    </div>
                    
                    <div class="skill-category">
                        <h4>Hardware & FPGA</h4>
                        <div class="skill-tags">
                            <span class="skill-tag">Verilog</span>
                            <span class="skill-tag">VHDL</span>
                            <span class="skill-tag">AutoCAD</span>
                            <span class="skill-tag">FPGA Design</span>
                        </div>
                    </div>
                    
                    <div class="skill-category">
                        <h4>Programming</h4>
                        <div class="skill-tags">
                            <span class="skill-tag">C++</span>
                            <span class="skill-tag">C</span>
                            <span class="skill-tag">Python</span>
                            <span class="skill-tag">PHP</span>
                        </div>
                    </div>
                </section>

                <!-- Languages -->
                <section class="languages">
                    <h3 class="section-title">Languages</h3>
                    <div class="language-item">
                        <span class="language-name">English</span>
                        <span class="language-level">Professional</span>
                    </div>
                    <div class="language-item">
                        <span class="language-name">Mandarin</span>
                        <span class="language-level">Professional</span>
                    </div>
                    <div class="language-item">
                        <span class="language-name">Cantonese</span>
                        <span class="language-level">Native</span>
                    </div>
                </section>

                <!-- Projects -->
                <section class="projects">
                    <h3 class="section-title">Projects</h3>
                    <div class="project-item">
                        <div class="project-header">
                            <div class="project-title">LifeTrack Mobile App</div>
                            <div class="project-status">In Development</div>
                        </div>
                        <div class="project-desc">Full-stack mobile app for tracking healthy habits with gamification.</div>
                        <div class="project-tech">
                            <span class="tech-tag">SwiftUI</span>
                            <span class="tech-tag">Kotlin</span>
                            <span class="tech-tag">Node.js</span>
                        </div>
                    </div>
                    
                    <div class="project-item">
                        <div class="project-header">
                            <div class="project-title">Personal Portfolio Website</div>
                        </div>
                        <div class="project-desc">Custom-built responsive portfolio website.</div>
                        <div class="project-tech">
                            <span class="tech-tag">HTML/CSS</span>
                            <span class="tech-tag">JavaScript</span>
                            <span class="tech-tag">PHP</span>
                        </div>
                    </div>
                    
                    <div class="project-item">
                        <div class="project-header">
                            <div class="project-title">FPGA Memory Controller</div>
                        </div>
                        <div class="project-desc">AXI4 and I2C memory controller designs.</div>
                        <div class="project-tech">
                            <span class="tech-tag">Verilog</span>
                            <span class="tech-tag">VHDL</span>
                        </div>
                    </div>
                </section>

                <!-- Additional Information -->
                <section class="additional-info">
                    <h3 class="section-title">Additional</h3>
                    <ul class="info-list">
                        <li>Experienced with 3D printers and laser cutters</li>
                        <li>Open-minded team player with strong listening skills</li>
                        <li>Trilingual capabilities supporting global collaboration</li>
                        <li>Technical versatility from hardware to full-stack</li>
                    </ul>
                </section>
            </div>
        </div>

        <!-- Footer -->
        <footer class="footer">
            <p>References available upon request | Updated: <span id="current-date"></span></p>
        </footer>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const now = new Date();
            const currentDate = now.toLocaleDateString('en-US', { year: 'numeric', month: 'long' });
            document.getElementById('current-date').textContent = currentDate;
        });
    </script>
</body>
</html>
