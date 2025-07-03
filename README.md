<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your GitHub Profile README</title>
    <!-- Tailwind CSS CDN - GitHub's rendering might be limited, but this provides basic styling -->
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        /* Custom styles to enhance the coffee aesthetic and animations */
        /* Note: External font imports like @import url(...) are generally not supported in GitHub READMEs. */

        body {
            font-family: sans-serif; /* Fallback to a common sans-serif font */
            background-color: #2D2D2D; /* Dark charcoal for contrast */
            color: #E0DCD4; /* Creamy off-white */
        }

        .coffee-gradient-bg {
            background: linear-gradient(135deg, #4A2B1D, #6F4E37, #C69A77); /* Deep brown to lighter coffee */
        }

        .coffee-text {
            color: #C69A77; /* Lighter coffee tone for highlights */
        }

        /* Coffee bean float animation - pure CSS, might work */
        .coffee-bean {
            animation: float 6s ease-in-out infinite;
            position: absolute;
            opacity: 0.7;
            filter: blur(0.5px);
        }

        .bean-1 { top: 10%; left: 5%; animation-delay: 0s; transform: scale(0.8); }
        .bean-2 { top: 30%; right: 10%; animation-delay: 1.5s; transform: scale(1.1); }
        .bean-3 { bottom: 20%; left: 15%; animation-delay: 3s; transform: scale(0.9); }
        .bean-4 { top: 50%; left: 30%; animation-delay: 4.5s; transform: scale(1.2); }
        .bean-5 { bottom: 10%; right: 5%; animation-delay: 2s; transform: scale(0.7); }

        @keyframes float {
            0% { transform: translateY(0) rotate(0deg); }
            50% { transform: translateY(-10px) rotate(5deg); }
            100% { transform: translateY(0) rotate(0deg); }
        }

        /* Subtle pulsating effect for social icons on hover - pure CSS, might work */
        .social-icon:hover {
            animation: pulse 1s infinite;
        }

        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.1); }
            100% { transform: scale(1); }
        }

        /* Background texture for the main content area */
        .content-bg {
            background-color: #3F3F3F; /* Slightly lighter dark gray */
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.3);
        }

        /* Card-like effect for sections */
        .section-card {
            background-color: #4A4A4A; /* Even lighter gray for sections */
            border-radius: 12px;
            padding: 1.5rem;
            margin-bottom: 1.5rem;
            box-shadow: 0 2px 8px rgba(0, 0, 0, 0.2);
        }

        /* Adjustments for headings */
        h1, h2, h3 {
            /* Using a generic serif font as external fonts are not supported */
            font-family: serif;
            color: #C69A77; /* Coffee tone for headings */
        }
    </style>
