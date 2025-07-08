<html lang="id">
 <head>
  <meta charset="utf-8"/>
  <meta content="width=device-width, initial-scale=1" name="viewport"/>
  <title>
   Lenovo Indonesia | Laptop, Desktop, &amp; Solusi Bisnis
  </title>
  <script src="https://cdn.tailwindcss.com">
  </script>
  <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" rel="stylesheet"/>
  <style>
   @keyframes fadeIn {
        from {
          opacity: 0;
          transform: translateY(20px);
        }
        to {
          opacity: 1;
          transform: translateY(0);
        }
      }
      .fade-in {
        animation: fadeIn 0.5s ease-out forwards;
      }
      .nav-link:hover::after {
        width: 100%;
      }
      .nav-link::after {
        content: "";
        display: block;
        width: 0;
        height: 2px;
        background: #ffc72c;
        transition: width 0.3s;
      }
      .dropdown:hover .dropdown-menu {
        display: block;
      }
      .product-card:hover {
        transform: translateY(-5px);
        box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
      }
      .modal-overlay {
        transition: opacity 0.3s ease;
      }
      .modal-content {
        transition: transform 0.3s ease;
      }
      /* Marquee container */
      #promo-marquee {
        background: #ffc72c;
        color: black;
        font-weight: 700;
        overflow: hidden;
        white-space: nowrap;
        position: relative;
        height: 2.5rem;
        display: flex;
        align-items: center;
      }
      #promo-marquee span {
        display: inline-block;
        padding-left: 100%;
        animation: marquee 15s linear infinite;
      }
      @keyframes marquee {
        0% {
          transform: translateX(0%);
        }
        100% {
          transform: translateX(-100%);
        }
      }
      /* Cart badge */
      #cart-count {
        position: absolute;
        top: -6px;
        right: -6px;
        background: #ffc72c;
        color: black;
        font-weight: 700;
        font-size: 0.7rem;
        width: 18px;
        height: 18px;
        border-radius: 9999px;
        display: flex;
        align-items: center;
        justify-content: center;
      }
      /* Scrollbar for cart modal */
      #cart-items {
        max-height: 300px;
        overflow-y: auto;
      }
  </style>
 </head>
 <body class="bg-gray-50 font-sans">
  <!-- 1. Marquee Promo Text at top -->
  <div aria-label="Informasi promo berjalan" id="promo-marquee">
   <span>
    🔥 Promo Spesial Lenovo! Diskon hingga 30% untuk produk pilihan. Jangan lewatkan kesempatan ini! 🔥
   </span>
  </div>
  <header class="bg-black text-white sticky top-0 z-50 shadow-lg" style="border-top: 4px solid #FFC72C">
   <div class="container mx-auto px-4 py-3 flex justify-between items-center">
    <div class="flex items-center space-x-2">
     <img alt="Logo Lenovo warna emas dengan teks putih" class="h-8" src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/8dc9418c-c6c5-4e2c-ae2b-3605b19a351c.png"/>
    </div>
    <nav class="hidden md:flex space-x-8">
     <a class="nav-link font-medium hover:text-yellow-400 flex items-center space-x-2" href="#products">
      <i class="fas fa-box-open"></i>
      <span>Products</span>
     </a>
     <a class="nav-link font-medium hover:text-yellow-400 flex items-center space-x-2" href="#solutions">
      <i class="fas fa-lightbulb"></i>
      <span>Solutions</span>
     </a>
     <a class="nav-link font-medium hover:text-yellow-400 flex items-center space-x-2" href="#services">
      <i class="fas fa-bell"></i>
      <span>Services</span>
     </a>
     <a class="nav-link font-medium hover:text-yellow-400 flex items-center space-x-2" href="#support">
      <i class="fas fa-headset"></i>
      <span>Support</span>
     </a>
     <a class="nav-link font-medium hover:text-yellow-400 flex items-center space-x-2" href="#locations">
      <i class="fas fa-map-marker-alt"></i>
      <span>Lokasi Lenovo</span>
     </a>
    </nav>
    <div class="flex items-center space-x-4 relative">
     <div class="relative group" id="auth-section">
     </div>
     <button aria-label="Buka keranjang belanja" class="relative text-xl hover:text-yellow-400 focus:outline-none focus:ring-2 focus:ring-yellow-400 rounded" id="cart-button">
      <i class="fas fa-shopping-cart">
      </i>
      <span class="hidden" id="cart-count">
       0
      </span>
     </button>
     <button aria-label="Buka menu mobile" class="md:hidden text-xl" id="mobile-menu-button">
      <i class="fas fa-bars">
      </i>
     </button>
    </div>
   </div>
   <div class="md:hidden hidden bg-gray-900 px-4 py-2" id="mobile-menu">
    <a class="block py-2 text-white hover:text-yellow-400 flex items-center space-x-2" href="#products">
     <i class="fas fa-box-open"></i>
     <span>Products</span>
    </a>
    <a class="block py-2 text-white hover:text-yellow-400 flex items-center space-x-2" href="#solutions">
     <i class="fas fa-lightbulb"></i>
     <span>Solutions</span>
    </a>
    <a class="block py-2 text-white hover:text-yellow-400 flex items-center space-x-2" href="#services">
     <i class="fas fa-bell"></i>
     <span>Services</span>
    </a>
    <a class="block py-2 text-white hover:text-yellow-400 flex items-center space-x-2" href="#support">
     <i class="fas fa-headset"></i>
     <span>Support</span>
    </a>
    <a class="block py-2 text-white hover:text-yellow-400 flex items-center space-x-2" href="#locations">
     <i class="fas fa-map-marker-alt"></i>
     <span>Lokasi Lenovo</span>
    </a>
   </div>
  </header>
  <section class="relative bg-gradient-to-r from-black to-gray-900 text-white overflow-hidden">
   <div class="container mx-auto px-4 py-20 md:py-28 flex flex-col md:flex-row items-center">
    <div class="md:w-1/2 z-10 mb-10 md:mb-0 fade-in">
     <h1 class="text-4xl md:text-5xl font-bold mb-4">
      Smarter Technology For All
     </h1>
     <p class="text-lg md:text-xl mb-8 text-gray-300">
      Temukan perangkat andal untuk bekerja, belajar, dan bermain dengan performa terbaik dari Lenovo.
     </p>
     <div class="flex flex-wrap gap-4">
      <a class="bg-yellow-500 hover:bg-yellow-600 text-black font-bold py-3 px-6 rounded-lg transition duration-300" href="#products">
       Jelajahi Produk
      </a>
      <a class="border-2 border-white hover:bg-white hover:text-black font-bold py-3 px-6 rounded-lg transition duration-300" href="#promo">
       Promo Spesial
      </a>
     </div>
    </div>
    <div class="md:w-1/2 z-10 flex justify-center fade-in">
     <img alt="Lenovo Yoga Slim Pro laptop tipis dengan layar sentuh, keyboard backlit, dan desain premium warna abu-abu metalik" class="rounded-lg shadow-2xl max-w-full h-auto" src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/73225ea4-c861-4677-bcc9-1188e190dd68.png"/>
    </div>
   </div>
   <div class="absolute -right-32 -bottom-32 w-96 h-96 rounded-full bg-gradient-to-r from-yellow-500 to-yellow-600 opacity-20 blur-3xl">
   </div>
  </section>
  <section class="container mx-auto px-4 py-16">
   <h2 class="text-3xl font-bold text-center mb-6">
    Cari Produk
   </h2>
   <div class="max-w-md mx-auto mb-12">
    <input aria-label="Cari produk" class="w-full px-4 py-3 rounded-lg border border-gray-300 focus:outline-none focus:ring-2 focus:ring-yellow-500" id="search-input" placeholder="Cari produk berdasarkan nama..." type="text"/>
   </div>
   <h2 class="text-3xl font-bold text-center mb-12">
    Kategori Produk
   </h2>
   <div class="grid grid-cols-2 md:grid-cols-5 gap-6">
    <div class="product-card bg-white rounded-xl shadow-md overflow-hidden transition duration-300 hover:shadow-xl">
     <div class="h-48 bg-gray-100 flex items-center justify-center">
      <img alt="Lenovo ThinkPad X1 Carbon - laptop bisnis premium tipis warna hitam dengan layar 14 inci" class="h-full object-contain" src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/8af121c3-bd2d-4ff2-8a89-1947802ef7b1.png"/>
     </div>
     <div class="p-4">
      <h3 class="font-bold text-lg mb-2">
       Laptop &amp; Notebook
      </h3>
      <p class="text-gray-600">
       Untuk bekerja dan produktivitas
      </p>
     </div>
    </div>
    <div class="product-card bg-white rounded-xl shadow-md overflow-hidden transition duration-300 hover:shadow-xl">
     <div class="h-48 bg-gray-100 flex items-center justify-center">
      <img alt="Lenovo IdeaCentre AIO desktop all-in-one dengan layar besar tanpa bezel" class="h-full object-contain" src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/1115c8a1-9e5d-4236-b7c4-ace803b2ceb6.png"/>
     </div>
     <div class="p-4">
      <h3 class="font-bold text-lg mb-2">
       Desktop
      </h3>
      <p class="text-gray-600">
       Kinerja tinggi untuk berbagai kebutuhan
      </p>
     </div>
    </div>
    <div class="product-card bg-white rounded-xl shadow-md overflow-hidden transition duration-300 hover:shadow-xl">
     <div class="h-48 bg-gray-100 flex items-center justify-center">
      <img alt="Lenovo Legion monitor gaming 27 inci dengan refresh rate 165Hz dan layar curved" class="h-full object-contain" src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/610b1623-17b1-4011-bd79-cecece36a531.png"/>
     </div>
     <div class="p-4">
      <h3 class="font-bold text-lg mb-2">
       Monitor
      </h3>
      <p class="text-gray-600">
       Pengalaman visual yang mengagumkan
      </p>
     </div>
    </div>
    <div class="product-card bg-white rounded-xl shadow-md overflow-hidden transition duration-300 hover:shadow-xl">
     <div class="h-48 bg-gray-100 flex items-center justify-center">
      <img alt="Handphone Lenovo terbaru dengan desain modern dan layar besar" class="h-full object-contain" height="300" src="https://storage.googleapis.com/a1aa/image/5f47f741-9e1a-4b05-25e5-982622f1ac43.jpg" width="400"/>
     </div>
     <div class="p-4">
      <h3 class="font-bold text-lg mb-2">
       Handphone
      </h3>
      <p class="text-gray-600">
       Smartphone dengan teknologi terkini
      </p>
     </div>
    </div>
    <div class="product-card bg-white rounded-xl shadow-md overflow-hidden transition duration-300 hover:shadow-xl">
     <div class="h-48 bg-gray-100 flex items-center justify-center">
      <img alt="Berbagai aksesoris Lenovo termasuk mouse nirkabel, keyboard mekanis, dan docking station" class="h-full object-contain" src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/1254638a-0032-4b2c-8f7b-8c6848cc2d81.png"/>
     </div>
     <div class="p-4">
      <h3 class="font-bold text-lg mb-2">
       Accessories
      </h3>
      <p class="text-gray-600">
       Lengkapi pengalaman komputasi Anda
      </p>
     </div>
    </div>
   </div>
  </section>
  <section class="bg-yellow-50 py-12" id="promo">
   <div class="container mx-auto px-4">
    <div class="bg-white rounded-2xl shadow-lg overflow-hidden">
     <div class="md:flex">
      <div class="md:w-1/2 p-8 md:p-12 flex flex-col justify-center">
       <div class="flex items-center mb-4">
        <span class="bg-yellow-100 text-yellow-800 text-xs font-medium px-2.5 py-0.5 rounded mr-2">
         PROMO
        </span>
        <span class="text-sm text-gray-600" id="promo-countdown-text">
         Berakhir dalam:
        </span>
       </div>
       <h2 class="text-3xl font-bold mb-4">
        Diskon Spesial Hingga 30%
       </h2>
       <p class="text-gray-600 mb-6">
        Dapatkan produk Lenovo pilihan dengan harga terbaik, hanya untuk waktu terbatas!
       </p>
       <div aria-atomic="true" aria-live="polite" class="flex space-x-4 mb-8" id="countdown">
        <div class="text-center">
         <div aria-label="Hari" class="text-3xl font-bold text-gray-800" id="days">
          00
         </div>
         <div class="text-xs text-gray-500">
          Hari
         </div>
        </div>
        <div class="text-center">
         <div aria-label="Jam" class="text-3xl font-bold text-gray-800" id="hours">
          00
         </div>
         <div class="text-xs text-gray-500">
          Jam
         </div>
        </div>
        <div class="text-center">
         <div aria-label="Menit" class="text-3xl font-bold text-gray-800" id="minutes">
          00
         </div>
         <div class="text-xs text-gray-500">
          Menit
         </div>
        </div>
        <div class="text-center">
         <div aria-label="Detik" class="text-3xl font-bold text-gray-800" id="seconds">
          00
         </div>
         <div class="text-xs text-gray-500">
          Detik
         </div>
        </div>
       </div>
       <a class="bg-yellow-500 hover:bg-yellow-600 text-black font-bold py-3 px-6 rounded-lg w-max transition duration-300" href="#products">
        Beli Sekarang
       </a>
      </div>
      <div class="md:w-1/2 bg-gray-100 flex items-center justify-center p-8">
       <img alt="Lenovo Legion 5 Pro laptop gaming dengan diskon 30% dan animasi kilauan emas" class="rounded-lg shadow-md max-w-full h-auto transform hover:scale-105 transition duration-500" src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/12d3048b-be86-4be3-b676-39ac4dccd27b.png"/>
      </div>
     </div>
    </div>
   </div>
  </section>
  <section class="container mx-auto px-4 py-16" id="products">
   <div class="text-center mb-12">
    <h2 class="text-3xl font-bold mb-4">
     Produk Unggulan Lenovo
    </h2>
    <p class="text-gray-600 max-w-2xl mx-auto">
     Pilih perangkat yang sesuai dengan kebutuhan Anda, mulai dari
        produktivitas sehari-hari hingga performa tinggi untuk gaming dan
        kreativitas.
    </p>
   </div>
   <div class="mb-8 flex justify-center flex-wrap gap-2">
    <div aria-label="Filter kategori produk" class="inline-flex rounded-md shadow-sm" role="group">
     <button class="px-4 py-2 text-sm font-medium bg-black text-white rounded-l-lg focus:z-10 focus:ring-2 focus:ring-yellow-500 filter-btn active" data-filter="all" type="button">
      Semua Produk
     </button>
     <button class="px-4 py-2 text-sm font-medium bg-white border-t border-b border-gray-200 hover:bg-gray-50 focus:z-10 focus:ring-2 focus:ring-yellow-500 filter-btn" data-filter="laptop" type="button">
      Laptop
     </button>
     <button class="px-4 py-2 text-sm font-medium bg-white border-t border-b border-gray-200 hover:bg-gray-50 focus:z-10 focus:ring-2 focus:ring-yellow-500 filter-btn" data-filter="desktop" type="button">
      Desktop
     </button>
     <button class="px-4 py-2 text-sm font-medium bg-white border-t border-b border-gray-200 hover:bg-gray-50 focus:z-10 focus:ring-2 focus:ring-yellow-500 filter-btn" data-filter="monitor" type="button">
      Monitor
     </button>
     <button class="px-4 py-2 text-sm font-medium bg-white border border-gray-200 rounded-r-lg hover:bg-gray-50 focus:z-10 focus:ring-2 focus:ring-yellow-500 filter-btn" data-filter="accessories" type="button">
      Aksesoris
     </button>
    </div>
   </div>
   <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8" id="product-list">
    <!-- Laptop -->
    <div class="product-card bg-white rounded-xl shadow-md overflow-hidden transition duration-300 hover:shadow-xl group" data-category="laptop" data-img-src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/9a7c96b4-f496-49b1-8128-73e4a32e7bf7.png" data-name="ThinkPad X1 Carbon Gen 10" data-price="Rp22.499.000">
     <div class="relative">
      <img alt="Lenovo ThinkPad X1 Carbon Gen 10 laptop bisnis premium warna hitam dengan layar 14 inci dan keyboard merah khas ThinkPad" class="w-full h-64 object-contain p-4" src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/9a7c96b4-f496-49b1-8128-73e4a32e7bf7.png"/>
      <div aria-label="Tombol aksi produk ThinkPad X1 Carbon Gen 10" class="absolute top-3 right-3 flex flex-col space-y-2">
       <button aria-label="Tambahkan ke favorit" class="w-8 h-8 bg-white rounded-full shadow flex items-center justify-center text-gray-700 hover:bg-gray-100 favorite-btn" type="button">
        <i class="far fa-heart">
        </i>
       </button>
       <button aria-label="Bandingkan produk" class="w-8 h-8 bg-white rounded-full shadow flex items-center justify-center text-gray-700 hover:bg-gray-100 compare-btn" type="button">
        <i class="fas fa-exchange-alt">
        </i>
       </button>
      </div>
     </div>
     <div class="p-6">
      <div class="flex justify-between items-start mb-2">
       <div>
        <h3 class="font-bold text-lg">
         ThinkPad X1 Carbon Gen 10
        </h3>
        <div class="flex items-center mt-1">
         <div class="flex text-yellow-400 mr-2">
          <i class="fas fa-star">
          </i>
          <i class="fas fa-star">
          </i>
          <i class="fas fa-star">
          </i>
          <i class="fas fa-star">
          </i>
          <i class="fas fa-star-half-alt">
          </i>
         </div>
         <span class="text-sm text-gray-500">
          (42)
         </span>
        </div>
       </div>
      </div>
      <p class="text-gray-600 text-sm mb-4">
       Laptop bisnis ultra-ringan dengan performa tinggi dan daya tahan
            militer.
      </p>
      <div class="flex flex-wrap gap-2 mb-4">
       <span class="text-xs bg-gray-100 px-2 py-1 rounded">
        Intel Core i7
       </span>
       <span class="text-xs bg-gray-100 px-2 py-1 rounded">
        14" 4K
       </span>
       <span class="text-xs bg-gray-100 px-2 py-1 rounded">
        16GB RAM
       </span>
       <span class="text-xs bg-gray-100 px-2 py-1 rounded">
        512GB SSD
       </span>
      </div>
      <div class="flex items-center justify-between">
       <div>
        <span class="text-gray-400 line-through text-sm">
         Rp25.999.000
        </span>
        <p class="text-xl font-bold text-gray-900">
         Rp22.499.000
        </p>
       </div>
       <button class="buy-btn bg-black hover:bg-gray-800 text-white px-4 py-2 rounded-lg transition duration-300 flex items-center add-to-cart-btn" type="button">
        <i class="fas fa-cart-plus mr-2">
        </i>
        Tambah ke Keranjang
       </button>
      </div>
     </div>
    </div>
    <div class="product-card bg-white rounded-xl shadow-md overflow-hidden transition duration-300 hover:shadow-xl group" data-category="laptop" data-img-src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/df1886a9-2d08-4391-bb29-b61f0ba98117.png" data-name="Legion 5 Pro" data-price="Rp24.999.000">
     <div class="relative">
      <img alt="Lenovo Legion 5 Pro laptop gaming dengan layar 16 inci QHD dan keyboard RGB warna biru neon" class="w-full h-64 object-contain p-4" src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/df1886a9-2d08-4391-bb29-b61f0ba98117.png"/>
      <div aria-label="Tombol aksi produk Legion 5 Pro" class="absolute top-3 right-3 flex flex-col space-y-2">
       <button aria-label="Tambahkan ke favorit" class="w-8 h-8 bg-white rounded-full shadow flex items-center justify-center text-gray-700 hover:bg-gray-100 favorite-btn" type="button">
        <i class="far fa-heart">
        </i>
       </button>
       <button aria-label="Bandingkan produk" class="w-8 h-8 bg-white rounded-full shadow flex items-center justify-center text-gray-700 hover:bg-gray-100 compare-btn" type="button">
        <i class="fas fa-exchange-alt">
        </i>
       </button>
      </div>
     </div>
     <div class="p-6">
      <div class="flex justify-between items-start mb-2">
       <div>
        <h3 class="font-bold text-lg">
         Legion 5 Pro
        </h3>
        <div class="flex items-center mt-1">
         <div class="flex text-yellow-400 mr-2">
          <i class="fas fa-star">
          </i>
          <i class="fas fa-star">
          </i>
          <i class="fas fa-star">
          </i>
          <i class="fas fa-star">
          </i>
          <i class="far fa-star">
          </i>
         </div>
         <span class="text-sm text-gray-500">
          (36)
         </span>
        </div>
       </div>
      </div>
      <p class="text-gray-600 text-sm mb-4">
       Laptop gaming dengan layar QHD 165Hz dan performa terbaik di kelasnya.
      </p>
      <div class="flex flex-wrap gap-2 mb-4">
       <span class="text-xs bg-gray-100 px-2 py-1 rounded">
        AMD Ryzen 7
       </span>
       <span class="text-xs bg-gray-100 px-2 py-1 rounded">
        16" QHD
       </span>
       <span class="text-xs bg-gray-100 px-2 py-1 rounded">
        32GB RAM
       </span>
       <span class="text-xs bg-gray-100 px-2 py-1 rounded">
        1TB SSD
       </span>
      </div>
      <div class="flex items-center justify-between">
       <div>
        <span class="text-gray-400 line-through text-sm">
         Rp28.999.000
        </span>
        <p class="text-xl font-bold text-gray-900">
         Rp24.999.000
        </p>
       </div>
       <button class="buy-btn bg-black hover:bg-gray-800 text-white px-4 py-2 rounded-lg transition duration-300 flex items-center add-to-cart-btn" type="button">
        <i class="fas fa-cart-plus mr-2">
        </i>
        Tambah ke Keranjang
       </button>
      </div>
     </div>
    </div>
    <div class="product-card bg-white rounded-xl shadow-md overflow-hidden transition duration-300 hover:shadow-xl group" data-category="laptop" data-img-src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/deed4b44-74c5-4c65-b07e-c7b861060b55.png" data-name="Yoga Slim 7i" data-price="Rp15.999.000">
     <div class="relative">
      <img alt="Lenovo Yoga Slim 7i laptop ultra tipis warna abu-abu metalik dengan layar sentuh dan bodi ramping" class="w-full h-64 object-contain p-4" src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/deed4b44-74c5-4c65-b07e-c7b861060b55.png"/>
      <div aria-label="Tombol aksi produk Yoga Slim 7i" class="absolute top-3 right-3 flex flex-col space-y-2">
       <button aria-label="Tambahkan ke favorit" class="w-8 h-8 bg-white rounded-full shadow flex items-center justify-center text-gray-700 hover:bg-gray-100 favorite-btn" type="button">
        <i class="far fa-heart">
        </i>
       </button>
       <button aria-label="Bandingkan produk" class="w-8 h-8 bg-white rounded-full shadow flex items-center justify-center text-gray-700 hover:bg-gray-100 compare-btn" type="button">
        <i class="fas fa-exchange-alt">
        </i>
       </button>
      </div>
     </div>
     <div class="p-6">
      <div class="flex justify-between items-start mb-2">
       <div>
        <h3 class="font-bold text-lg">
         Yoga Slim 7i
        </h3>
        <div class="flex items-center mt-1">
         <div class="flex text-yellow-400 mr-2">
          <i class="fas fa-star">
          </i>
          <i class="fas fa-star">
          </i>
          <i class="fas fa-star">
          </i>
          <i class="fas fa-star">
          </i>
          <i class="fas fa-star">
          </i>
         </div>
         <span class="text-sm text-gray-500">
          (58)
         </span>
        </div>
       </div>
      </div>
      <p class="text-gray-600 text-sm mb-4">
       Laptop ultra-tipis dengan performa tangguh dan desain premium.
      </p>
      <div class="flex flex-wrap gap-2 mb-4">
       <span class="text-xs bg-gray-100 px-2 py-1 rounded">
        Intel Evo
       </span>
       <span class="text-xs bg-gray-100 px-2 py-1 rounded">
        14" FHD
       </span>
       <span class="text-xs bg-gray-100 px-2 py-1 rounded">
        16GB RAM
       </span>
       <span class="text-xs bg-gray-100 px-2 py-1 rounded">
        1TB SSD
       </span>
      </div>
      <div class="flex items-center justify-between">
       <div>
        <span class="text-gray-400 line-through text-sm">
         Rp18.999.000
        </span>
        <p class="text-xl font-bold text-gray-900">
         Rp15.999.000
        </p>
       </div>
       <button class="buy-btn bg-black hover:bg-gray-800 text-white px-4 py-2 rounded-lg transition duration-300 flex items-center add-to-cart-btn" type="button">
        <i class="fas fa-cart-plus mr-2">
        </i>
        Tambah ke Keranjang
       </button>
      </div>
     </div>
    </div>
    <!-- Desktop -->
    <div class="product-card bg-white rounded-xl shadow-md overflow-hidden transition duration-300 hover:shadow-xl group" data-category="desktop" data-img-src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/1115c8a1-9e5d-4236-b7c4-ace803b2ceb6.png" data-name="IdeaCentre AIO 3" data-price="Rp12.499.000">
     <div class="relative">
      <img alt="Lenovo IdeaCentre AIO desktop all-in-one dengan layar besar tanpa bezel" class="w-full h-64 object-contain p-4" src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/1115c8a1-9e5d-4236-b7c4-ace803b2ceb6.png"/>
      <div aria-label="Tombol aksi produk IdeaCentre AIO 3" class="absolute top-3 right-3 flex flex-col space-y-2">
       <button aria-label="Tambahkan ke favorit" class="w-8 h-8 bg-white rounded-full shadow flex items-center justify-center text-gray-700 hover:bg-gray-100 favorite-btn" type="button">
        <i class="far fa-heart">
        </i>
       </button>
       <button aria-label="Bandingkan produk" class="w-8 h-8 bg-white rounded-full shadow flex items-center justify-center text-gray-700 hover:bg-gray-100 compare-btn" type="button">
        <i class="fas fa-exchange-alt">
        </i>
       </button>
      </div>
     </div>
     <div class="p-6">
      <div class="flex justify-between items-start mb-2">
       <div>
        <h3 class="font-bold text-lg">
         IdeaCentre AIO 3
        </h3>
        <div class="flex items-center mt-1">
         <div class="flex text-yellow-400 mr-2">
          <i class="fas fa-star">
          </i>
          <i class="fas fa-star">
          </i>
          <i class="fas fa-star">
          </i>
          <i class="fas fa-star-half-alt">
          </i>
          <i class="far fa-star">
          </i>
         </div>
         <span class="text-sm text-gray-500">
          (28)
         </span>
        </div>
       </div>
      </div>
      <p class="text-gray-600 text-sm mb-4">
       Desktop all-in-one dengan performa handal dan desain minimalis.
      </p>
      <div class="flex flex-wrap gap-2 mb-4">
       <span class="text-xs bg-gray-100 px-2 py-1 rounded">
        AMD Ryzen 5
       </span>
       <span class="text-xs bg-gray-100 px-2 py-1 rounded">
        23.8" FHD
       </span>
       <span class="text-xs bg-gray-100 px-2 py-1 rounded">
        8GB RAM
       </span>
       <span class="text-xs bg-gray-100 px-2 py-1 rounded">
        512GB SSD
       </span>
      </div>
      <div class="flex items-center justify-between">
       <div>
        <span class="text-gray-400 line-through text-sm">
         Rp14.999.000
        </span>
        <p class="text-xl font-bold text-gray-900">
         Rp12.499.000
        </p>
       </div>
       <button class="buy-btn bg-black hover:bg-gray-800 text-white px-4 py-2 rounded-lg transition duration-300 flex items-center add-to-cart-btn" type="button">
        <i class="fas fa-cart-plus mr-2">
        </i>
        Tambah ke Keranjang
       </button>
      </div>
     </div>
    </div>
    <!-- Monitor -->
    <div class="product-card bg-white rounded-xl shadow-md overflow-hidden transition duration-300 hover:shadow-xl group" data-category="monitor" data-img-src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/610b1623-17b1-4011-bd79-cecece36a531.png" data-name="Lenovo Legion Y27gq-25" data-price="Rp9.999.000">
     <div class="relative">
      <img alt="Lenovo Legion monitor gaming 27 inci dengan refresh rate 165Hz dan layar curved" class="w-full h-64 object-contain p-4" src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/610b1623-17b1-4011-bd79-cecece36a531.png"/>
      <div aria-label="Tombol aksi produk Lenovo Legion Y27gq-25" class="absolute top-3 right-3 flex flex-col space-y-2">
       <button aria-label="Tambahkan ke favorit" class="w-8 h-8 bg-white rounded-full shadow flex items-center justify-center text-gray-700 hover:bg-gray-100 favorite-btn" type="button">
        <i class="far fa-heart">
        </i>
       </button>
       <button aria-label="Bandingkan produk" class="w-8 h-8 bg-white rounded-full shadow flex items-center justify-center text-gray-700 hover:bg-gray-100 compare-btn" type="button">
        <i class="fas fa-exchange-alt">
        </i>
       </button>
      </div>
     </div>
     <div class="p-6">
      <div class="flex justify-between items-start mb-2">
       <div>
        <h3 class="font-bold text-lg">
         Lenovo Legion Y27gq-25
        </h3>
        <div class="flex items-center mt-1">
         <div class="flex text-yellow-400 mr-2">
          <i class="fas fa-star">
          </i>
          <i class="fas fa-star">
          </i>
          <i class="fas fa-star">
          </i>
          <i class="fas fa-star">
          </i>
          <i class="fas fa-star-half-alt">
          </i>
         </div>
         <span class="text-sm text-gray-500">
          (19)
         </span>
        </div>
       </div>
      </div>
      <p class="text-gray-600 text-sm mb-4">
       Monitor gaming 27 inci dengan refresh rate 165Hz dan layar curved.
      </p>
      <div class="flex flex-wrap gap-2 mb-4">
       <span class="text-xs bg-gray-100 px-2 py-1 rounded">
        27" Curved
       </span>
       <span class="text-xs bg-gray-100 px-2 py-1 rounded">
        QHD 2560x1440
       </span>
       <span class="text-xs bg-gray-100 px-2 py-1 rounded">
        165Hz Refresh Rate
       </span>
       <span class="text-xs bg-gray-100 px-2 py-1 rounded">
        1ms Response Time
       </span>
      </div>
      <div class="flex items-center justify-between">
       <div>
        <span class="text-gray-400 line-through text-sm">
         Rp11.499.000
        </span>
        <p class="text-xl font-bold text-gray-900">
         Rp9.999.000
        </p>
       </div>
       <button class="buy-btn bg-black hover:bg-gray-800 text-white px-4 py-2 rounded-lg transition duration-300 flex items-center add-to-cart-btn" type="button">
        <i class="fas fa-cart-plus mr-2">
        </i>
        Tambah ke Keranjang
       </button>
      </div>
     </div>
    </div>
    <!-- Handphone -->
    <div class="product-card bg-white rounded-xl shadow-md overflow-hidden transition duration-300 hover:shadow-xl group" data-category="handphone" data-img-src="https://placehold.co/400x300?text=Lenovo+Legion+Phone+Duel+2" data-name="Lenovo Legion Phone Duel 2" data-price="Rp9.499.000">
     <div class="relative">
      <img alt="Lenovo Legion Phone Duel 2 smartphone gaming dengan desain futuristik dan layar besar" class="w-full h-64 object-contain p-4" height="300" src="https://storage.googleapis.com/a1aa/image/3d343873-9e11-437c-6606-aca30a867fc9.jpg" width="400"/>
      <div aria-label="Tombol aksi produk Lenovo Legion Phone Duel 2" class="absolute top-3 right-3 flex flex-col space-y-2">
       <button aria-label="Tambahkan ke favorit" class="w-8 h-8 bg-white rounded-full shadow flex items-center justify-center text-gray-700 hover:bg-gray-100 favorite-btn" type="button">
        <i class="far fa-heart">
        </i>
       </button>
       <button aria-label="Bandingkan produk" class="w-8 h-8 bg-white rounded-full shadow flex items-center justify-center text-gray-700 hover:bg-gray-100 compare-btn" type="button">
        <i class="fas fa-exchange-alt">
        </i>
       </button>
      </div>
     </div>
     <div class="p-6">
      <div class="flex justify-between items-start mb-2">
       <div>
        <h3 class="font-bold text-lg">
         Lenovo Legion Phone Duel 2
        </h3>
        <div class="flex items-center mt-1">
         <div class="flex text-yellow-400 mr-2">
          <i class="fas fa-star">
          </i>
          <i class="fas fa-star">
          </i>
          <i class="fas fa-star">
          </i>
          <i class="fas fa-star">
          </i>
          <i class="fas fa-star">
          </i>
         </div>
         <span class="text-sm text-gray-500">
          (45)
         </span>
        </div>
       </div>
      </div>
      <p class="text-gray-600 text-sm mb-4">
       Smartphone gaming dengan performa tinggi dan desain futuristik.
      </p>
      <div class="flex flex-wrap gap-2 mb-4">
       <span class="text-xs bg-gray-100 px-2 py-1 rounded">
        Snapdragon 888
       </span>
       <span class="text-xs bg-gray-100 px-2 py-1 rounded">
        6.92" AMOLED
       </span>
       <span class="text-xs bg-gray-100 px-2 py-1 rounded">
        16GB RAM
       </span>
       <span class="text-xs bg-gray-100 px-2 py-1 rounded">
        512GB Storage
       </span>
      </div>
      <div class="flex items-center justify-between">
       <div>
        <span class="text-gray-400 line-through text-sm">
         Rp11.999.000
        </span>
        <p class="text-xl font-bold text-gray-900">
         Rp9.499.000
        </p>
       </div>
       <button class="buy-btn bg-black hover:bg-gray-800 text-white px-4 py-2 rounded-lg transition duration-300 flex items-center add-to-cart-btn" type="button">
        <i class="fas fa-cart-plus mr-2">
        </i>
        Tambah ke Keranjang
       </button>
      </div>
     </div>
    </div>
    <!-- Accessories -->
    <div class="product-card bg-white rounded-xl shadow-md overflow-hidden transition duration-300 hover:shadow-xl group" data-category="accessories" data-img-src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/1254638a-0032-4b2c-8f7b-8c6848cc2d81.png" data-name="Lenovo Wireless Mouse" data-price="Rp299.000">
     <div class="relative">
      <img alt="Berbagai aksesoris Lenovo termasuk mouse nirkabel, keyboard mekanis, dan docking station" class="w-full h-64 object-contain p-4" src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/1254638a-0032-4b2c-8f7b-8c6848cc2d81.png"/>
      <div aria-label="Tombol aksi produk Lenovo Wireless Mouse" class="absolute top-3 right-3 flex flex-col space-y-2">
       <button aria-label="Tambahkan ke favorit" class="w-8 h-8 bg-white rounded-full shadow flex items-center justify-center text-gray-700 hover:bg-gray-100 favorite-btn" type="button">
        <i class="far fa-heart">
        </i>
       </button>
       <button aria-label="Bandingkan produk" class="w-8 h-8 bg-white rounded-full shadow flex items-center justify-center text-gray-700 hover:bg-gray-100 compare-btn" type="button">
        <i class="fas fa-exchange-alt">
        </i>
       </button>
      </div>
     </div>
     <div class="p-6">
      <div class="flex justify-between items-start mb-2">
       <div>
        <h3 class="font-bold text-lg">
         Lenovo Wireless Mouse
        </h3>
        <div class="flex items-center mt-1">
         <div class="flex text-yellow-400 mr-2">
          <i class="fas fa-star">
          </i>
          <i class="fas fa-star">
          </i>
          <i class="fas fa-star">
          </i>
          <i class="fas fa-star-half-alt">
          </i>
          <i class="far fa-star">
          </i>
         </div>
         <span class="text-sm text-gray-500">
          (15)
         </span>
        </div>
       </div>
      </div>
      <p class="text-gray-600 text-sm mb-4">
       Mouse nirkabel ergonomis dengan koneksi Bluetooth dan baterai tahan lama.
      </p>
      <div class="flex flex-wrap gap-2 mb-4">
       <span class="text-xs bg-gray-100 px-2 py-1 rounded">
        Bluetooth 5.0
       </span>
       <span class="text-xs bg-gray-100 px-2 py-1 rounded">
        Ergonomic Design
       </span>
       <span class="text-xs bg-gray-100 px-2 py-1 rounded">
        Tahan Baterai 12 Bulan
       </span>
      </div>
      <div class="flex items-center justify-between">
       <div>
        <p class="text-xl font-bold text-gray-900">
         Rp299.000
        </p>
       </div>
       <button class="buy-btn bg-black hover:bg-gray-800 text-white px-4 py-2 rounded-lg transition duration-300 flex items-center add-to-cart-btn" type="button">
        <i class="fas fa-cart-plus mr-2">
        </i>
        Tambah ke Keranjang
       </button>
      </div>
     </div>
    </div>
   </div>
   <div class="text-center mt-12">
    <button class="px-6 py-3 border-2 border-black rounded-lg font-medium hover:bg-black hover:text-white transition duration-300">
     Lihat Semua Produk
    </button>
   </div>
  </section>
  <section class="bg-gray-900 text-white py-16" id="solutions">
   <div class="container mx-auto px-4">
    <div class="text-center mb-12">
     <h2 class="text-3xl font-bold mb-4">
      Solusi Lenovo untuk Segala Kebutuhan
     </h2>
     <p class="text-gray-300 max-w-2xl mx-auto">
      Temukan solusi teknologi yang sesuai dengan kebutuhan pribadi atau bisnis Anda.
     </p>
    </div>
    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
     <div class="bg-gray-800 rounded-xl p-6 hover:bg-gray-700 transition duration-300">
      <div class="w-16 h-16 bg-yellow-500 rounded-full flex items-center justify-center mb-4">
       <i class="fas fa-graduation-cap text-2xl text-white">
       </i>
      </div>
      <h3 class="text-xl font-bold mb-2">
       Pendidikan
      </h3>
      <p class="text-gray-300 mb-4">
       Perangkat hemat daya dengan fitur keamanan untuk pembelajaran jarak jauh dan kelas digital.
      </p>
      <a class="text-yellow-400 hover:text-yellow-300 font-medium flex items-center" href="https://www.lenovo.com/id/id/solutions/education/" rel="noopener noreferrer" target="_blank">
       Selengkapnya
       <i class="fas fa-chevron-right ml-2 text-sm">
       </i>
      </a>
     </div>
     <div class="bg-gray-800 rounded-xl p-6 hover:bg-gray-700 transition duration-300">
      <div class="w-16 h-16 bg-yellow-500 rounded-full flex items-center justify-center mb-4">
       <i class="fas fa-briefcase text-2xl text-white">
       </i>
      </div>
      <h3 class="text-xl font-bold mb-2">
       Bisnis
      </h3>
      <p class="text-gray-300 mb-4">
       Solusi IT komprehensif untuk produktivitas dan keamanan bisnis dari kecil hingga enterprise.
      </p>
      <a class="text-yellow-400 hover:text-yellow-300 font-medium flex items-center" href="https://www.lenovo.com/id/id/solutions/business/" rel="noopener noreferrer" target="_blank">
       Selengkapnya
       <i class="fas fa-chevron-right ml-2 text-sm">
       </i>
      </a>
     </div>
     <div class="bg-gray-800 rounded-xl p-6 hover:bg-gray-700 transition duration-300">
      <div class="w-16 h-16 bg-yellow-500 rounded-full flex items-center justify-center mb-4">
       <i class="fas fa-gamepad text-2xl text-white">
       </i>
      </div>
      <h3 class="text-xl font-bold mb-2">
       Gaming
      </h3>
      <p class="text-gray-300 mb-4">
       Perangkat gaming performa tinggi dengan pendingan optimal dan pengalaman visual memukau.
      </p>
      <a class="text-yellow-400 hover:text-yellow-300 font-medium flex items-center" href="https://www.lenovo.com/id/id/solutions/gaming/" rel="noopener noreferrer" target="_blank">
       Selengkapnya
       <i class="fas fa-chevron-right ml-2 text-sm">
       </i>
      </a>
     </div>
     <div class="bg-gray-800 rounded-xl p-6 hover:bg-gray-700 transition duration-300">
      <div class="w-16 h-16 bg-yellow-500 rounded-full flex items-center justify-center mb-4">
       <i class="fas fa-paint-brush text-2xl text-white">
       </i>
      </div>
      <h3 class="text-xl font-bold mb-2">
       Kreator
      </h3>
      <p class="text-gray-300 mb-4">
       Workstation dan perangkat akurasi tinggi untuk desainer, fotografer, dan konten kreator.
      </p>
      <a class="text-yellow-400 hover:text-yellow-300 font-medium flex items-center" href="https://www.lenovo.com/id/id/solutions/creators/" rel="noopener noreferrer" target="_blank">
       Selengkapnya
       <i class="fas fa-chevron-right ml-2 text-sm">
       </i>
      </a>
     </div>
    </div>
   </div>
  </section>
  <section class="container mx-auto px-4 py-16" id="services">
   <div class="text-center mb-12">
    <h2 class="text-3xl font-bold mb-4">
     Layanan Profesional Lenovo
    </h2>
    <p class="text-gray-600 max-w-2xl mx-auto">
     Dukungan lengkap untuk memastikan perangkat Anda selalu berjalan optimal.
    </p>
   </div>
   <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
    <div class="bg-white p-8 rounded-xl shadow-md border border-gray-100 hover:shadow-lg transition duration-300">
     <div class="w-16 h-16 bg-yellow-100 rounded-lg flex items-center justify-center mb-6">
      <i class="fas fa-tools text-2xl text-yellow-600">
      </i>
     </div>
     <h3 class="text-xl font-bold mb-4">
      Servis &amp; Perbaikan
     </h3>
     <p class="text-gray-600 mb-6">
      Layanan perbaikan resmi oleh teknisi bersertifikat dengan garansi resmi.
     </p>
     <ul class="space-y-3">
      <li class="flex">
       <i class="fas fa-check text-yellow-500 mt-1 mr-2">
       </i>
       <span>
        Diagnosis dan perbaikan hardware
       </span>
      </li>
      <li class="flex">
       <i class="fas fa-check text-yellow-500 mt-1 mr-2">
       </i>
       <span>
        Perangkatan software
       </span>
      </li>
      <li class="flex">
       <i class="fas fa-check text-yellow-500 mt-1 mr-2">
       </i>
       <span>
        Perbaikan layar &amp; keyboard
       </span>
      </li>
     </ul>
    </div>
    <div class="bg-white p-8 rounded-xl shadow-md border border-gray-100 hover:shadow-lg transition duration-300">
     <div class="w-16 h-16 bg-yellow-100 rounded-lg flex items-center justify-center mb-6">
      <i class="fas fa-laptop-medical text-2xl text-yellow-600">
      </i>
     </div>
     <h3 class="text-xl font-bold mb-4">
      Tune-up &amp; Optimasi
     </h3>
     <p class="text-gray-600 mb-6">
      Layanan pembersihan dan optimasi untuk mengembalikan performa perangkat.
     </p>
     <ul class="space-y-3">
      <li class="flex">
       <i class="fas fa-check text-yellow-500 mt-1 mr-2">
       </i>
       <span>
        Pembersihan deep cleaning
       </span>
      </li>
      <li class="flex">
       <i class="fas fa-check text-yellow-500 mt-1 mr-2">
       </i>
       <span>
        Optimasi sistem operasi
       </span>
      </li>
      <li class="flex">
       <i class="fas fa-check text-yellow-500 mt-1 mr-2">
       </i>
       <span>
        Penggantian thermal paste
       </span>
      </li>
     </ul>
    </div>
    <div class="bg-white p-8 rounded-xl shadow-md border border-gray-100 hover:shadow-lg transition duration-300">
     <div class="w-16 h-16 bg-yellow-100 rounded-lg flex items-center justify-center mb-6">
      <i class="fas fa-headset text-2xl text-yellow-600">
      </i>
     </div>
     <h3 class="text-xl font-bold mb-4">
      Konsultasi IT
     </h3>
     <p class="text-gray-600 mb-6">
      Solusi untuk kebutuhan komputasi pribadi maupun bisnis.
     </p>
     <ul class="space-y-3">
      <li class="flex">
       <i class="fas fa-check text-yellow-500 mt-1 mr-2">
       </i>
       <span>
        Rekomendasi perangkat
       </span>
      </li>
      <li class="flex">
       <i class="fas fa-check text-yellow-500 mt-1 mr-2">
       </i>
       <span>
        Set-up jaringan &amp; printer
       </span>
      </li>
      <li class="flex">
       <i class="fas fa-check text-yellow-500 mt-1 mr-2">
       </i>
       <span>
        Migrasi data
       </span>
      </li>
     </ul>
    </div>
   </div>
   <div class="text-center mt-12">
    <button class="px-6 py-3 bg-black hover:bg-gray-800 text-white rounded-lg font-medium transition duration-300">
     Hubungi Layanan Kami
    </button>
   </div>
  </section>
  <section class="bg-gray-50 py-16" id="support">
   <div class="container mx-auto px-4">
    <div class="text-center mb-12">
     <h2 class="text-3xl font-bold mb-4">
      Dukungan &amp; Bantuan
     </h2>
     <p class="text-gray-600 max-w-2xl mx-auto">
      Kami siap membantu Anda kapan saja dengan berbagai pilihan dukungan
          teknis.
     </p>
    </div>
    <div class="bg-white rounded-xl shadow-lg overflow-hidden">
     <div class="md:flex">
      <div class="md:w-1/2 p-8 md:p-12 bg-gray-900 text-white">
       <h3 class="text-2xl font-bold mb-4">
        Butuh Bantuan Cepat?
       </h3>
       <p class="text-gray-300 mb-6">
        Tim support kami siap menjawab pertanyaan Anda seputar produk dan
              solusi Lenovo.
       </p>
       <div class="space-y-4">
        <div class="flex items-start">
         <div class="flex-shrink-0 mt-1 mr-4 text-yellow-400">
          <i class="fas fa-headset text-xl">
          </i>
         </div>
         <div>
          <h4 class="font-bold">
           Live Chat 24/7
          </h4>
          <p class="text-sm text-gray-300">
           Chat langsung dengan agen support kami
          </p>
         </div>
        </div>
        <div class="flex items-start">
         <div class="flex-shrink-0 mt-1 mr-4 text-yellow-400">
          <i class="fas fa-phone-alt">
          </i>
         </div>
         <div>
          <h4 class="font-bold">
           021-1234-5678
          </h4>
          <p class="text-sm text-gray-300">
           Senin-Jumat, 09:00-17:00 WIB
          </p>
         </div>
        </div>
        <div class="flex items-start">
         <div class="flex-shrink-0 mt-1 mr-4 text-yellow-400">
          <i class="fas fa-envelope">
          </i>
         </div>
         <div>
          <h4 class="font-bold">
           support@lenovo.co.id
          </h4>
          <p class="text-sm text-gray-300">
           Respon dalam 1x24 jam kerja
          </p>
         </div>
        </div>
       </div>
      </div>
      <div class="md:w-1/2 p-8 md:p-12">
       <h3 class="text-2xl font-bold mb-4">
        Pusat Bantuan
       </h3>
       <div class="divide-y divide-gray-200">
        <div class="py-4">
         <a class="flex justify-between items-center hover:text-yellow-600" href="#">
          Panduan Pemula
          <i class="fas fa-chevron-right">
          </i>
         </a>
        </div>
        <div class="py-4">
         <a class="flex justify-between items-center hover:text-yellow-600" href="#">
          Unduh Driver &amp; Software
          <i class="fas fa-chevron-right">
          </i>
         </a>
        </div>
        <div class="py-4">
         <a class="flex justify-between items-center hover:text-yellow-600" href="#">
          FAQ Produk
          <i class="fas fa-chevron-right">
          </i>
         </a>
        </div>
        <div class="py-4">
         <a class="flex justify-between items-center hover:text-yellow-600" href="#">
          Panduan Garansi
          <i class="fas fa-chevron-right">
          </i>
         </a>
        </div>
        <div class="py-4">
         <a class="flex justify-between items-center hover:text-yellow-600" href="#">
          Pusat Servis Resmi
          <i class="fas fa-chevron-right">
          </i>
         </a>
        </div>
       </div>
      </div>
     </div>
    </div>
   </div>
  </section>
  <section class="bg-gray-900 text-white py-12">
   <div class="container mx-auto px-4">
    <div class="md:flex md:items-center md:justify-between">
     <div class="mb-8 md:mb-0">
      <h3 class="text-xl font-bold mb-4">
       Gabung dengan Komunitas Lenovo
      </h3>
      <p class="text-gray-300 max-w-lg">
       Ikuti kami di media sosial untuk info terbaru, tips &amp; trik, dan
            penawaran spesial.
      </p>
     </div>
     <div class="flex space-x-4">
      <a class="w-10 h-10 bg-gray-800 rounded-full flex items-center justify-center hover:bg-yellow-500 hover:text-black transition duration-300" href="https://www.facebook.com/LenovoID/" target="_blank">
       <i class="fab fa-facebook-f">
       </i>
      </a>
      <a class="w-10 h-10 bg-gray-800 rounded-full flex items-center justify-center hover:bg-yellow-500 hover:text-black transition duration-300" href="https://x.com/Lenovo_ID" target="_blank">
       <i class="fab fa-twitter">
       </i>
      </a>
      <a class="w-10 h-10 bg-gray-800 rounded-full flex items-center justify-center hover:bg-yellow-500 hover:text-black transition duration-300" href="https://www.instagram.com/lenovoid/" target="_blank">
       <i class="fab fa-instagram">
       </i>
      </a>
      <a class="w-10 h-10 bg-gray-800 rounded-full flex items-center justify-center hover:bg-yellow-500 hover:text-black transition duration-300" href="https://www.youtube.com/c/LenovoIndonesia" target="_blank">
       <i class="fab fa-youtube">
       </i>
      </a>
      <a class="w-10 h-10 bg-gray-800 rounded-full flex items-center justify-center hover:bg-yellow-500 hover:text-black transition duration-300" href="https://www.linkedin.com/company/lenovo/" target="_blank">
       <i class="fab fa-linkedin-in">
       </i>
      </a>
     </div>
    </div>
    <div class="border-t border-gray-800 my-8">
    </div>
    <div class="md:flex md:items-center md:justify-between">
     <div class="mb-8 md:mb-0">
      <h3 class="text-xl font-bold mb-4">
       Newsletter Lenovo
      </h3>
      <p class="text-gray-300 max-w-lg">
       Dapatkan info promo, produk baru, dan tips langsung ke inbox Anda.
      </p>
     </div>
     <form aria-label="Form berlangganan newsletter" class="flex flex-col sm:flex-row gap-4">
      <input aria-required="true" class="px-4 py-3 rounded-lg bg-gray-800 text-white border border-gray-700 focus:outline-none focus:ring-2 focus:ring-yellow-500 w-full sm:w-64" placeholder="Alamat email Anda" type="email"/>
      <button class="bg-yellow-500 hover:bg-yellow-600 text-black font-bold py-3 px-6 rounded-lg whitespace-nowrap" type="submit">
       Berlangganan
      </button>
     </form>
    </div>
   </div>
  </section>
  <section class="container mx-auto px-4 py-16" id="locations">
   <h2 class="text-3xl font-bold text-center mb-8">
    Lokasi Lenovo Indonesia
   </h2>
   <div class="grid grid-cols-1 md:grid-cols-2 gap-12">
    <div>
     <h3 class="text-xl font-semibold mb-4">
      Kantor Pusat Lenovo Indonesia
     </h3>
     <p class="mb-2">
      Jl. Jend. Sudirman Kav. 52-53, Jakarta Selatan, DKI Jakarta 12190
     </p>
     <p class="mb-2">
      Telepon: (021) 1234-5678
     </p>
     <p class="mb-6">
      Jam Operasional: Senin - Jumat, 09:00 - 17:00 WIB
     </p>
     <img alt="Gedung kantor pusat Lenovo Indonesia di Jakarta dengan desain modern dan logo Lenovo besar di depan" class="rounded-lg shadow-md w-full h-auto" height="400" src="https://storage.googleapis.com/a1aa/image/fe3bf94a-35cc-4fcc-4055-6814a39aeab9.jpg" width="600"/>
    </div>
    <div>
     <h3 class="text-xl font-semibold mb-4">
      Peta Lokasi Kantor Pusat
     </h3>
     <iframe allowfullscreen="" height="400" loading="lazy" referrerpolicy="no-referrer-when-downgrade" src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3966.1234567890123!2d106.816666!3d-6.230833!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e69f3e0a1b2c3d5%3A0x123456789abcdef!2sLenovo%20Indonesia%20Headquarters!5e0!3m2!1sen!2sid!4v1680000000000!5m2!1sen!2sid" style="border:0;" title="Peta lokasi kantor pusat Lenovo Indonesia" width="100%">
     </iframe>
    </div>
   </div>
  </section>
  <footer class="bg-black text-white py-12">
   <div class="container mx-auto px-4">
    <div class="grid grid-cols-2 md:grid-cols-4 lg:grid-cols-5 gap-8 mb-8">
     <div class="col-span-2">
      <img alt="Logo Lenovo putih dengan aksen emas" class="h-8 mb-4" src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/0ea21880-f06d-42cb-957b-d0865d5b29f2.png"/>
      <p class="text-gray-400 mb-4">
       Mengubah teknologi menjadi kemajuan yang bermanfaat bagi semua orang.
      </p>
      <div class="flex space-x-4">
       <a class="text-gray-400 hover:text-white" href="https://www.facebook.com/LenovoID/" target="_blank">
        <i class="fab fa-facebook-f">
        </i>
       </a>
       <a class="text-gray-400 hover:text-white" href="https://x.com/Lenovo_ID" target="_blank">
        <i class="fab fa-twitter">
        </i>
       </a>
       <a class="text-gray-400 hover:text-white" href="https://www.instagram.com/lenovoid/" target="_blank">
        <i class="fab fa-instagram">
        </i>
       </a>
       <a class="text-gray-400 hover:text-white" href="https://www.youtube.com/c/LenovoIndonesia" target="_blank">
        <i class="fab fa-youtube">
        </i>
       </a>
       <a class="text-gray-400 hover:text-white" href="https://www.linkedin.com/company/lenovo/" target="_blank">
        <i class="fab fa-linkedin-in">
        </i>
       </a>
      </div>
     </div>
     <div>
      <h4 class="font-bold text-lg mb-4">
       Tentang Lenovo
      </h4>
      <ul class="space-y-2">
       <li>
        <a class="text-gray-400 hover:text-white" href="#">
         Tentang Kami
        </a>
       </li>
       <li>
        <a class="text-gray-400 hover:text-white" href="#">
         Karir
        </a>
       </li>
       <li>
        <a class="text-gray-400 hover:text-white" href="#">
         Berita
        </a>
       </li>
       <li>
        <a class="text-gray-400 hover:text-white" href="#">
         Investor
        </a>
       </li>
       <li>
        <a class="text-gray-400 hover:text-white" href="#">
         Tanggung Jawab Sosial
        </a>
       </li>
      </ul>
     </div>
     <div>
      <h4 class="font-bold text-lg mb-4">
       Beli
      </h4>
      <ul class="space-y-2">
       <li>
        <a class="text-gray-400 hover:text-white" href="#products">
         Semua Produk
        </a>
       </li>
       <li>
        <a class="text-gray-400 hover:text-white" href="#">
         Promo
        </a>
       </li>
       <li>
        <a class="text-gray-400 hover:text-white" href="#">
         Lenovo Exclusive Store
        </a>
       </li>
       <li>
        <a class="text-gray-400 hover:text-white" href="#">
         Reseller
        </a>
       </li>
       <li>
        <a class="text-gray-400 hover:text-white" href="#">
         Cicilan 0%
        </a>
       </li>
      </ul>
     </div>
     <div>
      <h4 class="font-bold text-lg mb-4">
       Dukungan
      </h4>
      <ul class="space-y-2">
       <li>
        <a class="text-gray-400 hover:text-white" href="#support">
         Bantuan
        </a>
       </li>
       <li>
        <a class="text-gray-400 hover:text-white" href="#">
         Garansi
        </a>
       </li>
       <li>
        <a class="text-gray-400 hover:text-white" href="#">
         Driver &amp; Perangkat Lunak
        </a>
       </li>
       <li>
        <a class="text-gray-400 hover:text-white" href="#">
         Keamanan Produk
        </a>
       </li>
       <li>
        <a class="text-gray-400 hover:text-white" href="#">
         Hubungi Kami
        </a>
       </li>
      </ul>
     </div>
    </div>
    <div class="border-t border-gray-800 pt-8">
     <div class="flex flex-col md:flex-row justify-between items-center">
      <p class="text-gray-400 text-sm mb-4 md:mb-0">
       © 2025 Lenovo. Seluruh hak cipta dilindungi undang-undang.
      </p>
      <div class="flex flex-wrap gap-4">
       <a class="text-gray-400 hover:text-white text-sm" href="#">
        Syarat &amp; Ketentuan
       </a>
       <a class="text-gray-400 hover:text-white text-sm" href="#">
        Kebijakan Privasi
       </a>
       <a class="text-gray-400 hover:text-white text-sm" href="#">
        Pemberitahuan Cookie
       </a>
      </div>
     </div>
    </div>
   </div>
  </footer>
  <!-- Checkout Modal -->
  <div aria-labelledby="checkout-modal-title" aria-modal="true" class="modal-overlay fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center p-4 z-50 hidden opacity-0" id="checkout-modal" role="dialog">
   <div class="modal-content bg-white w-full max-w-md rounded-lg shadow-xl p-6 transform -translate-y-10">
    <div class="flex justify-between items-center mb-4">
     <h2 class="text-2xl font-bold" id="checkout-modal-title">
      Checkout
     </h2>
     <button aria-label="Tutup modal checkout" class="text-gray-500 hover:text-gray-800 text-2xl" id="close-checkout-modal">
      ×
     </button>
    </div>
    <div class="flex items-center border-b pb-4 mb-4">
     <img alt="Produk" class="w-20 h-20 object-contain rounded-md mr-4" id="checkout-product-img" src=""/>
     <div>
      <h3 class="font-bold" id="checkout-product-name">
       Nama Produk
      </h3>
      <p class="text-lg text-gray-800" id="checkout-product-price">
       Rp0
      </p>
     </div>
    </div>
    <form id="payment-form">
     <h3 class="font-semibold mb-3">
      Pilih Metode Pembayaran
     </h3>
     <div class="grid grid-cols-2 gap-4 mb-4">
      <label class="border rounded-lg p-3 flex items-center cursor-pointer has-[:checked]:bg-yellow-100 has-[:checked]:border-yellow-500">
       <input checked="" class="mr-3" name="paymentMethod" type="radio" value="OVO"/>
       <img alt="OVO" class="h-6" src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/eb/Logo_OVO_PNG.png/640px-Logo_OVO_PNG.png"/>
      </label>
      <label class="border rounded-lg p-3 flex items-center cursor-pointer has-[:checked]:bg-blue-100 has-[:checked]:border-blue-500">
       <input class="mr-3" name="paymentMethod" type="radio" value="DANA"/>
       <img alt="DANA" class="h-6" src="https://upload.wikimedia.org/wikipedia/commons/7/72/Logo_dana_blue.svg"/>
      </label>
     </div>
     <div class="mb-6">
      <label class="block text-sm font-medium text-gray-700 mb-1" for="phone-number">
       Nomor Telepon (terhubung ke OVO/DANA)
      </label>
      <input class="w-full px-3 py-2 border rounded-lg" id="phone-number" placeholder="081234567890" required="" type="tel"/>
     </div>
     <button class="w-full bg-black text-white py-3 rounded-lg hover:bg-gray-800 font-bold transition duration-300" type="submit">
      Bayar Sekarang
     </button>
    </form>
   </div>
  </div>
  <!-- Receipt Modal -->
  <div aria-labelledby="receipt-modal-title" aria-modal="true" class="modal-overlay fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center p-4 z-50 hidden opacity-0" id="receipt-modal" role="dialog">
   <div class="modal-content bg-white w-full max-w-sm rounded-lg shadow-xl transform -translate-y-10">
    <div class="p-6">
     <div class="text-center mb-6">
      <i class="fas fa-check-circle text-5xl text-green-500">
      </i>
      <h2 class="text-2xl font-bold mt-4" id="receipt-modal-title">
       Pembayaran Berhasil
      </h2>
     </div>
     <div class="bg-gray-50 rounded-lg p-4 space-y-3">
      <div class="flex justify-between text-sm">
       <span class="text-gray-500">
        Produk:
       </span>
       <span class="font-medium text-right" id="receipt-product-name">
        Nama Produk
       </span>
      </div>
      <div class="flex justify-between text-sm">
       <span class="text-gray-500">
        Total Pembayaran:
       </span>
       <span class="font-medium" id="receipt-price">
        Rp0
       </span>
      </div>
      <div class="flex justify-between text-sm">
       <span class="text-gray-500">
        Metode:
       </span>
       <span class="font-medium" id="receipt-method">
        OVO/DANA
       </span>
      </div>
      <div class="border-t my-2">
      </div>
      <div class="flex justify-between text-sm">
       <span class="text-gray-500">
        Waktu Transaksi:
       </span>
       <span class="font-medium" id="receipt-time">
        ...
       </span>
      </div>
      <div class="flex justify-between text-sm">
       <span class="text-gray-500">
        ID Transaksi:
       </span>
       <span class="font-medium" id="receipt-id">
        ...
       </span>
      </div>
     </div>
     <button class="w-full bg-black text-white mt-6 py-2 rounded-lg hover:bg-gray-800 font-bold transition duration-300" id="close-receipt-modal">
      Tutup
     </button>
    </div>
   </div>
  </div>
  <!-- Cart Modal -->
  <div aria-labelledby="cart-modal-title" aria-modal="true" class="modal-overlay fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center p-4 z-50 hidden opacity-0" id="cart-modal" role="dialog">
   <div class="modal-content bg-white w-full max-w-lg rounded-lg shadow-xl p-6 transform -translate-y-10 flex flex-col max-h-[90vh]">
    <div class="flex justify-between items-center mb-4">
     <h2 class="text-2xl font-bold" id="cart-modal-title">
      Keranjang Belanja
     </h2>
     <button aria-label="Tutup modal keranjang" class="text-gray-500 hover:text-gray-800 text-2xl" id="close-cart-modal">
      ×
     </button>
    </div>
    <div class="flex-grow overflow-y-auto divide-y divide-gray-200" id="cart-items">
     <p class="text-center text-gray-500 py-10" id="cart-empty-text">
      Keranjang Anda kosong.
     </p>
    </div>
    <div class="mt-4 border-t pt-4 flex justify-between items-center">
     <div>
      <span class="font-bold text-lg">
       Total:
      </span>
      <span class="text-lg" id="cart-total">
       Rp0
      </span>
     </div>
     <button class="bg-yellow-500 hover:bg-yellow-600 text-black font-bold py-2 px-6 rounded-lg transition duration-300 disabled:opacity-50 disabled:cursor-not-allowed" disabled="" id="cart-checkout-btn">
      Checkout
     </button>
    </div>
   </div>
  </div>
  <script>
   document.addEventListener("DOMContentLoaded", () => {
      // --- State Management Sederhana ---
      let currentUser = null;
      let cart = [];

      // --- Elemen DOM ---
      const authSection = document.getElementById("auth-section");
      const checkoutModal = document.getElementById("checkout-modal");
      const receiptModal = document.getElementById("receipt-modal");
      const cartModal = document.getElementById("cart-modal");
      const cartButton = document.getElementById("cart-button");
      const cartCount = document.getElementById("cart-count");
      const cartItemsContainer = document.getElementById("cart-items");
      const cartTotalEl = document.getElementById("cart-total");
      const cartCheckoutBtn = document.getElementById("cart-checkout-btn");

      // --- Template HTML untuk Auth ---
      const loginTemplate = `
            <button class="flex items-center space-x-1 px-3 py-2 bg-gray-800 rounded-lg hover:bg-gray-700">
                <i class="fas fa-user"></i>
                <span class="hidden md:inline">Masuk</span>
            </button>
            <div class="absolute right-0 mt-2 w-64 bg-white text-black rounded-md shadow-lg hidden group-hover:block p-4 z-[60]">
                <h3 class="font-bold mb-2 text-gray-800">Login / Register</h3>
                <p class="text-xs text-gray-500 mb-2">Akun akan dibuat otomatis jika belum ada.</p>
                <input type="email" id="login-email" placeholder="Email" class="w-full px-3 py-2 mb-2 border rounded" required>
                <input type="password" id="login-password" placeholder="Password" class="w-full px-3 py-2 mb-3 border rounded" required>
                <button id="login-submit-btn" class="w-full bg-black text-white py-2 rounded hover:bg-gray-800">Masuk</button>
            </div>
        `;

      const loggedInTemplate = (userName) => `
            <button class="flex items-center space-x-2 px-3 py-2 bg-gray-800 rounded-lg hover:bg-gray-700">
                <i class="fas fa-user-check"></i>
                <span class="hidden md:inline">Halo, ${userName}</span>
            </button>
            <div class="absolute right-0 mt-2 w-48 bg-white text-black rounded-md shadow-lg hidden group-hover:block p-2 z-[60]">
                <a href="#" class="block px-4 py-2 text-sm text-gray-700 hover:bg-gray-100 rounded">Profil Saya</a>
                <a href="#" class="block px-4 py-2 text-sm text-gray-700 hover:bg-gray-100 rounded">Pesanan Saya</a>
                <div class="border-t my-1"></div>
                <button id="logout-btn" class="w-full text-left px-4 py-2 text-sm text-red-600 hover:bg-gray-100 rounded">Keluar</button>
            </div>
        `;

      // --- Fungsi Auth ---
      const updateAuthUI = () => {
        if (currentUser) {
          authSection.innerHTML = loggedInTemplate(currentUser.name);
          document
            .getElementById("logout-btn")
            .addEventListener("click", handleLogout);
        } else {
          authSection.innerHTML = loginTemplate;
          document
            .getElementById("login-submit-btn")
            .addEventListener("click", handleLogin);
        }
      };

      const handleLogin = () => {
        const email = document.getElementById("login-email").value.trim();
        const password = document.getElementById("login-password").value.trim();
        if (!email || !password) {
          alert("Email dan Password tidak boleh kosong!");
          return;
        }
        // Simulasi pembuatan akun otomatis
        const namePart = email
          .split("@")[0]
          .replace(/[\._]/g, " ")
          .replace(/\b\w/g, (l) => l.toUpperCase());
        currentUser = { email: email, name: namePart };
        alert(`Selamat datang, ${currentUser.name}! Akun Anda telah berhasil dibuat/masuk.`);
        updateAuthUI();
      };

      const handleLogout = () => {
        currentUser = null;
        alert("Anda telah keluar.");
        updateAuthUI();
      };

      // --- Fungsi Modal ---
      const showModal = (modal) => {
        modal.classList.remove("hidden");
        setTimeout(() => modal.classList.add("opacity-100"), 10);
        setTimeout(
          () => modal.querySelector(".modal-content").classList.remove("-translate-y-10"),
          10
        );
      };

      const hideModal = (modal) => {
        modal.classList.remove("opacity-100");
        modal.querySelector(".modal-content").classList.add("-translate-y-10");
        setTimeout(() => modal.classList.add("hidden"), 300);
      };

      // --- Update Cart UI ---
      function updateCartUI() {
        if (cart.length === 0) {
          cartItemsContainer.innerHTML = `<p class="text-center text-gray-500 py-10" id="cart-empty-text">Keranjang Anda kosong.</p>`;
          cartCount.classList.add("hidden");
          cartCheckoutBtn.disabled = true;
          cartTotalEl.textContent = "Rp0";
          return;
        }
        cartCount.textContent = cart.reduce((acc, item) => acc + item.quantity, 0);
        cartCount.classList.remove("hidden");
        cartCheckoutBtn.disabled = false;

        let totalPrice = 0;
        cartItemsContainer.innerHTML = "";
        cart.forEach((item, index) => {
          // Parse price string to number
          const priceNum = parseInt(item.price.replace(/[^\d]/g, ""), 10);
          const itemTotal = priceNum * item.quantity;
          totalPrice += itemTotal;

          const itemEl = document.createElement("div");
          itemEl.className = "flex items-center py-4 space-x-4";
          itemEl.innerHTML = `
            <img src="${item.imgSrc}" alt="${item.name}" class="w-16 h-16 object-contain rounded-md" />
            <div class="flex-grow">
              <h4 class="font-semibold">${item.name}</h4>
              <p class="text-sm text-gray-600">${item.price} x ${item.quantity}</p>
            </div>
            <div class="flex items-center space-x-2">
              <button aria-label="Kurangi jumlah produk" class="text-gray-600 hover:text-red-600 remove-item-btn" data-index="${index}">
                <i class="fas fa-minus-circle fa-lg"></i>
              </button>
              <span class="font-semibold">${item.quantity}</span>
              <button aria-label="Tambah jumlah produk" class="text-gray-600 hover:text-green-600 add-item-btn" data-index="${index}">
                <i class="fas fa-plus-circle fa-lg"></i>
              </button>
            </div>
          `;
          cartItemsContainer.appendChild(itemEl);
        });
        cartTotalEl.textContent = "Rp" + totalPrice.toLocaleString("id-ID");
      }

      // --- Add to Cart ---
      function addToCart(product) {
        const existingIndex = cart.findIndex((item) => item.name === product.name);
        if (existingIndex !== -1) {
          cart[existingIndex].quantity += 1;
        } else {
          cart.push({ ...product, quantity: 1 });
        }
        updateCartUI();
      }

      // --- Remove from Cart ---
      function removeFromCart(index) {
        if (cart[index].quantity > 1) {
          cart[index].quantity -= 1;
        } else {
          cart.splice(index, 1);
        }
        updateCartUI();
      }

      // --- Increase quantity in Cart ---
      function increaseCartItem(index) {
        cart[index].quantity += 1;
        updateCartUI();
      }

      // --- Event Listener Checkout ---
      document.querySelectorAll(".add-to-cart-btn").forEach((button) => {
        button.addEventListener("click", (e) => {
          const card = e.target.closest(".product-card");
          const productName = card.dataset.name;
          const productPrice = card.dataset.price;
          const productImgSrc = card.dataset.imgSrc;

          addToCart({
            name: productName,
            price: productPrice,
            imgSrc: productImgSrc,
          });
          alert(`Produk "${productName}" berhasil ditambahkan ke keranjang.`);
        });
      });

      // --- Cart Modal Toggle ---
      cartButton.addEventListener("click", () => {
        updateCartUI();
        showModal(cartModal);
      });

      document.getElementById("close-cart-modal").addEventListener("click", () => {
        hideModal(cartModal);
      });

      // --- Cart Item Buttons (delegated) ---
      cartItemsContainer.addEventListener("click", (e) => {
        if (e.target.closest(".remove-item-btn")) {
          const index = parseInt(e.target.closest(".remove-item-btn").dataset.index, 10);
          removeFromCart(index);
        }
        if (e.target.closest(".add-item-btn")) {
          const index = parseInt(e.target.closest(".add-item-btn").dataset.index, 10);
          increaseCartItem(index);
        }
      });

      // --- Cart Checkout Button ---
      cartCheckoutBtn.addEventListener("click", () => {
        if (!currentUser) {
          alert("Silakan masuk terlebih dahulu untuk melanjutkan pembayaran.");
          return;
        }
        if (cart.length === 0) {
          alert("Keranjang Anda kosong.");
          return;
        }
        // Prepare checkout modal with first product in cart
        const firstProduct = cart[0];
        document.getElementById("checkout-product-name").textContent = firstProduct.name;
        document.getElementById("checkout-product-price").textContent = firstProduct.price;
        document.getElementById("checkout-product-img").src = firstProduct.imgSrc;

        showModal(checkoutModal);
        hideModal(cartModal);
      });

      // --- Close Checkout Modal ---
      document
        .getElementById("close-checkout-modal")
        .addEventListener("click", () => hideModal(checkoutModal));

      // --- Event Listener Form Pembayaran ---
      document.getElementById("payment-form").addEventListener("submit", (e) => {
        e.preventDefault();
        if (!currentUser) {
          alert("Silakan masuk terlebih dahulu untuk melanjutkan pembayaran.");
          return;
        }

        const phoneNumber = document.getElementById("phone-number").value.trim();
        if (!phoneNumber.match(/^[0-9]{10,13}$/)) {
          alert("Mohon masukkan nomor telepon yang valid.");
          return;
        }

        const paymentMethod = document.querySelector(
          'input[name="paymentMethod"]:checked'
        ).value;
        const productName = document.getElementById("checkout-product-name").textContent;
        const productPrice = document.getElementById("checkout-product-price").textContent;

        // Populate receipt
        document.getElementById("receipt-product-name").textContent = productName;
        document.getElementById("receipt-price").textContent = productPrice;
        document.getElementById("receipt-method").textContent = paymentMethod;
        document.getElementById("receipt-time").textContent = new Date().toLocaleString(
          "id-ID"
        );
        document.getElementById("receipt-id").textContent = "INV" + Date.now();

        // Clear cart after payment
        cart = [];
        updateCartUI();

        hideModal(checkoutModal);
        setTimeout(() => showModal(receiptModal), 350);
      });

      document
        .getElementById("close-receipt-modal")
        .addEventListener("click", () => hideModal(receiptModal));

      // --- Mobile Menu Toggle ---
      document
        .getElementById("mobile-menu-button")
        .addEventListener("click", function () {
          const menu = document.getElementById("mobile-menu");
          menu.classList.toggle("hidden");
        });

      // --- Countdown Timer to 11 July 2025 ---
      const countdownText = document.getElementById("promo-countdown-text");
      const countdownContainer = document.getElementById("countdown");
      const promoSection = document.getElementById("promo");

      function updateCountdown() {
        const now = new Date();
        const endDate = new Date("2025-07-11T23:59:59");
        const total = endDate - now;

        if (total <= 0) {
          // Waktu habis, ganti teks dan sembunyikan countdown
          countdownContainer.style.display = "none";
          countdownText.textContent = "❗Harga kembali normal";
          return;
        }

        const days = Math.floor(total / (1000 * 60 * 60 * 24));
        const hours = Math.floor((total % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
        const minutes = Math.floor((total % (1000 * 60 * 60)) / (1000 * 60));
        const seconds = Math.floor((total % (1000 * 60)) / 1000);

        document.getElementById("days").textContent = days.toString().padStart(2, "0");
        document.getElementById("hours").textContent = hours.toString().padStart(2, "0");
        document.getElementById("minutes").textContent = minutes.toString().padStart(2, "0");
        document.getElementById("seconds").textContent = seconds.toString().padStart(2, "0");
      }

      setInterval(updateCountdown, 1000);
      updateCountdown();

      // --- Smooth scrolling for anchor links ---
      document.querySelectorAll('a[href^="#"]').forEach((anchor) => {
        anchor.addEventListener("click", function (e) {
          const targetId = this.getAttribute("href");
          if (targetId === "#" || targetId === "") return;

          const targetElement = document.querySelector(targetId);
          if (targetElement) {
            e.preventDefault();
            window.scrollTo({
              top: targetElement.offsetTop - 80,
              behavior: "smooth",
            });
          }
        });
      });

      // --- Animate elements when scrolling ---
      const animateOnScroll = function () {
        const elements = document.querySelectorAll(".fade-in");

        elements.forEach((element) => {
          const elementPosition = element.getBoundingClientRect().top;
          const windowHeight = window.innerHeight;

          if (elementPosition < windowHeight - 100) {
            element.style.opacity = 1;
            element.style.transform = "translateY(0)";
          }
        });
      };

      window.addEventListener("scroll", animateOnScroll);

      // --- Filter Produk berdasarkan kategori ---
      const filterButtons = document.querySelectorAll(".filter-btn");
      const productList = document.getElementById("product-list");

      filterButtons.forEach((btn) => {
        btn.addEventListener("click", () => {
          filterButtons.forEach((b) => b.classList.remove("active", "bg-black", "text-white"));
          btn.classList.add("active", "bg-black", "text-white");

          const filter = btn.dataset.filter;
          const products = productList.querySelectorAll(".product-card");

          products.forEach((product) => {
            if (filter === "all" || product.dataset.category === filter) {
              product.style.display = "";
            } else {
              product.style.display = "none";
            }
          });
        });
      });

      // --- Search Produk berdasarkan nama ---
      const searchInput = document.getElementById("search-input");
      searchInput.addEventListener("input", () => {
        const query = searchInput.value.toLowerCase();
        const products = productList.querySelectorAll(".product-card");

        products.forEach((product) => {
          const name = product.dataset.name.toLowerCase();
          if (name.includes(query)) {
            product.style.display = "";
          } else {
            product.style.display = "none";
          }
        });
      });

      // --- Inisialisasi Aplikasi ---
      updateAuthUI();
      animateOnScroll(); // Jalankan sekali saat load
      updateCartUI();
    });
  </script>
 </body>
</html>
