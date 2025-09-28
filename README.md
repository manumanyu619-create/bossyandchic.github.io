<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BOSSY & CHIC - Wear Power. Own Style. | LLM Style Advisor</title>
    
    <!-- Load Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <style>
        /* --- Custom CSS & Font Setup --- */
        
        body {
            font-family: 'Inter', sans-serif;
            background-color: #000;
            color: #fff;
            min-height: 100vh;
        }

        .page-container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 1.5rem;
        }

        /* Define the Gold Color */
        :root {
            --shining-gold: #C5A352;
            --shining-gold-shadow: 0 0 10px rgba(197, 163, 82, 0.7);
        }

        /* --- Global 3D Gold Styling --- */
        
        /* Apply 3D Gold Shadow to the main header border */
        .header-gold-border {
            border-bottom: 2px solid var(--shining-gold); /* Thicker line */
            box-shadow: 0 3px 10px rgba(197, 163, 82, 0.6); /* Sharper shadow */
        }
        
        .logo-text {
            font-size: 2.2rem; /* Slightly larger logo */
            font-weight: 700;
            letter-spacing: 0.3rem;
        }

        /* Product Card Gold Border and Hover Effect */
        .product-card {
            border: 2px solid #1a1a1a; /* Thicker base border */
            transition: all 0.4s;
            box-shadow: 0 0 5px rgba(0, 0, 0, 0.5);
        }
        
        .product-card:hover {
            border-color: var(--shining-gold);
            box-shadow: 0 0 15px rgba(197, 163, 82, 0.9); /* More intense glow */
        }

        /* --- CTA Button Styling (Inverted Gold Look) --- */
        .btn-cta-gold-inverted {
            display: inline-block;
            border: 2px solid var(--shining-gold); /* Thicker border */
            background-color: transparent;
            color: var(--shining-gold);
            padding: 0.75rem 2.2rem;
            font-weight: 600;
            letter-spacing: 0.05em;
            text-transform: uppercase;
            box-shadow: 0 0 10px rgba(197, 163, 82, 0.7); /* Stronger shadow */
            transition: all 0.4s;
        }
        
        .btn-cta-gold-inverted:hover {
            background-color: var(--shining-gold);
            color: #000 !important;
            box-shadow: none; 
        }

        .btn-style-advisor {
            border: 1px solid var(--shining-gold);
            color: var(--shining-gold);
            transition: all 0.3s;
        }
        .btn-style-advisor:hover {
            background-color: var(--shining-gold);
            color: #000;
        }

        /* --- Hero Section Specific Styles --- */
        .hero-section {
            height: 75vh;
            position: relative;
            /* Bottom line of the hero section is shining gold */
            border-bottom: 3px solid var(--shining-gold); /* HD Thickness */
            box-shadow: 0 5px 20px rgba(197, 163, 82, 0.6); /* HD Shadow */
        }

        /* Modal Styles */
        .modal {
            display: none;
            position: fixed;
            z-index: 100;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            overflow: auto;
            background-color: rgba(0,0,0,0.9);
        }

        .modal-content {
            background-color: #111;
            margin: 5% auto;
            padding: 40px;
            border: 3px solid var(--shining-gold);
            width: 90%;
            max-width: 700px;
            box-shadow: var(--shining-gold-shadow);
        }
        
        .close-btn {
            color: var(--shining-gold);
            float: right;
            font-size: 28px;
            font-weight: bold;
            transition: color 0.3s;
        }

        .close-btn:hover,
        .close-btn:focus {
            color: #fff;
            text-decoration: none;
            cursor: pointer;
        }

    </style>
