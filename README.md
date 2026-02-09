<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Masarapu Naga Karishma Mounika | Data & Business Analytics Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                        serif: ['Playfair Display', 'serif'],
                    },
                    colors: {
                        primary: '#0f172a',
                        secondary: '#1e293b',
                        accent: '#3b82f6',
                        'accent-light': '#60a5fa',
                        'warm-gray': '#f8fafc',
                    },
                    animation: {
                        'fade-in-up': 'fadeInUp 0.8s ease-out',
                        'float': 'float 6s ease-in-out infinite',
                        'pulse-slow': 'pulse 4s cubic-bezier(0.4, 0, 0.6, 1) infinite',
                    },
                    keyframes: {
                        fadeInUp: {
                            '0%': { opacity: '0', transform: 'translateY(30px)' },
                            '100%': { opacity: '1', transform: 'translateY(0)' },
                        },
                        float: {
                            '0%, 100%': { transform: 'translateY(0)' },
                            '50%': { transform: 'translateY(-20px)' },
                        }
                    }
                }
            }
        }
    </script>
    <style>
        .glass-effect {
            background: rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        .gradient-text {
            background: linear-gradient(135deg, #3b82f6 0%, #8b5cf6 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        .skill-card {
            transition: all 0.3s ease;
        }
        .skill-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 40px rgba(59, 130, 246, 0.15);
        }
        .timeline-line {
            background: linear-gradient(to bottom, #3b82f6, #8b5cf6);
        }
        .project-card {
            background: linear-gradient(135deg, #1e293b 0%, #0f172a 100%);
        }
        .hero-bg {
            background: radial-gradient(circle at 50% 50%, rgba(59, 130, 246, 0.1) 0%, transparent 50%);
        }
        .noise-bg {
            position: relative;
        }
        .noise-bg::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 200 200' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noiseFilter'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.65' numOctaves='3' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noiseFilter)' opacity='0.02'/%3E%3C/svg%3E");
            pointer-events: none;
        }
    </style>
</head>
<body class="bg-primary text-gray-100 font-sans antialiased overflow-x-hidden noise-bg">

    <!-- Navigation -->
    <nav class="fixed w-full z-50 transition-all duration-300" id="navbar">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-20">
                <div class="flex-shrink-0 flex items-center">
                    <span class="font-serif text-2xl font-bold gradient-text">M.N.K.M.</span>
                </div>
                <div class="hidden md:block">
                    <div class="ml-10 flex items-baseline space-x-8">
                        <a href="#home" class="hover:text-accent-light transition-colors px-3 py-2 rounded-md text-sm font-medium">Home</a>
                        <a href="#about" class="hover:text-accent-light transition-colors px-3 py-2 rounded-md text-sm font-medium">About</a>
                        <a href="#experience" class="hover:text-accent-light transition-colors px-3 py-2 rounded-md text-sm font-medium">Experience</a>
                        <a href="#projects" class="hover:text-accent-light transition-colors px-3 py-2 rounded-md text-sm font-medium">Projects</a>
                        <a href="#skills" class="hover:text-accent-light transition-colors px-3 py-2 rounded-md text-sm font-medium">Skills</a>
                        <a href="#contact" class="bg-accent hover:bg-accent-light text-white px-6 py-2 rounded-full text-sm font-medium transition-all transform hover:scale-105">Contact</a>
                    </div>
                </div>
                <div class="-mr-2 flex md:hidden">
                    <button onclick="toggleMobileMenu()" class="inline-flex items-center justify-center p-2 rounded-md text-gray-400 hover:text-white hover:bg-secondary focus:outline-none">
                        <i class="fas fa-bars text-xl"></i>
                    </button>
                </div>
            </div>
        </div>
        <!-- Mobile menu -->
        <div class="md:hidden hidden glass-effect" id="mobile-menu">
            <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3">
                <a href="#home" class="block px-3 py-2 rounded-md text-base font-medium hover:bg-secondary">Home</a>
                <a href="#about" class="block px-3 py-2 rounded-md text-base font-medium hover:bg-secondary">About</a>
                <a href="#experience" class="block px-3 py-2 rounded-md text-base font-medium hover:bg-secondary">Experience</a>
                <a href="#projects" class="block px-3 py-2 rounded-md text-base font-medium hover:bg-secondary">Projects</a>
                <a href="#skills" class="block px-3 py-2 rounded-md text-base font-medium hover:bg-secondary">Skills</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="relative min-h-screen flex items-center justify-center hero-bg pt-20">
        <div class="absolute inset-0 overflow-hidden">
            <div class="absolute -top-40 -right-40 w-96 h-96 bg-blue-500 rounded-full mix-blend-multiply filter blur-3xl opacity-20 animate-float"></div>
            <div class="absolute -bottom-40 -left-40 w-96 h-96 bg-purple-500 rounded-full mix-blend-multiply filter blur-3xl opacity-20 animate-float" style="animation-delay: 2s;"></div>
        </div>
        
        <div class="relative max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center z-10">
            <div class="animate-fade-in-up">
                <p class="text-accent-light font-medium tracking-widest uppercase mb-4 text-sm">Data & Business Analytics Professional</p>
                <h1 class="font-serif text-5xl md:text-7xl font-bold mb-6 leading-tight">
                    Masarapu Naga<br>
                    <span class="gradient-text">Karishma Mounika</span>
                </h1>
                <p class="text-xl md:text-2xl text-gray-400 mb-8 max-w-3xl mx-auto font-light">
                    Transforming complex data into strategic insights. Specializing in SQL, Python, Power BI, and Risk Analytics.
                </p>
                <div class="flex flex-col sm:flex-row gap-4 justify-center items-center">
                    <a href="#projects" class="bg-accent hover:bg-accent-light text-white px-8 py-4 rounded-full font-semibold transition-all transform hover:scale-105 shadow-lg shadow-blue-500/30">
                        View My Work
                    </a>
                    <a href="#contact" class="border-2 border-gray-600 hover:border-accent text-gray-300 hover:text-white px-8 py-4 rounded-full font-semibold transition-all">
                        Get In Touch
                    </a>
                </div>
            </div>
            
            <div class="mt-16 grid grid-cols-2 md:grid-cols-4 gap-8 max-w-4xl mx-auto">
                <div class="glass-effect p-6 rounded-2xl">
                    <div class="text-3xl font-bold text-accent mb-1">2+</div>
                    <div class="text-sm text-gray-400">Years Experience</div>
                </div>
                <div class="glass-effect p-6 rounded-2xl">
                    <div class="text-3xl font-bold text-accent mb-1">$2B+</div>
                    <div class="text-sm text-gray-400">AUM Analyzed</div>
                </div>
                <div class="glass-effect p-6 rounded-2xl">
                    <div class="text-3xl font-bold text-accent mb-1">20%</div>
                    <div class="text-sm text-gray-400">Efficiency Gain</div>
                </div>
                <div class="glass-effect p-6 rounded-2xl">
                    <div class="text-3xl font-bold text-accent mb-1">3.74</div>
                    <div class="text-sm text-gray-400">GPA</div>
                </div>
            </div>
        </div>
        
        <div class="absolute bottom-10 left-1/2 transform -translate-x-1/2 animate-bounce">
            <i class="fas fa-chevron-down text-gray-500 text-2xl"></i>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-24 bg-secondary/30">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid md:grid-cols-2 gap-16 items-center">
                <div class="relative">
                    <div class="absolute inset-0 bg-gradient-to-r from-blue-500 to-purple-600 rounded-3xl transform rotate-3 opacity-20"></div>
                    <div class="relative bg-secondary p-8 rounded-3xl border border-gray-700">
                        <div class="flex items-center gap-4 mb-6">
                            <div class="w-16 h-16 bg-accent/20 rounded-full flex items-center justify-center">
                                <i class="fas fa-graduation-cap text-2xl text-accent"></i>
                            </div>
                            <div>
                                <h3 class="font-bold text-lg">Education</h3>
                                <p class="text-gray-400 text-sm">Academic Background</p>
                            </div>
                        </div>
                        <div class="space-y-4">
                            <div class="border-l-2 border-accent pl-4">
                                <h4 class="font-semibold text-white">MS in Business Data Analytics</h4>
                                <p class="text-accent-light text-sm">Lawrence Technological University</p>
                                <p class="text-gray-500 text-xs mt-1">Jan 2024 - Dec 2025 • GPA: 3.74/4.0</p>
                            </div>
                            <div class="border-l-2 border-gray-600 pl-4">
                                <h4 class="font-semibold text-white">BTech in Civil Engineering</h4>
                                <p class="text-accent-light text-sm">NIT Durgapur, India</p>
                                <p class="text-gray-500 text-xs mt-1">Aug 2018 - May 2022</p>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div>
                    <h2 class="text-accent-light font-medium tracking-widest uppercase mb-2 text-sm">About Me</h2>
                    <h3 class="font-serif text-4xl font-bold mb-6">Bridging Data & Business Strategy</h3>
                    <p class="text-gray-400 text-lg leading-relaxed mb-6">
                        Data and Business Analytics professional with 2 years of experience driving data-driven decision-making through actionable insights, data visualization, and exploratory data analysis. Experienced in SQL, Python, Excel, and Power BI, with a strong focus on contact operations analytics, data quality management, and governance.
                    </p>
                    <p class="text-gray-400 text-lg leading-relaxed mb-8">
                        Proven ability to translate business requirements into strategic initiatives, collaborate cross-functionally, and present data stories to business leaders and senior stakeholders. Currently pursuing Master's at Lawrence Technological University to deepen expertise in advanced analytics.
                    </p>
                    
                    <div class="flex flex-wrap gap-3">
                        <span class="px-4 py-2 bg-accent/10 text-accent-light rounded-full text-sm border border-accent/20">Risk Analytics</span>
                        <span class="px-4 py-2 bg-accent/10 text-accent-light rounded-full text-sm border border-accent/20">Data Visualization</span>
                        <span class="px-4 py-2 bg-accent/10 text-accent-light rounded-full text-sm border border-accent/20">Business Intelligence</span>
                        <span class="px-4 py-2 bg-accent/10 text-accent-light rounded-full text-sm border border-accent/20">Process Improvement</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Experience Section -->
    <section id="experience" class="py-24 relative">
        <div class="max-w-5xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-accent-light font-medium tracking-widest uppercase mb-2 text-sm">Career Path</h2>
                <h3 class="font-serif text-4xl font-bold">Professional Experience</h3>
            </div>

            <div class="relative">
                <!-- Timeline line -->
                <div class="absolute left-1/2 transform -translate-x-1/2 w-1 h-full timeline-line rounded-full hidden md:block"></div>

                <!-- HSBC Role -->
                <div class="relative mb-12 md:mb-24">
                    <div class="md:flex items-center justify-between">
                        <div class="md:w-5/12 md:text-right pr-8">
                            <div class="glass-effect p-6 rounded-2xl hover:border-accent/50 transition-all duration-300">
                                <span class="text-accent-light font-semibold text-sm">Feb 2022 - Dec 2023</span>
                                <h4 class="text-xl font-bold mt-2 mb-1">Credit Risk Analyst</h4>
                                <p class="text-gray-400 text-sm mb-3">HSBC Electronic Data Processing (India) Pvt. Ltd., Bangalore</p>
                                <p class="text-gray-500 text-sm">Decision Sciences – GSC's</p>
                            </div>
                        </div>
                        <div class="absolute left-1/2 transform -translate-x-1/2 w-4 h-4 bg-accent rounded-full border-4 border-primary z-10 hidden md:block"></div>
                        <div class="md:w-5/12 pl-8 mt-4 md:mt-0">
                            <ul class="space-y-2 text-gray-400 text-sm">
                                <li class="flex items-start gap-2">
                                    <i class="fas fa-check-circle text-accent mt-1 text-xs"></i>
                                    <span>Analyzed financial datasets using Excel, SQL, and Tableau for $2B+ AUM portfolios</span>
                                </li>
                                <li class="flex items-start gap-2">
                                    <i class="fas fa-check-circle text-accent mt-1 text-xs"></i>
                                    <span>Monitored KPIs and validated insights for senior stakeholder reporting</span>
                                </li>
                                <li class="flex items-start gap-2">
                                    <i class="fas fa-check-circle text-accent mt-1 text-xs"></i>
                                    <span>Achieved 20% improvement in reporting workflows through process optimization</span>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>

                <!-- Internship -->
                <div class="relative mb-12">
                    <div class="md:flex items-center justify-between flex-row-reverse">
                        <div class="md:w-5/12 md:text-left pl-8">
                            <div class="glass-effect p-6 rounded-2xl hover:border-accent/50 transition-all duration-300">
                                <span class="text-accent-light font-semibold text-sm">June 2021</span>
                                <h4 class="text-xl font-bold mt-2 mb-1">Summer Intern</h4>
                                <p class="text-gray-400 text-sm mb-3">Dilip Buildcon Ltd.</p>
                                <p class="text-gray-500 text-sm">Visakhapatnam, Andhra Pradesh</p>
                            </div>
                        </div>
                        <div class="absolute left-1/2 transform -translate-x-1/2 w-4 h-4 bg-gray-600 rounded-full border-4 border-primary z-10 hidden md:block"></div>
                        <div class="md:w-5/12 pr-8 mt-4 md:mt-0 md:text-right">
                            <p class="text-gray-400 text-sm">Construction practices analysis for highway projects (Anandapuram to Anakapalli)</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="py-24 bg-secondary/30">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-accent-light font-medium tracking-widest uppercase mb-2 text-sm">Portfolio</h2>
                <h3 class="font-serif text-4xl font-bold mb-4">Featured Projects</h3>
                <p class="text-gray-400 max-w-2xl mx-auto">Demonstrating expertise in data visualization, machine learning, and business intelligence through practical applications.</p>
            </div>

            <div class="grid md:grid-cols-3 gap-8">
                <!-- Project 1 -->
                <div class="project-card rounded-2xl overflow-hidden border border-gray-700 group hover:border-accent/50 transition-all duration-300">
                    <div class="h-48 bg-gradient-to-br from-red-600 to-orange-600 flex items-center justify-center relative overflow-hidden">
                        <i class="fas fa-chart-pie text-6xl text-white/20 group-hover:scale-110 transition-transform duration-500"></i>
                        <div class="absolute inset-0 bg-black/20 group-hover:bg-black/10 transition-colors"></div>
                        <div class="absolute bottom-4 left-4">
                            <span class="px-3 py-1 bg-white/20 backdrop-blur-md rounded-full text-xs text-white">Power BI</span>
                        </div>
                    </div>
                    <div class="p-6">
                        <h4 class="text-xl font-bold mb-2 group-hover:text-accent-light transition-colors">Wendy's Menu Analysis</h4>
                        <p class="text-gray-400 text-sm mb-4">Business Intelligence Dashboard Project translating complex menu data into actionable insights for business leaders.</p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="text-xs px-2 py-1 bg-gray-800 rounded text-gray-400">Power Query</span>
                            <span class="text-xs px-2 py-1 bg-gray-800 rounded text-gray-400">DAX</span>
                            <span class="text-xs px-2 py-1 bg-gray-800 rounded text-gray-400">Excel</span>
                        </div>
                        <div class="flex items-center text-accent-light text-sm font-medium group-hover:gap-2 transition-all">
                            <span>View Project</span>
                            <i class="fas fa-arrow-right ml-2 group-hover:translate-x-1 transition-transform"></i>
                        </div>
                    </div>
                </div>

                <!-- Project 2 -->
                <div class="project-card rounded-2xl overflow-hidden border border-gray-700 group hover:border-accent/50 transition-all duration-300">
                    <div class="h-48 bg-gradient-to-br from-blue-600 to-cyan-600 flex items-center justify-center relative overflow-hidden">
                        <i class="fas fa-baby text-6xl text-white/20 group-hover:scale-110 transition-transform duration-500"></i>
                        <div class="absolute inset-0 bg-black/20 group-hover:bg-black/10 transition-colors"></div>
                        <div class="absolute bottom-4 left-4">
                            <span class="px-3 py-1 bg-white/20 backdrop-blur-md rounded-full text-xs text-white">Python</span>
                        </div>
                    </div>
                    <div class="p-6">
                        <h4 class="text-xl font-bold mb-2 group-hover:text-accent-light transition-colors">Newborn Baby Names Analysis</h4>
                        <p class="text-gray-400 text-sm mb-4">Exploratory data analysis on U.S. baby name datasets analyzing trends across years, gender, and regions.</p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="text-xs px-2 py-1 bg-gray-800 rounded text-gray-400">Pandas</span>
                            <span class="text-xs px-2 py-1 bg-gray-800 rounded text-gray-400">NumPy</span>
                            <span class="text-xs px-2 py-1 bg-gray-800 rounded text-gray-400">Matplotlib</span>
                            <span class="text-xs px-2 py-1 bg-gray-800 rounded text-gray-400">Seaborn</span>
                        </div>
                        <div class="flex items-center text-accent-light text-sm font-medium group-hover:gap-2 transition-all">
                            <span>View Project</span>
                            <i class="fas fa-arrow-right ml-2 group-hover:translate-x-1 transition-transform"></i>
                        </div>
                    </div>
                </div>

                <!-- Project 3 -->
                <div class="project-card rounded-2xl overflow-hidden border border-gray-700 group hover:border-accent/50 transition-all duration-300">
                    <div class="h-48 bg-gradient-to-br from-purple-600 to-pink-600 flex items-center justify-center relative overflow-hidden">
                        <i class="fas fa-brain text-6xl text-white/20 group-hover:scale-110 transition-transform duration-500"></i>
                        <div class="absolute inset-0 bg-black/20 group-hover:bg-black/10 transition-colors"></div>
                        <div class="absolute bottom-4 left-4">
                            <span class="px-3 py-1 bg-white/20 backdrop-blur-md rounded-full text-xs text-white">ML</span>
                        </div>
                    </div>
                    <div class="p-6">
                        <h4 class="text-xl font-bold mb-2 group-hover:text-accent-light transition-colors">Interactive ML Simulations</h4>
                        <p class="text-gray-400 text-sm mb-4">Browser-based visualizations of K-Means, KNN, and Neural Networks with dynamic parameter controls.</p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="text-xs px-2 py-1 bg-gray-800 rounded text-gray-400">JavaScript</span>
                            <span class="text-xs px-2 py-1 bg-gray-800 rounded text-gray-400">Algorithms</span>
                            <span class="text-xs px-2 py-1 bg-gray-800 rounded text-gray-400">Visualization</span>
                        </div>
                        <div class="flex items-center text-accent-light text-sm font-medium group-hover:gap-2 transition-all">
                            <span>View Project</span>
                            <i class="fas fa-arrow-right ml-2 group-hover:translate-x-1 transition-transform"></i>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="py-24">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-accent-light font-medium tracking-widest uppercase mb-2 text-sm">Expertise</h2>
                <h3 class="font-serif text-4xl font-bold">Technical Skills</h3>
            </div>

            <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-6">
                <!-- Data & Reporting -->
                <div class="skill-card glass-effect p-6 rounded-2xl border border-gray-700">
                    <div class="w-12 h-12 bg-blue-500/20 rounded-xl flex items-center justify-center mb-4">
                        <i class="fas fa-database text-blue-400 text-xl"></i>
                    </div>
                    <h4 class="font-bold text-lg mb-3">Data & Reporting</h4>
                    <ul class="space-y-2 text-gray-400 text-sm">
                        <li class="flex items-center gap-2"><i class="fas fa-circle text-xs text-blue-400"></i> Advanced Excel</li>
                        <li class="flex items-center gap-2"><i class="fas fa-circle text-xs text-blue-400"></i> Power BI & Tableau</li>
                        <li class="flex items-center gap-2"><i class="fas fa-circle text-xs text-blue-400"></i> Power Query & DAX</li>
                        <li class="flex items-center gap-2"><i class="fas fa-circle text-xs text-blue-400"></i> SQL</li>
                        <li class="flex items-center gap-2"><i class="fas fa-circle text-xs text-blue-400"></i> Dashboard Development</li>
                    </ul>
                </div>

                <!-- Technical & Analytics -->
                <div class="skill-card glass-effect p-6 rounded-2xl border border-gray-700">
                    <div class="w-12 h-12 bg-purple-500/20 rounded-xl flex items-center justify-center mb-4">
                        <i class="fas fa-code text-purple-400 text-xl"></i>
                    </div>
                    <h4 class="font-bold text-lg mb-3">Technical & Analytics</h4>
                    <ul class="space-y-2 text-gray-400 text-sm">
                        <li class="flex items-center gap-2"><i class="fas fa-circle text-xs text-purple-400"></i> Python (Pandas, NumPy)</li>
                        <li class="flex items-center gap-2"><i class="fas fa-circle text-xs text-purple-400"></i> ETL Processes</li>
                        <li class="flex items-center gap-2"><i class="fas fa-circle text-xs text-purple-400"></i> Data Visualization</li>
                        <li class="flex items-center gap-2"><i class="fas fa-circle text-xs text-purple-400"></i> Statistical Analysis</li>
                        <li class="flex items-center gap-2"><i class="fas fa-circle text-xs text-purple-400"></i> Root Cause Analysis</li>
                    </ul>
                </div>

                <!-- Business & Consulting -->
                <div class="skill-card glass-effect p-6 rounded-2xl border border-gray-700">
                    <div class="w-12 h-12 bg-green-500/20 rounded-xl flex items-center justify-center mb-4">
                        <i class="fas fa-briefcase text-green-400 text-xl"></i>
                    </div>
                    <h4 class="font-bold text-lg mb-3">Business Skills</h4>
                    <ul class="space-y-2 text-gray-400 text-sm">
                        <li class="flex items-center gap-2"><i class="fas fa-circle text-xs text-green-400"></i> Business Analytics</li>
                        <li class="flex items-center gap-2"><i class="fas fa-circle text-xs text-green-400"></i> Requirements Gathering</li>
                        <li class="flex items-center gap-2"><i class="fas fa-circle text-xs text-green-400"></i> Data Governance</li>
                        <li class="flex items-center gap-2"><i class="fas fa-circle text-xs text-green-400"></i> Process Improvement</li>
                        <li class="flex items-center gap-2"><i class="fas fa-circle text-xs text-green-400"></i> Stakeholder Communication</li>
                    </ul>
                </div>

                <!-- Certifications -->
                <div class="skill-card glass-effect p-6 rounded-2xl border border-gray-700">
                    <div class="w-12 h-12 bg-yellow-500/20 rounded-xl flex items-center justify-center mb-4">
                        <i class="fas fa-certificate text-yellow-400 text-xl"></i>
                    </div>
                    <h4 class="font-bold text-lg mb-3">Certifications</h4>
                    <ul class="space-y-2 text-gray-400 text-sm">
                        <li class="flex items-center gap-2"><i class="fas fa-check text-xs text-yellow-400"></i> Microsoft Certified: Power BI Data Analyst Associate</li>
                        <li class="flex items-center gap-2"><i class="fas fa-check text-xs text-yellow-400"></i> PCAD – Certified Python Data Analyst</li>
                        <li class="flex items-center gap-2"><i class="fas fa-check text-xs text-yellow-400"></i> Data Visualization for Data Analysis</li>
                        <li class="flex items-center gap-2"><i class="fas fa-check text-xs text-yellow-400"></i> SQL Essential Training</li>
                        <li class="flex items-center gap-2"><i class="fas fa-check text-xs text-yellow-400"></i> Inbound Marketing</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Achievements Section -->
    <section class="py-16 bg-secondary/30">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="glass-effect rounded-3xl p-8 md:p-12 border border-gray-700">
                <div class="flex flex-col md:flex-row items-center gap-8">
                    <div class="flex-1">
                        <h3 class="font-serif text-3xl font-bold mb-4">Leadership & Achievements</h3>
                        <div class="space-y-4">
                            <div class="flex items-start gap-4">
                                <div class="w-10 h-10 bg-accent/20 rounded-full flex items-center justify-center flex-shrink-0 mt-1">
                                    <i class="fas fa-award text-accent"></i>
                                </div>
                                <div>
                                    <h4 class="font-semibold text-lg">Zero Waste Management Technical Lead</h4>
                                    <p class="text-gray-400 text-sm">NIT Durgapur • Organized seminars and workshops as student representative</p>
                                </div>
                            </div>
                            <div class="flex items-start gap-4">
                                <div class="w-10 h-10 bg-accent/20 rounded-full flex items-center justify-center flex-shrink-0 mt-1">
                                    <i class="fas fa-users text-accent"></i>
                                </div>
                                <div>
                                    <h4 class="font-semibold text-lg">IEEE Student Branch Member</h4>
                                    <p class="text-gray-400 text-sm">NIT Durgapur • Organized research-oriented events for junior students</p>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="flex-shrink-0">
                        <div class="w-32 h-32 bg-gradient-to-br from-accent to-purple-600 rounded-full flex items-center justify-center animate-pulse-slow">
                            <i class="fas fa-trophy text-4xl text-white"></i>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-24">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <h2 class="text-accent-light font-medium tracking-widest uppercase mb-2 text-sm">Get In Touch</h2>
            <h3 class="font-serif text-4xl font-bold mb-6">Let's Work Together</h3>
            <p class="text-gray-400 mb-12 max-w-2xl mx-auto">
                I'm currently open to data analytics and business intelligence opportunities. Whether you have a question or just want to say hi, feel free to reach out!
            </p>

            <div class="grid md:grid-cols-3 gap-6 mb-12">
                <a href="mailto:mounika5625@gmail.com" class="glass-effect p-6 rounded-2xl border border-gray-700 hover:border-accent/50 transition-all group">
                    <div class="w-12 h-12 bg-red-500/20 rounded-full flex items-center justify-center mx-auto mb-4 group-hover:scale-110 transition-transform">
                        <i class="fas fa-envelope text-red-400 text-xl"></i>
                    </div>
                    <h4 class="font-semibold mb-1">Email</h4>
                    <p class="text-gray-400 text-sm">mounika5625@gmail.com</p>
                </a>

                <a href="tel:+19472418399" class="glass-effect p-6 rounded-2xl border border-gray-700 hover:border-accent/50 transition-all group">
                    <div class="w-12 h-12 bg-green-500/20 rounded-full flex items-center justify-center mx-auto mb-4 group-hover:scale-110 transition-transform">
                        <i class="fas fa-phone text-green-400 text-xl"></i>
                    </div>
                    <h4 class="font-semibold mb-1">Phone</h4>
                    <p class="text-gray-400 text-sm">+1 (947) 241-8399</p>
                </a>

                <a href="https://www.linkedin.com/in/masarapu-naga-karishmamounika-38a1741b4" target="_blank" class="glass-effect p-6 rounded-2xl border border-gray-700 hover:border-accent/50 transition-all group">
                    <div class="w-12 h-12 bg-blue-600/20 rounded-full flex items-center justify-center mx-auto mb-4 group-hover:scale-110 transition-transform">
                        <i class="fab fa-linkedin text-blue-400 text-xl"></i>
                    </div>
                    <h4 class="font-semibold mb-1">LinkedIn</h4>
                    <p class="text-gray-400 text-sm">Connect with me</p>
                </a>
            </div>

            <div class="glass-effect rounded-2xl p-8 border border-gray-700">
                <form class="space-y-4 text-left" onsubmit="event.preventDefault(); alert('Thank you for your message! I will get back to you soon.');">
                    <div class="grid md:grid-cols-2 gap-4">
                        <div>
                            <label class="block text-sm font-medium text-gray-400 mb-2">Name</label>
                            <input type="text" class="w-full bg-primary border border-gray-700 rounded-lg px-4 py-3 text-white focus:border-accent focus:outline-none transition-colors" placeholder="Your name">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-400 mb-2">Email</label>
                            <input type="email" class="w-full bg-primary border border-gray-700 rounded-lg px-4 py-3 text-white focus:border-accent focus:outline-none transition-colors" placeholder="your@email.com">
                        </div>
                    </div>
                    <div>
                        <label class="block text-sm font-medium text-gray-400 mb-2">Message</label>
                        <textarea rows="4" class="w-full bg-primary border border-gray-700 rounded-lg px-4 py-3 text-white focus:border-accent focus:outline-none transition-colors" placeholder="Your message..."></textarea>
                    </div>
                    <button type="submit" class="w-full bg-accent hover:bg-accent-light text-white font-semibold py-4 rounded-lg transition-all transform hover:scale-[1.02]">
                        Send Message
                    </button>
                </form>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-secondary/50 border-t border-gray-800 py-8">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-col md:flex-row justify-between items-center gap-4">
            <div class="text-gray-500 text-sm">
                © 2024 Masarapu Naga Karishma Mounika. All rights reserved.
            </div>
            <div class="flex gap-6">
                <a href="https://www.linkedin.com/in/masarapu-naga-karishmamounika-38a1741b4" target="_blank" class="text-gray-400 hover:text-accent-light transition-colors">
                    <i class="fab fa-linkedin text-xl"></i>
                </a>
                <a href="mailto:mounika5625@gmail.com" class="text-gray-400 hover:text-accent-light transition-colors">
                    <i class="fas fa-envelope text-xl"></i>
                </a>
            </div>
        </div>
    </footer>

    <script>
        // Mobile menu toggle
        function toggleMobileMenu() {
            const menu = document.getElementById('mobile-menu');
            menu.classList.toggle('hidden');
        }

        // Navbar scroll effect
        window.addEventListener('scroll', function() {
            const navbar = document.getElementById('navbar');
            if (window.scrollY > 50) {
                navbar.classList.add('bg-primary/90', 'backdrop-blur-md', 'shadow-lg');
            } else {
                navbar.classList.remove('bg-primary/90', 'backdrop-blur-md', 'shadow-lg');
            }
        });

        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                    // Close mobile menu if open
                    document.getElementById('mobile-menu').classList.add('hidden');
                }
            });
        });

        // Intersection Observer for fade-in animations
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = '1';
                    entry.target.style.transform = 'translateY(0)';
                }
            });
        }, observerOptions);

        // Observe elements for animation
        document.querySelectorAll('.glass-effect, .project-card, .skill-card').forEach((el) => {
            el.style.opacity = '0';
            el.style.transform = 'translateY(20px)';
            el.style.transition = 'opacity 0.6s ease-out, transform 0.6s ease-out';
            observer.observe(el);
        });
    </script>
</body>
</html>