</head>
<body class="p-4 sm:p-6 md:p-8">
    <div class="max-w-4xl mx-auto rounded-xl overflow-hidden content-bg">
        <!-- Header Banner with Coffee Aesthetic and Animation -->
        <header class="relative coffee-gradient-bg text-white p-8 sm:p-10 text-center rounded-t-xl overflow-hidden">
            <!-- Floating Coffee Beans -->
            <div class="coffee-bean bean-1 text-4xl transform -rotate-12">☕</div>
            <div class="coffee-bean bean-2 text-5xl transform rotate-6">☕</div>
            <div class="coffee-bean bean-3 text-3xl transform rotate-18">☕</div>
            <div class="coffee-bean bean-4 text-6xl transform -rotate-8">☕</div>
            <div class="coffee-bean bean-5 text-4xl transform rotate-20">☕</div>

            <h1 class="text-4xl sm:text-5xl md:text-6xl font-bold mb-2 leading-tight relative z-10">
                Brewing Something <span class="coffee-text">Great</span>!
            </h1>
            <p class="text-lg sm:text-xl relative z-10">
                A coffee-fueled developer, constantly learning & growing.
            </p>
        </header>

        <!-- Main Content Area -->
        <main class="p-6 sm:p-8 md:p-10">
            <!-- About Me Section -->
            <section class="section-card">
                <h2 class="text-2xl sm:text-3xl font-semibold mb-4 border-b-2 border-coffee-text pb-2">
                    <span class="coffee-text">☕</span> About Me
                </h2>
                <p class="text-base sm:text-lg mb-4">
                    Hey there! I'm <strong class="coffee-text">Your Name</strong>, a passionate [Your Profession/Role, e.g., Software Developer, UX Designer, Data Scientist] always eager to sip on new challenges and stir up innovative solutions.
                </p>
                <p class="text-base sm:text-lg">
                    When I'm not coding, you can usually find me brewing a fresh cup of coffee, exploring new coffee shops, or just enjoying the aroma of a well-crafted espresso. I believe in continuous learning, just like a perfect brew requires precision and dedication!
                </p>
            </section>

            <!-- Skills Section -->
            <section class="section-card">
                <h2 class="text-2xl sm:text-3xl font-semibold mb-4 border-b-2 border-coffee-text pb-2">
                    <span class="coffee-text">💡</span> My Skillset (Freshly Roasted)
                </h2>
                <div class="flex flex-wrap gap-3">
                    <span class="bg-gradient-to-r from-orange-600 to-amber-500 text-white px-4 py-1 rounded-full text-sm font-medium shadow-md">JavaScript</span>
                    <span class="bg-gradient-to-r from-blue-600 to-cyan-500 text-white px-4 py-1 rounded-full text-sm font-medium shadow-md">React</span>
                    <span class="bg-gradient-to-r from-green-600 to-emerald-500 text-white px-4 py-1 rounded-full text-sm font-medium shadow-md">Node.js</span>
                    <span class="bg-gradient-to-r from-purple-600 to-fuchsia-500 text-white px-4 py-1 rounded-full text-sm font-medium shadow-md">Python</span>
                    <span class="bg-gradient-to-r from-gray-700 to-gray-500 text-white px-4 py-1 rounded-full text-sm font-medium shadow-md">Git</span>
                    <span class="bg-gradient-to-r from-red-600 to-pink-500 text-white px-4 py-1 rounded-full text-sm font-medium shadow-md">HTML & CSS</span>
                    <!-- Add more skills as needed -->
                </div>
            </section>

            <!-- Projects Section -->
            <section class="section-card">
                <h2 class="text-2xl sm:text-3xl font-semibold mb-4 border-b-2 border-coffee-text pb-2">
                    <span class="coffee-text">🚀</span> Projects (My Latest Brews)
                </h2>
                <div class="grid grid-cols-1 sm:grid-cols-2 gap-6">
                    <div class="bg-gray-600 p-4 rounded-lg shadow-md hover:scale-105 transition-transform duration-300">
                        <h3 class="text-xl font-semibold mb-2 coffee-text">Project A</h3>
                        <p class="text-sm text-gray-300 mb-2">A fantastic project using [Technologies].</p>
                        <a href="https://github.com/yourusername/project-a" target="_blank" class="text-blue-400 hover:underline">View on GitHub &rarr;</a>
                    </div>
                    <div class="bg-gray-600 p-4 rounded-lg shadow-md hover:scale-105 transition-transform duration-300">
                        <h3 class="text-xl font-semibold mb-2 coffee-text">Project B</h3>
                        <p class="text-sm text-gray-300 mb-2">My second amazing creation, built with [Technologies].</p>
                        <a href="https://github.com/yourusername/project-b" target="_blank" class="text-blue-400 hover:underline">View on GitHub &rarr;</a>
                    </div>
                    <!-- Add more projects as needed -->
                </div>
            </section>

            <!-- Connect Section -->
            <section class="section-card">
                <h2 class="text-2xl sm:text-3xl font-semibold mb-4 border-b-2 border-coffee-text pb-2">
                    <span class="coffee-text">🔗</span> Let's Connect! (Grab a Coffee?)
                </h2>
                <div class="flex flex-wrap justify-center gap-6">
                    <a href="https://linkedin.com/in/yourprofile" target="_blank" class="social-icon text-4xl text-blue-500 hover:text-blue-400 transition-colors duration-300" title="LinkedIn">
                        <!-- LinkedIn SVG Icon -->
                        <svg viewBox="0 0 24 24" width="1em" height="1em" stroke="currentColor" stroke-width="2" fill="none" stroke-linecap="round" stroke-linejoin="round" class="w-10 h-10">
                            <path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"></path>
                            <rect x="2" y="9" width="4" height="12"></rect>
                            <circle cx="4" cy="4" r="2"></circle>
                        </svg>
                    </a>
                    <a href="https://twitter.com/yourhandle" target="_blank" class="social-icon text-4xl text-blue-400 hover:text-blue-300 transition-colors duration-300" title="Twitter">
                        <!-- Twitter SVG Icon -->
                        <svg viewBox="0 0 24 24" width="1em" height="1em" stroke="currentColor" stroke-width="2" fill="none" stroke-linecap="round" stroke-linejoin="round" class="w-10 h-10">
                            <path d="M23 3a10.9 10.9 0 0 1-3.14 1.53 4.48 4.48 0 0 0-7.86 3v1A10.66 10.66 0 0 1 3 4s-4 9 5 13a11.64 11.64 0 0 1-7 2c9 5 20 0 20-11.5a4.5 4.5 0 0 0-.08-.83A7.72 7.72 0 0 0 23 3z"></path>
                        </svg>
                    </a>
                    <a href="mailto:your.email@example.com" class="social-icon text-4xl text-red-500 hover:text-red-400 transition-colors duration-300" title="Email">
                        <!-- Email SVG Icon -->
                        <svg viewBox="0 0 24 24" width="1em" height="1em" stroke="currentColor" stroke-width="2" fill="none" stroke-linecap="round" stroke-linejoin="round" class="w-10 h-10">
                            <path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"></path>
                            <polyline points="22,6 12,13 2,6"></polyline>
                        </svg>
                    </a>
                    <a href="https://github.com/yourusername" target="_blank" class="social-icon text-4xl text-gray-300 hover:text-white transition-colors duration-300" title="GitHub">
                        <!-- GitHub SVG Icon -->
                        <svg viewBox="0 0 24 24" width="1em" height="1em" stroke="currentColor" stroke-width="2" fill="none" stroke-linecap="round" stroke-linejoin="round" class="w-10 h-10">
                            <path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 3 8.38 8.38 0 0 0 12 2a8.38 8.38 0 0 0-7.91 1 5.07 5.07 0 0 0-.09 1.77A5.44 5.44 0 0 0 2 10.77c0 5.46 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path>
                        </svg>
                    </a>
                </div>
            </section>
        </main>

        <!-- Footer -->
        <footer class="p-6 sm:p-8 text-center text-sm text-gray-400 rounded-b-xl border-t border-gray-700">
            <p>Crafted with ☕ and ✨ by Your Name</p>
        </footer>
    </div>
</body>
</html>