</head>
<body class="font-sans antialiased">
    
    <!-- 1. Header (Sticky) - With Shining Gold Border -->
    <header class="sticky top-0 z-20 bg-black pt-12 pb-5 header-gold-border">
        <div class="page-container flex flex-col items-center">
            <!-- Logo -->
            <a href="#" class="logo-text text-white mb-2 tracking-widest uppercase">BOSSY & CHIC</a>
            
            <!-- Navigation Links - Gold Hover Effect -->
            <nav class="flex justify-center space-x-8 text-xs font-medium tracking-widest uppercase">
                <a href="#about" class="text-white hover:text-shining-gold transition">ABOUT</a>
                <a href="#collection" class="text-white hover:text-shining-gold transition">COLLECTION</a>
                <a href="#contact" class="text-white hover:text-shining-gold transition">CONTACT</a>
                <a href="#" class="text-shining-gold font-bold hover:text-white transition">CART (0)</a>
            </nav>
        </div>
    </header>

    <main>
        
        <!-- 2. Hero Section - With Shining Gold Bottom Line -->
        <section class="hero-section">
            <img src="https://placehold.co/1200x800/111/FFF?text=Fashion+Power+Shot" 
                 alt="Model wearing a tailored black suit" 
                 class="w-full h-full object-cover object-position-center-top opacity-90">
            <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 text-white text-center">
                <h1 class="text-white text-shadow-lg font-extrabold" style="font-size: clamp(2.5rem, 8vw, 4.5rem); letter-spacing: 0.2rem; text-transform: uppercase;">
                    WEAR POWER.<br>OWN STYLE.
                </h1>
            </div>
        </section>
        
        <!-- 3. About & Brand Story Section -->
        <section id="about" class="py-28 border-b border-gray-900">
            <div class="page-container text-center max-w-4xl">
                <h2 class="text-3xl font-semibold uppercase mb-6 tracking-wider" style="color: var(--shining-gold);">The New Standard in Power Dressing</h2>
                <p class="text-lg text-gray-300 mb-10 font-light max-w-2xl mx-auto">
                    We craft tailored pieces that embody strength, precision, and modern luxury. Every seam, every cut, is an intentional statement designed for the woman who sets the agenda.
                </p>
                <a href="#" class="btn-cta-gold-inverted text-sm">DISCOVER OUR PHILOSOPHY</a>
            </div>
        </section>

        <!-- 4. Featured Product Collection Grid (The Clothes and Rates) -->
        <section id="collection" class="py-28">
            <div class="page-container">
                <h2 class="text-center text-3xl font-semibold uppercase mb-16 tracking-wider" style="color: var(--shining-gold);">The Signature Collection</h2>
                
                <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8">
                    
                    <!-- Product 1: The Executive Blazer -->
                    <div class="group product-card">
                        <img src="https://placehold.co/400x500/000/FFF?text=Blazer" alt="Executive Blazer" class="w-full h-auto mb-4 transition duration-300">
                        <div class="text-left p-4">
                            <h3 class="text-sm uppercase tracking-widest font-semibold">The Executive Blazer</h3>
                            <p class="text-xl font-bold mt-1" style="color: var(--shining-gold);">$399.00</p>
                            <button onclick="generateStyleAdvice('The Executive Blazer')" class="btn-style-advisor text-xs py-1 px-3 mt-2 tracking-widest uppercase hover:text-black hover:bg-shining-gold block w-full transition duration-300">
                                ✨ Get Style Advisor
                            </button>
                        </div>
                    </div>

                    <!-- Product 2: The Trouser -->
                    <div class="group product-card">
                        <img src="https://placehold.co/400x500/000/FFF?text=Trouser" alt="Boardroom Trouser" class="w-full h-auto mb-4 transition duration-300">
                        <div class="text-left p-4">
                            <h3 class="text-sm uppercase tracking-widest font-semibold">The Boardroom Trouser</h3>
                            <p class="text-xl font-bold mt-1" style="color: var(--shining-gold);">$189.00</p>
                            <button onclick="generateStyleAdvice('The Boardroom Trouser')" class="btn-style-advisor text-xs py-1 px-3 mt-2 tracking-widest uppercase hover:text-black hover:bg-shining-gold block w-full transition duration-300">
                                ✨ Get Style Advisor
                            </button>
                        </div>
                    </div>
                    
                    <!-- Product 3: The Sheath Dress -->
                    <div class="group product-card">
                        <img src="https://placehold.co/400x500/000/FFF?text=Dress" alt="Manhattan Sheath Dress" class="w-full h-auto mb-4 transition duration-300">
                        <div class="text-left p-4">
                            <h3 class="text-sm uppercase tracking-widest font-semibold">Manhattan Sheath Dress</h3>
                            <p class="text-xl font-bold mt-1" style="color: var(--shining-gold);">$249.00</p>
                            <button onclick="generateStyleAdvice('Manhattan Sheath Dress')" class="btn-style-advisor text-xs py-1 px-3 mt-2 tracking-widest uppercase hover:text-black hover:bg-shining-gold block w-full transition duration-300">
                                ✨ Get Style Advisor
                            </button>
                        </div>
                    </div>

                    <!-- Product 4: The Silk Blouse -->
                    <div class="group product-card">
                        <img src="https://placehold.co/400x500/000/FFF?text=Blouse" alt="Signature Silk Blouse" class="w-full h-auto mb-4 transition duration-300">
                        <div class="text-left p-4">
                            <h3 class="text-sm uppercase tracking-widest font-semibold">Signature Silk Blouse</h3>
                            <p class="text-xl font-bold mt-1" style="color: var(--shining-gold);">$119.00</p>
                            <button onclick="generateStyleAdvice('Signature Silk Blouse')" class="btn-style-advisor text-xs py-1 px-3 mt-2 tracking-widest uppercase hover:text-black hover:bg-shining-gold block w-full transition duration-300">
                                ✨ Get Style Advisor
                            </button>
                        </div>
                    </div>
                </div>

                <div class="text-center mt-20">
                    <a href="#" class="btn-cta-gold-inverted text-base">SHOP ALL NEW ARRIVALS</a>
                </div>
            </div>
        </section>
        
        <!-- 5. Contact / Call-to-Action Banner (Reversed Colors with Gold Accent) -->
        <section id="contact" class="bg-white text-black py-20 border-t border-b border-gray-300">
            <div class="page-container text-center">
                <h2 class="text-3xl font-semibold uppercase mb-3 tracking-wider text-black">DEFINE YOUR NEXT MOVE</h2>
                <p class="text-lg mb-8 max-w-2xl mx-auto text-gray-700">Sign up for our exclusive email list and receive 15% off your first tailored piece.</p>
                
                <div class="flex justify-center max-w-xl mx-auto">
                    <!-- Simple form layout -->
                    <input type="email" placeholder="ENTER YOUR EMAIL ADDRESS" 
                           class="p-4 w-full border border-gray-400 bg-white text-black text-sm uppercase mr-2 focus:ring-0 focus:border-black"
                           style="box-shadow: 0 0 5px rgba(0, 0, 0, 0.2);">
                    <button class="bg-black text-white p-4 text-sm uppercase font-semibold hover:bg-gray-800 transition"
                            style="box-shadow: 0 0 5px rgba(0, 0, 0, 0.4);">
                        SUBSCRIBE
                    </button>
                </div>
            </div>
        </section>

    </main>

    <!-- 6. Footer - Subtle Gold Line -->
    <footer class="py-10 bg-black">
        <div class="page-container text-center text-xs text-gray-400">
            <hr class="mb-4 mx-auto border-t-1 w-24" style="border-color: var(--shining-gold); box-shadow: var(--shining-gold-shadow);">
            <p class="mb-2">&copy; 2025 BOSSY & CHIC. All Rights Reserved. | Designed for Power.</p>
            <p>Privacy Policy | Terms of Service | Shipping & Returns</p>
        </div>
    </footer>

    <!-- LLM Style Advisor Modal -->
    <div id="styleModal" class="modal" onclick="hideModal()">
        <div class="modal-content" onclick="event.stopPropagation()">
            <span class="close-btn" onclick="hideModal()">&times;</span>
            <h2 class="text-2xl font-bold uppercase mb-4" style="color: var(--shining-gold);">
                <span id="modalProductTitle"></span> Styling Advisor
            </h2>
            <div id="modalLoading" class="text-center py-10">
                <svg class="animate-spin h-5 w-5 mr-3 inline text-white" viewBox="0 0 24 24">...</svg>
                <span class="text-lg">Generating personalized styling advice...</span>
            </div>
            <div id="modalContent" class="text-gray-300 text-sm">
                <!-- LLM response will be injected here -->
            </div>
        </div>
    </div>

    <script>
        const apiKey = "";
        const apiUrl = `https://generativelanguage.googleapis.com/v1beta/models/gemini-2.5-flash-preview-05-20:generateContent?key=${apiKey}`;
        
        const modal = document.getElementById('styleModal');
        const modalContent = document.getElementById('modalContent');
        const modalLoading = document.getElementById('modalLoading');
        const modalProductTitle = document.getElementById('modalProductTitle');
        
        /**
         * Converts Markdown text to HTML for display in the modal.
         * Very basic conversion for simple formatting (headings, bold, lists).
         */
        function markdownToHtml(markdown) {
            let html = markdown;
            
            // Convert headings (assuming ## for simplicity)
            html = html.replace(/## (.*)/g, '<h3 class="text-xl font-semibold mt-4 mb-2" style="color:var(--shining-gold)">$1</h3>');
            
            // Convert bold
            html = html.replace(/\*\*(.*?)\*\*/g, '<strong>$1</strong>');
            
            // Convert newlines to paragraphs (basic block handling)
            html = html.replace(/\n\n/g, '</p><p>');
            html = html.replace(/\n/g, '<br>');

            return '<p>' + html + '</p>';
        }

        function showModal() {
            modal.style.display = 'block';
        }

        function hideModal() {
            modal.style.display = 'none';
        }

        /**
         * Robust fetch wrapper with exponential backoff for API calls.
         */
        async function exponentialBackoffFetch(url, options, maxRetries = 5) {
            for (let i = 0; i < maxRetries; i++) {
                try {
                    const response = await fetch(url, options);
                    if (response.ok) {
                        return response;
                    }
                    if (response.status === 429 && i < maxRetries - 1) {
                        const delay = Math.pow(2, i) * 1000 + Math.random() * 1000;
                        await new Promise(resolve => setTimeout(resolve, delay));
                        continue;
                    }
                    throw new Error(`API error: ${response.statusText}`);
                } catch (error) {
                    if (i === maxRetries - 1) throw error;
                    const delay = Math.pow(2, i) * 1000 + Math.random() * 1000;
                    await new Promise(resolve => setTimeout(resolve, delay));
                }
            }
            throw new Error('Fetch failed after multiple retries.');
        }

        /**
         * Calls the Gemini API to generate styling advice for a given product.
         */
        async function generateStyleAdvice(productName) {
            modalProductTitle.textContent = productName;
            modalContent.innerHTML = '';
            modalLoading.style.display = 'block';
            showModal();

            const systemPrompt = `You are a world-class luxury fashion stylist for the high-end brand 'BOSSY & CHIC'. Your goal is to provide concise, sophisticated, and confidence-boosting styling advice for tailored power clothing. Output must be formatted strictly in Markdown. For the suggested item, create three distinct styling looks: 1. Boardroom Look, 2. Power Lunch Look, 3. Evening Gala Look. Use high-end, evocative language.`;
            
            const userQuery = `Provide styling advice for the product: ${productName}.`;

            const payload = {
                contents: [{ parts: [{ text: userQuery }] }],
                systemInstruction: {
                    parts: [{ text: systemPrompt }]
                },
                tools: [{ "google_search": {} }],
            };

            try {
                const response = await exponentialBackoffFetch(apiUrl, {
                    method: 'POST',
                    headers: { 'Content-Type': 'application/json' },
                    body: JSON.stringify(payload)
                });

                const result = await response.json();
                const text = result.candidates?.[0]?.content?.parts?.[0]?.text;
                
                if (text) {
                    modalContent.innerHTML = markdownToHtml(text);
                } else {
                    modalContent.innerHTML = '<p class="text-red-500">Sorry, the Style Advisor could not generate advice for this item right now. Please try again later.</p>';
                    console.error("Gemini response lacked text content.", result);
                }

            } catch (error) {
                modalContent.innerHTML = `<p class="text-red-500">Error connecting to the Style Advisor. Please check your connection or try again. (${error.message})</p>`;
                console.error("API Call failed:", error);
            } finally {
                modalLoading.style.display = 'none';
            }
        }
    </script>

</body>
</html>
