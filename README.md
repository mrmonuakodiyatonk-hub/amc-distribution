<!DOCTYPE html>
<html lang="hi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AMC DISTRIBUTION - कलाकार बनें, न कि क्लर्क</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Configure Tailwind for custom colors (using a vibrant Emerald green/teal accent) -->
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        'accent': '#10b981', // Emerald 500
                        'dark-bg': '#0f172a', // Slate 900
                        'dark-card': '#1e293b', // Slate 800
                    },
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    },
                }
            }
        }
    </script>
    <!-- Inter Font and Custom Styles -->
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@100..900&display=swap');
        body {
            font-family: 'Inter', sans-serif;
            background-color: #0f172a; /* Slate 900 for dark background */
        }
        .hero-background {
            /* Mimicking the dark gradient/texture from the reference site */
            background: linear-gradient(to bottom, #0f172a, #1e293b);
            position: relative;
            overflow: hidden;
        }
        .hero-background::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background-image: radial-gradient(circle at center, rgba(16, 185, 129, 0.1) 0%, transparent 70%); /* Subtle glow effect */
            z-index: 0;
        }
        .nav-link:hover {
            color: #10b981;
            text-shadow: 0 0 8px rgba(16, 185, 129, 0.5);
        }
        .cta-shadow {
            box-shadow: 0 0 20px rgba(16, 185, 129, 0.7);
        }
    </style>
