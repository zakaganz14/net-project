<!DOCTYPE html>
<html lang="id" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SinyalPro | Layanan Unblock IMEI Terpercaya</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
    <!-- FontAwesome for Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    },
                    colors: {
                        dark: '#0f172a',
                        darker: '#020617',
                        primary: '#06b6d4', // Cyan 500
                        secondary: '#8b5cf6', // Violet 500
                    },
                    animation: {
                        blob: "blob 7s infinite",
                        'fade-in-up': 'fadeInUp 1s ease-out forwards',
                    },
                    keyframes: {
                        blob: {
                            "0%": { transform: "translate(0px, 0px) scale(1)" },
                            "33%": { transform: "translate(30px, -50px) scale(1.1)" },
                            "66%": { transform: "translate(-20px, 20px) scale(0.9)" },
                            "100%": { transform: "translate(0px, 0px) scale(1)" },
                        },
                        fadeInUp: {
                            "0%": { opacity: 0, transform: "translateY(20px)" },
                            "100%": { opacity: 1, transform: "translateY(0)" },
                        }
                    }
                }
            }
        }
    </script>
    <style>
        body {
            background-color: #020617;
            color: #f8fafc;
            overflow-x: hidden;
        }
        /* Custom Glassmorphism Card */
        .glass-card {
            background: rgba(255, 255, 255, 0.03);
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.05);
        }
        .glass-nav {
            background: rgba(2, 6, 23, 0.8);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
            border-bottom: 1px solid rgba(255, 255, 255, 0.05);
        }
        /* Digital Glowing Text */
        .text-glow {
            text-shadow: 0 0 20px rgba(6, 182, 212, 0.5);
        }
    </style>
