<html lang="vi" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PHÁT LỘC FOREST - Chuyên Keo Giống, Kết Nối Vườn Ươm & Mở Điểm Bán 0 Đồng</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts: Roboto / Inter chuẩn Flatsome tiếng Việt -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">
    <!-- Font Awesome 6 Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">

    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    },
                    colors: {
                        brand: {
                            dark: '#1E5B2E',   /* Xanh đậm chuẩn logo Phát Lộc */
                            light: '#6FAF3A',  /* Xanh lá mầm chuẩn logo Phát Lộc */
                            orange: '#F08A24', /* Cam chuẩn chữ FOREST */
                            bg: '#F7FAF7',     /* Nền xám xanh nhạt nhẹ nhàng */
                        }
                    },
                    maxWidth: {
                        'flatsome': '1200px', /* Kích thước Row chuẩn của Flatsome */
                    }
                }
            }
        }
    </script>

    <style>
        html, body {
            font-family: 'Inter', sans-serif;
            color: #222222;
            background-color: #ffffff;
            overflow-x: hidden;
        }
        /* Container chuẩn Flatsome 1200px */
        .fs-container {
            max-width: 1200px;
            margin-left: auto;
            margin-right: auto;
            padding-left: 15px;
            padding-right: 15px;
        }
        /* Flatsome Section Title Style (Normal / Center / Bolder) */
        .fs-section-title {
            display: flex;
            align-items: center;
            justify-content: space-between;
            border-bottom: 2px solid #ececec;
            margin-bottom: 20px;
            padding-bottom: 10px;
        }
        .fs-section-title h2 {
            position: relative;
            font-weight: 700;
            text-transform: uppercase;
            color: #1E5B2E;
            margin-bottom: -12px;
            padding-bottom: 10px;
            border-bottom: 3px solid #1E5B2E;
        }
        /* Tối ưu ảnh sản phẩm vuông chuẩn Flatsome 1:1 */
        .product-thumb-wrapper {
            aspect-ratio: 1 / 1;
            overflow: hidden;
            background-color: #f5f5f5;
        }
        .product-thumb-wrapper img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.35s ease;
        }
        .product-card:hover .product-thumb-wrapper img {
            transform: scale(1.04);
        }
    </style>