</head>
<body class="text-gray-100">

    <!-- नेविगेशन बार (Navigation Bar) -->
    <header class="sticky top-0 z-50 bg-dark-bg/90 backdrop-blur-sm shadow-xl shadow-slate-900/50">
        <nav class="container mx-auto px-4 sm:px-6 lg:px-8 py-4 flex justify-between items-center">
            <!-- लोगो -->
            <div class="text-3xl font-extrabold text-accent">
                AMC DISTRIBUTION
            </div>
            <!-- डेस्कटॉप लिंक्स -->
            <div class="hidden md:flex space-x-8 text-lg font-medium">
                <a href="#services" class="nav-link transition duration-300">सेवाएं</a>
                <a href="#stores" class="nav-link transition duration-300">स्टोर्स</a>
                <a href="#pricing" class="nav-link transition duration-300">मूल्य निर्धारण</a>
                <button class="bg-accent hover:bg-emerald-600 text-dark-bg font-bold py-2 px-6 rounded-full transition duration-300 shadow-lg">
                    शुरू करें
                </button>
            </div>
            <!-- मोबाइल मेनू बटन -->
            <button class="md:hidden text-gray-200 focus:outline-none" onclick="document.getElementById('mobile-menu').classList.toggle('hidden')">
                <svg class="w-7 h-7" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M4 6h16M4 12h16m-7 6h7"></path></svg>
            </button>
        </nav>
    </header>

    <!-- मोबाइल मेन्यू -->
    <div id="mobile-menu" class="hidden md:hidden bg-dark-card absolute w-full z-40 shadow-2xl">
        <div class="flex flex-col space-y-4 p-5 text-center font-medium">
            <a href="#services" class="py-2 hover:text-accent rounded-lg transition duration-200" onclick="document.getElementById('mobile-menu').classList.add('hidden')">सेवाएं</a>
            <a href="#stores" class="py-2 hover:text-accent rounded-lg transition duration-200" onclick="document.getElementById('mobile-menu').classList.add('hidden')">स्टोर्स</a>
            <a href="#pricing" class="py-2 hover:text-accent rounded-lg transition duration-200" onclick="document.getElementById('mobile-menu').classList.add('hidden')">मूल्य निर्धारण</a>
            <button class="w-full bg-accent hover:bg-emerald-600 text-dark-bg font-bold py-3 rounded-full mt-2 shadow-md">
                शुरू करें
            </button>
        </div>
    </div>

    <main>
        <!-- हीरो सेक्शन (Hero Section) -->
        <section class="hero-background pt-24 pb-32 text-center relative z-10">
            <div class="container mx-auto px-4">
                <h1 class="text-5xl sm:text-7xl font-extrabold mb-6 leading-tight text-white">
                    अपने संगीत को <span class="text-accent">दुनिया भर में</span> रिलीज़ करें
                </h1>
                <p class="text-xl sm:text-2xl text-gray-400 mb-12 max-w-4xl mx-auto font-light">
                    Spotify, Apple Music, YouTube, और 150+ अन्य प्लेटफ़ॉर्म पर सबसे तेज़ और सबसे पारदर्शी तरीके से अपने श्रोताओं तक पहुँचे।
                </p>
                <a href="#pricing" class="inline-block bg-accent hover:bg-emerald-600 text-dark-bg text-xl font-bold py-3 px-10 rounded-full transition duration-500 transform hover:scale-105 cta-shadow">
                    अभी वितरण शुरू करें
                </a>
            </div>
        </section>

        <!-- मुख्य विशेषताएँ / क्यों चुनें (Why Choose Us) -->
        <section id="services" class="py-16 sm:py-24 bg-dark-card/50">
            <div class="container mx-auto px-4">
                <h2 class="text-4xl font-bold text-center mb-16 text-white">हम क्यों सर्वश्रेष्ठ हैं?</h2>
                
                <div class="grid grid-cols-1 md:grid-cols-3 gap-8 md:gap-12 max-w-6xl mx-auto">
                    
                    <!-- फीचर कार्ड 1: रॉयल्टी -->
                    <div class="bg-dark-card p-8 rounded-xl shadow-2xl border-t-4 border-accent transition duration-500 hover:shadow-accent/30">
                        <div class="text-accent mb-4">
                             <!-- Emoji Icon: Money Bag -->
                            <span class="text-5xl">💰</span>
                        </div>
                        <h3 class="text-2xl font-semibold mb-3 text-white">100% रॉयल्टी का विकल्प</h3>
                        <p class="text-gray-400">आपकी मेहनत की कमाई पूरी तरह से आपकी हो सकती है। प्रो योजना में 100% रॉयल्टी रखें।</p>
                    </div>

                    <!-- फीचर कार्ड 2: वितरण गति -->
                    <div class="bg-dark-card p-8 rounded-xl shadow-2xl border-t-4 border-accent transition duration-500 hover:shadow-accent/30">
                        <div class="text-accent mb-4">
                            <!-- Emoji Icon: Rocket -->
                            <span class="text-5xl">🚀</span>
                        </div>
                        <h3 class="text-2xl font-semibold mb-3 text-white">सबसे तेज़ वितरण</h3>
                        <p class="text-gray-400">आपके ट्रैक को 24-48 घंटों के भीतर प्रमुख स्टोर पर लाइव करें। रिलीज़ डेट का नियंत्रण आपके हाथों में।</p>
                    </div>

                    <!-- फीचर कार्ड 3: समर्थन और विश्लेषण -->
                    <div class="bg-dark-card p-8 rounded-xl shadow-2xl border-t-4 border-accent transition duration-500 hover:shadow-accent/30">
                        <div class="text-accent mb-4">
                            <!-- Emoji Icon: Bar Chart -->
                            <span class="text-5xl">📈</span>
                        </div>
                        <h3 class="text-2xl font-semibold mb-3 text-white">विस्तृत विश्लेषण</h3>
                        <p class="text-gray-400">आपकी श्रोताओं कहाँ हैं? सटीक डेटा और विस्तृत प्रदर्शन रिपोर्ट के साथ अपने करियर को ट्रैक करें।</p>
                    </div>

                </div>
            </div>
        </section>

        <!-- स्टोर सेक्शन (Stores Section) -->
        <section id="stores" class="py-16 sm:py-24 bg-dark-bg">
            <div class="container mx-auto px-4 text-center">
                <h2 class="text-4xl font-bold mb-6 text-white">सभी प्रमुख डिजिटल स्टोर पर पहुँचें</h2>
                <p class="text-xl text-gray-400 mb-12 max-w-3xl mx-auto">
                    हम आपके संगीत को उन सभी स्थानों पर पहुंचाते हैं जहाँ आपके श्रोता हैं, दुनिया भर में 150+ से अधिक स्टोर।
                </p>

                <!-- स्टोर लोगो ग्रिड (Mockup using placehold.co and Tailwind classes) -->
                <div class="grid grid-cols-3 md:grid-cols-6 gap-6 opacity-80 max-w-5xl mx-auto">
                    <!-- Spotify -->
                    <div class="bg-white/10 p-4 rounded-lg flex justify-center items-center h-20 hover:scale-105 transition duration-300">
                        <img src="https://placehold.co/100x30/1DB954/white?text=Spotify" alt="Spotify Logo" class="h-6 w-auto" onerror="this.onerror=null; this.src='https://placehold.co/100x30/1DB954/white?text=Spotify';" />
                    </div>
                    <!-- Apple Music -->
                    <div class="bg-white/10 p-4 rounded-lg flex justify-center items-center h-20 hover:scale-105 transition duration-300">
                        <img src="https://placehold.co/100x30/FC3C44/white?text=Apple+Music" alt="Apple Music Logo" class="h-6 w-auto" onerror="this.onerror=null; this.src='https://placehold.co/100x30/FC3C44/white?text=Apple+Music';" />
                    </div>
                    <!-- JioSaavn -->
                    <div class="bg-white/10 p-4 rounded-lg flex justify-center items-center h-20 hover:scale-105 transition duration-300">
                        <img src="https://placehold.co/100x30/000000/FDC51A?text=JioSaavn" alt="JioSaavn Logo" class="h-6 w-auto" onerror="this.onerror=null; this.src='https://placehold.co/100x30/000000/FDC51A?text=JioSaavn';" />
                    </div>
                    <!-- YouTube Music -->
                    <div class="bg-white/10 p-4 rounded-lg flex justify-center items-center h-20 hover:scale-105 transition duration-300">
                        <img src="https://placehold.co/100x30/FF0000/white?text=YouTube+Music" alt="YouTube Music Logo" class="h-6 w-auto" onerror="this.onerror=null; this.src='https://placehold.co/100x30/FF0000/white?text=YouTube+Music';" />
                    </div>
                    <!-- Amazon Music -->
                    <div class="bg-white/10 p-4 rounded-lg flex justify-center items-center h-20 hover:scale-105 transition duration-300">
                        <img src="https://placehold.co/100x30/232F3E/white?text=Amazon" alt="Amazon Music Logo" class="h-6 w-auto" onerror="this.onerror=null; this.src='https://placehold.co/100x30/232F3E/white?text=Amazon';" />
                    </div>
                    <!-- Gaana -->
                    <div class="bg-white/10 p-4 rounded-lg flex justify-center items-center h-20 hover:scale-105 transition duration-300">
                        <img src="https://placehold.co/100x30/009688/white?text=Gaana" alt="Gaana Logo" class="h-6 w-auto" onerror="this.onerror=null; this.src='https://placehold.co/100x30/009688/white?text=Gaana';" />
                    </div>
                </div>
            </div>
        </section>


        <!-- मूल्य निर्धारण सेक्शन (Pricing Section) -->
        <section id="pricing" class="py-16 sm:py-24 bg-dark-card/50">
            <div class="container mx-auto px-4">
                <h2 class="text-4xl font-bold text-center mb-6 text-white">सरल और पारदर्शी मूल्य निर्धारण</h2>
                <p class="text-xl text-gray-400 text-center mb-16">
                    अपनी ज़रूरत के हिसाब से योजना चुनें। दोनों ही मुफ़्त हैं!
                </p>

                <div class="flex flex-col lg:flex-row justify-center items-stretch gap-8 max-w-5xl mx-auto">
                    
                    <!-- प्लान 1: मुफ़्त (Free) -->
                    <div class="w-full lg:w-1/2 bg-dark-card p-8 rounded-xl shadow-2xl border-t-4 border-gray-600 flex flex-col justify-between transform hover:scale-[1.02] transition duration-500">
                        <div>
                            <h3 class="text-3xl font-bold mb-4 text-white">बुनियादी मुफ़्त योजना</h3>
                            <p class="text-5xl font-extrabold mb-6 text-accent">
                                ₹0
                                <span class="text-lg font-normal text-gray-400">/ प्रति वर्ष</span>
                            </p>
                            <p class="text-gray-400 mb-6">उन कलाकारों के लिए जो अभी शुरुआत कर रहे हैं।</p>
                            <ul class="space-y-4 mb-8 text-gray-300">
                                <li class="flex items-start"><span class="text-accent text-2xl mr-3 leading-none">✓</span> <span class="pt-1">असीमित रिलीज़</span></li>
                                <li class="flex items-start"><span class="text-accent text-2xl mr-3 leading-none">✓</span> <span class="pt-1">80% रॉयल्टी रखें (20% कमीशन)</span></li>
                                <li class="flex items-start"><span class="text-accent text-2xl mr-3 leading-none">✓</span> <span class="pt-1">सभी प्रमुख स्टोर पर वितरण</span></li>
                                <li class="flex items-start"><span class="text-red-400 text-2xl mr-3 leading-none">✗</span> <span class="pt-1">YouTube Content ID</span></li>
                            </ul>
                        </div>
                        <button class="w-full bg-gray-600 hover:bg-gray-700 text-white font-bold py-3 rounded-full transition duration-300 mt-4">
                            मुफ़्त में साइन अप करें
                        </button>
                    </div>

                    <!-- प्लान 2: प्रो (Pro) - अब यह भी मुफ़्त है, लेकिन 100% रॉयल्टी के साथ -->
                    <div class="w-full lg:w-1/2 bg-dark-card p-8 rounded-xl shadow-2xl border-t-4 border-accent flex flex-col justify-between transform lg:scale-105 hover:scale-[1.07] transition duration-500 relative">
                        <span class="absolute top-0 right-0 -mt-3 -mr-3 bg-accent text-dark-bg text-sm font-bold py-1 px-4 rounded-full uppercase shadow-xl">लोकप्रिय</span>
                        <div>
                            <h3 class="text-3xl font-bold mb-4 text-accent">प्रो मुफ़्त योजना</h3>
                            <p class="text-5xl font-extrabold mb-6 text-white">
                                ₹0
                                <span class="text-lg font-normal text-gray-400">/ हमेशा के लिए*</span>
                            </p>
                            <p class="text-gray-400 mb-6">पेशेवर कलाकारों के लिए जो अपनी 100% कमाई चाहते हैं।</p>
                            <ul class="space-y-4 mb-8 text-gray-300">
                                <li class="flex items-start"><span class="text-accent text-2xl mr-3 leading-none">✓</span> <span class="pt-1">असीमित रिलीज़</span></li>
                                <li class="flex items-start"><span class="text-accent text-2xl mr-3 leading-none">✓</span> <span class="pt-1">*100% रॉयल्टी रखें (जीरो कमीशन)*</span></li>
                                <li class="flex items-start"><span class="text-accent text-2xl mr-3 leading-none">✓</span> <span class="pt-1">YouTube Content ID शामिल</span></li>
                                <li class="flex items-start"><span class="text-accent text-2xl mr-3 leading-none">✓</span> <span class="pt-1">प्राथमिकता वाला सपोर्ट</span></li>
                            </ul>
                            <p class="text-xs text-gray-500 italic">*100% रॉयल्टी पाने के लिए एक बार छोटा सा सेटअप शुल्क लागू हो सकता है।</p>
                        </div>
                        <button class="w-full bg-accent hover:bg-emerald-600 text-dark-bg font-bold text-lg py-3 rounded-full transition duration-300 mt-4 shadow-xl cta-shadow">
                            प्रो में अपग्रेड करें
                        </button>
                    </div>

                </div>
            </div>
        </section>

        <!-- अंतिम CTA (Final Call to Action) -->
        <section class="py-16 bg-dark-bg border-t border-accent/20">
            <div class="container mx-auto px-4 text-center">
                <h2 class="text-3xl sm:text-4xl font-bold mb-4 text-white">आपका करियर इंतज़ार कर रहा है।</h2>
                <p class="text-xl text-gray-400 mb-8">अपने संगीत को दुनिया भर में तुरंत रिलीज़ करें।</p>
                <a href="#pricing" class="inline-block bg-accent hover:bg-emerald-600 text-dark-bg text-xl font-bold py-3 px-10 rounded-full transition duration-300 transform hover:scale-105 shadow-2xl cta-shadow">
                    आज ही जुड़ें
                </a>
            </div>
        </section>

    </main>

    <!-- फ़ूटर (Footer) -->
    <footer class="bg-dark-bg/80 py-12 border-t border-gray-700">
        <div class="container mx-auto px-4 grid grid-cols-2 md:grid-cols-4 gap-8 text-sm">
            
            <!-- कॉलम 1: लोगो और विवरण -->
            <div>
                <h3 class="text-2xl font-extrabold text-accent mb-4">AMC DISTRIBUTION</h3>
                <p class="text-gray-400">संगीत का वितरण, सरल बनाया गया।</p>
            </div>

            <!-- कॉलम 2: कंपनी -->
            <div>
                <h4 class="font-bold text-lg mb-4 text-white">कंपनी</h4>
                <ul class="space-y-2">
                    <li><a href="#" class="text-gray-400 hover:text-accent transition duration-200">हमारे बारे में</a></li>
                    <li><a href="#" class="text-gray-400 hover:text-accent transition duration-200">संपर्क</a></li>
                    <li><a href="#" class="text-gray-400 hover:text-accent transition duration-200">प्रेस</a></li>
                </ul>
            </div>

            <!-- कॉलम 3: कानूनी -->
            <div>
                <h4 class="font-bold text-lg mb-4 text-white">कानूनी</h4>
                <ul class="space-y-2">
                    <li><a href="#" class="text-gray-400 hover:text-accent transition duration-200">सेवा की शर्तें</a></li>
                    <li><a href="#" class="text-gray-400 hover:text-accent transition duration-200">गोपनीयता नीति</a></li>
                    <li><a href="#" class="text-gray-400 hover:text-accent transition duration-200">रॉयल्टी नियम</a></li>
                </ul>
            </div>

            <!-- कॉलम 4: संसाधन -->
            <div>
                <h4 class="font-bold text-lg mb-4 text-white">संसाधन</h4>
                <ul class="space-y-2">
                    <li><a href="#" class="text-gray-400 hover:text-accent transition duration-200">ब्लॉग</a></li>
                    <li><a href="#" class="text-gray-400 hover:text-accent transition duration-200">सहायता केंद्र</a></li>
                    <li><a href="#" class="text-gray-400 hover:text-accent transition duration-200">FAQs</a></li>
                </ul>
            </div>
        </div>

        <!-- कॉपीराइट -->
        <div class="mt-10 pt-6 border-t border-gray-800 text-center text-gray-500 text-sm">
            &copy; <span id="current-year"></span> AMC DISTRIBUTION। सर्वाधिकार सुरक्षित।
        </div>
    </footer>

    <!-- JavaScript to update current year -->
    <script>
        document.getElementById('current-year').textContent = new Date().getFullYear();
    </script>

</body>
</html>