</head>
<body class="antialiased font-sans relative">

    <!-- Digital Background Decorations (Glowing Orbs) -->
    <div class="fixed inset-0 z-[-1] overflow-hidden pointer-events-none">
        <div class="absolute top-0 left-1/4 w-96 h-96 bg-primary rounded-full mix-blend-screen filter blur-[120px] opacity-20 animate-blob"></div>
        <div class="absolute top-1/4 right-1/4 w-96 h-96 bg-secondary rounded-full mix-blend-screen filter blur-[120px] opacity-20 animate-blob animation-delay-2000"></div>
        <div class="absolute -bottom-32 left-1/2 w-96 h-96 bg-blue-500 rounded-full mix-blend-screen filter blur-[120px] opacity-20 animate-blob animation-delay-4000"></div>
    </div>

    <!-- Navigation -->
    <nav class="fixed w-full z-50 glass-nav transition-all duration-300">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex items-center justify-between h-20">
                <div class="flex-shrink-0 flex items-center gap-2 cursor-pointer">
                    <i class="fa-solid fa-microchip text-primary text-2xl"></i>
                    <span class="font-bold text-2xl tracking-wider text-white">Sinyal<span class="text-primary text-glow">Pro</span></span>
                </div>
                <div class="hidden md:block">
                    <div class="ml-10 flex items-baseline space-x-8">
                        <a href="#beranda" class="hover:text-primary transition-colors px-3 py-2 rounded-md text-sm font-medium">Beranda</a>
                        <a href="#edukasi" class="hover:text-primary transition-colors px-3 py-2 rounded-md text-sm font-medium">Edukasi IMEI</a>
                        <a href="#harga" class="hover:text-primary transition-colors px-3 py-2 rounded-md text-sm font-medium">Harga</a>
                        <a href="#faq" class="hover:text-primary transition-colors px-3 py-2 rounded-md text-sm font-medium">FAQ</a>
                        <a href="https://wa.me/6281234567890" target="_blank" class="bg-gradient-to-r from-primary to-blue-600 hover:from-blue-500 hover:to-primary text-white px-6 py-2.5 rounded-full text-sm font-bold transition-all shadow-[0_0_15px_rgba(6,182,212,0.3)] hover:shadow-[0_0_25px_rgba(6,182,212,0.6)]">
                            Konsultasi WA
                        </a>
                    </div>
                </div>
                <!-- Mobile menu button -->
                <div class="-mr-2 flex md:hidden">
                    <button type="button" onclick="toggleMobileMenu()" class="inline-flex items-center justify-center p-2 rounded-md text-gray-400 hover:text-white hover:bg-white/10 focus:outline-none">
                        <i class="fa-solid fa-bars text-xl"></i>
                    </button>
                </div>
            </div>
        </div>
        <!-- Mobile Menu Panel -->
        <div id="mobile-menu" class="hidden md:hidden glass-card border-t border-white/10 absolute w-full">
            <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3">
                <a href="#beranda" class="block px-3 py-2 rounded-md text-base font-medium hover:bg-white/10">Beranda</a>
                <a href="#edukasi" class="block px-3 py-2 rounded-md text-base font-medium hover:bg-white/10">Edukasi IMEI</a>
                <a href="#harga" class="block px-3 py-2 rounded-md text-base font-medium hover:bg-white/10">Harga</a>
                <a href="#faq" class="block px-3 py-2 rounded-md text-base font-medium hover:bg-white/10">FAQ</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="beranda" class="pt-32 pb-20 lg:pt-48 lg:pb-32 px-4 sm:px-6 lg:px-8 max-w-7xl mx-auto min-h-screen flex items-center">
        <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
            <div class="animate-fade-in-up">
                <div class="inline-flex items-center gap-2 px-3 py-1 rounded-full glass-card text-primary text-sm font-semibold mb-6 border border-primary/30">
                    <span class="w-2 h-2 rounded-full bg-primary animate-pulse"></span>
                    Sistem Bypass V.4.2 Aktif
                </div>
                <h1 class="text-4xl sm:text-5xl lg:text-6xl font-bold leading-tight mb-6">
                    Bebaskan Sinyal HP Anda <br />
                    <span class="text-transparent bg-clip-text bg-gradient-to-r from-primary to-secondary">Tanpa Batas Jaringan</span>
                </h1>
                <p class="text-gray-400 text-lg mb-8 max-w-lg leading-relaxed">
                    Solusi profesional untuk masalah IMEI terblokir. Nikmati jaringan All Operator Indonesia (Telkomsel, XL, Indosat, dll) pada iPhone & Android Ex-Inter Anda secara instan dan aman.
                </p>
                <div class="flex flex-col sm:flex-row gap-4">
                    <a href="#harga" class="text-center bg-white text-dark font-bold px-8 py-3.5 rounded-full hover:bg-gray-200 transition-colors">
                        Lihat Paket
                    </a>
                    <a href="https://wa.me/6281234567890" target="_blank" class="text-center glass-card border border-white/20 hover:bg-white/10 text-white font-bold px-8 py-3.5 rounded-full transition-all flex items-center justify-center gap-2">
                        <i class="fa-brands fa-whatsapp text-green-400 text-xl"></i> Chat Admin
                    </a>
                </div>
                
                <div class="mt-10 flex items-center gap-6 text-sm text-gray-400">
                    <div class="flex items-center gap-2">
                        <i class="fa-solid fa-shield-halved text-primary"></i> 100% Aman
                    </div>
                    <div class="flex items-center gap-2">
                        <i class="fa-solid fa-bolt text-yellow-400"></i> Proses Cepat
                    </div>
                    <div class="flex items-center gap-2">
                        <i class="fa-solid fa-headset text-secondary"></i> Support 24/7
                    </div>
                </div>
            </div>
            
            <!-- Digital Phone Mockup Graphic -->
            <div class="relative hidden lg:block animate-fade-in-up" style="animation-delay: 0.2s;">
                <div class="relative w-80 mx-auto">
                    <!-- Phone Frame -->
                    <div class="relative z-10 glass-card border border-white/20 p-2 rounded-[2.5rem] shadow-2xl">
                        <div class="bg-darker rounded-[2rem] overflow-hidden h-[600px] border border-white/5 relative flex flex-col items-center justify-center">
                            <!-- Screen Content -->
                            <i class="fa-solid fa-signal text-5xl text-primary mb-4 animate-pulse"></i>
                            <h3 class="text-2xl font-bold text-white mb-2">Sinyal Ditemukan</h3>
                            <p class="text-gray-400 text-sm text-center px-6">LTE / 5G Network Active<br>All Operator Supported</p>
                            
                            <!-- Fake UI Elements -->
                            <div class="absolute top-4 left-6 right-6 flex justify-between text-xs text-gray-500">
                                <span>12:00</span>
                                <div class="flex gap-1 items-center">
                                    <i class="fa-solid fa-wifi"></i>
                                    <i class="fa-solid fa-battery-full"></i>
                                </div>
                            </div>
                        </div>
                    </div>
                    <!-- Glow behind phone -->
                    <div class="absolute inset-0 bg-gradient-to-tr from-primary to-secondary rounded-[2.5rem] filter blur-2xl opacity-30 transform scale-105 z-0"></div>
                </div>
            </div>
        </div>
    </section>

    <!-- Edukasi Section -->
    <section id="edukasi" class="py-20 relative border-t border-white/5 bg-dark">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">Mengapa Sinyal Anda Hilang?</h2>
                <p class="text-gray-400 max-w-2xl mx-auto">Pahami masalah regulasi IMEI pada perangkat Ex-Inter (luar negeri) dan bagaimana kami dapat membantu menyelesaikannya secara profesional.</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Edukasi Card 1 -->
                <div class="glass-card p-8 rounded-2xl hover:bg-white/5 transition-colors relative overflow-hidden group">
                    <div class="absolute top-0 right-0 w-32 h-32 bg-red-500/10 rounded-full filter blur-2xl group-hover:bg-red-500/20 transition-all"></div>
                    <div class="w-14 h-14 bg-red-500/20 rounded-xl flex items-center justify-center text-red-400 text-2xl mb-6">
                        <i class="fa-solid fa-ban"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3 text-white">Regulasi Pemerintah</h3>
                    <p class="text-gray-400 text-sm leading-relaxed">
                        Sejak 2020, pemerintah Indonesia memberlakukan aturan pemblokiran sinyal (No Service) untuk perangkat yang dibeli dari luar negeri (Ex-Inter) jika pajaknya belum dibayarkan di Bea Cukai.
                    </p>
                </div>

                <!-- Edukasi Card 2 -->
                <div class="glass-card p-8 rounded-2xl hover:bg-white/5 transition-colors relative overflow-hidden group">
                    <div class="absolute top-0 right-0 w-32 h-32 bg-primary/10 rounded-full filter blur-2xl group-hover:bg-primary/20 transition-all"></div>
                    <div class="w-14 h-14 bg-primary/20 rounded-xl flex items-center justify-center text-primary text-2xl mb-6">
                        <i class="fa-solid fa-server"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3 text-white">Sistem Bypass / Tembak</h3>
                    <p class="text-gray-400 text-sm leading-relaxed">
                        Kami mendaftarkan IMEI Anda melalui server khusus untuk mem-bypass pemblokiran. Proses ini bersifat digital, tidak perlu membongkar HP, dan sinyal akan kembali normal 100%.
                    </p>
                </div>

                <!-- Edukasi Card 3 -->
                <div class="glass-card p-8 rounded-2xl hover:bg-white/5 transition-colors relative overflow-hidden group">
                    <div class="absolute top-0 right-0 w-32 h-32 bg-green-500/10 rounded-full filter blur-2xl group-hover:bg-green-500/20 transition-all"></div>
                    <div class="w-14 h-14 bg-green-500/20 rounded-xl flex items-center justify-center text-green-400 text-2xl mb-6">
                        <i class="fa-solid fa-shield-check"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3 text-white">Aman & Terjamin</h3>
                    <p class="text-gray-400 text-sm leading-relaxed">
                        Proses pendaftaran kami aman untuk data privasi Anda. Kami hanya memerlukan 15 digit nomor IMEI. Perangkat bebas di-restart, update iOS/Android, dan berganti kartu SIM.
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Pricing Section -->
    <section id="harga" class="py-20 relative">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">Investasi Transparan, <span class="text-primary text-glow">Sinyal Maksimal</span></h2>
                <p class="text-gray-400 max-w-2xl mx-auto">Pilih paket yang sesuai dengan kebutuhan Anda. Jaminan uang kembali jika sinyal gagal naik.</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8 max-w-5xl mx-auto">
                <!-- Paket 3 Bulan -->
                <div class="glass-card rounded-3xl p-8 border border-white/10 flex flex-col mt-4 md:mt-8">
                    <h3 class="text-xl font-bold text-gray-300 mb-2">Paket Trial</h3>
                    <div class="text-primary font-semibold mb-4">Garansi 3 Bulan</div>
                    <div class="text-4xl font-bold text-white mb-6">Rp 150<span class="text-xl text-gray-500">.000</span></div>
                    
                    <ul class="space-y-4 mb-8 flex-grow">
                        <li class="flex items-start gap-3 text-gray-400 text-sm">
                            <i class="fa-solid fa-check text-green-400 mt-1"></i> Sinyal All Operator
                        </li>
                        <li class="flex items-start gap-3 text-gray-400 text-sm">
                            <i class="fa-solid fa-check text-green-400 mt-1"></i> Bebas Update OS
                        </li>
                        <li class="flex items-start gap-3 text-gray-400 text-sm">
                            <i class="fa-solid fa-check text-green-400 mt-1"></i> Garansi Penuh 3 Bulan
                        </li>
                        <li class="flex items-start gap-3 text-gray-500 text-sm line-through">
                            <i class="fa-solid fa-xmark mt-1"></i> Support Ganti Simcard Bebas
                        </li>
                    </ul>
                    <a href="https://wa.me/6281234567890?text=Halo%20SinyalPro,%20saya%20tertarik%20dengan%20Paket%20Trial%203%20Bulan" target="_blank" class="w-full block text-center glass-card hover:bg-white/10 border border-white/20 text-white font-bold py-3 rounded-xl transition-colors">
                        Pesan Sekarang
                    </a>
                </div>

                <!-- Paket VIP (Highlighted) -->
                <div class="glass-card rounded-3xl p-8 border border-primary/50 relative transform md:-translate-y-4 shadow-[0_0_30px_rgba(6,182,212,0.15)] bg-gradient-to-b from-primary/10 to-transparent flex flex-col">
                    <div class="absolute top-0 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-gradient-to-r from-primary to-blue-500 text-white px-4 py-1 rounded-full text-xs font-bold tracking-wide shadow-lg">
                        PALING LARIS
                    </div>
                    <h3 class="text-xl font-bold text-white mb-2">Paket Pro</h3>
                    <div class="text-primary font-semibold mb-4">Garansi 1 Tahun (Best Value)</div>
                    <div class="text-4xl font-bold text-white mb-6">Rp 350<span class="text-xl text-gray-500">.000</span></div>
                    
                    <ul class="space-y-4 mb-8 flex-grow">
                        <li class="flex items-start gap-3 text-gray-300 text-sm">
                            <i class="fa-solid fa-check text-primary mt-1"></i> Sinyal All Operator (4G/5G)
                        </li>
                        <li class="flex items-start gap-3 text-gray-300 text-sm">
                            <i class="fa-solid fa-check text-primary mt-1"></i> Bebas Update iOS / Android
                        </li>
                        <li class="flex items-start gap-3 text-gray-300 text-sm">
                            <i class="fa-solid fa-check text-primary mt-1"></i> Bebas Ganti Simcard
                        </li>
                        <li class="flex items-start gap-3 text-gray-300 text-sm">
                            <i class="fa-solid fa-check text-primary mt-1"></i> Prioritas Antrian Server
                        </li>
                    </ul>
                    <a href="https://wa.me/6281234567890?text=Halo%20SinyalPro,%20saya%20tertarik%20dengan%20Paket%20Pro%201%20Tahun" target="_blank" class="w-full block text-center bg-gradient-to-r from-primary to-blue-600 hover:from-blue-500 hover:to-primary text-white font-bold py-3 rounded-xl transition-all shadow-lg">
                        Pesan Sekarang
                    </a>
                </div>

                <!-- Paket Permanen Resmi -->
                <div class="glass-card rounded-3xl p-8 border border-white/10 flex flex-col mt-4 md:mt-8">
                    <h3 class="text-xl font-bold text-gray-300 mb-2">Paket Resmi</h3>
                    <div class="text-secondary font-semibold mb-4">Permanen Bea Cukai</div>
                    <div class="text-3xl font-bold text-white mb-6">Hubungi Admin</div>
                    
                    <ul class="space-y-4 mb-8 flex-grow">
                        <li class="flex items-start gap-3 text-gray-400 text-sm">
                            <i class="fa-solid fa-check text-green-400 mt-1"></i> Terdaftar Resmi Kemkominfo
                        </li>
                        <li class="flex items-start gap-3 text-gray-400 text-sm">
                            <i class="fa-solid fa-check text-green-400 mt-1"></i> Permanen Seumur Hidup
                        </li>
                        <li class="flex items-start gap-3 text-gray-400 text-sm">
                            <i class="fa-solid fa-check text-green-400 mt-1"></i> Aman Reset Pabrik
                        </li>
                        <li class="flex items-start gap-3 text-gray-400 text-sm">
                            <i class="fa-solid fa-info-circle text-gray-500 mt-1"></i> Harga Menyesuaikan Tipe HP
                        </li>
                    </ul>
                    <a href="https://wa.me/6281234567890?text=Halo%20SinyalPro,%20saya%20ingin%20konsultasi%20untuk%20Unblock%20Permanen%20Resmi" target="_blank" class="w-full block text-center glass-card hover:bg-white/10 border border-white/20 text-white font-bold py-3 rounded-xl transition-colors">
                        Konsultasi Harga
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- FAQ Section -->
    <section id="faq" class="py-20 bg-darker border-t border-white/5 relative">
        <div class="max-w-3xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-12">
                <h2 class="text-3xl font-bold mb-4">Pertanyaan Seputar <span class="text-primary text-glow">IMEI</span></h2>
                <p class="text-gray-400">Temukan jawaban cepat untuk pertanyaan yang sering diajukan pelanggan kami.</p>
            </div>

            <div class="space-y-4">
                <!-- FAQ Item 1 -->
                <details class="group glass-card border border-white/10 rounded-xl p-6 [&_summary::-webkit-details-marker]:hidden cursor-pointer">
                    <summary class="flex items-center justify-between font-semibold text-white">
                        <span>Berapa lama proses pendaftaran IMEI?</span>
                        <span class="transition group-open:rotate-180">
                            <i class="fa-solid fa-chevron-down text-primary"></i>
                        </span>
                    </summary>
                    <p class="text-gray-400 mt-4 text-sm leading-relaxed">
                        Proses pengerjaan normal membutuhkan waktu 15 - 45 menit tergantung antrian server. Untuk beberapa kasus tertentu, bisa memakan waktu hingga 1x24 jam. Kami selalu berusaha memberikan pelayanan tercepat.
                    </p>
                </details>

                <!-- FAQ Item 2 -->
                <details class="group glass-card border border-white/10 rounded-xl p-6 [&_summary::-webkit-details-marker]:hidden cursor-pointer">
                    <summary class="flex items-center justify-between font-semibold text-white">
                        <span>Apakah data di HP saya aman? Harus dikirimkah HP-nya?</span>
                        <span class="transition group-open:rotate-180">
                            <i class="fa-solid fa-chevron-down text-primary"></i>
                        </span>
                    </summary>
                    <p class="text-gray-400 mt-4 text-sm leading-relaxed">
                        Sangat aman. Anda <strong>TIDAK PERLU</strong> mengirimkan HP Anda kepada kami. Proses dilakukan secara digital, kami hanya membutuhkan 15 digit angka IMEI (*#06#) perangkat Anda. Data privasi (foto, chat, password) tetap aman 100%.
                    </p>
                </details>

                <!-- FAQ Item 3 -->
                <details class="group glass-card border border-white/10 rounded-xl p-6 [&_summary::-webkit-details-marker]:hidden cursor-pointer">
                    <summary class="flex items-center justify-between font-semibold text-white">
                        <span>Bagaimana jika sinyal kembali hilang sebelum masa garansi habis?</span>
                        <span class="transition group-open:rotate-180">
                            <i class="fa-solid fa-chevron-down text-primary"></i>
                        </span>
                    </summary>
                    <p class="text-gray-400 mt-4 text-sm leading-relaxed">
                        Jika sinyal kembali "No Service" selama masa garansi masih aktif, Anda cukup melapor ke Admin kami. Kami akan melakukan suntik ulang secara <strong>GRATIS</strong> tanpa biaya tambahan sepeser pun.
                    </p>
                </details>

                <!-- FAQ Item 4 -->
                <details class="group glass-card border border-white/10 rounded-xl p-6 [&_summary::-webkit-details-marker]:hidden cursor-pointer">
                    <summary class="flex items-center justify-between font-semibold text-white">
                        <span>Apakah boleh Update iOS / Android atau Factory Reset?</span>
                        <span class="transition group-open:rotate-180">
                            <i class="fa-solid fa-chevron-down text-primary"></i>
                        </span>
                    </summary>
                    <p class="text-gray-400 mt-4 text-sm leading-relaxed">
                        Untuk Paket 3 Bulan dan 1 Tahun, Anda bebas melakukan update OS. Namun kami <strong>TIDAK MENYARANKAN</strong> untuk melakukan Factory Reset (Kembali ke pengaturan pabrik). Untuk keamanan Factory Reset, kami sarankan mengambil Paket Permanen Resmi.
                    </p>
                </details>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-darker pt-16 pb-8 border-t border-white/5">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-12 mb-12">
                <div class="md:col-span-2">
                    <div class="flex items-center gap-2 mb-4">
                        <i class="fa-solid fa-microchip text-primary text-2xl"></i>
                        <span class="font-bold text-2xl tracking-wider text-white">Sinyal<span class="text-primary text-glow">Pro</span></span>
                    </div>
                    <p class="text-gray-400 text-sm mb-6 max-w-sm">
                        Solusi digital terbaik untuk layanan registrasi dan unblock IMEI perangkat telekomunikasi di Indonesia. Cepat, Terpercaya, dan Bergaransi.
                    </p>
                    <div class="flex space-x-4">
                        <a href="#" class="w-10 h-10 rounded-full glass-card flex items-center justify-center text-gray-400 hover:text-white hover:border-primary transition-colors">
                            <i class="fa-brands fa-instagram"></i>
                        </a>
                        <a href="#" class="w-10 h-10 rounded-full glass-card flex items-center justify-center text-gray-400 hover:text-white hover:border-primary transition-colors">
                            <i class="fa-brands fa-facebook-f"></i>
                        </a>
                        <a href="#" class="w-10 h-10 rounded-full glass-card flex items-center justify-center text-gray-400 hover:text-white hover:border-primary transition-colors">
                            <i class="fa-brands fa-tiktok"></i>
                        </a>
                    </div>
                </div>
                
                <div>
                    <h4 class="text-white font-bold mb-4">Tautan Cepat</h4>
                    <ul class="space-y-2 text-sm text-gray-400">
                        <li><a href="#beranda" class="hover:text-primary transition-colors">Beranda</a></li>
                        <li><a href="#edukasi" class="hover:text-primary transition-colors">Edukasi & Info</a></li>
                        <li><a href="#harga" class="hover:text-primary transition-colors">Daftar Harga</a></li>
                        <li><a href="#faq" class="hover:text-primary transition-colors">Tanya Jawab (FAQ)</a></li>
                    </ul>
                </div>

                <div>
                    <h4 class="text-white font-bold mb-4">Hubungi Kami</h4>
                    <ul class="space-y-3 text-sm text-gray-400">
                        <li class="flex items-start gap-3">
                            <i class="fa-brands fa-whatsapp text-primary mt-1"></i>
                            <span>+62 812-3456-7890<br>(Chat Only)</span>
                        </li>
                        <li class="flex items-start gap-3">
                            <i class="fa-solid fa-envelope text-primary mt-1"></i>
                            <span>support@sinyalpro.com</span>
                        </li>
                        <li class="flex items-start gap-3">
                            <i class="fa-solid fa-clock text-primary mt-1"></i>
                            <span>Setiap Hari<br>09:00 - 22:00 WIB</span>
                        </li>
                    </ul>
                </div>
            </div>
            
            <div class="border-t border-white/10 pt-8 flex flex-col md:flex-row justify-between items-center text-xs text-gray-500">
                <p>&copy; 2026 SinyalPro Digital Services. Hak Cipta Dilindungi.</p>
                <p class="mt-2 md:mt-0">
                    <span class="text-gray-400">Disclaimer:</span> Kami bertindak sebagai jasa perantara teknis pendaftaran jaringan, patuhi selalu hukum yang berlaku.
                </p>
            </div>
        </div>
    </footer>

    <!-- Interactive Scripts -->
    <script>
        // Mobile Menu Toggle
        function toggleMobileMenu() {
            const menu = document.getElementById('mobile-menu');
            if (menu.classList.contains('hidden')) {
                menu.classList.remove('hidden');
            } else {
                menu.classList.add('hidden');
            }
        }

        // Navbar scroll effect (add background blur on scroll)
        window.addEventListener('scroll', () => {
            const nav = document.querySelector('nav');
            if (window.scrollY > 10) {
                nav.classList.add('shadow-lg');
                nav.style.background = 'rgba(2, 6, 23, 0.9)';
            } else {
                nav.classList.remove('shadow-lg');
                nav.style.background = 'rgba(2, 6, 23, 0.8)';
            }
        });

        // Close mobile menu when clicking a link
        document.querySelectorAll('#mobile-menu a').forEach(link => {
            link.addEventListener('click', () => {
                document.getElementById('mobile-menu').classList.add('hidden');
            });
        });
    </script>
</body>
</html>
