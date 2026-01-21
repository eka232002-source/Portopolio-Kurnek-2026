<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portofolio | Kurnia Eka Apsari</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@600;700&family=Inter:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        :root {
            --bg-color: #ffffff;
            --text-color: #1f2937;
            --accent-color: #6366f1;
            --glass-bg: rgba(255, 255, 255, 0.7);
        }
        .dark {
            --bg-color: #0f172a;
            --text-color: #f1f5f9;
            --accent-color: #818cf8;
            --glass-bg: rgba(15, 23, 42, 0.7);
        }
        body {
            background-color: var(--bg-color);
            color: var(--text-color);
            font-family: 'Inter', sans-serif;
            transition: background-color 0.5s ease, color 0.5s ease;
            overflow-x: hidden;
        }
        .cursive {
            font-family: 'Dancing Script', cursive;
        }
        .animate-float {
            animation: float 3s ease-in-out infinite;
        }
        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-15px); }
        }
        .fade-in {
            opacity: 0;
            transform: translateY(20px);
            transition: all 0.8s ease-out;
        }
        .fade-in.visible {
            opacity: 1;
            transform: translateY(0);
        }
        .theme-toggle {
            position: fixed;
            right: 20px;
            top: 50%;
            transform: translateY(-50%);
            z-index: 100;
        }
        .glass {
            background: var(--glass-bg);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        /* Custom color for Cum Laude badge in Dark/Light */
        .cum-laude {
            background-color: #fef3c7;
            color: #92400e;
        }
        .dark .cum-laude {
            background-color: #92400e;
            color: #fef3c7;
        }
    </style>
</head>
<body>

    <!-- Mode Toggle (Sisi Kanan) -->
    <div class="theme-toggle">
        <button onclick="toggleTheme()" class="p-4 rounded-full shadow-2xl bg-indigo-600 text-white hover:scale-110 transition flex flex-col items-center gap-2">
            <i id="theme-icon" class="fas fa-moon"></i>
            <span class="text-[10px] uppercase font-bold tracking-widest" style="writing-mode: vertical-rl;">TEMA</span>
        </button>
    </div>

    <!-- Header / Hero Section -->
    <section class="min-h-screen flex items-center justify-center px-6 relative">
        <div class="container mx-auto flex flex-col md:flex-row items-center gap-12">
            <div class="md:w-1/2 text-center md:text-left order-2 md:order-1 fade-in">
                <h2 class="text-indigo-500 font-semibold tracking-widest uppercase mb-2">Sarjana Ilmu Komunikasi</h2>
                <h1 class="text-5xl md:text-7xl font-bold mb-4 cursive">Kurnia Eka Apsari</h1>
                <p class="text-lg opacity-80 mb-8 max-w-lg leading-relaxed">
                    Disiplin, rajin, dan berkomitmen memberikan pelayanan prima. Berpengalaman dalam administrasi publik dan konten digital berbasis AI.
                </p>
                <div class="flex flex-wrap justify-center md:justify-start gap-4">
                    <a href="https://Wa.me/6285932551750" target="_blank" class="px-8 py-3 bg-green-500 text-white rounded-full hover:shadow-xl hover:scale-105 transition flex items-center gap-2">
                        <i class="fab fa-whatsapp"></i> Hubungi WA
                    </a>
                    <a href="#experience" class="px-8 py-3 border border-indigo-500 rounded-full hover:bg-indigo-500 hover:text-white transition">Lihat Pengalaman</a>
                </div>
            </div>
            <div class="md:w-1/2 flex justify-center order-1 md:order-2">
                <div class="relative animate-float">
                    <div class="absolute -inset-4 bg-indigo-500/20 rounded-full blur-2xl"></div>
                    <!-- Foto Persegi Kurnia -->
                    <img src="https://i.postimg.cc/3yMXRSX6/3y-MXRSX6.jpg" alt="Kurnia Eka Apsari" class="relative w-64 h-64 md:w-80 md:h-80 object-cover rounded-3xl shadow-2xl border-4 border-white/20">
                </div>
            </div>
        </div>
    </section>

    <!-- About Me Section -->
    <section id="about" class="py-24 px-6 bg-slate-50/50 dark:bg-slate-900/50">
        <div class="container mx-auto max-w-4xl text-center fade-in">
            <h2 class="text-4xl font-bold mb-10 cursive">Tentang Saya</h2>
            <div class="glass p-8 md:p-12 rounded-3xl shadow-xl leading-relaxed">
                <p class="text-xl italic">
                    "Lulusan S1 Ilmu Komunikasi yang memiliki pengalaman kerja sebagai Administrasi Pelayanan Kependudukan di Kelurahan Mustika Jaya. Saya terbiasa menjadi garda terdepan dalam menyambut tamu dengan ramah, melakukan screening kebutuhan warga, serta mengelola pemberkasan surat-menyurat secara akurat. Memiliki kemampuan komunikasi yang baik dalam menangani berbagai karakter masyarakat dan berkomitmen memberikan pelayanan prima (service excellence) dengan cepat dan solutif."
                </p>
            </div>
        </div>
    </section>

    <!-- Experience Section -->
    <section id="experience" class="py-24 px-6">
        <div class="container mx-auto">
            <h2 class="text-4xl font-bold mb-16 text-center cursive">Pengalaman</h2>
            <div class="grid md:grid-cols-3 gap-8">
                
                <!-- Exp 1: Sekretaris -->
                <div class="glass p-6 rounded-2xl shadow-lg fade-in border border-gray-100 dark:border-gray-800">
                    <img src="https://i.postimg.cc/GHzD3nHr/GHzD3nHr.jpg" class="w-full h-40 object-cover rounded-xl mb-4" alt="Sertifikat Sekretaris">
                    <h3 class="font-bold text-xl mb-2">Sekretaris 2 LDK Al-Ghazi</h3>
                    <p class="text-sm opacity-70 mb-4">Maret 2022 - Maret 2023. Manajemen administrasi dan koordinasi organisasi kampus.</p>
                    <a href="https://postimg.cc/GHzD3nHr" target="_blank" class="text-indigo-500 font-bold hover:underline">Klik Sertifikat <i class="fas fa-external-link-alt"></i></a>
                </div>

                <!-- Exp 2: LKN -->
                <div class="glass p-6 rounded-2xl shadow-lg fade-in border border-gray-100 dark:border-gray-800">
                    <img src="https://i.postimg.cc/VSRK9VNp/VSRK9VNp.jpg" class="w-full h-40 object-cover rounded-xl mb-4" alt="Medali Perak">
                    <h3 class="font-bold text-xl mb-2">Medali Perak Biologi LKN</h3>
                    <p class="text-sm opacity-70 mb-4">26-28 November 2022. Kompetensi Nasional tingkat mahasiswa.</p>
                    <a href="https://postimg.cc/VSRK9VNp" target="_blank" class="text-indigo-500 font-bold hover:underline">Klik Sertifikat <i class="fas fa-external-link-alt"></i></a>
                </div>

                <!-- Exp 3: Berita -->
                <div class="glass p-6 rounded-2xl shadow-lg fade-in border border-gray-100 dark:border-gray-800">
                    <img src="https://i.postimg.cc/kVbJYzZ5/kVb-JYz-Z5.jpg" class="w-full h-40 object-cover rounded-xl mb-4" alt="Berita Kota">
                    <h3 class="font-bold text-xl mb-2">Penulis Berita Digital</h3>
                    <p class="text-sm opacity-70 mb-4">6 Januari 2022. Menulis artikel di Berita-kota.com.</p>
                    <a href="https://postimg.cc/kVbJYzZ5" target="_blank" class="text-indigo-500 font-bold hover:underline">Klik Foto Berita <i class="fas fa-external-link-alt"></i></a>
                </div>

            </div>
        </div>
    </section>

    <!-- Pelatihan & Seminar Section -->
    <section class="py-24 px-6 bg-indigo-50/20 dark:bg-slate-900/50">
        <div class="container mx-auto">
            <h2 class="text-4xl font-bold mb-16 text-center cursive">Pelatihan & Seminar</h2>
            <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-6">
                
                <!-- Kominfo -->
                <div class="glass p-4 rounded-xl fade-in text-center">
                    <img src="https://i.postimg.cc/KKsSmjy1/KKs-Smjy1.jpg" class="w-full h-32 object-cover rounded-lg mb-3" alt="Kominfo">
                    <h4 class="font-bold text-sm">Digital Marketing Kominfo</h4>
                    <a href="https://postimg.cc/KKsSmjy1" target="_blank" class="text-indigo-500 text-xs mt-2 block">Lihat Foto</a>
                </div>

                <!-- Trans 7 -->
                <div class="glass p-4 rounded-xl fade-in text-center">
                    <img src="https://i.postimg.cc/23dqSNVy/23dq-SNVy.jpg" class="w-full h-32 object-cover rounded-lg mb-3" alt="Trans 7">
                    <h4 class="font-bold text-sm">Webinar Broadcasting Trans 7</h4>
                    <a href="https://postimg.cc/23dqSNVy" target="_blank" class="text-indigo-500 text-xs mt-2 block">Lihat Foto</a>
                </div>

                <!-- SCTV -->
                <div class="glass p-4 rounded-xl fade-in text-center">
                    <img src="https://i.postimg.cc/pyYTHNdS/py-YTHNd-S.jpg" class="w-full h-32 object-cover rounded-lg mb-3" alt="SCTV">
                    <h4 class="font-bold text-sm">Personal Branding SCTV</h4>
                    <a href="https://postimg.cc/pyYTHNdS" target="_blank" class="text-indigo-500 text-xs mt-2 block">Lihat Foto</a>
                </div>

                <!-- Data Science -->
                <div class="glass p-4 rounded-xl fade-in text-center">
                    <img src="https://i.postimg.cc/f3tnTdf3/f3tn-Tdf3.jpg" class="w-full h-32 object-cover rounded-lg mb-3" alt="Data Science">
                    <h4 class="font-bold text-sm">Data Science Sang Surya</h4>
                    <a href="https://postimg.cc/f3tnTdf3" target="_blank" class="text-indigo-500 text-xs mt-2 block">Lihat Foto</a>
                </div>

                <!-- Rakamin -->
                <div class="glass p-4 rounded-xl fade-in text-center">
                    <img src="https://i.postimg.cc/dhWw0wM9/dh-Ww0w-M9.jpg" class="w-full h-32 object-cover rounded-lg mb-3" alt="Rakamin">
                    <h4 class="font-bold text-sm">UI/UX Rakamin</h4>
                    <a href="https://postimg.cc/dhWw0wM9" target="_blank" class="text-indigo-500 text-xs mt-2 block">Lihat Foto</a>
                </div>

                <!-- Magang -->
                <div class="glass p-4 rounded-xl fade-in text-center">
                    <img src="https://i.postimg.cc/ZBWMLzDf/ZBWMLz-Df.jpg" class="w-full h-32 object-cover rounded-lg mb-3" alt="Magang">
                    <h4 class="font-bold text-sm">Magang Mustika Jaya</h4>
                    <a href="https://postimg.cc/ZBWMLzDf" target="_blank" class="text-indigo-500 text-xs mt-2 block">Lihat Foto</a>
                </div>

                <!-- Generative AI -->
                <div class="glass p-4 rounded-xl fade-in text-center">
                    <img src="https://i.postimg.cc/q6RMwqdh/q6-RMwqdh.jpg" class="w-full h-32 object-cover rounded-lg mb-3" alt="AI">
                    <h4 class="font-bold text-sm">Generative AI Specialist</h4>
                    <a href="https://postimg.cc/q6RMwqdh" target="_blank" class="text-indigo-500 text-xs mt-2 block">Lihat Sertifikat</a>
                </div>

            </div>
        </div>
    </section>

    <!-- Education Section -->
    <section class="py-24 px-6">
        <div class="container mx-auto text-center fade-in">
            <h2 class="text-4xl font-bold mb-12 cursive">Pendidikan</h2>
            <div class="flex flex-col md:flex-row justify-center gap-12 items-center">
                <div class="space-y-4">
                    <i class="fas fa-graduation-cap text-6xl text-indigo-500 mb-2"></i>
                    <h3 class="text-2xl font-bold">Institut Bisnis Muhammadiyah Bekasi</h3>
                    <p class="text-lg">S1 Ilmu Komunikasi</p>
                    <span class="px-4 py-1 cum-laude rounded-full text-xs font-bold">IPK: 3.62 (Cum Laude)</span>
                    <div class="mt-4 max-w-sm mx-auto text-sm opacity-70">
                        Mata Kuliah: Komunikasi Bisnis, Manajemen Pemasaran, Public Relations, Etika & Hukum Komunikasi.
                    </div>
                </div>
                <div class="hidden md:block w-px h-48 bg-gray-300 dark:bg-gray-700"></div>
                <div class="space-y-2">
                    <h3 class="text-2xl font-bold">MAN 2 Kota Bekasi</h3>
                    <p class="text-lg">IPS (Nilai: 86.00)</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Project Gallery Section -->
    <section class="py-24 px-6 bg-slate-900 text-white rounded-[50px] mx-4">
        <div class="container mx-auto">
            <h2 class="text-4xl font-bold mb-16 text-center cursive">Galeri Projek (KKN & Magang)</h2>
            <div class="grid grid-cols-2 md:grid-cols-5 gap-4">
                <img src="https://i.postimg.cc/Hrk3ttfc/Hrk3ttfc.jpg" class="rounded-xl h-48 w-full object-cover hover:scale-105 transition shadow-lg" alt="KKN">
                <img src="https://i.postimg.cc/d7BySMrh/d7BySMrh.jpg" class="rounded-xl h-48 w-full object-cover hover:scale-105 transition shadow-lg" alt="Magang">
                <img src="https://i.postimg.cc/wyr3S9vv/wyr3S9vv.jpg" class="rounded-xl h-48 w-full object-cover hover:scale-105 transition shadow-lg" alt="KKN">
                <img src="https://i.postimg.cc/kBsP4fQ2/kBsP4fQ2.jpg" class="rounded-xl h-48 w-full object-cover hover:scale-105 transition shadow-lg" alt="KKN">
                <img src="https://i.postimg.cc/Hc0dtHyK/Hc0dtHyK.jpg" class="rounded-xl h-48 w-full object-cover hover:scale-105 transition shadow-lg" alt="KKN">
                <img src="https://i.postimg.cc/crzyw6zQ/crzyw6zQ.jpg" class="rounded-xl h-48 w-full object-cover hover:scale-105 transition shadow-lg" alt="Magang">
                <img src="https://i.postimg.cc/hXmwmsxb/hXmwmsxb.jpg" class="rounded-xl h-48 w-full object-cover hover:scale-105 transition shadow-lg" alt="Magang">
                <img src="https://i.postimg.cc/vg8Q8TT6/vg8Q8TT6.jpg" class="rounded-xl h-48 w-full object-cover hover:scale-105 transition shadow-lg" alt="AI Project">
                <img src="https://i.postimg.cc/Sn20r82D/Sn20r82D.jpg" class="rounded-xl h-48 w-full object-cover hover:scale-105 transition shadow-lg" alt="n8n Chatbot">
                <img src="https://i.postimg.cc/K4qsHjyw/K4qsHjyw.jpg" class="rounded-xl h-48 w-full object-cover hover:scale-105 transition shadow-lg" alt="KKN">
            </div>
        </div>
    </section>

    <!-- Video Projects Section -->
    <section class="py-24 px-6">
        <div class="container mx-auto max-w-4xl text-center">
            <h2 class="text-4xl font-bold mb-12 cursive">Projek Video</h2>
            <div class="grid md:grid-cols-3 gap-8">
                <a href="https://vt.tiktok.com/ZS5foF925/" target="_blank" class="glass p-8 rounded-3xl hover:bg-indigo-500 hover:text-white transition group">
                    <i class="fab fa-tiktok text-4xl mb-4 text-pink-500 group-hover:text-white"></i>
                    <h4 class="font-bold">n8n Invoice</h4>
                </a>
                <a href="https://vt.tiktok.com/ZS55JycsD/" target="_blank" class="glass p-8 rounded-3xl hover:bg-indigo-500 hover:text-white transition group">
                    <i class="fab fa-tiktok text-4xl mb-4 text-blue-500 group-hover:text-white"></i>
                    <h4 class="font-bold">BBPVP Bekasi AI</h4>
                </a>
                <a href="https://www.instagram.com/p/DTVWl1Nj7C6/" target="_blank" class="glass p-8 rounded-3xl hover:bg-indigo-500 hover:text-white transition group">
                    <i class="fab fa-instagram text-4xl mb-4 text-purple-500 group-hover:text-white"></i>
                    <h4 class="font-bold">Instagram Project</h4>
                </a>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section class="py-24 px-6 bg-slate-50 dark:bg-slate-900/50">
        <div class="container mx-auto text-center fade-in">
            <h2 class="text-4xl font-bold mb-10 cursive">Keahlian</h2>
            <div class="flex flex-wrap justify-center gap-3 max-w-2xl mx-auto">
                <span class="px-6 py-2 rounded-full border border-indigo-500">Komunikasi</span>
                <span class="px-6 py-2 rounded-full border border-indigo-500">Kerja Tim</span>
                <span class="px-6 py-2 rounded-full border border-indigo-500">Manajemen Waktu</span>
                <span class="px-6 py-2 rounded-full border border-indigo-500">Kepemimpinan</span>
                <span class="px-6 py-2 rounded-full border border-indigo-500">Marketing</span>
                <span class="px-6 py-2 rounded-full border border-indigo-500">Desain</span>
                <span class="px-6 py-2 rounded-full border border-indigo-500">Edit Video</span>
                <span class="px-6 py-2 rounded-full border border-indigo-500">Fotografer</span>
                <span class="px-6 py-2 rounded-full border border-indigo-500">MS Office</span>
            </div>
        </div>
    </section>

    <!-- Footer & Contact -->
    <footer class="py-20 px-6 bg-slate-900 text-white text-center">
        <div class="container mx-auto">
            <h2 class="text-4xl font-bold mb-8 cursive">Hubungi Saya</h2>
            <div class="flex justify-center flex-wrap gap-8 mb-12">
                <a href="mailto:eka23200@gmail.com" class="hover:text-indigo-400 transition"><i class="fas fa-envelope mr-2"></i> eka23200@gmail.com</a>
                <a href="https://Wa.me/6285932551750" target="_blank" class="hover:text-green-400 transition"><i class="fab fa-whatsapp mr-2"></i> 0859-3255-1750</a>
                <a href="https://www.linkedin.com/in/kurnia-eka-apsari-075559269/" target="_blank" class="hover:text-blue-400 transition"><i class="fab fa-linkedin mr-2"></i> LinkedIn</a>
            </div>
            <div class="flex justify-center gap-6 mb-12 text-2xl">
                <a href="https://www.instagram.com/akira_isamasu_zuina_16" target="_blank" class="hover:scale-125 transition"><i class="fab fa-instagram"></i></a>
                <a href="https://www.tiktok.com/@akiraisamasuzuina_19" target="_blank" class="hover:scale-125 transition"><i class="fab fa-tiktok"></i></a>
                <a href="https://github.com/new" target="_blank" class="hover:scale-125 transition"><i class="fab fa-github"></i></a>
            </div>
            <p class="text-sm opacity-50">&copy; 2024 Kurnia Eka Apsari. Seluruh Hak Cipta Dilindungi.</p>
        </div>
    </footer>

    <script>
        // Theme Toggle Logic
        function toggleTheme() {
            document.body.classList.toggle('dark');
            const icon = document.getElementById('theme-icon');
            if(document.body.classList.contains('dark')) {
                icon.classList.replace('fa-moon', 'fa-sun');
                localStorage.setItem('theme', 'dark');
            } else {
                icon.classList.replace('fa-sun', 'fa-moon');
                localStorage.setItem('theme', 'light');
            }
        }

        // Check for saved theme
        if (localStorage.getItem('theme') === 'dark') {
            document.body.classList.add('dark');
            document.getElementById('theme-icon').classList.replace('fa-moon', 'fa-sun');
        }

        // Scroll Animation
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                }
            });
        }, { threshold: 0.1 });

        document.querySelectorAll('.fade-in').forEach(el => observer.observe(el));
    </script>
</body>
</html>
