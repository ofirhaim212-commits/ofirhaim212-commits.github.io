# ofirhaim212-commits.github.io
<!DOCTYPE html>
<html lang="he" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>מערכת הנדסית היברידית | יועץ מומחה</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Rubik:wght@300;400;500;700&display=swap" rel="stylesheet">
    <script src="https://cdnjs.cloudflare.com/ajax/libs/marked/9.1.6/marked.min.js"></script>
    <style>
        body {
            font-family: 'Rubik', sans-serif;
            background-color: #0f172a; /* tailwind slate-900 */
            color: #f8fafc; /* tailwind slate-50 */
        }
        
        .glass-panel {
            background: rgba(30, 41, 59, 0.7); /* slate-800 with opacity */
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }

        .neon-glow {
            box-shadow: 0 0 15px rgba(6, 182, 212, 0.5); /* cyan-500 glow */
        }
        
        .neon-text {
            text-shadow: 0 0 10px rgba(6, 182, 212, 0.8);
        }

        /* Custom Scrollbar for Chat */
        #chat-messages::-webkit-scrollbar {
            width: 6px;
        }
        #chat-messages::-webkit-scrollbar-track {
            background: #1e293b; 
        }
        #chat-messages::-webkit-scrollbar-thumb {
            background: #334155; 
            border-radius: 4px;
        }
        #chat-messages::-webkit-scrollbar-thumb:hover {
            background: #475569; 
        }
        
        /* Markdown Styles in Chat */
        .prose p { margin-bottom: 0.5rem; }
        .prose ul { list-style-type: disc; padding-inline-start: 1.25rem; margin-bottom: 0.5rem; }
        .prose strong { font-weight: 700; color: #fff; }
    </style>
</head>
<body class="antialiased min-h-screen flex flex-col relative overflow-x-hidden">

    <!-- Background Decoration -->
    <div class="fixed inset-0 z-0 pointer-events-none opacity-20">
        <div class="absolute top-0 right-0 w-96 h-96 bg-cyan-600 rounded-full mix-blend-multiply filter blur-3xl opacity-50 animate-blob"></div>
        <div class="absolute top-0 left-0 w-96 h-96 bg-blue-600 rounded-full mix-blend-multiply filter blur-3xl opacity-50 animate-blob animation-delay-2000"></div>
    </div>

    <!-- Header -->
    <header class="relative z-10 glass-panel border-b border-slate-700/50 py-4">
        <div class="container mx-auto px-6 flex justify-between items-center">
            <div class="text-2xl font-bold text-transparent bg-clip-text bg-gradient-to-r from-cyan-400 to-blue-500 neon-text">
                הנדסת מערכות 2.0
            </div>
            <nav class="hidden md:flex space-x-reverse space-x-6 text-sm font-medium text-slate-300">
                <a href="#methodology" class="hover:text-cyan-400 transition-colors">המתודולוגיה</a>
                <a href="#lifecycle" class="hover:text-cyan-400 transition-colors">מחזור חיים</a>
                <a href="#cta" class="hover:text-cyan-400 transition-colors">משאבים</a>
                <a href="#contact" class="hover:text-cyan-400 transition-colors">צור קשר</a>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="relative z-10 flex-grow flex items-center py-20">
        <div class="container mx-auto px-6">
            <div class="flex flex-col lg:flex-row items-center gap-12">
                <!-- Text Content -->
                <div class="lg:w-1/2 flex flex-col items-start text-right">
                    <div class="inline-block px-3 py-1 mb-6 rounded-full glass-panel text-cyan-400 text-sm font-semibold border-cyan-500/30">
                        ייעוץ אסטרטגי וניהול פרויקטים
                    </div>
                    <h1 class="text-4xl md:text-5xl lg:text-6xl font-bold leading-tight mb-6">
                        ניהול פרויקטים והנדסת מערכת <br>
                        <span class="text-transparent bg-clip-text bg-gradient-to-r from-cyan-400 to-blue-500">בשילוב AI</span>
                    </h1>
                    <p class="text-lg text-slate-400 mb-8 max-w-xl">
                        הגשר בין משמעת צבאית קפדנית למהירות פיתוח אזרחית. שימוש בבינה מלאכותית כמכפיל כוח משלב הדרישות ועד הייצור.
                    </p>
                    <a href="#contact" class="px-8 py-3 bg-gradient-to-r from-cyan-600 to-blue-600 hover:from-cyan-500 hover:to-blue-500 text-white font-medium rounded-lg shadow-lg hover:shadow-cyan-500/25 transition-all duration-300">
                        התחל עכשיו
                    </a>
                </div>
                
                <!-- Hero Image -->
                <div class="lg:w-1/2 w-full relative">
                    <div class="absolute -inset-1 bg-gradient-to-r from-cyan-500 to-blue-600 rounded-xl blur opacity-30"></div>
                    <img src="gpt-image-2_A_hyper-realistic_cinematic_3D_illustration_of_a_futuristic_Project_Management_W-0.jpg" 
                         alt="Futuristic Project Management Interface" 
                         class="relative rounded-xl shadow-2xl w-full h-auto object-cover border border-slate-700 neon-glow"
                         onerror="this.src='https://placehold.co/800x500/1e293b/06b6d4?text=Project+Management+AI'">
                </div>
            </div>
        </div>
    </section>

    <!-- Methodology Section -->
    <section id="methodology" class="relative z-10 py-20 bg-slate-900/50">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">המתודולוגיה ההיברידית</h2>
                <p class="text-slate-400 max-w-2xl mx-auto">מעבר חכם מסביבה קשיחה לסביבה גמישה, תוך שמירה על בקרת איכות קפדנית.</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8 relative">
                <!-- Connection Line (Desktop) -->
                <div class="hidden md:block absolute top-1/2 left-0 right-0 h-0.5 bg-gradient-to-r from-orange-500/20 via-cyan-500/50 to-blue-500/20 -z-10 transform -translate-y-1/2"></div>

                <!-- Step 1: Military -->
                <div class="glass-panel p-8 rounded-2xl flex flex-col items-center text-center relative">
                    <div class="w-16 h-16 rounded-full bg-orange-900/50 text-orange-400 flex items-center justify-center mb-6 border border-orange-500/30">
                        <svg class="w-8 h-8" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m5.618-4.016A11.955 11.955 0 0112 2.944a11.955 11.955 0 01-8.618 3.04A12.02 12.02 0 003 9c0 5.591 3.824 10.29 9 11.622 5.176-1.332 9-6.03 9-11.622 0-1.042-.133-2.052-.382-3.016z"></path></svg>
                    </div>
                    <h3 class="text-xl font-bold mb-3 text-orange-400">סביבה צבאית</h3>
                    <p class="text-sm text-slate-300">
                        תהליך טורי, קשיח עם אוריינטציה לאפס תקלות. מיקוד בניהול סיכונים הרמטי ועמידה בתקנים מחמירים (MIL-STD).
                    </p>
                </div>

                <!-- Step 2: AI Copilot -->
                <div class="glass-panel p-8 rounded-2xl flex flex-col items-center text-center relative border-cyan-500/50 neon-glow transform md:-translate-y-4">
                    <div class="w-20 h-20 rounded-full bg-cyan-900/50 text-cyan-400 flex items-center justify-center mb-6 border border-cyan-400 shadow-[0_0_15px_rgba(6,182,212,0.5)]">
                        <svg class="w-10 h-10" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M9.75 17L9 20l-1 1h8l-1-1-.75-3M3 13h18M5 17h14a2 2 0 002-2V5a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"></path></svg>
                    </div>
                    <h3 class="text-2xl font-bold mb-3 text-cyan-400">ה-AI כטייס משנה</h3>
                    <p class="text-sm text-slate-300 mb-4">
                        ייעול סקרי תכן. ה-AI מצליב נתונים, מזהה אנומליות ומציף קונפליקטים, בעוד <strong class="text-white">המהנדס מקבל את ההחלטה האסטרטגית</strong>.
                    </p>
                </div>

                <!-- Step 3: Civilian Agile -->
                <div class="glass-panel p-8 rounded-2xl flex flex-col items-center text-center relative">
                    <div class="w-16 h-16 rounded-full bg-blue-900/50 text-blue-400 flex items-center justify-center mb-6 border border-blue-500/30">
                        <svg class="w-8 h-8" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z"></path></svg>
                    </div>
                    <h3 class="text-xl font-bold mb-3 text-blue-400">סביבה אזרחית</h3>
                    <p class="text-sm text-slate-300">
                        פיתוח גמיש (Agile), מהיר ואיטרטיבי. התמקדות באופטימיזציה של החזר השקעה (ROI) וקיצור זמן ההגעה לשוק.
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Lifecycle Phases Section -->
    <section id="lifecycle" class="relative z-10 py-20">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">מחזור חיים הנדסי מועצם AI</h2>
                <p class="text-slate-400 max-w-2xl mx-auto">שילוב כלי בינה מלאכותית בכל שלב בפרויקט להאצת פיתוח ומניעת כשלים.</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
                <!-- Phase 1 -->
                <div class="glass-panel p-6 rounded-2xl border-t-4 border-t-cyan-500 hover:-translate-y-2 transition-transform duration-300">
                    <div class="text-4xl font-black text-slate-700 mb-4 opacity-50">01</div>
                    <h3 class="text-xl font-bold mb-4 text-white">זיהוי צורך והנדסת דרישות</h3>
                    <ul class="text-slate-300 space-y-2 text-sm">
                        <li class="flex items-start gap-2">
                            <svg class="w-5 h-5 text-cyan-400 shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                            ניתוח מכרזים ו-SOW בעזרת LLM
                        </li>
                        <li class="flex items-start gap-2">
                            <svg class="w-5 h-5 text-cyan-400 shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                            חילוץ דרישות אוטומטי (SRD)
                        </li>
                        <li class="flex items-start gap-2">
                            <svg class="w-5 h-5 text-cyan-400 shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                            זיהוי פערים (Gaps) וסתירות לוגיות
                        </li>
                    </ul>
                </div>

                <!-- Phase 2 -->
                <div class="glass-panel p-6 rounded-2xl border-t-4 border-t-blue-500 hover:-translate-y-2 transition-transform duration-300">
                    <div class="text-4xl font-black text-slate-700 mb-4 opacity-50">02</div>
                    <h3 class="text-xl font-bold mb-4 text-white">סקרי תכן וארכיטקטורה</h3>
                    <ul class="text-slate-300 space-y-2 text-sm">
                        <li class="flex items-start gap-2">
                            <svg class="w-5 h-5 text-blue-400 shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                            ייעול סקרי PDR/CDR
                        </li>
                        <li class="flex items-start gap-2">
                            <svg class="w-5 h-5 text-blue-400 shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                            תכן גנרטיבי לחלופות פיזיקליות
                        </li>
                        <li class="flex items-start gap-2">
                            <svg class="w-5 h-5 text-blue-400 shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                            מודלים הנדסיים מונחי AI (MBSE)
                        </li>
                    </ul>
                </div>

                <!-- Phase 3 -->
                <div class="glass-panel p-6 rounded-2xl border-t-4 border-t-indigo-500 hover:-translate-y-2 transition-transform duration-300">
                    <div class="text-4xl font-black text-slate-700 mb-4 opacity-50">03</div>
                    <h3 class="text-xl font-bold mb-4 text-white">פיתוח ואינטגרציה</h3>
                    <ul class="text-slate-300 space-y-2 text-sm">
                        <li class="flex items-start gap-2">
                            <svg class="w-5 h-5 text-indigo-400 shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                            מניעת עיכובים בנתיב הקריטי בזמן אמת
                        </li>
                        <li class="flex items-start gap-2">
                            <svg class="w-5 h-5 text-indigo-400 shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                            בקרת סטטוס חכמה וסנכרון צוותים
                        </li>
                        <li class="flex items-start gap-2">
                            <svg class="w-5 h-5 text-indigo-400 shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                            אוטומציית אימות (V&V) וגזירת בדיקות
                        </li>
                    </ul>
                </div>

                <!-- Phase 4 -->
                <div class="glass-panel p-6 rounded-2xl border-t-4 border-t-purple-500 hover:-translate-y-2 transition-transform duration-300">
                    <div class="text-4xl font-black text-slate-700 mb-4 opacity-50">04</div>
                    <h3 class="text-xl font-bold mb-4 text-white">העברה לייצור ותיקוף</h3>
                    <ul class="text-slate-300 space-y-2 text-sm">
                        <li class="flex items-start gap-2">
                            <svg class="w-5 h-5 text-purple-400 shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                            בקרת תצורה חכמה (Design Freeze)
                        </li>
                        <li class="flex items-start gap-2">
                            <svg class="w-5 h-5 text-purple-400 shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                            זיהוי חוסרי רכיבים טרם ייצור ב-BOM
                        </li>
                        <li class="flex items-start gap-2">
                            <svg class="w-5 h-5 text-purple-400 shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                            בקרת איכות ויזואלית (Vision AI)
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- CTA Section -->
    <section id="cta" class="relative z-10 py-16 bg-slate-900/50">
        <div class="container mx-auto px-6 text-center">
            <div class="max-w-3xl mx-auto glass-panel p-10 rounded-3xl border border-slate-700 shadow-2xl relative overflow-hidden">
                <div class="absolute top-0 right-0 w-64 h-64 bg-cyan-600/10 rounded-full blur-3xl -z-10 transform translate-x-1/2 -translate-y-1/2"></div>
                <h2 class="text-3xl font-bold mb-4">מוכנים לצלול לעומק?</h2>
                <p class="text-slate-300 mb-8 text-lg">
                    הורידו את המצגת המלאה המפרטת את ארבעת שלבי היישום של בינה מלאכותית בהנדסת מערכות וניהול פרויקטים, משלב הדרישות ועד העברה לייצור.
                </p>
                <a href="ניהול פרויקטים והנדסת מערכת בשילוב AI.pdf" target="_blank" class="inline-flex items-center gap-2 px-8 py-4 bg-white text-slate-900 font-bold rounded-lg hover:bg-slate-200 transition-colors shadow-[0_0_20px_rgba(255,255,255,0.3)]">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 10v6m0 0l-3-3m3 3l3-3m2 8H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z"></path></svg>
                    לצפייה במצגת המלאה
                </a>
            </div>
        </div>
    </section>

    <!-- Contact Form Section -->
    <section id="contact" class="relative z-10 py-20">
        <div class="container mx-auto px-6">
            <div class="max-w-2xl mx-auto glass-panel p-8 md:p-12 rounded-3xl border border-slate-700 relative overflow-hidden">
                <div class="text-center mb-10">
                    <h2 class="text-3xl font-bold mb-4 text-white">השארת פרטים</h2>
                    <p class="text-slate-400">תנו לנו לסייע לכם למנף את הפרויקט הבא באמצעות כלים חכמים והכוונה מדויקת.</p>
                </div>
                
                <form class="space-y-6">
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                        <div class="space-y-2">
                            <label for="fullName" class="block text-sm font-medium text-slate-300">שם מלא</label>
                            <input type="text" id="fullName" class="w-full bg-slate-900/80 border border-slate-600 rounded-lg px-4 py-3 text-white focus:outline-none focus:border-cyan-500 focus:ring-1 focus:ring-cyan-500 transition-all" placeholder="הכנס שם מלא" required>
                        </div>
                        <div class="space-y-2">
                            <label for="email" class="block text-sm font-medium text-slate-300">דוא"ל</label>
                            <input type="email" id="email" class="w-full bg-slate-900/80 border border-slate-600 rounded-lg px-4 py-3 text-white focus:outline-none focus:border-cyan-500 focus:ring-1 focus:ring-cyan-500 transition-all" placeholder="you@company.com" required>
                        </div>
                    </div>
                    
                    <div class="space-y-2">
                        <label for="projectPhase" class="block text-sm font-medium text-slate-300">שלב נוכחי בפרויקט</label>
                        <select id="projectPhase" class="w-full bg-slate-900/80 border border-slate-600 rounded-lg px-4 py-3 text-white focus:outline-none focus:border-cyan-500 focus:ring-1 focus:ring-cyan-500 transition-all appearance-none" required>
                            <option value="" disabled selected>בחר שלב בפרויקט...</option>
                            <option value="initiation">שלב א': זיהוי צורך והנדסת דרישות</option>
                            <option value="design">שלב ב': סקרי תכן וארכיטקטורה (PDR/CDR)</option>
                            <option value="execution">שלב ג': פיתוח, ניהול משימות ואינטגרציה</option>
                            <option value="production">שלב ד': העברה לייצור ותיקוף</option>
                        </select>
                    </div>

                    <div class="space-y-2">
                        <label for="challenge" class="block text-sm font-medium text-slate-300">האתגר המרכזי</label>
                        <textarea id="challenge" rows="4" class="w-full bg-slate-900/80 border border-slate-600 rounded-lg px-4 py-3 text-white focus:outline-none focus:border-cyan-500 focus:ring-1 focus:ring-cyan-500 transition-all resize-none" placeholder="תאר את צוואר הבקבוק או האתגר המרכזי שאתה חווה..." required></textarea>
                    </div>

                    <button type="submit" class="w-full py-4 bg-gradient-to-r from-cyan-600 to-blue-600 hover:from-cyan-500 hover:to-blue-500 text-white font-bold rounded-lg shadow-lg hover:shadow-cyan-500/25 transition-all duration-300">
                        שלח פנייה
                    </button>
                </form>
            </div>
        </div>
    </section>

    <!-- Chatbot Widget -->
    <div class="fixed bottom-6 right-6 z-50 flex flex-col items-end">
        <!-- Chat Window -->
        <div id="chat-window" class="hidden w-80 sm:w-96 glass-panel rounded-2xl shadow-2xl border border-cyan-500/30 mb-4 overflow-hidden flex flex-col transition-all duration-300 transform origin-bottom-right" style="height: 500px; max-height: calc(100vh - 120px);">
            <!-- Chat Header -->
            <div class="bg-slate-800/80 p-4 border-b border-slate-700 flex justify-between items-center">
                <div class="flex items-center gap-3">
                    <div class="w-8 h-8 rounded-full bg-gradient-to-r from-cyan-500 to-blue-500 flex items-center justify-center shadow-lg">
                        <svg class="w-5 h-5 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9.75 17L9 20l-1 1h8l-1-1-.75-3M3 13h18M5 17h14a2 2 0 002-2V5a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"></path></svg>
                    </div>
                    <div>
                        <h4 class="font-bold text-sm text-cyan-50">מהנדס מערכת AI</h4>
                        <span class="text-xs text-cyan-400 flex items-center gap-1"><span class="w-1.5 h-1.5 rounded-full bg-cyan-400 animate-pulse"></span> מחובר</span>
                    </div>
                </div>
                <button onclick="toggleChat()" class="text-slate-400 hover:text-white transition-colors">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"></path></svg>
                </button>
            </div>
            
            <!-- Chat Messages -->
            <div id="chat-messages" class="flex-1 p-4 overflow-y-auto flex flex-col gap-4">
                <!-- Initial Message will be injected here -->
            </div>
            
            <!-- Typing Indicator (Hidden by default) -->
            <div id="typing-indicator" class="hidden px-4 pb-2">
                <div class="flex gap-1 items-center bg-slate-800 w-fit p-2 rounded-2xl rounded-br-none border border-slate-700">
                    <div class="w-1.5 h-1.5 bg-cyan-400 rounded-full animate-bounce" style="animation-delay: 0s"></div>
                    <div class="w-1.5 h-1.5 bg-cyan-400 rounded-full animate-bounce" style="animation-delay: 0.2s"></div>
                    <div class="w-1.5 h-1.5 bg-cyan-400 rounded-full animate-bounce" style="animation-delay: 0.4s"></div>
                </div>
            </div>

            <!-- Chat Input -->
            <div class="p-3 bg-slate-800/80 border-t border-slate-700">
                <form id="chat-form" class="flex gap-2 relative">
                    <input type="text" id="chat-input" placeholder="הקלד הודעה..." 
                           class="flex-1 bg-slate-900 text-sm text-white placeholder-slate-400 rounded-full py-2 px-4 border border-slate-600 focus:outline-none focus:border-cyan-500 focus:ring-1 focus:ring-cyan-500 transition-all">
                    <button type="submit" id="send-btn" class="w-10 h-10 rounded-full bg-gradient-to-r from-cyan-600 to-blue-600 flex items-center justify-center text-white hover:shadow-[0_0_10px_rgba(6,182,212,0.5)] transition-all disabled:opacity-50">
                        <svg class="w-5 h-5 transform -rotate-90 ml-1" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 19l9 2-9-18-9 18 9-2zm0 0v-8"></path></svg>
                    </button>
                </form>
            </div>
        </div>

        <!-- Chat Toggle Button -->
        <button onclick="toggleChat()" id="chat-toggle-btn" class="w-14 h-14 rounded-full bg-gradient-to-r from-cyan-600 to-blue-600 text-white shadow-[0_0_20px_rgba(6,182,212,0.4)] flex items-center justify-center hover:scale-110 transition-transform">
            <svg class="w-7 h-7" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 10h.01M12 10h.01M16 10h.01M9 16H5a2 2 0 01-2-2V6a2 2 0 012-2h14a2 2 0 012 2v8a2 2 0 01-2 2h-5l-5 5v-5z"></path></svg>
        </button>
    </div>

    <script>
        // Configuration
        const API_KEY = ""; // Intentionally empty for the environment
        const API_URL = `https://generativelanguage.googleapis.com/v1beta/models/gemini-3-flash-preview:generateContent?key=${API_KEY}`;
        
        const SYSTEM_PROMPT = `You are an Expert AI Systems Engineering Consultant. Speak strict professional Hebrew. Guide engineers using the Hybrid Methodology. Recommend AI tools. Always state that the AI does the data processing while the engineer makes the strategic decisions.`;
        
        const INITIAL_MESSAGE = "שלום. אני יועץ בכיר להנדסת מערכות וניהול פרויקטים. כדי שנוכל להתקדם בצורה מדויקת: מהו השלב הנוכחי בפרויקט שאתה עובד עליו כעת? ומהו צוואר הבקבוק או המשימה המרכזית שאתה מתמודד איתה כרגע?";

        // State
        let isChatOpen = false;
        let chatHistory = [];
        let isWaitingForResponse = false;

        // DOM Elements
        const chatWindow = document.getElementById('chat-window');
        const chatToggleBtn = document.getElementById('chat-toggle-btn');
        const chatMessages = document.getElementById('chat-messages');
        const chatForm = document.getElementById('chat-form');
        const chatInput = document.getElementById('chat-input');
        const sendBtn = document.getElementById('send-btn');
        const typingIndicator = document.getElementById('typing-indicator');

        // Initialize marked.js configuration
        if(typeof marked !== 'undefined') {
            marked.setOptions({
                breaks: true,
                gfm: true
            });
        }

        // Initialize chat
        function initChat() {
            addMessageToUI('model', INITIAL_MESSAGE);
            chatHistory.push({
                role: 'model',
                parts: [{ text: INITIAL_MESSAGE }]
            });
        }

        // Toggle Chat Window
        function toggleChat() {
            isChatOpen = !isChatOpen;
            if (isChatOpen) {
                chatWindow.classList.remove('hidden');
                // Small delay to allow display:block to apply before animation
                setTimeout(() => {
                    chatWindow.style.opacity = '1';
                    chatWindow.style.transform = 'scale(1)';
                    chatInput.focus();
                }, 10);
            } else {
                chatWindow.style.opacity = '0';
                chatWindow.style.transform = 'scale(0.95)';
                setTimeout(() => {
                    chatWindow.classList.add('hidden');
                }, 300);
            }
        }

        // Add message to UI
        function addMessageToUI(role, text) {
            const messageDiv = document.createElement('div');
            messageDiv.classList.add('flex', 'w-full', 'mb-2');
            
            if (role === 'user') {
                messageDiv.classList.add('justify-end');
                messageDiv.innerHTML = `
                    <div class="bg-cyan-600 text-white px-4 py-2 rounded-2xl rounded-bl-none max-w-[85%] text-sm shadow-md">
                        ${escapeHTML(text)}
                    </div>
                `;
            } else {
                messageDiv.classList.add('justify-start');
                
                // Parse Markdown if available, otherwise just escape
                let formattedText = text;
                if(typeof marked !== 'undefined') {
                    formattedText = marked.parse(text);
                } else {
                    formattedText = escapeHTML(text).replace(/\n/g, '<br>');
                }

                messageDiv.innerHTML = `
                    <div class="bg-slate-800 border border-slate-700 text-slate-200 px-4 py-3 rounded-2xl rounded-br-none max-w-[90%] text-sm shadow-md prose prose-invert prose-sm">
                        ${formattedText}
                    </div>
                `;
            }
            
            chatMessages.appendChild(messageDiv);
            scrollToBottom();
        }

        function scrollToBottom() {
            chatMessages.scrollTop = chatMessages.scrollHeight;
        }

        function escapeHTML(str) {
            return str.replace(/[&<>'"]/g, 
                tag => ({
                    '&': '&amp;',
                    '<': '&lt;',
                    '>': '&gt;',
                    "'": '&#39;',
                    '"': '&quot;'
                }[tag] || tag)
            );
        }

        function setTypingStatus(isTyping) {
            isWaitingForResponse = isTyping;
            if (isTyping) {
                typingIndicator.classList.remove('hidden');
                chatInput.disabled = true;
                sendBtn.disabled = true;
                sendBtn.classList.add('opacity-50');
            } else {
                typingIndicator.classList.add('hidden');
                chatInput.disabled = false;
                sendBtn.disabled = false;
                sendBtn.classList.remove('opacity-50');
                chatInput.focus();
            }
            scrollToBottom();
        }

        // Handle Form Submission
        chatForm.addEventListener('submit', async (e) => {
            e.preventDefault();
            if (isWaitingForResponse) return;

            const userText = chatInput.value.trim();
            if (!userText) return;

            // Update UI
            chatInput.value = '';
            addMessageToUI('user', userText);
            
            // Update History
            chatHistory.push({
                role: 'user',
                parts: [{ text: userText }]
            });

            setTypingStatus(true);

            // Call API
            try {
                const payload = {
                    contents: chatHistory,
                    systemInstruction: {
                        parts: [{ text: SYSTEM_PROMPT }]
                    }
                };

                const response = await fetch(API_URL, {
                    method: 'POST',
                    headers: { 'Content-Type': 'application/json' },
                    body: JSON.stringify(payload)
                });

                if (!response.ok) {
                    throw new Error(`HTTP error! status: ${response.status}`);
                }

                const result = await response.json();
                
                if (result.candidates && result.candidates.length > 0 && result.candidates[0].content) {
                    const botResponse = result.candidates[0].content.parts[0].text;
                    
                    // Update History
                    chatHistory.push({
                        role: 'model',
                        parts: [{ text: botResponse }]
                    });
                    
                    // Update UI
                    addMessageToUI('model', botResponse);
                } else {
                    throw new Error("Invalid response structure");
                }

            } catch (error) {
                console.error("Chat API Error:", error);
                addMessageToUI('model', "שגיאה בתקשורת עם השרת. אנא נסה שוב מאוחר יותר.");
                // Remove the last user message from history so they can retry easily if needed
                chatHistory.pop();
            } finally {
                setTypingStatus(false);
            }
        });

        // Start
        window.addEventListener('DOMContentLoaded', initChat);

    </script>
</body>
</html>
