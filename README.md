<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Moch. Fajri Ramdhani - Blockchain Developer Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    colors: {
                        primary: {
                            light: '#3b82f6',
                            dark: '#1e40af'
                        },
                        secondary: {
                            light: '#10b981',
                            dark: '#059669'
                        }
                    },
                    animation: {
                        'fade-in': 'fadeIn 0.5s ease-in-out',
                        'slide-up': 'slideUp 0.5s ease-out'
                    },
                    keyframes: {
                        fadeIn: {
                            '0%': { opacity: '0' },
                            '100%': { opacity: '1' }
                        },
                        slideUp: {
                            '0%': { 
                                opacity: '0',
                                transform: 'translateY(20px)'
                            },
                            '100%': { 
                                opacity: '1',
                                transform: 'translateY(0)'
                            }
                        }
                    }
                }
            }
        }
    </script>
    <style>
        .gradient-text {
            background-clip: text;
            -webkit-background-clip: text;
            color: transparent;
        }
        
        .card-hover:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
        }
        
        .skill-bar {
            transition: width 1.5s ease-in-out;
        }
        
        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
            100% { transform: translateY(0px); }
        }
        
        .float-animation {
            animation: float 3s ease-in-out infinite;
        }
    </style>
</head>
<body class="bg-gray-100 dark:bg-gray-900 text-gray-800 dark:text-gray-200 transition-colors duration-300">
    <!-- Theme Toggle -->
    <div class="fixed top-4 right-4 z-50">
        <button id="theme-toggle" class="p-2 rounded-full bg-white/80 dark:bg-gray-800/80 shadow-lg backdrop-blur-sm">
            <i class="fas fa-moon text-gray-800 dark:text-yellow-300"></i>
        </button>
    </div>

    <!-- Navigation -->
    <header class="sticky top-0 z-40 backdrop-blur-md bg-white/50 dark:bg-gray-900/50 shadow-sm">
        <nav class="max-w-6xl mx-auto px-4 py-3 flex justify-between items-center">
            <div class="flex items-center space-x-2">
                <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/b5f8495b-2d13-4907-8572-66aeb0606228.png" alt="Blockchain logo with interconnected nodes and blue gradient background" class="rounded-full w-4 h-4" style="outline: rgb(0, 0, 0) dotted 1px; outline-offset: 1px;">
                <span class="text-xl font-bold" style="outline: rgb(0, 0, 0) dotted 3px; outline-offset: 1px;">Moch. Fajri Ramdhani</span>
            </div>
            <div class="hidden md:flex space-x-6">
                <a href="#home" class="hover:text-primary-light dark:hover:text-primary-dark transition">Home</a>
                <a href="#projects" class="hover:text-primary-light dark:hover:text-primary-dark transition">Projects</a>
                <a href="#skills" class="hover:text-primary-light dark:hover:text-primary-dark transition">Skills</a>
                <a href="#contact" class="hover:text-primary-light dark:hover:text-primary-dark transition">Contact</a>
            </div>
            <button class="md:hidden">
                <i class="fas fa-bars"></i>
            </button>
        </nav>
    </header>

    <!-- Hero Section -->
    <section id="home" class="min-h-[80vh] flex items-center justify-center">
        <div class="max-w-6xl mx-auto px-4 py-16 md:py-24 grid md:grid-cols-2 gap-12 items-center">
            <div class="space-y-6 animate-fade-in">
                <div class="text-sm font-medium px-3 py-1 rounded-full bg-blue-100 dark:bg-blue-900 text-blue-600 dark:text-blue-200 w-fit">
                    Blockchain Developer
                </div>
                <h1 class="text-4xl md:text-6xl font-bold leading-tight">
                    Building the Future with
                    <span class="gradient-text bg-gradient-to-r from-blue-600 to-green-500 dark:from-blue-400 dark:to-green-400">Blockchain</span>
                </h1>
                <p class="text-lg text-gray-600 dark:text-gray-400 leading-relaxed">
                    I create secure, decentralized applications that leverage the power of blockchain technology to solve real-world problems with transparency and efficiency.
                </p>
                <div class="flex space-x-4">
                    <a href="#projects" class="px-6 py-3 bg-blue-600 hover:bg-blue-700 dark:bg-blue-500 dark:hover:bg-blue-600 text-white rounded-lg font-medium transition">
                        View Projects
                    </a>
                    <a href="#contact" class="px-6 py-3 border border-gray-300 dark:border-gray-700 hover:bg-gray-200 dark:hover:bg-gray-800 rounded-lg font-medium transition">
                        Contact Me
                    </a>
                </div>
            </div>
            <div class="relative float-animation">
                <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/f05185fa-ffa1-4d19-a316-7096235e2781.png" alt="3D illustration of blockchain nodes interconnected with glowing lines and blue-purple gradient background" class="rounded-2xl shadow-xl">
                <div class="absolute -bottom-6 -right-6 bg-yellow-200 dark:bg-purple-700 p-3 rounded-lg shadow-lg transform rotate-3">
                    <div class="font-bold">5+ Years Experience</div>
                    <div class="text-xs">in Blockchain Dev</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="py-16 bg-white dark:bg-gray-800">
        <div class="max-w-6xl mx-auto px-4">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">Blockchain Projects</h2>
                <p class="max-w-2xl mx-auto text-gray-600 dark:text-gray-400">
                    Explore my decentralized applications built with various blockchain technologies
                </p>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Project 1 -->
                <div class="bg-gray-50 dark:bg-gray-700 rounded-xl overflow-hidden shadow-md card-hover transition-all duration-300">
                    <div class="h-48 overflow-hidden">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/e1138a8f-93e9-40b8-9f56-7283a8c44742.png" alt="Dashboard interface of a DeFi application showing liquidity pools and trading charts with dark theme" class="w-full h-full object-cover">
                    </div>
                    <div class="p-6">
                        <div class="flex items-center space-x-2 mb-3">
                            <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/8f674c9d-e025-44bc-99c5-f1038484800a.png" alt="Ethereum logo with classic orange color" class="h-6 w-6">
                            <span class="text-sm font-medium text-gray-600 dark:text-gray-400">Ethereum</span>
                        </div>
                        <h3 class="text-xl font-bold mb-2">DeFi Yield Aggregator</h3>
                        <p class="text-gray-600 dark:text-gray-300 mb-4">
                            A protocol that automatically moves funds between DeFi platforms to maximize yield returns.
                        </p>
                        <div class="flex flex-wrap gap-2">
                            <span class="px-2 py-1 bg-blue-100 dark:bg-blue-900 text-blue-800 dark:text-blue-200 text-xs rounded">Solidity</span>
                            <span class="px-2 py-1 bg-yellow-100 dark:bg-yellow-900 text-yellow-800 dark:text-yellow-200 text-xs rounded">Web3.js</span>
                            <span class="px-2 py-1 bg-red-100 dark:bg-red-900 text-red-800 dark:text-red-200 text-xs rounded">Hardhat</span>
                        </div>
                    </div>
                    <div class="px-6 py-3 border-t border-gray-200 dark:border-gray-600 flex justify-between items-center">
                        <a href="#" class="text-blue-600 dark:text-blue-400 hover:underline text-sm font-medium">View Project</a>
                        <a href="#" class="text-gray-500 hover:text-gray-700 dark:hover:text-gray-300">
                            <i class="fab fa-github"></i>
                        </a>
                    </div>
                </div>
                
                <!-- Project 2 -->
                <div class="bg-gray-50 dark:bg-gray-700 rounded-xl overflow-hidden shadow-md card-hover transition-all duration-300">
                    <div class="h-48 overflow-hidden">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/20b4e325-429d-4bcb-8b09-9a53c1919598.png" alt="NFT marketplace showing digital art gallery with various colored NFT cards" class="w-full h-full object-cover">
                    </div>
                    <div class="p-6">
                        <div class="flex items-center space-x-2 mb-3">
                            <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/f0aff1c4-305f-437b-812b-259cde01802e.png" alt="Polygon logo with purple color gradient" class="h-6 w-6">
                            <span class="text-sm font-medium text-gray-600 dark:text-gray-400">Polygon</span>
                        </div>
                        <h3 class="text-xl font-bold mb-2">NFT Marketplace</h3>
                        <p class="text-gray-600 dark:text-gray-300 mb-4">
                            A gas-efficient NFT platform with lazy minting and batch operations for artists and collectors.
                        </p>
                        <div class="flex flex-wrap gap-2">
                            <span class="px-2 py-1 bg-indigo-100 dark:bg-indigo-900 text-indigo-800 dark:text-indigo-200 text-xs rounded">IPFS</span>
                            <span class="px-2 py-1 bg-green-100 dark:bg-green-900 text-green-800 dark:text-green-200 text-xs rounded">React</span>
                            <span class="px-2 py-1 bg-purple-100 dark:bg-purple-900 text-purple-800 dark:text-purple-200 text-xs rounded">Ethers.js</span>
                        </div>
                    </div>
                    <div class="px-6 py-3 border-t border-gray-200 dark:border-gray-600 flex justify-between items-center">
                        <a href="#" class="text-blue-600 dark:text-blue-400 hover:underline text-sm font-medium">View Project</a>
                        <a href="#" class="text-gray-500 hover:text-gray-700 dark:hover:text-gray-300">
                            <i class="fab fa-github"></i>
                        </a>
                    </div>
                </div>
                
                <!-- Project 3 -->
                <div class="bg-gray-50 dark:bg-gray-700 rounded-xl overflow-hidden shadow-md card-hover transition-all duration-300">
                    <div class="h-48 overflow-hidden">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/c1f2f2e6-64d3-4d9d-863a-c758462c8277.png" alt="Staking interface showing token amounts, rewards calculation and lock periods with modern UI" class="w-full h-full object-cover">
                    </div>
                    <div class="p-6">
                        <div class="flex items-center space-x-2 mb-3">
                            <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/f6832b21-fbce-4165-b38f-2fafc60cd812.png" alt="Solana logo with green gradient" class="h-6 w-6">
                            <span class="text-sm font-medium text-gray-600 dark:text-gray-400">Solana</span>
                        </div>
                        <h3 class="text-xl font-bold mb-2">Token Staking Platform</h3>
                        <p class="text-gray-600 dark:text-gray-300 mb-4">
                            A high-performance staking dApp with flexible lock periods and compounding rewards.
                        </p>
                        <div class="flex flex-wrap gap-2">
                            <span class="px-2 py-1 bg-blue-100 dark:bg-blue-900 text-blue-800 dark:text-blue-200 text-xs rounded">Rust</span>
                            <span class="px-2 py-1 bg-orange-100 dark:bg-orange-900 text-orange-800 dark:text-orange-200 text-xs rounded">Anchor</span>
                            <span class="px-2 py-1 bg-pink-100 dark:bg-pink-900 text-pink-800 dark:text-pink-200 text-xs rounded">Next.js</span>
                        </div>
                    </div>
                    <div class="px-6 py-3 border-t border-gray-200 dark:border-gray-600 flex justify-between items-center">
                        <a href="#" class="text-blue-600 dark:text-blue-400 hover:underline text-sm font-medium">View Project</a>
                        <a href="#" class="text-gray-500 hover:text-gray-700 dark:hover:text-gray-300">
                            <i class="fab fa-github"></i>
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="py-16 bg-gray-50 dark:bg-gray-900">
        <div class="max-w-6xl mx-auto px-4">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">Technical Skills</h2>
                <p class="max-w-2xl mx-auto text-gray-600 dark:text-gray-400">
                    My expertise spans across various blockchain technologies and development tools
                </p>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <div class="space-y-6">
                    <h3 class="text-2xl font-bold text-center">Blockchain Technologies</h3>
                    
                    <!-- Skill 1 -->
                    <div class="skill-item">
                        <div class="flex justify-between mb-1">
                            <span class="font-medium">Solidity</span>
                            <span class="text-sm text-gray-500">95%</span>
                        </div>
                        <div class="w-full bg-gray-200 dark:bg-gray-700 rounded-full h-2.5">
                            <div class="skill-bar bg-blue-600 h-2.5 rounded-full" style="width: 95%"></div>
                        </div>
                    </div>
                    
                    <!-- Skill 2 -->
                    <div class="skill-item">
                        <div class="flex justify-between mb-1">
                            <span class="font-medium">EVM Architecture</span>
                            <span class="text-sm text-gray-500">90%</span>
                        </div>
                        <div class="w-full bg-gray-200 dark:bg-gray-700 rounded-full h-2.5">
                            <div class="skill-bar bg-blue-600 h-2.5 rounded-full" style="width: 90%"></div>
                        </div>
                    </div>
                    
                    <!-- Skill 3 -->
                    <div class="skill-item">
                        <div class="flex justify-between mb-1">
                            <span class="font-medium">Smart Contract Security</span>
                            <span class="text-sm text-gray-500">88%</span>
                        </div>
                        <div class="w-full bg-gray-200 dark:bg-gray-700 rounded-full h-2.5">
                            <div class="skill-bar bg-blue-600 h-2.5 rounded-full" style="width: 88%"></div>
                        </div>
                    </div>
                </div>
                
                <div class="space-y-6">
                    <h3 class="text-2xl font-bold text-center">Development Tools</h3>
                    
                    <!-- Skill 4 -->
                    <div class="skill-item">
                        <div class="flex justify-between mb-1">
                            <span class="font-medium">Hardhat</span>
                            <span class="text-sm text-gray-500">93%</span>
                        </div>
                        <div class="w-full bg-gray-200 dark:bg-gray-700 rounded-full h-2.5">
                            <div class="skill-bar bg-green-600 h-2.5 rounded-full" style="width: 93%"></div>
                        </div>
                    </div>
                    
                    <!-- Skill 5 -->
                    <div class="skill-item">
                        <div class="flex justify-between mb-1">
                            <span class="font-medium">Web3.js/Ethers.js</span>
                            <span class="text-sm text-gray-500">91%</span>
                        </div>
                        <div class="w-full bg-gray-200 dark:bg-gray-700 rounded-full h-2.5">
                            <div class="skill-bar bg-green-600 h-2.5 rounded-full" style="width: 91%"></div>
                        </div>
                    </div>
                    
                    <!-- Skill 6 -->
                    <div class="skill-item">
                        <div class="flex justify-between mb-1">
                            <span class="font-medium">IPFS</span>
                            <span class="text-sm text-gray-500">85%</span>
                        </div>
                        <div class="w-full bg-gray-200 dark:bg-gray-700 rounded-full h-2.5">
                            <div class="skill-bar bg-green-600 h-2.5 rounded-full" style="width: 85%"></div>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="mt-12 grid grid-cols-2 md:grid-cols-4 gap-4 text-center">
                <div class="p-4 bg-white dark:bg-gray-800 rounded-lg shadow-sm">
                    <div class="text-blue-600 dark:text-blue-400 text-3xl mb-2">
                        <i class="fab fa-ethereum"></i>
                    </div>
                    <div class="font-medium">Ethereum</div>
                </div>
                <div class="p-4 bg-white dark:bg-gray-800 rounded-lg shadow-sm">
                    <div class="text-purple-600 dark:text-purple-400 text-3xl mb-2">
                        <i class="fas fa-layer-group"></i>
                    </div>
                    <div class="font-medium">Polygon</div>
                </div>
                <div class="p-4 bg-white dark:bg-gray-800 rounded-lg shadow-sm">
                    <div class="text-green-600 dark:text-green-400 text-3xl mb-2">
                        <i class="fas fa-bolt"></i>
                    </div>
                    <div class="font-medium">Solana</div>
                </div>
                <div class="p-4 bg-white dark:bg-gray-800 rounded-lg shadow-sm">
                    <div class="text-red-600 dark:text-red-400 text-3xl mb-2">
                        <i class="fas fa-link"></i>
                    </div>
                    <div class="font-medium">Chainlink</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-16">
        <div class="max-w-4xl mx-auto px-4">
            <div class="text-center mb-12">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">Get In Touch</h2>
                <p class="max-w-2xl mx-auto text-gray-600 dark:text-gray-400">
                    Have a blockchain project in mind? Let's discuss how I can help bring it to life.
                </p>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <div>
                    <h3 class="text-xl font-bold mb-4">Contact Information</h3>
                    <div class="space-y-4">
                        <div class="flex items-start space-x-4">
                        <div class="text-blue-600 dark:text-blue-400 text-xl mt-1">
                            <i class="fas fa-envelope"></i>
                        </div>
                        <div>
                            <h4 class="font-medium">Email</h4>
                            <p class="text-gray-600 dark:text-gray-400" style="outline: rgb(0, 0, 0) dotted 3px; outline-offset: 1px;">mochfajriramdhani003@gmail.com</p>
                        </div>
                    </div>
                        <div class="flex items-start space-x-4">
                            <div class="text-blue-600 dark:text-blue-400 text-xl mt-1">
                                <i class="fas fa-globe"></i>
                            </div>
                            <div>
                                <h4 class="font-medium">Website</h4>
                                <p class="text-gray-600 dark:text-gray-400">mochfajriramdhani.dev</p>
                            </div>
                        </div>
                        <div class="flex items-start space-x-4">
                            <div class="text-blue-600 dark:text-blue-400 text-xl mt-1">
                                <i class="fab fa-github"></i>
                            </div>
                            <div>
                                <h4 class="font-medium">GitHub</h4>
                                <!-- GitHub link removed as requested -->
                            </div>
                        </div>
                        <div class="flex items-start space-x-4">
                            <div class="text-blue-600 dark:text-blue-400 text-xl mt-1">
                                <i class="fab fa-twitter"></i>
                            </div>
                            <div>
                                <h4 class="font-medium">Twitter</h4>
                                <p class="text-gray-600 dark:text-gray-400">@ramdhani_f80795</p>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div>
                    <form class="space-y-5">
                        <div>
                            <label for="name" class="block text-sm font-medium mb-1">Your Name</label>
                            <input type="text" id="name" class="w-full px-4 py-2 rounded-lg border border-gray-300 dark:border-gray-700 focus:ring-2 focus:ring-blue-500 dark:bg-gray-800 dark:text-white outline-none transition">
                        </div>
                        <div>
                            <label for="email" class="block text-sm font-medium mb-1">Email Address</label>
                            <input type="email" id="email" class="w-full px-4 py-2 rounded-lg border border-gray-300 dark:border-gray-700 focus:ring-2 focus:ring-blue-500 dark:bg-gray-800 dark:text-white outline-none transition">
                        </div>
                        <div>
                            <label for="subject" class="block text-sm font-medium mb-1">Subject</label>
                            <input type="text" id="subject" class="w-full px-4 py-2 rounded-lg border border-gray-300 dark:border-gray-700 focus:ring-2 focus:ring-blue-500 dark:bg-gray-800 dark:text-white outline-none transition">
                        </div>
                        <div>
                            <label for="message" class="block text-sm font-medium mb-1">Message</label>
                            <textarea id="message" rows="4" class="w-full px-4 py-2 rounded-lg border border-gray-300 dark:border-gray-700 focus:ring-2 focus:ring-blue-500 dark:bg-gray-800 dark:text-white outline-none transition"></textarea>
                        </div>
                        <button type="submit" class="w-full bg-blue-600 hover:bg-blue-700 dark:bg-blue-500 dark:hover:bg-blue-600 text-white px-6 py-3 rounded-lg font-medium transition">
                            Send Message
                        </button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="py-8 bg-gray-800 dark:bg-gray-950 text-gray-300">
        <div class="max-w-6xl mx-auto px-4 text-center">
            <div class="flex justify-center space-x-6 mb-6">
                <a href="https://twitter.com/yourprofile" target="_blank" class="text-gray-400 hover:text-white transition">
                    <i class="fab fa-twitter text-xl"></i>
                </a>
                <a href="#" class="text-gray-400 hover:text-white transition">
                    <i class="fab fa-github text-xl"></i>
                </a>
                <a href="#" class="text-gray-400 hover:text-white transition">
                    <i class="fab fa-linkedin-in text-xl"></i>
                </a>
                <a href="#" class="text-gray-400 hover:text-white transition">
                    <i class="fab fa-telegram text-xl"></i>
                </a>
            </div>
            <p>© <script>document.write(new Date().getFullYear())</script> Moch. Fajri Ramdhani. All rights reserved.</p>
        </div>
    </footer>

    <script>
        // Theme toggle functionality
        document.getElementById('theme-toggle').addEventListener('click', function() {
            document.documentElement.classList.toggle('dark');
            const icon = this.querySelector('i');
            if (document.documentElement.classList.contains('dark')) {
                icon.classList.remove('fa-moon');
                icon.classList.add('fa-sun');
                icon.classList.add('text-yellow-300');
                icon.classList.remove('text-gray-800');
            } else {
                icon.classList.remove('fa-sun');
                icon.classList.remove('text-yellow-300');
                icon.classList.add('fa-moon');
                icon.classList.add('text-gray-800');
            }
        });

        // Check for saved theme preference or use color scheme preference
        if (localStorage.getItem('color-theme') === 'dark' || (!localStorage.getItem('color-theme') && window.matchMedia('(prefers-color-scheme: dark)').matches)) {
            document.documentElement.classList.add('dark');
            document.getElementById('theme-toggle').innerHTML = '<i class="fas fa-sun text-yellow-300"></i>';
        } else {
            document.documentElement.classList.remove('dark');
            document.getElementById('theme-toggle').innerHTML = '<i class="fas fa-moon text-gray-800"></i>';
        }

        // Animate skill bars when they come into view
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    const skillBars = entry.target.querySelectorAll('.skill-bar');
                    skillBars.forEach(bar => {
                        // Already has width style from HTML, just trigger transition with a small delay
                        setTimeout(() => {
                            bar.style.transition = 'width 1.5s ease-in-out';
                        }, 200);
                    });
                }
            });
        }, {threshold: 0.1});

        document.querySelectorAll('.skill-item').forEach(item => {
            observer.observe(item);
        });

        // Smooth scrolling for all links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>