</head>
<body class="antialiased selection:bg-brand-dark selection:text-white">

    <!-- =====================================================================
         1. FLATSOME TOP BAR (Header Top - Đã xóa thanh đen trên cùng)
    ====================================================================== -->
    <div class="bg-brand-dark text-white text-xs sm:text-sm py-2">
        <div class="fs-container flex flex-col sm:flex-row items-center justify-between gap-1.5 text-center sm:text-left">
            <p class="font-medium">
                Chào mừng bà con đến với <strong class="text-amber-300">CÔNG TY TNHH PHÁT LỘC FOREST</strong> — Hotline: <a href="tel:0788583898" class="font-bold text-amber-300 hover:underline">0788.583.898</a>
            </p>
            <div class="flex items-center gap-3 text-xs">
                <a href="https://zalo.me/0788583898" target="_blank" rel="noopener noreferrer" class="bg-blue-500 hover:bg-blue-600 text-white font-semibold px-2.5 py-0.5 rounded flex items-center gap-1 transition">
                    <i class="fa-solid fa-comment-dots"></i> Chat Zalo
                </a>
                <a href="https://www.facebook.com/phatlocforest" target="_blank" rel="noopener noreferrer" class="bg-[#1877F2] hover:opacity-90 text-white font-semibold px-2.5 py-0.5 rounded flex items-center gap-1 transition">
                    <i class="fa-brands fa-facebook-f"></i> Facebook
                </a>
                <button onclick="openLogoModal()" class="hidden md:inline-flex text-green-100 hover:text-amber-300 items-center gap-1 underline">
                    <i class="fa-solid fa-download"></i> Lấy Logo
                </button>
            </div>
        </div>
    </div>

    <!-- =====================================================================
         2. FLATSOME HEADER MAIN & BOTTOM NAVIGATION (Giống mẫu caygiong4s.com)
    ====================================================================== -->
    <header class="bg-white border-b border-gray-200 sticky top-0 z-40 shadow-sm">
        <div class="fs-container py-2.5 sm:py-3 flex items-center justify-between gap-2 sm:gap-4">
            
            <!-- Mobile Menu Button -->
            <button onclick="toggleMobileMenu()" class="lg:hidden text-gray-700 hover:text-brand-dark w-9 h-9 flex items-center justify-center rounded border border-gray-200 shrink-0" aria-label="Mở menu">
                <i class="fa-solid fa-bars text-lg"></i>
            </button>

            <!-- LOGO PHÁT LỘC FOREST (Đã xóa dải màu bên dưới như yêu cầu) -->
            <a href="#trang-chu" class="flex items-center gap-2 sm:gap-3 group min-w-0 flex-1 lg:flex-initial">
                <!-- SVG Logo tái tạo chuẩn xác từ ảnh gốc nhưng đã cắt bỏ thanh mã màu bên dưới -->
                <div class="w-11 h-11 sm:w-16 sm:h-16 shrink-0 flex items-center justify-center">
                    <svg id="phatloc-clean-logo-icon" viewBox="0 0 220 220" class="w-full h-full" xmlns="http://www.w3.org/2000/svg">
                        <!-- Vòng tròn trắng nền -->
                        <circle cx="110" cy="110" r="98" fill="#ffffff"/>
                        <!-- Vòng cung xanh đậm bên trái & dưới (#1E5B2E) -->
                        <path d="M 115 12 A 98 98 0 1 0 198 152 A 92 92 0 1 1 132 20 Z" fill="#1E5B2E"/>
                        <!-- Vòng cung cam bên phải trên (#F08A24) -->
                        <path d="M 96 20 A 94 94 0 0 1 192 162 A 98 98 0 0 0 115 12 Z" fill="#F08A24"/>
                        <!-- Chữ P xanh đậm có chiếc lá âm bản bên trong (#1E5B2E) -->
                        <path d="M 60 66 H 96 C 114 66 125 76 125 91 C 125 106 114 116 96 116 H 78 V 148 H 60 V 66 Z" fill="#1E5B2E"/>
                        <!-- Chiếc lá trắng bên trong chữ P -->
                        <path d="M 74 114 C 74 92 86 80 106 80 C 106 98 95 108 77 109 C 81 98 89 91 98 87 C 87 90 78 98 74 114 Z" fill="#ffffff"/>
                        <!-- Chữ L màu cam bên phải (#F08A24) -->
                        <path d="M 142 104 L 158 96 V 134 H 184 V 150 H 142 V 104 Z" fill="#F08A24"/>
                        <!-- Cây mầm ở giữa: Thân cây (#1E5B2E) -->
                        <path d="M 122 165 L 124 85 L 128 85 L 131 165 Z" fill="#1E5B2E"/>
                        <path d="M 125 126 L 111 110 L 114 108 L 126 121 Z" fill="#1E5B2E"/>
                        <path d="M 127 110 L 146 92 L 149 95 L 128 116 Z" fill="#1E5B2E"/>
                        <!-- 3 chiếc lá xanh non (#6FAF3A) -->
                        <!-- Lá đỉnh -->
                        <path d="M 126 36 C 142 52 142 75 126 90 C 110 75 110 52 126 36 Z" fill="#6FAF3A"/>
                        <path d="M 126 44 V 88" stroke="#ffffff" stroke-width="1.5" stroke-linecap="round"/>
                        <!-- Lá phải -->
                        <path d="M 168 73 C 166 93 153 104 135 103 C 137 85 150 74 168 73 Z" fill="#6FAF3A"/>
                        <path d="M 161 78 L 137 101" stroke="#ffffff" stroke-width="1.4" stroke-linecap="round"/>
                        <!-- Lá trái -->
                        <path d="M 102 95 C 116 98 123 109 120 122 C 107 118 100 108 102 95 Z" fill="#6FAF3A"/>
                        <!-- Đồi đất màu xanh dưới chân (#1E5B2E & #6FAF3A) -->
                        <path d="M 48 158 C 78 150 118 158 148 186 C 122 198 80 196 48 158 Z" fill="#1E5B2E"/>
                        <path d="M 88 189 C 106 178 126 178 144 189 C 126 196 106 196 88 189 Z" fill="#ffffff"/>
                        <path d="M 92 190 C 108 182 124 182 140 190 C 124 196 108 196 92 190 Z" fill="#1E5B2E"/>
                        <path d="M 134 168 C 150 160 168 162 180 168 C 172 180 160 187 149 190 C 144 181 139 174 134 168 Z" fill="#6FAF3A"/>
                    </svg>
                </div>
                <div class="min-w-0">
                    <div class="text-base sm:text-2xl font-extrabold tracking-tight leading-none truncate">
                        <span class="text-brand-dark">PHÁT LỘC</span> <span class="text-brand-orange">FOREST</span>
                    </div>
                    <div class="text-[9px] sm:text-xs font-semibold text-brand-dark tracking-tight sm:tracking-wider mt-1 truncate">
                        ƯƠM MẦM GIÁ TRỊ – PHÁT TRIỂN BỀN VỮNG
                    </div>
                </div>
            </a>

            <!-- Thanh tìm kiếm sản phẩm (Giống caygiong4s.com) -->
            <div class="hidden md:flex flex-1 max-w-md mx-4">
                <div class="relative w-full flex">
                    <input type="text" id="searchInput" oninput="filterProductsBySearch(this.value)" placeholder="Tìm kiếm keo mô, keo hom, bạch đàn, cây lâm nghiệp..." class="w-full border border-gray-300 rounded-l px-3.5 py-2 text-sm focus:outline-none focus:border-brand-dark">
                    <button class="bg-brand-dark hover:bg-brand-light text-white px-4 py-2 rounded-r transition" aria-label="Tìm kiếm">
                        <i class="fa-solid fa-magnifying-glass"></i>
                    </button>
                </div>
            </div>

            <!-- Cụm nút Liên Hệ: Zalo, Facebook & Hotline Tư Vấn Ngay -->
            <div class="flex items-center gap-1.5 sm:gap-2 shrink-0">
                <a href="https://zalo.me/0788583898" target="_blank" rel="noopener noreferrer" class="hidden sm:inline-flex items-center gap-1.5 bg-[#0068FF] hover:opacity-90 text-white font-bold text-xs px-3 py-2.5 rounded transition shadow-sm" title="Chat Zalo 0788.583.898">
                    <i class="fa-solid fa-comment-dots text-sm"></i>
                    <span>Zalo</span>
                </a>
                <a href="https://www.facebook.com/phatlocforest" target="_blank" rel="noopener noreferrer" class="hidden sm:inline-flex items-center gap-1.5 bg-[#1877F2] hover:opacity-90 text-white font-bold text-xs px-3 py-2.5 rounded transition shadow-sm" title="Fanpage Phát Lộc Forest">
                    <i class="fa-brands fa-facebook-f text-sm"></i>
                    <span class="hidden xl:inline">Facebook</span>
                </a>
                <a href="tel:0788583898" class="bg-brand-dark hover:bg-brand-light text-white font-bold text-xs sm:text-sm px-2.5 sm:px-3.5 py-2 rounded flex items-center gap-1.5 sm:gap-2 transition shadow-sm">
                    <i class="fa-solid fa-phone-volume text-amber-300"></i>
                    <div class="text-left leading-tight">
                        <span class="hidden sm:block text-[10px] font-normal text-green-100 uppercase">Tư vấn ngay</span>
                        <span class="text-[11px] sm:text-sm">0788.583.898</span>
                    </div>
                </a>
            </div>
        </div>

        <!-- Thanh tìm kiếm trên Mobile -->
        <div class="md:hidden px-3 pb-2.5">
            <div class="relative w-full flex">
                <input type="text" oninput="filterProductsBySearch(this.value)" placeholder="Tìm giống keo, cây lâm nghiệp..." class="w-full border border-gray-300 rounded-l px-3 py-1.5 text-sm focus:outline-none focus:border-brand-dark">
                <button class="bg-brand-dark text-white px-3.5 py-1.5 rounded-r text-sm">
                    <i class="fa-solid fa-magnifying-glass"></i>
                </button>
            </div>
        </div>

        <!-- Flatsome Header Bottom (Thanh Menu Ngang) -->
        <nav class="hidden lg:block bg-brand-dark text-white">
            <div class="fs-container flex items-center justify-between">
                <ul class="flex items-center text-sm font-semibold uppercase tracking-wide">
                    <li><a href="#trang-chu" class="block px-4 py-3 bg-brand-light text-white">Trang chủ</a></li>
                    <li><a href="#gioi-thieu" class="block px-4 py-3 hover:bg-brand-light transition">Giới thiệu</a></li>
                    <li><a href="#keo-giong" class="block px-4 py-3 hover:bg-brand-light transition">Chuyên Keo Giống</a></li>
                    <li><a href="#cay-lam-nghiep" class="block px-4 py-3 hover:bg-brand-light transition">Cây Giống Lâm Nghiệp</a></li>
                    <li><a href="#ket-noi-vuon-uom" class="block px-4 py-3 hover:bg-brand-light transition">Kết Nối Vườn Ươm</a></li>
                    <li><a href="#mo-diem-ban" class="block px-4 py-3 bg-brand-orange text-white hover:opacity-95 transition"><i class="fa-solid fa-handshake mr-1"></i> Mở Điểm Bán 0 Đồng</a></li>
                    <li><a href="#du-an-thuc-te" class="block px-4 py-3 hover:bg-brand-light transition">Dự Án & Hình Ảnh</a></li>
                    <li><a href="#lien-he" class="block px-4 py-3 hover:bg-brand-light transition">Liên Hệ</a></li>
                </ul>
            </div>
        </nav>

        <!-- Menu Mobile sổ xuống -->
        <div id="mobileMenu" class="hidden lg:hidden bg-white border-t border-gray-200 px-4 py-3 space-y-2 text-sm font-semibold uppercase">
            <a href="#trang-chu" onclick="toggleMobileMenu()" class="block py-2 text-brand-dark border-b border-gray-100">Trang chủ</a>
            <a href="#gioi-thieu" onclick="toggleMobileMenu()" class="block py-2 text-gray-700 border-b border-gray-100">Giới thiệu Phát Lộc Forest</a>
            <a href="#keo-giong" onclick="toggleMobileMenu()" class="block py-2 text-gray-700 border-b border-gray-100">Chuyên Keo Giống Chủ Lực</a>
            <a href="#cay-lam-nghiep" onclick="toggleMobileMenu()" class="block py-2 text-gray-700 border-b border-gray-100">Cây Giống Lâm Nghiệp</a>
            <a href="#ket-noi-vuon-uom" onclick="toggleMobileMenu()" class="block py-2 text-gray-700 border-b border-gray-100">Kết Nối Vườn Ươm Uy Tín</a>
            <a href="#mo-diem-ban" onclick="toggleMobileMenu()" class="block py-2 text-brand-orange font-bold border-b border-gray-100">Hướng Dẫn Mở Điểm Bán 0 Đồng</a>
            <a href="#du-an-thuc-te" onclick="toggleMobileMenu()" class="block py-2 text-gray-700 border-b border-gray-100">Dự Án & Hình Ảnh Thực Tế</a>
            <a href="#lien-he" onclick="toggleMobileMenu()" class="block py-2 text-gray-700 border-b border-gray-100">Địa Chỉ & Liên Hệ</a>
            <div class="pt-2 flex items-center gap-2">
                <a href="https://zalo.me/0788583898" target="_blank" rel="noopener noreferrer" class="flex-1 bg-[#0068FF] text-white text-center py-2 rounded text-xs font-bold">
                    <i class="fa-solid fa-comment-dots mr-1"></i> Chat Zalo
                </a>
                <a href="https://www.facebook.com/phatlocforest" target="_blank" rel="noopener noreferrer" class="flex-1 bg-[#1877F2] text-white text-center py-2 rounded text-xs font-bold">
                    <i class="fa-brands fa-facebook-f mr-1"></i> Facebook
                </a>
            </div>
        </div>
    </header>

    <!-- =====================================================================
         3. HERO SECTION + 4 CAM KẾT + 3 ICON BOX (Thiết kế Banner đẹp & chuẩn Mobile)
    ====================================================================== -->
    <section id="trang-chu" class="py-4 sm:py-6 bg-brand-bg border-b border-gray-200">
        <div class="fs-container">
            <!-- Row 1: Banner chính thiết kế nổi bật với nền xanh rừng lâm nghiệp sang trọng -->
            <div class="relative rounded-xl overflow-hidden shadow-md border border-brand-dark/20 bg-gradient-to-br from-[#133E1E] via-brand-dark to-[#256D38] text-white">
                <!-- Họa tiết ánh sáng nền tinh tế -->
                <div class="absolute -top-24 -right-24 w-72 h-72 rounded-full bg-brand-light/20 blur-2xl pointer-events-none"></div>
                <div class="absolute -bottom-24 -left-24 w-72 h-72 rounded-full bg-brand-orange/15 blur-2xl pointer-events-none"></div>

                <div class="relative z-10 grid grid-cols-1 lg:grid-cols-12 gap-6 p-4 sm:p-8 lg:p-10 items-center">
                    <!-- Cột nội dung Banner -->
                    <div class="lg:col-span-7 space-y-3.5 sm:space-y-4">
                        <div class="inline-flex items-center gap-2 bg-white/15 backdrop-blur-sm border border-white/20 text-amber-300 font-bold text-[11px] sm:text-xs px-3 py-1.5 rounded-full uppercase tracking-wider">
                            <i class="fa-solid fa-seedling text-brand-light"></i>
                            <span>CÔNG TY TNHH PHÁT LỘC FOREST • ĐỨC PHÚ, ĐÀ NẴNG</span>
                        </div>

                        <h1 class="text-xl sm:text-3xl lg:text-4xl font-extrabold text-white leading-snug sm:leading-tight">
                            CHUYÊN KEO GIỐNG CHUẨN ĐẦU DÒNG &amp; <span class="text-amber-300">KẾT NỐI VƯỜN ƯƠM UY TÍN</span>
                        </h1>

                        <p class="text-green-50 text-xs sm:text-base leading-relaxed">
                            Cung ứng keo lai nuôi cấy mô, keo giâm hom, keo tai tượng hạt ngoại và cây lâm nghiệp chất lượng cao. Đồng hành cùng bà con và đối tác phát triển mô hình <strong class="text-amber-300">Mở Điểm Bán Cây Giống 0 Đồng</strong> bền vững.
                        </p>

                        <!-- 4 Dấu tích cam kết nổi bật trên nền Banner -->
                        <div class="grid grid-cols-1 sm:grid-cols-2 gap-2.5 pt-1">
                            <div class="flex items-center gap-2.5 bg-white/10 border border-white/10 rounded-lg px-3 py-2 text-xs sm:text-sm font-medium text-white">
                                <i class="fa-solid fa-circle-check text-amber-300 text-base shrink-0"></i>
                                <span>100% giống keo chuẩn, rễ trắng khỏe</span>
                            </div>
                            <div class="flex items-center gap-2.5 bg-white/10 border border-white/10 rounded-lg px-3 py-2 text-xs sm:text-sm font-medium text-white">
                                <i class="fa-solid fa-circle-check text-amber-300 text-base shrink-0"></i>
                                <span>Kết nối trực tiếp vườn ươm giá gốc</span>
                            </div>
                            <div class="flex items-center gap-2.5 bg-white/10 border border-white/10 rounded-lg px-3 py-2 text-xs sm:text-sm font-medium text-white">
                                <i class="fa-solid fa-circle-check text-amber-300 text-base shrink-0"></i>
                                <span>Hỗ trợ mở điểm bán vốn 0 đồng</span>
                            </div>
                            <div class="flex items-center gap-2.5 bg-white/10 border border-white/10 rounded-lg px-3 py-2 text-xs sm:text-sm font-medium text-white">
                                <i class="fa-solid fa-circle-check text-amber-300 text-base shrink-0"></i>
                                <span>Đồng hành kỹ thuật trồng rừng trọn đời</span>
                            </div>
                        </div>

                        <!-- Cụm nút hành động chia 2 cột đều đẹp trên điện thoại -->
                        <div class="pt-2 grid grid-cols-2 sm:flex sm:flex-wrap gap-2.5">
                            <a href="tel:0788583898" class="bg-brand-orange hover:opacity-95 text-white font-bold text-xs sm:text-sm px-4 py-3 rounded-lg transition flex items-center justify-center gap-2 shadow">
                                <i class="fa-solid fa-phone-volume"></i>
                                <span>0788.583.898</span>
                            </a>
                            <a href="#mo-diem-ban" class="bg-white text-brand-dark hover:bg-amber-300 font-bold text-xs sm:text-sm px-4 py-3 rounded-lg transition flex items-center justify-center gap-2 shadow">
                                <i class="fa-solid fa-store text-brand-orange"></i>
                                <span>MỞ ĐIỂM BÁN 0Đ</span>
                            </a>
                            <a href="https://zalo.me/0788583898" target="_blank" rel="noopener noreferrer" class="bg-[#0068FF] hover:opacity-95 text-white font-bold text-xs sm:text-sm px-4 py-2.5 sm:py-3 rounded-lg transition flex items-center justify-center gap-1.5 shadow">
                                <i class="fa-solid fa-comment-dots"></i>
                                <span>Chat Zalo</span>
                            </a>
                            <a href="https://www.facebook.com/phatlocforest" target="_blank" rel="noopener noreferrer" class="bg-[#1877F2] hover:opacity-95 text-white font-bold text-xs sm:text-sm px-4 py-2.5 sm:py-3 rounded-lg transition flex items-center justify-center gap-1.5 shadow">
                                <i class="fa-brands fa-facebook-f"></i>
                                <span>Facebook</span>
                            </a>
                        </div>
                    </div>

                    <!-- Cột Hình ảnh thực tế vườn ươm trên Banner -->
                    <div class="lg:col-span-5">
                        <div class="bg-white p-2 sm:p-2.5 rounded-xl shadow-lg">
                            <div class="relative rounded-lg overflow-hidden">
                                <img src="https://images.unsplash.com/photo-1530836369250-ef72a3f5cda8?auto=format&fit=crop&w=900&q=80" 
                                     onerror="this.src='https://placehold.co/600x420/1E5B2E/FFFFFF?text=Vuon+Uom+Phat+Loc+Forest'"
                                     alt="Vườn ươm keo giống Phát Lộc Forest" 
                                     class="w-full h-52 sm:h-72 object-cover">
                                <div class="absolute bottom-0 inset-x-0 bg-gradient-to-t from-black/80 via-black/40 to-transparent p-3 sm:p-4 text-white">
                                    <p class="font-bold text-xs sm:text-sm text-amber-300 uppercase">Vườn Ươm Liên Kết Phát Lộc Forest</p>
                                    <p class="text-[11px] sm:text-xs text-gray-100 mt-0.5">Cây giống đảo bầu kỹ, đủ nắng, giao tận chân rừng</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Row 2: 3 Icon Box điểm mạnh (Giống hệt cấu trúc 3 cột dưới Banner của caygiong4s.com) -->
            <div class="grid grid-cols-1 md:grid-cols-3 gap-3 sm:gap-4 mt-4 sm:mt-5">
                <div class="bg-white p-4 sm:p-5 rounded-lg border border-gray-200 flex items-start gap-3.5 shadow-sm">
                    <div class="w-11 h-11 sm:w-12 sm:h-12 rounded-full bg-brand-dark/10 text-brand-dark flex items-center justify-center shrink-0 text-lg sm:text-xl">
                        <i class="fa-solid fa-seedling"></i>
                    </div>
                    <div>
                        <h3 class="font-bold text-brand-dark text-sm sm:text-base uppercase">Tỉ Lệ Sống Trên 98%</h3>
                        <p class="text-gray-600 text-xs sm:text-sm mt-1 leading-relaxed">
                            Cây giống được đảo bầu, huấn luyện nắng kỹ lưỡng tại vườn ươm đạt chuẩn trước khi xuất giao cho bà con trồng rừng.
                        </p>
                    </div>
                </div>

                <div class="bg-white p-4 sm:p-5 rounded-lg border border-gray-200 flex items-start gap-3.5 shadow-sm">
                    <div class="w-11 h-11 sm:w-12 sm:h-12 rounded-full bg-brand-orange/15 text-brand-orange flex items-center justify-center shrink-0 text-lg sm:text-xl">
                        <i class="fa-solid fa-truck-fast"></i>
                    </div>
                    <div>
                        <h3 class="font-bold text-brand-dark text-sm sm:text-base uppercase">Giao Cây Tận Nơi Nhanh Chóng</h3>
                        <p class="text-gray-600 text-xs sm:text-sm mt-1 leading-relaxed">
                            Hệ thống xe tải chuyên chở cây giống từ vườn ươm liên kết gần nhất đến tận chân lô rừng, giữ nguyên bầu đất.
                        </p>
                    </div>
                </div>

                <div class="bg-white p-4 sm:p-5 rounded-lg border border-gray-200 flex items-start gap-3.5 shadow-sm">
                    <div class="w-11 h-11 sm:w-12 sm:h-12 rounded-full bg-brand-light/15 text-brand-light flex items-center justify-center shrink-0 text-lg sm:text-xl">
                        <i class="fa-solid fa-handshake-angle"></i>
                    </div>
                    <div>
                        <h3 class="font-bold text-brand-dark text-sm sm:text-base uppercase">Mở Điểm Bán Vốn 0 Đồng</h3>
                        <p class="text-gray-600 text-xs sm:text-sm mt-1 leading-relaxed">
                            Hỗ trợ bảng hiệu, quy trình bảo quản cây, nguồn hàng trực tiếp từ vườn ươm uy tín và chuyển giao khách hàng khu vực.
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- =====================================================================
         4. SECTION GIỚI THIỆU NGẮN & DANH MỤC CHỦ LỰC (3 CỘT CHUẨN CAYGIONG4S)
    ====================================================================== -->
    <section id="gioi-thieu" class="py-8 sm:py-10 bg-white">
        <div class="fs-container">
            <!-- Khối giới thiệu Phát Lộc Forest -->
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 items-center mb-10 pb-8 border-b border-gray-200">
                <div class="lg:col-span-7 space-y-3">
                    <h2 class="text-xl sm:text-2xl font-extrabold text-brand-dark uppercase">
                        CÔNG TY TNHH PHÁT LỘC FOREST
                    </h2>
                    <p class="text-gray-700 text-sm sm:text-base leading-relaxed">
                        Đặt trụ sở tại <strong>Thôn Trung Hòa, Xã Đức Phú, TP Đà Nẵng</strong>, <strong>Phát Lộc Forest</strong> là đơn vị chuyên sản xuất, tuyển chọn và cung ứng cây keo giống lâm nghiệp chất lượng cao (keo nuôi cấy mô, keo lai giâm hom, keo hạt ngoại) cùng mạng lưới kết nối các vườn ươm đạt chuẩn trên toàn khu vực.
                    </p>
                    <p class="text-gray-700 text-sm sm:text-base leading-relaxed">
                        Với phương châm <em>“Ươm mầm giá trị – Phát triển bền vững”</em>, chúng tôi không chỉ mang đến nguồn cây giống khỏe mạnh, sinh trưởng nhanh, kháng bệnh tốt cho bà con trồng rừng mà còn tiên phong xây dựng mạng lưới <strong>Điểm Bán Cây Giống 0 Đồng</strong> giúp kết nối trực tiếp vườn ươm uy tín tới từng xã, thôn.
                    </p>
                </div>
                <div class="lg:col-span-5 bg-brand-bg p-6 rounded border-l-4 border-brand-dark">
                    <p class="italic text-gray-700 text-sm sm:text-base leading-relaxed">
                        “Trồng rừng là đầu tư dài hạn của bà con nông dân. Chọn đúng cây giống chuẩn ngay từ đầu chính là bảo hiểm vững chắc nhất cho năng suất gỗ thu hoạch sau 4 – 5 năm.”
                    </p>
                    <div class="mt-4 pt-3 border-t border-gray-200 flex items-center justify-between">
                        <div>
                            <p class="font-bold text-brand-dark text-sm">CÔNG TY TNHH PHÁT LỘC FOREST</p>
                            <p class="text-xs text-gray-500">MST: 4001334115 • Hotline: 0788.583.898</p>
                        </div>
                        <a href="https://www.facebook.com/phatlocforest" target="_blank" rel="noopener noreferrer" class="text-xs font-semibold text-brand-dark hover:underline">
                            Xem Fanpage <i class="fa-solid fa-arrow-right ml-1"></i>
                        </a>
                    </div>
                </div>
            </div>

            <!-- 3 Danh mục cốt lõi (3 cột giống Danh Mục Sản Phẩm trên caygiong4s.com) -->
            <div class="text-center mb-6">
                <h2 class="text-xl sm:text-2xl font-bold text-brand-dark uppercase">LĨNH VỰC HOẠT ĐỘNG CHỦ LỰC</h2>
                <p class="text-gray-500 text-sm mt-1">Giải pháp toàn diện từ vườn ươm keo giống đến điểm phân phối tại địa phương</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
                <!-- Cột 1 -->
                <a href="#keo-giong" class="group block border border-gray-200 rounded overflow-hidden hover:border-brand-dark transition bg-white">
                    <div class="h-48 overflow-hidden bg-gray-100">
                        <img src="https://images.unsplash.com/photo-1592150621744-aca64f48394a?auto=format&fit=crop&w=700&q=80" 
                             onerror="this.src='https://placehold.co/600x400/1E5B2E/FFFFFF?text=Chuyen+Keo+Giong'"
                             alt="Chuyên Keo Giống" class="w-full h-full object-cover group-hover:scale-105 transition duration-300">
                    </div>
                    <div class="p-4 text-center">
                        <h3 class="font-bold text-brand-dark text-base uppercase group-hover:text-brand-orange transition">1. CHUYÊN KEO GIỐNG CHỦ LỰC</h3>
                        <p class="text-gray-600 text-xs sm:text-sm mt-1">
                            Keo lai nuôi cấy mô (BV10, BV16, BV32, BV73, AH1, AH7), keo giâm hom, keo tai tượng hạt Úc chuẩn F1.
                        </p>
                    </div>
                </a>

                <!-- Cột 2 -->
                <a href="#ket-noi-vuon-uom" class="group block border border-gray-200 rounded overflow-hidden hover:border-brand-dark transition bg-white">
                    <div class="h-48 overflow-hidden bg-gray-100">
                        <img src="https://images.unsplash.com/photo-1585320806297-9794b3e4eeae?auto=format&fit=crop&w=700&q=80" 
                             onerror="this.src='https://placehold.co/600x400/6FAF3A/FFFFFF?text=Ket+Noi+Vuon+Uom'"
                             alt="Kết nối vườn ươm uy tín" class="w-full h-full object-cover group-hover:scale-105 transition duration-300">
                    </div>
                    <div class="p-4 text-center">
                        <h3 class="font-bold text-brand-dark text-base uppercase group-hover:text-brand-orange transition">2. KẾT NỐI VƯỜN ƯƠM UY TÍN</h3>
                        <p class="text-gray-600 text-xs sm:text-sm mt-1">
                            Liên kết chuỗi vườn ươm có chứng nhận nguồn giống, kiểm định chất lượng cây trước khi xuất vườn.
                        </p>
                    </div>
                </a>

                <!-- Cột 3 -->
                <a href="#mo-diem-ban" class="group block border border-gray-200 rounded overflow-hidden hover:border-brand-dark transition bg-white">
                    <div class="h-48 overflow-hidden bg-gray-100">
                        <img src="https://images.unsplash.com/photo-1542601906990-b4d3fb778b09?auto=format&fit=crop&w=700&q=80" 
                             onerror="this.src='https://placehold.co/600x400/F08A24/FFFFFF?text=Mo+Diem+Ban+0+Dong'"
                             alt="Hướng dẫn mở điểm bán 0 đồng" class="w-full h-full object-cover group-hover:scale-105 transition duration-300">
                    </div>
                    <div class="p-4 text-center">
                        <h3 class="font-bold text-brand-dark text-base uppercase group-hover:text-brand-orange transition">3. HƯỚNG DẪN MỞ ĐIỂM BÁN 0Đ</h3>
                        <p class="text-gray-600 text-xs sm:text-sm mt-1">
                            Hợp tác mở điểm phân phối cây giống tại địa phương không cần vốn nhập hàng, hỗ trợ từ A-Z.
                        </p>
                    </div>
                </a>
            </div>
        </div>
    </section>

    <!-- =====================================================================
         5. SECTION SẢN PHẨM 1: CHUYÊN KEO GIỐNG & BẠCH ĐÀN
         - Chia 2 cột trên điện thoại (grid-cols-2), 4 cột trên máy tính (lg:grid-cols-4)
         - TUYỆT ĐỐI KHÔNG ĐỂ NHÃN DÁN (SALE / HOT / % GIẢM GIÁ) TRÊN TRANG CHỦ
    ====================================================================== -->
    <section id="keo-giong" class="py-8 bg-brand-bg">
        <div class="fs-container">
            <!-- Flatsome Section Header -->
            <div class="fs-section-title flex-wrap gap-2">
                <h2 class="text-lg sm:text-xl">CHUYÊN KEO GIỐNG & BẠCH ĐÀN CHỦ LỰC</h2>
                <div class="flex flex-wrap items-center gap-3 text-xs sm:text-sm text-gray-600">
                    <span class="hover:text-brand-dark cursor-pointer" onclick="filterCategory('all')">Tất cả</span>
                    <span>•</span>
                    <span class="hover:text-brand-dark cursor-pointer" onclick="filterCategory('keo-mo')">Keo nuôi cấy mô</span>
                    <span>•</span>
                    <span class="hover:text-brand-dark cursor-pointer" onclick="filterCategory('keo-hom')">Keo lai giâm hom</span>
                    <span>•</span>
                    <span class="hover:text-brand-dark cursor-pointer" onclick="filterCategory('keo-hat')">Keo tai tượng</span>
                </div>
            </div>

            <!-- LƯỚI SẢN PHẨM: 2 cột trên điện thoại (grid-cols-2), 4 cột trên máy tính (lg:grid-cols-4) -->
            <!-- Hoàn toàn sạch sẽ, KHÔNG có bất kỳ nhãn dán (badge) nào -->
            <div id="keoProductGrid" class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-3 sm:gap-5">
                
                <!-- Sản phẩm 1 -->
                <div class="product-card bg-white border border-gray-200 rounded overflow-hidden flex flex-col justify-between" data-cat="keo-mo" data-name="Keo Lai Nuôi Cấy Mô BV10">
                    <div>
                        <div class="product-thumb-wrapper">
                            <img src="https://images.unsplash.com/photo-1592150621744-aca64f48394a?auto=format&fit=crop&w=600&q=80" alt="Keo Lai Nuôi Cấy Mô BV10">
                        </div>
                        <div class="p-3 text-center">
                            <h3 class="text-sm sm:text-base font-semibold text-gray-800 hover:text-brand-dark line-clamp-2">
                                Keo Lai Nuôi Cấy Mô BV10
                            </h3>
                            <p class="text-xs text-gray-500 mt-1">Chống chịu gió bão, năng suất gỗ cao</p>
                            <p class="text-brand-dark font-bold text-sm sm:text-base mt-1.5">1.200 ₫ / cây</p>
                        </div>
                    </div>
                    <div class="px-3 pb-3">
                        <button onclick="openOrderModal('Keo Lai Nuôi Cấy Mô BV10', '1.200 ₫ / cây')" class="w-full border border-brand-dark text-brand-dark hover:bg-brand-dark hover:text-white text-xs sm:text-sm font-semibold py-2 rounded transition">
                            Đặt cây tại vườn
                        </button>
                    </div>
                </div>

                <!-- Sản phẩm 2 -->
                <div class="product-card bg-white border border-gray-200 rounded overflow-hidden flex flex-col justify-between" data-cat="keo-mo" data-name="Keo Lai Nuôi Cấy Mô BV32">
                    <div>
                        <div class="product-thumb-wrapper">
                            <img src="https://images.unsplash.com/photo-1530836369250-ef72a3f5cda8?auto=format&fit=crop&w=600&q=80" alt="Keo Lai Nuôi Cấy Mô BV32">
                        </div>
                        <div class="p-3 text-center">
                            <h3 class="text-sm sm:text-base font-semibold text-gray-800 hover:text-brand-dark line-clamp-2">
                                Keo Lai Nuôi Cấy Mô BV32
                            </h3>
                            <p class="text-xs text-gray-500 mt-1">Thân thẳng, ít cành nhánh, lớn nhanh</p>
                            <p class="text-brand-dark font-bold text-sm sm:text-base mt-1.5">1.200 ₫ / cây</p>
                        </div>
                    </div>
                    <div class="px-3 pb-3">
                        <button onclick="openOrderModal('Keo Lai Nuôi Cấy Mô BV32', '1.200 ₫ / cây')" class="w-full border border-brand-dark text-brand-dark hover:bg-brand-dark hover:text-white text-xs sm:text-sm font-semibold py-2 rounded transition">
                            Đặt cây tại vườn
                        </button>
                    </div>
                </div>

                <!-- Sản phẩm 3 -->
                <div class="product-card bg-white border border-gray-200 rounded overflow-hidden flex flex-col justify-between" data-cat="keo-mo" data-name="Keo Mô AH1 & AH7 Chuẩn Dòng">
                    <div>
                        <div class="product-thumb-wrapper">
                            <img src="https://images.unsplash.com/photo-1523348837708-15d4a09cfac2?auto=format&fit=crop&w=600&q=80" alt="Keo Mô AH1 & AH7 Chuẩn Dòng">
                        </div>
                        <div class="p-3 text-center">
                            <h3 class="text-sm sm:text-base font-semibold text-gray-800 hover:text-brand-dark line-clamp-2">
                                Keo Mô AH1 & AH7 Chuẩn Dòng
                            </h3>
                            <p class="text-xs text-gray-500 mt-1">Kháng bệnh chết héo, thích nghi đất đồi</p>
                            <p class="text-brand-dark font-bold text-sm sm:text-base mt-1.5">1.250 ₫ / cây</p>
                        </div>
                    </div>
                    <div class="px-3 pb-3">
                        <button onclick="openOrderModal('Keo Mô AH1 & AH7 Chuẩn Dòng', '1.250 ₫ / cây')" class="w-full border border-brand-dark text-brand-dark hover:bg-brand-dark hover:text-white text-xs sm:text-sm font-semibold py-2 rounded transition">
                            Đặt cây tại vườn
                        </button>
                    </div>
                </div>

                <!-- Sản phẩm 4 -->
                <div class="product-card bg-white border border-gray-200 rounded overflow-hidden flex flex-col justify-between" data-cat="keo-mo" data-name="Keo Lai Mô BV71 - BV73 - BV75">
                    <div>
                        <div class="product-thumb-wrapper">
                            <img src="https://images.unsplash.com/photo-1466692476868-aef1dfb1e735?auto=format&fit=crop&w=600&q=80" alt="Keo Lai Mô BV71 - BV73 - BV75">
                        </div>
                        <div class="p-3 text-center">
                            <h3 class="text-sm sm:text-base font-semibold text-gray-800 hover:text-brand-dark line-clamp-2">
                                Keo Lai Mô BV71 - BV73 - BV75
                            </h3>
                            <p class="text-xs text-gray-500 mt-1">Bộ rễ cọc khỏe, sinh khối vượt trội</p>
                            <p class="text-brand-dark font-bold text-sm sm:text-base mt-1.5">1.200 ₫ / cây</p>
                        </div>
                    </div>
                    <div class="px-3 pb-3">
                        <button onclick="openOrderModal('Keo Lai Mô BV71 - BV73 - BV75', '1.200 ₫ / cây')" class="w-full border border-brand-dark text-brand-dark hover:bg-brand-dark hover:text-white text-xs sm:text-sm font-semibold py-2 rounded transition">
                            Đặt cây tại vườn
                        </button>
                    </div>
                </div>

                <!-- Sản phẩm 5 -->
                <div class="product-card bg-white border border-gray-200 rounded overflow-hidden flex flex-col justify-between" data-cat="keo-hom" data-name="Keo Lai Giâm Hom Tuyển Chọn">
                    <div>
                        <div class="product-thumb-wrapper">
                            <img src="https://images.unsplash.com/photo-1585320806297-9794b3e4eeae?auto=format&fit=crop&w=600&q=80" alt="Keo Lai Giâm Hom Tuyển Chọn">
                        </div>
                        <div class="p-3 text-center">
                            <h3 class="text-sm sm:text-base font-semibold text-gray-800 hover:text-brand-dark line-clamp-2">
                                Keo Lai Giâm Hom Tuyển Chọn
                            </h3>
                            <p class="text-xs text-gray-500 mt-1">Hom đầu dòng, bầu rễ trắng kín</p>
                            <p class="text-brand-dark font-bold text-sm sm:text-base mt-1.5">750 ₫ / cây</p>
                        </div>
                    </div>
                    <div class="px-3 pb-3">
                        <button onclick="openOrderModal('Keo Lai Giâm Hom Tuyển Chọn', '750 ₫ / cây')" class="w-full border border-brand-dark text-brand-dark hover:bg-brand-dark hover:text-white text-xs sm:text-sm font-semibold py-2 rounded transition">
                            Đặt cây tại vườn
                        </button>
                    </div>
                </div>

                <!-- Sản phẩm 6 -->
                <div class="product-card bg-white border border-gray-200 rounded overflow-hidden flex flex-col justify-between" data-cat="keo-hat" data-name="Keo Tai Tượng Hạt Ngoại Úc">
                    <div>
                        <div class="product-thumb-wrapper">
                            <img src="https://images.unsplash.com/photo-1500651230702-0e2d8a49d4ad?auto=format&fit=crop&w=600&q=80" alt="Keo Tai Tượng Hạt Ngoại Úc">
                        </div>
                        <div class="p-3 text-center">
                            <h3 class="text-sm sm:text-base font-semibold text-gray-800 hover:text-brand-dark line-clamp-2">
                                Keo Tai Tượng Hạt Ngoại Úc
                            </h3>
                            <p class="text-xs text-gray-500 mt-1">Hạt nhập khẩu Úc, rễ cọc ăn sâu</p>
                            <p class="text-brand-dark font-bold text-sm sm:text-base mt-1.5">850 ₫ / cây</p>
                        </div>
                    </div>
                    <div class="px-3 pb-3">
                        <button onclick="openOrderModal('Keo Tai Tượng Hạt Ngoại Úc', '850 ₫ / cây')" class="w-full border border-brand-dark text-brand-dark hover:bg-brand-dark hover:text-white text-xs sm:text-sm font-semibold py-2 rounded transition">
                            Đặt cây tại vườn
                        </button>
                    </div>
                </div>

                <!-- Sản phẩm 7 -->
                <div class="product-card bg-white border border-gray-200 rounded overflow-hidden flex flex-col justify-between" data-cat="keo-hat" data-name="Keo Lá Tràm (Tràm Bông Vàng)">
                    <div>
                        <div class="product-thumb-wrapper">
                            <img src="https://images.unsplash.com/photo-1416879595882-3373a0480b5b?auto=format&fit=crop&w=600&q=80" alt="Keo Lá Tràm (Tràm Bông Vàng)">
                        </div>
                        <div class="p-3 text-center">
                            <h3 class="text-sm sm:text-base font-semibold text-gray-800 hover:text-brand-dark line-clamp-2">
                                Keo Lá Tràm (Tràm Bông Vàng)
                            </h3>
                            <p class="text-xs text-gray-500 mt-1">Chịu hạn tốt, phù hợp vùng đất cát, sỏi</p>
                            <p class="text-brand-dark font-bold text-sm sm:text-base mt-1.5">750 ₫ / cây</p>
                        </div>
                    </div>
                    <div class="px-3 pb-3">
                        <button onclick="openOrderModal('Keo Lá Tràm (Tràm Bông Vàng)', '750 ₫ / cây')" class="w-full border border-brand-dark text-brand-dark hover:bg-brand-dark hover:text-white text-xs sm:text-sm font-semibold py-2 rounded transition">
                            Đặt cây tại vườn
                        </button>
                    </div>
                </div>

                <!-- Sản phẩm 8 -->
                <div class="product-card bg-white border border-gray-200 rounded overflow-hidden flex flex-col justify-between" data-cat="keo-mo" data-name="Bạch Đàn Mô Cao Sản DH32-29">
                    <div>
                        <div class="product-thumb-wrapper">
                            <img src="https://images.unsplash.com/photo-1518531933037-91b2f5f229cc?auto=format&fit=crop&w=600&q=80" alt="Bạch Đàn Mô Cao Sản DH32-29">
                        </div>
                        <div class="p-3 text-center">
                            <h3 class="text-sm sm:text-base font-semibold text-gray-800 hover:text-brand-dark line-clamp-2">
                                Bạch Đàn Mô Cao Sản DH32-29
                            </h3>
                            <p class="text-xs text-gray-500 mt-1">Chu kỳ thu hoạch ngắn, trữ lượng cao</p>
                            <p class="text-brand-dark font-bold text-sm sm:text-base mt-1.5">1.500 ₫ / cây</p>
                        </div>
                    </div>
                    <div class="px-3 pb-3">
                        <button onclick="openOrderModal('Bạch Đàn Mô Cao Sản DH32-29', '1.500 ₫ / cây')" class="w-full border border-brand-dark text-brand-dark hover:bg-brand-dark hover:text-white text-xs sm:text-sm font-semibold py-2 rounded transition">
                            Đặt cây tại vườn
                        </button>
                    </div>
                </div>

            </div>

            <!-- Thanh CTA ngang dưới danh mục giống caygiong4s.com -->
            <div class="mt-6 bg-white border border-gray-200 rounded p-4 text-center text-sm sm:text-base">
                Đặt số lượng lớn cho dự án trồng rừng hoặc nhận báo giá sỉ tại vườn ươm Phát Lộc Forest ⇒ 
                <a href="tel:0788583898" class="font-bold text-brand-orange hover:underline ml-1">Gọi ngay 0788.583.898</a>
            </div>
        </div>
    </section>

    <!-- =====================================================================
         6. SECTION SẢN PHẨM 2: CÂY GIỐNG LÂM NGHIỆP & GỖ QUÝ
         - Chia 2 cột trên điện thoại (grid-cols-2), 4 cột trên máy tính (lg:grid-cols-4)
         - KHÔNG NHÃN DÁN TRANG CHỦ
    ====================================================================== -->
    <section id="cay-lam-nghiep" class="py-8 bg-white">
        <div class="fs-container">
            <div class="fs-section-title flex-wrap gap-2">
                <h2 class="text-lg sm:text-xl">CÂY GIỐNG LÂM NGHIỆP & CÂY GỖ LỚN</h2>
                <div class="text-xs sm:text-sm text-gray-600">
                    Quế Trà My • Sao đen • Dầu rái • Lát hoa • Giáng hương
                </div>
            </div>

            <!-- LƯỚI SẢN PHẨM 2 CỘT MOBILE / 4 CỘT DESKTOP -->
            <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-3 sm:gap-5">
                <!-- SP Lâm nghiệp 1 -->
                <div class="product-card bg-white border border-gray-200 rounded overflow-hidden flex flex-col justify-between" data-name="Cây Quế Trà My Giống">
                    <div>
                        <div class="product-thumb-wrapper">
                            <img src="https://images.unsplash.com/photo-1542601906990-b4d3fb778b09?auto=format&fit=crop&w=600&q=80" alt="Cây Quế Trà My Giống">
                        </div>
                        <div class="p-3 text-center">
                            <h3 class="text-sm sm:text-base font-semibold text-gray-800 hover:text-brand-dark line-clamp-2">
                                Cây Quế Trà My Giống Chuẩn
                            </h3>
                            <p class="text-xs text-gray-500 mt-1">Hàm lượng tinh dầu cao, hợp đất đồi</p>
                            <p class="text-brand-dark font-bold text-sm sm:text-base mt-1.5">2.500 ₫ / cây</p>
                        </div>
                    </div>
                    <div class="px-3 pb-3">
                        <button onclick="openOrderModal('Cây Quế Trà My Giống Chuẩn', '2.500 ₫ / cây')" class="w-full border border-brand-dark text-brand-dark hover:bg-brand-dark hover:text-white text-xs sm:text-sm font-semibold py-2 rounded transition">
                            Đặt cây tại vườn
                        </button>
                    </div>
                </div>

                <!-- SP Lâm nghiệp 2 -->
                <div class="product-card bg-white border border-gray-200 rounded overflow-hidden flex flex-col justify-between" data-name="Cây Sao Đen Lâm Nghiệp">
                    <div>
                        <div class="product-thumb-wrapper">
                            <img src="https://images.unsplash.com/photo-1502082553048-f009c37129b9?auto=format&fit=crop&w=600&q=80" alt="Cây Sao Đen Lâm Nghiệp">
                        </div>
                        <div class="p-3 text-center">
                            <h3 class="text-sm sm:text-base font-semibold text-gray-800 hover:text-brand-dark line-clamp-2">
                                Cây Sao Đen Giống Lâm Nghiệp
                            </h3>
                            <p class="text-xs text-gray-500 mt-1">Cây gỗ lớn bền vững, trồng xen keo</p>
                            <p class="text-brand-dark font-bold text-sm sm:text-base mt-1.5">3.500 ₫ / cây</p>
                        </div>
                    </div>
                    <div class="px-3 pb-3">
                        <button onclick="openOrderModal('Cây Sao Đen Giống Lâm Nghiệp', '3.500 ₫ / cây')" class="w-full border border-brand-dark text-brand-dark hover:bg-brand-dark hover:text-white text-xs sm:text-sm font-semibold py-2 rounded transition">
                            Đặt cây tại vườn
                        </button>
                    </div>
                </div>

                <!-- SP Lâm nghiệp 3 -->
                <div class="product-card bg-white border border-gray-200 rounded overflow-hidden flex flex-col justify-between" data-name="Cây Dầu Rái Giống">
                    <div>
                        <div class="product-thumb-wrapper">
                            <img src="https://images.unsplash.com/photo-1448375240586-882707db888b?auto=format&fit=crop&w=600&q=80" alt="Cây Dầu Rái Giống">
                        </div>
                        <div class="p-3 text-center">
                            <h3 class="text-sm sm:text-base font-semibold text-gray-800 hover:text-brand-dark line-clamp-2">
                                Cây Dầu Rái Giống
                            </h3>
                            <p class="text-xs text-gray-500 mt-1">Thân thẳng, chịu hạn, giá trị gỗ cao</p>
                            <p class="text-brand-dark font-bold text-sm sm:text-base mt-1.5">3.500 ₫ / cây</p>
                        </div>
                    </div>
                    <div class="px-3 pb-3">
                        <button onclick="openOrderModal('Cây Dầu Rái Giống', '3.500 ₫ / cây')" class="w-full border border-brand-dark text-brand-dark hover:bg-brand-dark hover:text-white text-xs sm:text-sm font-semibold py-2 rounded transition">
                            Đặt cây tại vườn
                        </button>
                    </div>
                </div>

                <!-- SP Lâm nghiệp 4 -->
                <div class="product-card bg-white border border-gray-200 rounded overflow-hidden flex flex-col justify-between" data-name="Cây Lát Hoa Giống">
                    <div>
                        <div class="product-thumb-wrapper">
                            <img src="https://images.unsplash.com/photo-1513836279014-a89f7a76ae86?auto=format&fit=crop&w=600&q=80" alt="Cây Lát Hoa Giống">
                        </div>
                        <div class="p-3 text-center">
                            <h3 class="text-sm sm:text-base font-semibold text-gray-800 hover:text-brand-dark line-clamp-2">
                                Cây Lát Hoa Giống (Gỗ Lát)
                            </h3>
                            <p class="text-xs text-gray-500 mt-1">Phát triển nhanh, vân gỗ đẹp có giá trị</p>
                            <p class="text-brand-dark font-bold text-sm sm:text-base mt-1.5">3.500 ₫ / cây</p>
                        </div>
                    </div>
                    <div class="px-3 pb-3">
                        <button onclick="openOrderModal('Cây Lát Hoa Giống (Gỗ Lát)', '3.500 ₫ / cây')" class="w-full border border-brand-dark text-brand-dark hover:bg-brand-dark hover:text-white text-xs sm:text-sm font-semibold py-2 rounded transition">
                            Đặt cây tại vườn
                        </button>
                    </div>
                </div>

                <!-- SP Lâm nghiệp 5 -->
                <div class="product-card bg-white border border-gray-200 rounded overflow-hidden flex flex-col justify-between" data-name="Cây Giáng Hương Giống">
                    <div>
                        <div class="product-thumb-wrapper">
                            <img src="https://images.unsplash.com/photo-1473448912268-2022ce9509d8?auto=format&fit=crop&w=600&q=80" alt="Cây Giáng Hương Giống">
                        </div>
                        <div class="p-3 text-center">
                            <h3 class="text-sm sm:text-base font-semibold text-gray-800 hover:text-brand-dark line-clamp-2">
                                Cây Giáng Hương Giống
                            </h3>
                            <p class="text-xs text-gray-500 mt-1">Cây gỗ quý nhóm 1 & cây công trình</p>
                            <p class="text-brand-dark font-bold text-sm sm:text-base mt-1.5">3.500 ₫ / cây</p>
                        </div>
                    </div>
                    <div class="px-3 pb-3">
                        <button onclick="openOrderModal('Cây Giáng Hương Giống', '3.500 ₫ / cây')" class="w-full border border-brand-dark text-brand-dark hover:bg-brand-dark hover:text-white text-xs sm:text-sm font-semibold py-2 rounded transition">
                            Đặt cây tại vườn
                        </button>
                    </div>
                </div>

                <!-- SP Lâm nghiệp 6 -->
                <div class="product-card bg-white border border-gray-200 rounded overflow-hidden flex flex-col justify-between" data-name="Cây Xà Cừ Giống">
                    <div>
                        <div class="product-thumb-wrapper">
                            <img src="https://images.unsplash.com/photo-1509316975850-ff9c5deb0cd9?auto=format&fit=crop&w=600&q=80" alt="Cây Xà Cừ Giống">
                        </div>
                        <div class="p-3 text-center">
                            <h3 class="text-sm sm:text-base font-semibold text-gray-800 hover:text-brand-dark line-clamp-2">
                                Cây Xà Cừ Giống (Lấy Gỗ & Bóng Mát)
                            </h3>
                            <p class="text-xs text-gray-500 mt-1">Sức sống mạnh, thích nghi mọi loại đất</p>
                            <p class="text-brand-dark font-bold text-sm sm:text-base mt-1.5">3.500 ₫ / cây</p>
                        </div>
                    </div>
                    <div class="px-3 pb-3">
                        <button onclick="openOrderModal('Cây Xà Cừ Giống', '3.500 ₫ / cây')" class="w-full border border-brand-dark text-brand-dark hover:bg-brand-dark hover:text-white text-xs sm:text-sm font-semibold py-2 rounded transition">
                            Đặt cây tại vườn
                        </button>
                    </div>
                </div>

                <!-- SP Lâm nghiệp 7 -->
                <div class="product-card bg-white border border-gray-200 rounded overflow-hidden flex flex-col justify-between" data-name="Cây Phi Lao Chắn Gió">
                    <div>
                        <div class="product-thumb-wrapper">
                            <img src="https://images.unsplash.com/photo-1511497584788-876760111969?auto=format&fit=crop&w=600&q=80" alt="Cây Phi Lao Chắn Gió">
                        </div>
                        <div class="p-3 text-center">
                            <h3 class="text-sm sm:text-base font-semibold text-gray-800 hover:text-brand-dark line-clamp-2">
                                Cây Phi Lao Giống Rừng Phòng Hộ
                            </h3>
                            <p class="text-xs text-gray-500 mt-1">Chắn cát, chắn gió ven biển miền Trung</p>
                            <p class="text-brand-dark font-bold text-sm sm:text-base mt-1.5">3.000 ₫ / cây</p>
                        </div>
                    </div>
                    <div class="px-3 pb-3">
                        <button onclick="openOrderModal('Cây Phi Lao Giống Rừng Phòng Hộ', '3.000 ₫ / cây')" class="w-full border border-brand-dark text-brand-dark hover:bg-brand-dark hover:text-white text-xs sm:text-sm font-semibold py-2 rounded transition">
                            Đặt cây tại vườn
                        </button>
                    </div>
                </div>

                <!-- SP Lâm nghiệp 8 -->
                <div class="product-card bg-white border border-gray-200 rounded overflow-hidden flex flex-col justify-between" data-name="Cây Gáo Vàng Giống">
                    <div>
                        <div class="product-thumb-wrapper">
                            <img src="https://images.unsplash.com/photo-1523348837708-15d4a09cfac2?auto=format&fit=crop&w=600&q=80" alt="Cây Gáo Vàng Giống">
                        </div>
                        <div class="p-3 text-center">
                            <h3 class="text-sm sm:text-base font-semibold text-gray-800 hover:text-brand-dark line-clamp-2">
                                Cây Gáo Vàng Giống (Thiên Ngân)
                            </h3>
                            <p class="text-xs text-gray-500 mt-1">Tốc độ sinh trưởng nhanh, ưa đất ẩm</p>
                            <p class="text-brand-dark font-bold text-sm sm:text-base mt-1.5">2.700 ₫ / cây</p>
                        </div>
                    </div>
                    <div class="px-3 pb-3">
                        <button onclick="openOrderModal('Cây Gáo Vàng Giống (Thiên Ngân)', '2.700 ₫ / cây')" class="w-full border border-brand-dark text-brand-dark hover:bg-brand-dark hover:text-white text-xs sm:text-sm font-semibold py-2 rounded transition">
                            Đặt cây tại vườn
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- =====================================================================
         7. SECTION: KẾT NỐI VƯỜN ƯƠM UY TÍN (Theo yêu cầu chuyên môn)
    ====================================================================== -->
    <section id="ket-noi-vuon-uom" class="py-10 bg-brand-bg border-t border-b border-gray-200">
        <div class="fs-container">
            <div class="fs-section-title">
                <h2 class="text-lg sm:text-xl">HỆ THỐNG KẾT NỐI VƯỜN ƯƠM UY TÍN</h2>
            </div>

            <p class="text-gray-700 text-sm sm:text-base mb-6 leading-relaxed">
                <strong>Phát Lộc Forest</strong> xây dựng mạng lưới liên kết chặt chẽ với các vườn ươm đạt chuẩn tại Đà Nẵng, Quảng Nam và khu vực Miền Trung – Tây Nguyên. Chúng tôi kiểm soát đồng bộ từ cây đầu dòng, quy trình đóng bầu, đảo cây đến khâu bốc xếp vận chuyển:
            </p>

            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-4">
                <div class="bg-white p-5 rounded border border-gray-200">
                    <div class="text-brand-dark font-extrabold text-2xl mb-2">01.</div>
                    <h3 class="font-bold text-brand-dark text-base uppercase">Thẩm Định Nguồn Giống</h3>
                    <p class="text-gray-600 text-xs sm:text-sm mt-1.5 leading-relaxed">
                        Chỉ liên kết với vườn ươm có vườn cây đầu dòng rõ ràng, cây mô/hom đúng dòng BV, AH, có hồ sơ chứng nhận lô giống.
                    </p>
                </div>

                <div class="bg-white p-5 rounded border border-gray-200">
                    <div class="text-brand-dark font-extrabold text-2xl mb-2">02.</div>
                    <h3 class="font-bold text-brand-dark text-base uppercase">Huấn Luyện Cây Xuất Vườn</h3>
                    <p class="text-gray-600 text-xs sm:text-sm mt-1.5 leading-relaxed">
                        Cây đủ tuổi (chiều cao 25–35cm), thân hóa gỗ cứng cáp, đã đảo bầu cắt rễ và dãi nắng hoàn toàn trước khi giao.
                    </p>
                </div>

                <div class="bg-white p-5 rounded border border-gray-200">
                    <div class="text-brand-dark font-extrabold text-2xl mb-2">03.</div>
                    <h3 class="font-bold text-brand-dark text-base uppercase">Tối Ưu Cự Ly Giao Nhận</h3>
                    <p class="text-gray-600 text-xs sm:text-sm mt-1.5 leading-relaxed">
                        Điều phối cây từ vườn ươm liên kết gần khu vực trồng rừng của khách hàng nhất để giảm chi phí vận chuyển và giữ cây tươi khỏe.
                    </p>
                </div>

                <div class="bg-white p-5 rounded border border-gray-200">
                    <div class="text-brand-dark font-extrabold text-2xl mb-2">04.</div>
                    <h3 class="font-bold text-brand-dark text-base uppercase">Hợp Tác Bao Tiêu Đầu Ra</h3>
                    <p class="text-gray-600 text-xs sm:text-sm mt-1.5 leading-relaxed">
                        Các chủ vườn ươm tham gia mạng lưới Phát Lộc Forest được hỗ trợ phân phối sản lượng ổn định qua hệ thống điểm bán.
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- =====================================================================
         8. SECTION: HƯỚNG DẪN MỞ ĐIỂM BÁN 0 ĐỒNG (Trọng tâm chiến lược)
    ====================================================================== -->
    <section id="mo-diem-ban" class="py-10 bg-white">
        <div class="fs-container">
            <div class="fs-section-title">
                <h2 class="text-lg sm:text-xl">HƯỚNG DẪN MỞ ĐIỂM BÁN CÂY GIỐNG 0 ĐỒNG</h2>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 items-start">
                <!-- Cột trái: Hướng dẫn chi tiết 4 bước -->
                <div class="lg:col-span-7 space-y-4">
                    <p class="text-gray-700 text-sm sm:text-base leading-relaxed">
                        Nhằm giúp bà con nông dân tiếp cận nguồn keo giống chuẩn ngay tại địa phương, <strong>CÔNG TY TNHH PHÁT LỘC FOREST</strong> triển khai chương trình <strong>“Mở Điểm Bán Cây Giống 0 Đồng”</strong> dành cho các đại lý vật tư nông nghiệp, chủ rừng hoặc cá nhân có mặt bằng tại các xã miền núi, trung du:
                    </p>

                    <div class="space-y-3 pt-2">
                        <div class="p-4 rounded bg-brand-bg border border-gray-200 flex gap-3.5">
                            <div class="w-9 h-9 rounded bg-brand-dark text-white font-bold flex items-center justify-center shrink-0">1</div>
                            <div>
                                <h3 class="font-bold text-brand-dark text-sm sm:text-base">Không Cần Vốn Nhập Hàng Trước (0 Đồng Vốn)</h3>
                                <p class="text-xs sm:text-sm text-gray-600 mt-1">
                                    Điểm bán được cấp cây mẫu trưng bày và bảng báo giá chuẩn từ Phát Lộc Forest. Khi có đơn đặt hàng của bà con, vườn ươm sẽ xuất giao cây trực tiếp về điểm bán hoặc chân rừng.
                                </p>
                            </div>
                        </div>

                        <div class="p-4 rounded bg-brand-bg border border-gray-200 flex gap-3.5">
                            <div class="w-9 h-9 rounded bg-brand-dark text-white font-bold flex items-center justify-center shrink-0">2</div>
                            <div>
                                <h3 class="font-bold text-brand-dark text-sm sm:text-base">Hỗ Trợ Bảng Hiệu & Truyền Thông Tìm Khách</h3>
                                <p class="text-xs sm:text-sm text-gray-600 mt-1">
                                    Cung cấp miễn phí bạt/bảng hiệu “Điểm Phân Phối Keo Giống Phát Lộc Forest”, tài liệu nhận biết cây mô – cây hom và chuyển giao khách hàng đặt qua Fanpage/Website về đúng điểm bán tại xã.
                                </p>
                            </div>
                        </div>

                        <div class="p-4 rounded bg-brand-bg border border-gray-200 flex gap-3.5">
                            <div class="w-9 h-9 rounded bg-brand-dark text-white font-bold flex items-center justify-center shrink-0">3</div>
                            <div>
                                <h3 class="font-bold text-brand-dark text-sm sm:text-base">Hướng Dẫn Kỹ Thuật Bảo Quản & Chăm Sóc Cây</h3>
                                <p class="text-xs sm:text-sm text-gray-600 mt-1">
                                    Đội ngũ kỹ thuật hướng dẫn chi tiết cách xếp bầu, tưới giữ ẩm tại điểm tập kết và kỹ thuật bón lót, trồng dặm để tư vấn cho người mua.
                                </p>
                            </div>
                        </div>

                        <div class="p-4 rounded bg-brand-bg border border-gray-200 flex gap-3.5">
                            <div class="w-9 h-9 rounded bg-brand-orange text-white font-bold flex items-center justify-center shrink-0">4</div>
                            <div>
                                <h3 class="font-bold text-brand-dark text-sm sm:text-base">Chiết Khấu Rõ Ràng & Đồng Hành Lâu Dài</h3>
                                <p class="text-xs sm:text-sm text-gray-600 mt-1">
                                    Chính sách hoa hồng minh bạch theo từng vạn cây xuất bán, bảo vệ khu vực độc quyền cấp thôn/xã cho đối tác điểm bán.
                                </p>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Cột phải: Form đăng ký mở điểm bán 0đ / Kết nối vườn ươm -->
                <div class="lg:col-span-5 bg-brand-bg p-6 rounded border-2 border-brand-dark">
                    <h3 class="text-lg font-extrabold text-brand-dark uppercase text-center">
                        ĐĂNG KÝ MỞ ĐIỂM BÁN 0 ĐỒNG
                    </h3>
                    <p class="text-xs text-center text-gray-600 mt-1 mb-4">
                        Hoặc liên hệ trực tiếp Hotline/Zalo: <strong class="text-brand-orange">0788.583.898</strong>
                    </p>

                    <form onsubmit="submitPartnerForm(event)" class="space-y-3">
                        <div>
                            <label class="block text-xs font-semibold text-gray-700 mb-1">Họ và tên anh/chị *</label>
                            <input type="text" id="partnerName" required placeholder="Nhập họ và tên..." class="w-full border border-gray-300 rounded px-3 py-2 text-sm bg-white focus:outline-none focus:border-brand-dark">
                        </div>
                        <div>
                            <label class="block text-xs font-semibold text-gray-700 mb-1">Số điện thoại / Zalo *</label>
                            <input type="tel" id="partnerPhone" required placeholder="Ví dụ: 09xx.xxx.xxx" class="w-full border border-gray-300 rounded px-3 py-2 text-sm bg-white focus:outline-none focus:border-brand-dark">
                        </div>
                        <div>
                            <label class="block text-xs font-semibold text-gray-700 mb-1">Khu vực (Xã/Huyện/Tỉnh) *</label>
                            <input type="text" id="partnerArea" required placeholder="Nhập địa chỉ dự kiến mở điểm bán..." class="w-full border border-gray-300 rounded px-3 py-2 text-sm bg-white focus:outline-none focus:border-brand-dark">
                        </div>
                        <div>
                            <label class="block text-xs font-semibold text-gray-700 mb-1">Nhu cầu hợp tác</label>
                            <select id="partnerType" class="w-full border border-gray-300 rounded px-3 py-2 text-sm bg-white focus:outline-none focus:border-brand-dark">
                                <option value="Đăng ký mở Điểm Bán Cây Giống 0 Đồng">Đăng ký mở Điểm Bán Cây Giống 0 Đồng</option>
                                <option value="Chủ vườn ươm đăng ký kết nối đầu ra">Chủ vườn ươm đăng ký kết nối đầu ra</option>
                                <option value="Đặt mua keo giống số lượng lớn trồng rừng">Đặt mua keo giống số lượng lớn trồng rừng</option>
                            </select>
                        </div>
                        <button type="submit" class="w-full bg-brand-orange hover:opacity-95 text-white font-bold text-sm uppercase py-3 rounded transition shadow">
                            GỬI ĐĂNG KÝ NGAY
                        </button>
                    </form>
                    <div id="partnerSuccessMsg" class="hidden mt-3 p-3 bg-green-100 border border-green-300 text-brand-dark text-xs rounded"></div>
                </div>
            </div>
        </div>
    </section>

    <!-- =====================================================================
         9. SECTION: DỰ ÁN & HÌNH ẢNH THỰC TẾ TRÊN FACEBOOK ĐƯA LÊN WEB
    ====================================================================== -->
    <section id="du-an-thuc-te" class="py-10 bg-brand-bg border-t border-gray-200">
        <div class="fs-container">
            <div class="fs-section-title flex-wrap gap-2">
                <h2 class="text-lg sm:text-xl">DỰ ÁN & HÌNH ẢNH XUẤT VƯỜN THỰC TẾ</h2>
                <a href="https://www.facebook.com/phatlocforest" target="_blank" rel="noopener noreferrer" class="text-xs sm:text-sm font-semibold text-brand-dark hover:underline">
                    Xem thêm trên Facebook Phát Lộc Forest <i class="fa-solid fa-up-right-from-square ml-1"></i>
                </a>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
                <!-- Dự án 1 -->
                <article class="bg-white border border-gray-200 rounded overflow-hidden">
                    <div class="h-52 overflow-hidden bg-gray-100">
                        <img src="https://images.unsplash.com/photo-1592150621744-aca64f48394a?auto=format&fit=crop&w=700&q=80" alt="Xuất vườn lô keo lai mô BV10 & AH1" class="w-full h-full object-cover">
                    </div>
                    <div class="p-4">
                        <h3 class="font-bold text-brand-dark text-base hover:text-brand-orange transition">
                            Xuất Vườn Lô Keo Mô & Keo Hom Phục Vụ Vụ Trồng Rừng Mới
                        </h3>
                        <p class="text-gray-600 text-xs sm:text-sm mt-2 leading-relaxed">
                            Kiểm tra bầu rễ trắng khỏe, thân cứng cáp và bốc xếp lên xe tải bàn giao tận chân lô rừng cho các hộ trồng rừng tại khu vực Quảng Nam – Đà Nẵng.
                        </p>
                    </div>
                </article>

                <!-- Dự án 2 -->
                <article class="bg-white border border-gray-200 rounded overflow-hidden">
                    <div class="h-52 overflow-hidden bg-gray-100">
                        <img src="https://images.unsplash.com/photo-1530836369250-ef72a3f5cda8?auto=format&fit=crop&w=700&q=80" alt="Liên kết vườn ươm đạt chuẩn" class="w-full h-full object-cover">
                    </div>
                    <div class="p-4">
                        <h3 class="font-bold text-brand-dark text-base hover:text-brand-orange transition">
                            Chuẩn Hóa Quy Trình Đảo Bầu & Huấn Luyện Cây Tại Vườn Ươm Liên Kết
                        </h3>
                        <p class="text-gray-600 text-xs sm:text-sm mt-2 leading-relaxed">
                            Đội ngũ Phát Lộc Forest trực tiếp kiểm định chất lượng luống cây keo giống tại hệ thống vườn ươm vệ tinh trước khi đưa vào mạng lưới phân phối.
                        </p>
                    </div>
                </article>

                <!-- Dự án 3 -->
                <article class="bg-white border border-gray-200 rounded overflow-hidden">
                    <div class="h-52 overflow-hidden bg-gray-100">
                        <img src="https://images.unsplash.com/photo-1542601906990-b4d3fb778b09?auto=format&fit=crop&w=700&q=80" alt="Khai trương điểm bán cây giống 0 đồng" class="w-full h-full object-cover">
                    </div>
                    <div class="p-4">
                        <h3 class="font-bold text-brand-dark text-base hover:text-brand-orange transition">
                            Đồng Hành Cùng Đối Tác Mở Điểm Bán Cây Giống 0 Đồng Tại Các Xã
                        </h3>
                        <p class="text-gray-600 text-xs sm:text-sm mt-2 leading-relaxed">
                            Lắp đặt bảng hiệu, tập huấn kỹ thuật phân biệt giống keo chuẩn và bàn giao lô cây mẫu đầu tiên cho các điểm bán liên kết của Phát Lộc Forest.
                        </p>
                    </div>
                </article>
            </div>
        </div>
    </section>

    <!-- =====================================================================
         10. SECTION: BÀI VIẾT KỸ THUẬT TRỒNG RỪNG (Giống Bài Viết Nổi Bật caygiong4s)
    ====================================================================== -->
    <section class="py-10 bg-white">
        <div class="fs-container">
            <div class="fs-section-title">
                <h2 class="text-lg sm:text-xl">BÀI VIẾT & KỸ THUẬT TRỒNG KEO NĂNG SUẤT CAO</h2>
            </div>

            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-5">
                <div class="border border-gray-200 rounded overflow-hidden bg-white">
                    <img src="https://images.unsplash.com/photo-1466692476868-aef1dfb1e735?auto=format&fit=crop&w=500&q=80" alt="So sánh keo mô và keo hom" class="w-full h-40 object-cover">
                    <div class="p-3.5">
                        <h3 class="font-bold text-gray-800 text-sm hover:text-brand-dark line-clamp-2">
                            Phân Biệt Keo Lai Nuôi Cấy Mô Và Keo Lai Giâm Hom Khi Trồng Rừng Gỗ Lớn
                        </h3>
                        <p class="text-xs text-gray-500 mt-1.5 line-clamp-2">
                            Hướng dẫn bà con lựa chọn dòng keo phù hợp với địa hình đồi dốc, vùng hay có gió bão để đạt trữ lượng gỗ cao nhất...
                        </p>
                    </div>
                </div>

                <div class="border border-gray-200 rounded overflow-hidden bg-white">
                    <img src="https://images.unsplash.com/photo-1585320806297-9794b3e4eeae?auto=format&fit=crop&w=500&q=80" alt="Mật độ trồng keo" class="w-full h-40 object-cover">
                    <div class="p-3.5">
                        <h3 class="font-bold text-gray-800 text-sm hover:text-brand-dark line-clamp-2">
                            Khoảng Cách & Mật Độ Trồng Keo Chuẩn Kỹ Thuật Lâm Nghiệp Hiện Nay
                        </h3>
                        <p class="text-xs text-gray-500 mt-1.5 line-clamp-2">
                            Cách tính số lượng cây giống cần đặt trên 1 hecta đất rừng theo mục đích trồng rừng gỗ dăm hay rừng gỗ xẻ...
                        </p>
                    </div>
                </div>

                <div class="border border-gray-200 rounded overflow-hidden bg-white">
                    <img src="https://images.unsplash.com/photo-1523348837708-15d4a09cfac2?auto=format&fit=crop&w=500&q=80" alt="Phòng bệnh chết héo keo" class="w-full h-40 object-cover">
                    <div class="p-3.5">
                        <h3 class="font-bold text-gray-800 text-sm hover:text-brand-dark line-clamp-2">
                            Bí Quyết Chọn Giống Keo Kháng Bệnh Chết Héo (Ceratocystis) Hiệu Quả
                        </h3>
                        <p class="text-xs text-gray-500 mt-1.5 line-clamp-2">
                            Các dòng keo BV32, BV73, AH1, AH7 được tuyển chọn giúp hạn chế tối đa nấm bệnh gây hại trong mùa mưa ẩm...
                        </p>
                    </div>
                </div>

                <div class="border border-gray-200 rounded overflow-hidden bg-white">
                    <img src="https://images.unsplash.com/photo-1500651230702-0e2d8a49d4ad?auto=format&fit=crop&w=500&q=80" alt="Kinh nghiệm mở điểm bán cây giống" class="w-full h-40 object-cover">
                    <div class="p-3.5">
                        <h3 class="font-bold text-gray-800 text-sm hover:text-brand-dark line-clamp-2">
                            Quy Trình Mở Điểm Bán Cây Giống 0 Đồng Cùng Phát Lộc Forest Tại Địa Phương
                        </h3>
                        <p class="text-xs text-gray-500 mt-1.5 line-clamp-2">
                            Giải pháp tăng thu nhập bền vững vào mùa vụ trồng rừng mà không lo rủi ro tồn đọng vốn nhập cây...
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- =====================================================================
         11. FOOTER CHUẨN MẪU CAYGIONG4S.COM (4 Cột thông tin rõ ràng)
    ====================================================================== -->
    <footer id="lien-he" class="bg-brand-dark text-white pt-12 pb-20 sm:pb-8">
        <div class="fs-container">
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8 pb-8 border-b border-white/15 text-sm">
                
                <!-- Cột 1: Thông tin pháp lý Công ty -->
                <div class="space-y-2.5">
                    <h3 class="text-base font-extrabold uppercase text-amber-300 tracking-wide">
                        CÔNG TY TNHH PHÁT LỘC FOREST
                    </h3>
                    <p class="text-green-100 text-xs italic">
                        “Ươm mầm giá trị – Phát triển bền vững”
                    </p>
                    <ul class="space-y-2 text-gray-100 text-xs sm:text-sm pt-1">
                        <li><strong>- Mã số thuế:</strong> 4001334115</li>
                        <li><strong>- Địa chỉ:</strong> Thửa số 473, Tờ bản đồ số 31, Thôn Trung Hòa, Xã Đức Phú, TP Đà Nẵng</li>
                        <li><strong>- Hotline / Zalo:</strong> <a href="tel:0788583898" class="text-amber-300 font-bold hover:underline">0788.583.898</a></li>
                        <li><strong>- Website:</strong> <a href="https://phatlocforest.com" class="hover:underline">phatlocforest.com</a></li>
                        <li><strong>- Fanpage:</strong> <a href="https://www.facebook.com/phatlocforest" target="_blank" rel="noopener noreferrer" class="hover:underline">fb.com/phatlocforest</a></li>
                    </ul>
                </div>

                <!-- Cột 2: Sản phẩm & Dịch vụ -->
                <div class="space-y-2.5">
                    <h3 class="text-base font-extrabold uppercase text-amber-300 tracking-wide">
                        SẢN PHẨM & DỊCH VỤ
                    </h3>
                    <ul class="space-y-2 text-gray-100 text-xs sm:text-sm">
                        <li><a href="#keo-giong" class="hover:text-amber-300">- Chuyên keo lai nuôi cấy mô (BV, AH)</a></li>
                        <li><a href="#keo-giong" class="hover:text-amber-300">- Keo lai giâm hom tuyển chọn</a></li>
                        <li><a href="#keo-giong" class="hover:text-amber-300">- Keo tai tượng hạt ngoại Úc</a></li>
                        <li><a href="#cay-lam-nghiep" class="hover:text-amber-300">- Cây giống lâm nghiệp & gỗ quý</a></li>
                        <li><a href="#ket-noi-vuon-uom" class="hover:text-amber-300">- Kết nối mạng lưới vườn ươm uy tín</a></li>
                        <li><a href="#mo-diem-ban" class="hover:text-amber-300">- Hợp tác mở điểm bán cây giống 0 đồng</a></li>
                    </ul>
                </div>

                <!-- Cột 3: Hỗ trợ khách hàng & Chính sách -->
                <div class="space-y-2.5">
                    <h3 class="text-base font-extrabold uppercase text-amber-300 tracking-wide">
                        HỖ TRỢ BÀ CON & ĐỐI TÁC
                    </h3>
                    <ul class="space-y-2 text-gray-100 text-xs sm:text-sm">
                        <li><a href="#mo-diem-ban" class="hover:text-amber-300">- Hướng dẫn mở điểm bán 0 đồng</a></li>
                        <li><a href="#ket-noi-vuon-uom" class="hover:text-amber-300">- Chính sách liên kết vườn ươm</a></li>
                        <li><a href="#keo-giong" class="hover:text-amber-300">- Chính sách vận chuyển & giao cây tận nơi</a></li>
                        <li><a href="#keo-giong" class="hover:text-amber-300">- Cam kết chất lượng & bảo hành nguồn giống</a></li>
                        <li><a href="#du-an-thuc-te" class="hover:text-amber-300">- Kỹ thuật trồng & chăm sóc rừng keo</a></li>
                        <li>
                            <button onclick="openLogoModal()" class="text-amber-300 hover:underline text-left">
                                - Tải Logo Phát Lộc Forest (Đã xóa dải màu)
                            </button>
                        </li>
                    </ul>
                </div>

                <!-- Cột 4: Kết nối Zalo & Facebook -->
                <div class="space-y-3">
                    <h3 class="text-base font-extrabold uppercase text-amber-300 tracking-wide">
                        KẾT NỐI VỚI PHÁT LỘC FOREST
                    </h3>
                    <div class="bg-white/10 p-3.5 rounded border border-white/15 space-y-2.5">
                        <p class="font-bold text-sm text-white">Kênh tư vấn trực tuyến 24/7</p>
                        <p class="text-xs text-green-100">Cập nhật hình ảnh lô keo giống xuất vườn và hỗ trợ mở điểm bán 0 đồng mỗi ngày.</p>
                        <div class="flex flex-wrap gap-2 pt-1">
                            <a href="https://zalo.me/0788583898" target="_blank" rel="noopener noreferrer" class="inline-flex items-center gap-1.5 bg-[#0068FF] text-white font-bold text-xs px-3 py-2 rounded hover:opacity-90 transition">
                                <i class="fa-solid fa-comment-dots"></i> Chat Zalo
                            </a>
                            <a href="https://www.facebook.com/phatlocforest" target="_blank" rel="noopener noreferrer" class="inline-flex items-center gap-1.5 bg-[#1877F2] text-white font-bold text-xs px-3 py-2 rounded hover:opacity-90 transition">
                                <i class="fa-brands fa-facebook-f"></i> Fanpage Facebook
                            </a>
                        </div>
                    </div>
                    <p class="text-xs text-green-100">
                        <i class="fa-solid fa-location-dot text-amber-300 mr-1"></i> Thôn Trung Hòa, Xã Đức Phú, TP Đà Nẵng
                    </p>
                </div>

            </div>

            <!-- Bản quyền dưới cùng -->
            <div class="pt-5 flex flex-col sm:flex-row items-center justify-between text-xs text-green-100/80 gap-2">
                <p>© 2026 <strong>CÔNG TY TNHH PHÁT LỘC FOREST (phatlocforest.com)</strong>. All rights reserved.</p>
                <p>Hotline / Zalo: <strong>0788.583.898</strong></p>
            </div>
        </div>
    </footer>

    <!-- =====================================================================
         CỤM NÚT LIÊN HỆ NỔI (ZALO, FACEBOOK, GỌI ĐIỆN)
         - Trên máy tính: Nút nổi góc trái dưới
         - Trên điện thoại: Thanh liên hệ cố định dưới đáy gọn gàng, KHÔNG che chữ
    ====================================================================== -->
    <!-- Giao diện Máy tính (Desktop Floating Buttons) -->
    <div class="hidden sm:flex fixed bottom-5 left-5 z-40 flex-col gap-2.5">
        <a href="https://www.facebook.com/phatlocforest" target="_blank" rel="noopener noreferrer" class="bg-[#1877F2] hover:opacity-95 text-white font-bold text-sm px-4 py-2.5 rounded-full shadow-lg flex items-center gap-2 border-2 border-white transition">
            <span class="w-6 h-6 rounded-full bg-white text-[#1877F2] flex items-center justify-center shrink-0">
                <i class="fa-brands fa-facebook-f text-sm"></i>
            </span>
            <span>Facebook</span>
        </a>

        <a href="https://zalo.me/0788583898" target="_blank" rel="noopener noreferrer" class="bg-[#0068FF] hover:opacity-95 text-white font-bold text-sm px-4 py-2.5 rounded-full shadow-lg flex items-center gap-2 border-2 border-white transition">
            <span class="w-6 h-6 rounded-full bg-white text-[#0068FF] flex items-center justify-center shrink-0 font-extrabold text-[10px]">
                Zalo
            </span>
            <span>Chat Zalo</span>
        </a>

        <a href="tel:0788583898" class="bg-brand-dark hover:bg-brand-light text-white font-bold text-sm px-4 py-2.5 rounded-full shadow-lg flex items-center gap-2 border-2 border-white transition">
            <i class="fa-solid fa-phone-volume animate-pulse text-amber-300"></i>
            <span>0788.583.898</span>
        </a>
    </div>

    <!-- Giao diện Điện thoại (Thanh liên hệ cố định dưới đáy màn hình, không che nội dung bài viết) -->
    <div class="sm:hidden fixed bottom-0 inset-x-0 z-40 bg-white border-t border-gray-200 shadow-[0_-2px_10px_rgba(0,0,0,0.08)] grid grid-cols-3 gap-1.5 p-2">
        <a href="tel:0788583898" class="bg-brand-dark text-white font-bold text-xs py-2.5 rounded flex items-center justify-center gap-1.5 shadow-sm">
            <i class="fa-solid fa-phone-volume text-amber-300 animate-pulse"></i>
            <span>0788.583.898</span>
        </a>
        <a href="https://zalo.me/0788583898" target="_blank" rel="noopener noreferrer" class="bg-[#0068FF] text-white font-bold text-xs py-2.5 rounded flex items-center justify-center gap-1.5 shadow-sm">
            <i class="fa-solid fa-comment-dots"></i>
            <span>Chat Zalo</span>
        </a>
        <a href="https://www.facebook.com/phatlocforest" target="_blank" rel="noopener noreferrer" class="bg-[#1877F2] text-white font-bold text-xs py-2.5 rounded flex items-center justify-center gap-1.5 shadow-sm">
            <i class="fa-brands fa-facebook-f"></i>
            <span>Facebook</span>
        </a>
    </div>

    <!-- =====================================================================
         MODAL 1: ĐẶT CÂY GIỐNG NHANH (Không dùng alert)
    ====================================================================== -->
    <div id="orderModal" class="fixed inset-0 bg-black/60 z-50 hidden items-center justify-center p-4">
        <div class="bg-white rounded max-w-md w-full p-6 shadow-xl border border-gray-200 relative">
            <button onclick="closeOrderModal()" class="absolute top-3 right-3 text-gray-400 hover:text-gray-700 p-1">
                <i class="fa-solid fa-xmark text-xl"></i>
            </button>
            <h3 class="text-lg font-extrabold text-brand-dark uppercase">ĐẶT CÂY GIỐNG TẠI VƯỜN</h3>
            <p id="selectedProductTitle" class="text-sm font-bold text-brand-orange mt-1"></p>

            <form onsubmit="submitOrderForm(event)" class="space-y-3 mt-4">
                <div>
                    <label class="block text-xs font-semibold text-gray-700 mb-1">Họ và tên khách hàng *</label>
                    <input type="text" required placeholder="Nhập tên của bạn..." class="w-full border border-gray-300 rounded px-3 py-2 text-sm">
                </div>
                <div>
                    <label class="block text-xs font-semibold text-gray-700 mb-1">Số điện thoại liên hệ *</label>
                    <input type="tel" required placeholder="Nhập số điện thoại..." class="w-full border border-gray-300 rounded px-3 py-2 text-sm">
                </div>
                <div>
                    <label class="block text-xs font-semibold text-gray-700 mb-1">Số lượng cây dự kiến & Địa chỉ giao</label>
                    <input type="text" placeholder="Ví dụ: 15.000 cây giao về Đức Phú..." class="w-full border border-gray-300 rounded px-3 py-2 text-sm">
                </div>
                <button type="submit" class="w-full bg-brand-dark hover:bg-brand-light text-white font-bold text-sm uppercase py-2.5 rounded transition">
                    GỬI YÊU CẦU BÁO GIÁ
                </button>
            </form>
            <div id="orderSuccessBox" class="hidden mt-3 p-3 bg-green-100 text-brand-dark text-xs rounded font-medium">
                Cảm ơn quý khách! Phát Lộc Forest (0788.583.898) đã ghi nhận thông tin và sẽ liên hệ tư vấn ngay.
            </div>
        </div>
    </div>

    <!-- =====================================================================
         MODAL 2: XEM & TẢI LOGO PHÁT LỘC FOREST ĐÃ XÓA DẢI MÀU BÊN DƯỚI
    ====================================================================== -->
    <div id="logoModal" class="fixed inset-0 bg-black/60 z-50 hidden items-center justify-center p-4">
        <div class="bg-white rounded max-w-lg w-full p-6 shadow-xl border border-gray-200 relative text-center">
            <button onclick="closeLogoModal()" class="absolute top-3 right-3 text-gray-400 hover:text-gray-700 p-1">
                <i class="fa-solid fa-xmark text-xl"></i>
            </button>
            <h3 class="text-base sm:text-lg font-extrabold text-brand-dark uppercase">
                LOGO PHÁT LỘC FOREST (ĐÃ XÓA DẢI MÀU BÊN DƯỚI)
            </h3>
            <p class="text-xs text-gray-500 mt-1">
                Đã cắt bỏ hoàn toàn thanh 3 mã màu ở dưới cùng để bạn đưa thẳng lên Header Flatsome.
            </p>

            <!-- Bản xem trước Logo đầy đủ (Biểu tượng + Chữ + Slogan, không có dải màu) -->
            <div class="my-4 p-4 border border-gray-200 rounded bg-white flex justify-center">
                <svg id="fullCleanLogoSvg" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 600 450" class="w-full max-w-[360px] h-auto">
                    <rect width="600" height="450" fill="#ffffff"/>
                    <g transform="translate(190, 20)">
                        <!-- Vòng cung xanh đậm (#1E5B2E) -->
                        <path d="M 115 12 A 98 98 0 1 0 198 152 A 92 92 0 1 1 132 20 Z" fill="#1E5B2E"/>
                        <!-- Vòng cung cam (#F08A24) -->
                        <path d="M 96 20 A 94 94 0 0 1 192 162 A 98 98 0 0 0 115 12 Z" fill="#F08A24"/>
                        <!-- Chữ P xanh đậm -->
                        <path d="M 60 66 H 96 C 114 66 125 76 125 91 C 125 106 114 116 96 116 H 78 V 148 H 60 V 66 Z" fill="#1E5B2E"/>
                        <!-- Chiếc lá âm bản trong chữ P -->
                        <path d="M 74 114 C 74 92 86 80 106 80 C 106 98 95 108 77 109 C 81 98 89 91 98 87 C 87 90 78 98 74 114 Z" fill="#ffffff"/>
                        <!-- Chữ L cam -->
                        <path d="M 142 104 L 158 96 V 134 H 184 V 150 H 142 V 104 Z" fill="#F08A24"/>
                        <!-- Thân cây mầm -->
                        <path d="M 122 165 L 124 85 L 128 85 L 131 165 Z" fill="#1E5B2E"/>
                        <path d="M 125 126 L 111 110 L 114 108 L 126 121 Z" fill="#1E5B2E"/>
                        <path d="M 127 110 L 146 92 L 149 95 L 128 116 Z" fill="#1E5B2E"/>
                        <!-- 3 chiếc lá xanh non (#6FAF3A) -->
                        <path d="M 126 36 C 142 52 142 75 126 90 C 110 75 110 52 126 36 Z" fill="#6FAF3A"/>
                        <path d="M 126 44 V 88" stroke="#ffffff" stroke-width="1.5" stroke-linecap="round"/>
                        <path d="M 168 73 C 166 93 153 104 135 103 C 137 85 150 74 168 73 Z" fill="#6FAF3A"/>
                        <path d="M 161 78 L 137 101" stroke="#ffffff" stroke-width="1.4" stroke-linecap="round"/>
                        <path d="M 102 95 C 116 98 123 109 120 122 C 107 118 100 108 102 95 Z" fill="#6FAF3A"/>
                        <!-- Đồi đất -->
                        <path d="M 48 158 C 78 150 118 158 148 186 C 122 198 80 196 48 158 Z" fill="#1E5B2E"/>
                        <path d="M 88 189 C 106 178 126 178 144 189 C 126 196 106 196 88 189 Z" fill="#ffffff"/>
                        <path d="M 92 190 C 108 182 124 182 140 190 C 124 196 108 196 92 190 Z" fill="#1E5B2E"/>
                        <path d="M 134 168 C 150 160 168 162 180 168 C 172 180 160 187 149 190 C 144 181 139 174 134 168 Z" fill="#6FAF3A"/>
                    </g>
                    <!-- Dòng chữ PHÁT LỘC FOREST -->
                    <text x="300" y="325" text-anchor="middle" font-family="Inter, Arial, sans-serif" font-weight="800" font-size="48">
                        <tspan fill="#1E5B2E">PHÁT LỘC </tspan>
                        <tspan fill="#F08A24">FOREST</tspan>
                    </text>
                    <!-- Dòng slogan -->
                    <line x1="45" y1="368" x2="105" y2="368" stroke="#1E5B2E" stroke-width="2.5"/>
                    <text x="300" y="375" text-anchor="middle" font-family="Inter, Arial, sans-serif" font-weight="600" font-size="19" fill="#1E5B2E">
                        ƯƠM MẦM GIÁ TRỊ <tspan fill="#F08A24">–</tspan> PHÁT TRIỂN BỀN VỮNG
                    </text>
                    <line x1="495" y1="368" x2="555" y2="368" stroke="#1E5B2E" stroke-width="2.5"/>
                </svg>
            </div>

            <div class="flex flex-wrap justify-center gap-3">
                <button onclick="downloadCleanLogoPNG()" class="bg-brand-dark hover:bg-brand-light text-white font-bold text-xs sm:text-sm px-4 py-2.5 rounded transition flex items-center gap-2">
                    <i class="fa-solid fa-image"></i> Tải Logo .PNG (Nền Trắng Sạch)
                </button>
                <button onclick="downloadCleanLogoSVG()" class="bg-brand-orange hover:opacity-95 text-white font-bold text-xs sm:text-sm px-4 py-2.5 rounded transition flex items-center gap-2">
                    <i class="fa-solid fa-bezier-curve"></i> Tải Logo .SVG (Vector Sắc Nét)
                </button>
            </div>
        </div>
    </div>

    <!-- =====================================================================
         JAVASCRIPT XỬ LÝ TƯƠNG TÁC
    ====================================================================== -->
    <script>
        // Bật/tắt Menu Mobile
        function toggleMobileMenu() {
            const menu = document.getElementById('mobileMenu');
            menu.classList.toggle('hidden');
        }

        // Lọc sản phẩm theo danh mục keo
        function filterCategory(cat) {
            const cards = document.querySelectorAll('#keoProductGrid .product-card');
            cards.forEach(card => {
                if (cat === 'all' || card.dataset.cat === cat) {
                    card.classList.remove('hidden');
                } else {
                    card.classList.add('hidden');
                }
            });
        }

        // Tìm kiếm nhanh sản phẩm
        function filterProductsBySearch(keyword) {
            const q = keyword.trim().toLowerCase();
            const allCards = document.querySelectorAll('.product-card');
            allCards.forEach(card => {
                const name = (card.dataset.name || '').toLowerCase();
                if (!q || name.includes(q)) {
                    card.classList.remove('hidden');
                } else {
                    card.classList.add('hidden');
                }
            });
        }

        // Mở/đóng Modal Đặt hàng
        function openOrderModal(productName, price) {
            document.getElementById('selectedProductTitle').textContent = productName + ' — ' + price;
            document.getElementById('orderSuccessBox').classList.add('hidden');
            const modal = document.getElementById('orderModal');
            modal.classList.remove('hidden');
            modal.classList.add('flex');
        }

        function closeOrderModal() {
            const modal = document.getElementById('orderModal');
            modal.classList.add('hidden');
            modal.classList.remove('flex');
        }

        function submitOrderForm(e) {
            e.preventDefault();
            document.getElementById('orderSuccessBox').classList.remove('hidden');
            e.target.reset();
        }

        // Xử lý Form Đăng ký Mở Điểm Bán 0 Đồng
        function submitPartnerForm(e) {
            e.preventDefault();
            const name = document.getElementById('partnerName').value;
            const phone = document.getElementById('partnerPhone').value;
            const area = document.getElementById('partnerArea').value;
            const type = document.getElementById('partnerType').value;
            const msgBox = document.getElementById('partnerSuccessMsg');
            msgBox.innerHTML = `<strong>Đăng ký thành công!</strong> Cảm ơn anh/chị <strong>${name}</strong> (${phone} - ${area}) đã đăng ký <em>"${type}"</em>. Bộ phận phát triển điểm bán <strong>Phát Lộc Forest (0788.583.898)</strong> sẽ liên hệ hướng dẫn ngay!`;
            msgBox.classList.remove('hidden');
            e.target.reset();
        }

        // Mở/đóng Modal Tải Logo Đã Xóa Dải Màu
        function openLogoModal() {
            const modal = document.getElementById('logoModal');
            modal.classList.remove('hidden');
            modal.classList.add('flex');
        }

        function closeLogoModal() {
            const modal = document.getElementById('logoModal');
            modal.classList.add('hidden');
            modal.classList.remove('flex');
        }

        // Tải Logo sạch định dạng SVG
        function downloadCleanLogoSVG() {
            const svgEl = document.getElementById('fullCleanLogoSvg');
            const serializer = new XMLSerializer();
            const source = serializer.serializeToString(svgEl);
            const blob = new Blob([source], { type: 'image/svg+xml;charset=utf-8' });
            const url = URL.createObjectURL(blob);
            const a = document.createElement('a');
            a.href = url;
            a.download = 'logo-phatlocforest-clean.svg';
            document.body.appendChild(a);
            a.click();
            document.body.removeChild(a);
            URL.revokeObjectURL(url);
        }

        // Tải Logo sạch định dạng PNG (Đã xóa dải màu bên dưới)
        function downloadCleanLogoPNG() {
            const svgEl = document.getElementById('fullCleanLogoSvg');
            const serializer = new XMLSerializer();
            const svgString = serializer.serializeToString(svgEl);
            const canvas = document.createElement('canvas');
            canvas.width = 1200;
            canvas.height = 900;
            const ctx = canvas.getContext('2d');
            const img = new Image();
            const svgBlob = new Blob([svgString], { type: 'image/svg+xml;charset=utf-8' });
            const url = URL.createObjectURL(svgBlob);

            img.onload = function () {
                ctx.fillStyle = '#ffffff';
                ctx.fillRect(0, 0, canvas.width, canvas.height);
                ctx.drawImage(img, 0, 0, canvas.width, canvas.height);
                URL.revokeObjectURL(url);
                const pngUrl = canvas.toDataURL('image/png');
                const a = document.createElement('a');
                a.href = pngUrl;
                a.download = 'logo-phatlocforest-khong-dai-mau.png';
                document.body.appendChild(a);
                a.click();
                document.body.removeChild(a);
            };
            img.src = url;
        }
    </script>
</body>
</html>
