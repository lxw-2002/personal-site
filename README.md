# personal-site<html lang="ja-JP"><head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>盧暁文の個人紹介</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdn.jsdelivr.net/npm/font-awesome@4.7.0/css/font-awesome.min.css" rel="stylesheet">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        primary: '#4B5563',
                        secondary: '#9CA3AF',
                        accent: '#F59E0B',
                        light: '#F9FAFB',
                        dark: '#1F2937',
                    },
                    fontFamily: {
                        sans: ['Inter', 'system-ui', 'sans-serif'],
                    },
                }
            }
        }
    </script>
    <style type="text/tailwindcss">
        @layer utilities {
            .content-auto {
                content-visibility: auto;
            }
            .text-shadow {
                text-shadow: 0 2px 4px rgba(0,0,0,0.1);
            }
            .bg-blur {
                backdrop-filter: blur(8px);
            }
            .scrollbar-hide::-webkit-scrollbar {
                display: none;
            }
            .scrollbar-hide {
                -ms-overflow-style: none;
                scrollbar-width: none;
            }
        }
    </style>
</head>
<body class="bg-gray-50 text-gray-800 font-sans antialiased">
    <!-- ナビゲーションバー -->
    <header id="navbar" class="fixed w-full z-50 transition-all duration-300">
        <nav class="bg-primary/90 bg-blur text-white shadow-md">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="flex justify-between h-16">
                    <div class="flex items-center">
                        <span class="text-xl font-bold tracking-tight">盧暁文</span>
                    </div>
                    <div class="hidden md:flex items-center space-x-8">
                        <a href="#about" class="text-white hover:text-accent transition-colors duration-200">自己紹介</a>
                        <a href="#interests" class="text-white hover:text-accent transition-colors duration-200">趣味</a>
                        <a href="#hometown" class="text-white hover:text-accent transition-colors duration-200">故郷</a>
                        <a href="#dreams" class="text-white hover:text-accent transition-colors duration-200">将来の夢</a>
                    </div>
                    <div class="md:hidden flex items-center">
                        <button id="mobile-menu-button" class="text-white hover:text-accent">
                            <i class="fa fa-bars text-xl"></i>
                        </button>
                    </div>
                </div>
            </div>
            <!-- モバイルメニュー -->
            <div id="mobile-menu" class="hidden md:hidden bg-primary/95 bg-blur">
                <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3">
                    <a href="#about" class="block px-3 py-2 text-white hover:bg-gray-700 rounded-md">自己紹介</a>
                    <a href="#interests" class="block px-3 py-2 text-white hover:bg-gray-700 rounded-md">趣味</a>
                    <a href="#hometown" class="block px-3 py-2 text-white hover:bg-gray-700 rounded-md">故郷</a>
                    <a href="#dreams" class="block px-3 py-2 text-white hover:bg-gray-700 rounded-md">将来の夢</a>
                </div>
            </div>
        </nav>
    </header>

    <!-- ヒーローセクション -->
    <section class="relative h-screen flex items-center justify-center overflow-hidden">
        <div class="absolute inset-0 bg-cover bg-center" style="background-image: url('https://picsum.photos/id/1018/1920/1080'); filter: brightness(0.6);"></div>
        <div class="relative z-10 text-center px-4">
            <h1 class="text-[clamp(2.5rem,8vw,5rem)] font-bold text-white mb-4 text-shadow">
                盧暁文
            </h1>
            <p class="text-[clamp(1.2rem,3vw,1.8rem)] text-white mb-8 max-w-3xl mx-auto text-shadow">
                第一工科大学学生・小説愛好家・旅行者・音楽ファン
            </p>
            <div class="flex flex-wrap justify-center gap-4">
                <a href="#about" class="bg-accent hover:bg-amber-500 text-white font-medium py-3 px-6 rounded-full transition-all duration-300 transform hover:scale-105 shadow-lg">詳しく見る</a>
                <a href="#hometown" class="bg-transparent border-2 border-white hover:bg-white/10 text-white font-medium py-3 px-6 rounded-full transition-all duration-300 transform hover:scale-105">
                    私の故郷
                </a>
            </div>
        </div>
        <div class="absolute bottom-10 left-0 right-0 flex justify-center animate-bounce">
            <a href="#about" class="text-white">
                <i class="fa fa-angle-down text-3xl"></i>
            </a>
        </div>
    </section>

    <!-- 自己紹介 -->
    <section id="about" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-[clamp(1.8rem,5vw,3rem)] font-bold text-primary mb-4">自己紹介</h2>
                <div class="w-24 h-1 bg-accent mx-auto rounded-full"></div>
            </div>
            <div class="max-w-3xl mx-auto">
                <div>
                    <h3 class="text-2xl font-semibold text-primary mb-6">私について</h3>
                    <p class="text-gray-600 mb-4 text-lg leading-relaxed">
                        盧暁文と申します。現在、第一工科大学に在籍し、コンピュータサイエンスを専攻しています。テクノロジーとイノベーションに情熱を持ち、新しい知識の領域を探索することが好きです。
                    </p>
                    <p class="text-gray-600 mb-6 text-lg leading-relaxed">
                        勉強以外の時間は、小説を読んだり、旅行したり、音楽を聴いたりして過ごします。これらの趣味は私の生活を豊かにするだけでなく、世界を異なる角度から見ることができ、新しいインスピレーションを得ることができます。
                    </p>
                    <div class="flex flex-wrap gap-4 mb-8">
                        <span class="bg-gray-100 text-primary px-4 py-2 rounded-full text-sm font-medium">コンピュータサイエンス</span>
                        <span class="bg-gray-100 text-primary px-4 py-2 rounded-full text-sm font-medium">小説愛好家</span>
                        <span class="bg-gray-100 text-primary px-4 py-2 rounded-full text-sm font-medium">旅行者</span>
                        <span class="bg-gray-100 text-primary px-4 py-2 rounded-full text-sm font-medium">音楽ファン</span>
                    </div>
                    <div class="flex items-center space-x-4">
                        <a href="#interests" class="text-accent hover:text-amber-600 font-medium flex items-center transition-colors duration-200">
                            私の趣味を知る <i class="fa fa-arrow-right ml-2"></i>
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 趣味 -->
    <section id="interests" class="py-20 bg-gray-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-[clamp(1.8rem,5vw,3rem)] font-bold text-primary mb-4">趣味</h2>
                <div class="w-24 h-1 bg-accent mx-auto rounded-full"></div>
            </div>
            <div class="grid md:grid-cols-3 gap-8">
                <!-- 趣味1：小説を読む -->
                <div class="bg-white rounded-xl shadow-lg overflow-hidden transform transition-all duration-300 hover:-translate-y-2 hover:shadow-xl">
                    <div class="h-60 overflow-hidden">
                        <img src="https://picsum.photos/id/24/600/400" alt="小説を読む" class="w-full h-full object-cover transition-transform duration-500 hover:scale-110">
                    </div>
                    <div class="p-6">
                        <div class="w-12 h-12 bg-primary/10 rounded-full flex items-center justify-center mb-4">
                            <i class="fa fa-book text-primary text-xl"></i>
                        </div>
                        <h3 class="text-xl font-semibold text-primary mb-3">小説を読む</h3>
                        <p class="text-gray-600 mb-4">
                            私はさまざまなジャンルの小説、特にSF、サスペンス、文学作品を読むのが大好きです。読書を通じて、異なる人生を体験し、視野を広げ、心を豊かにすることができます。
                        </p>
                        <div class="flex items-center text-sm text-gray-500">
                            <i class="fa fa-heart text-accent mr-1"></i>
                            <span>好きな作家：劉慈欣、東野圭吾</span>
                        </div>
                    </div>
                </div>

                <!-- 趣味2：旅行 -->
                <div class="bg-white rounded-xl shadow-lg overflow-hidden transform transition-all duration-300 hover:-translate-y-2 hover:shadow-xl">
                    <div class="h-60 overflow-hidden">
                        <img src="https://picsum.photos/id/10/600/400" alt="旅行" class="w-full h-full object-cover transition-transform duration-500 hover:scale-110">
                    </div>
                    <div class="p-6">
                        <div class="w-12 h-12 bg-primary/10 rounded-full flex items-center justify-center mb-4">
                            <i class="fa fa-plane text-primary text-xl"></i>
                        </div>
                        <h3 class="text-xl font-semibold text-primary mb-3">旅行</h3>
                        <p class="text-gray-600 mb-4">
                            旅行は私の生活の中で欠かせない部分です。さまざまな都市や文化を探検し、地元の料理を味わい、新しい友達を作り、世界の多様性を感じるのが好きです。
                        </p>
                        <div class="flex items-center text-sm text-gray-500">
                            <i class="fa fa-map-marker text-accent mr-1"></i>
                            <span>忘れられない旅行：チベット、雲南</span>
                        </div>
                    </div>
                </div>

                <!-- 趣味3：音楽を聴く -->
                <div class="bg-white rounded-xl shadow-lg overflow-hidden transform transition-all duration-300 hover:-translate-y-2 hover:shadow-xl">
                    <div class="h-60 overflow-hidden">
                        <img src="https://picsum.photos/id/96/600/400" alt="音楽を聴く" class="w-full h-full object-cover transition-transform duration-500 hover:scale-110">
                    </div>
                    <div class="p-6">
                        <div class="w-12 h-12 bg-primary/10 rounded-full flex items-center justify-center mb-4">
                            <i class="fa fa-music text-primary text-xl"></i>
                        </div>
                        <h3 class="text-xl font-semibold text-primary mb-3">音楽を聴く</h3>
                        <p class="text-gray-600 mb-4">
                            音楽は私の心の安らぎです。勉強中、仕事中、リラックス中いつでも音楽を聴くのが好きです。クラシックからポップ、ロックからジャズまで、さまざまなタイプの音楽を楽しみます。
                        </p>
                        <div class="flex items-center text-sm text-gray-500">
                            <i class="fa fa-headphones text-accent mr-1"></i>
                            <span>好きな歌手：周杰倫、陳奕迅</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 故郷の大連 -->
    <section id="hometown" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-[clamp(1.8rem,5vw,3rem)] font-bold text-primary mb-4">私の故郷</h2>
                <div class="w-24 h-1 bg-accent mx-auto rounded-full"></div>
            </div>
            <div class="grid md:grid-cols-2 gap-12 items-center">
                <div>
                    <h3 class="text-2xl font-semibold text-primary mb-6">大連</h3>
                    <p class="text-gray-600 mb-4 text-lg leading-relaxed">
                        大連は、中国東北の遼東半島の南端に位置する美しい海浜都市で、私の故郷です。三面を海に囲まれ、気候が宜人で、魅力的なビーチ、ヨーロッパ風の建築、豊富な海鮮料理で知られています。
                    </p>
                    <p class="text-gray-600 mb-6 text-lg leading-relaxed">
                        大連の都市景観は自然美と人文的魅力が融合しています。星海広場、棒棰島、金石滩などの観光地は数多くの観光客を引き付けています。また、大連には深い歴史的底蘊があり、ロシア風情街、中山広場などはこの都市の独特な歴史的痕跡を垣間見ることができます。
                    </p>
                    <div class="grid grid-cols-2 gap-4 mb-8">
                        <div class="flex items-center">
                            <i class="fa fa-map-marker text-accent mr-3 text-xl"></i>
                            <div>
                                <h4 class="font-medium text-primary">地理位置</h4>
                                <p class="text-gray-600 text-sm">中国遼寧省东南部</p>
                            </div>
                        </div>
                        <div class="flex items-center">
                            <i class="fa fa-sun-o text-accent mr-3 text-xl"></i>
                            <div>
                                <h4 class="font-medium text-primary">気候</h4>
                                <p class="text-gray-600 text-sm">温帯季節風気候</p>
                            </div>
                        </div>
                        <div class="flex items-center">
                            <i class="fa fa-cutlery text-accent mr-3 text-xl"></i>
                            <div>
                                <h4 class="font-medium text-primary">特色美食</h4>
                                <p class="text-gray-600 text-sm">海鮮、焖子、海菜饅頭</p>
                            </div>
                        </div>
                        <div class="flex items-center">
                            <i class="fa fa-tree text-accent mr-3 text-xl"></i>
                            <div>
                                <h4 class="font-medium text-primary">著名観光地</h4>
                                <p class="text-gray-600 text-sm">星海広場、金石滩、老虎灘</p>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="grid grid-cols-2 gap-4">
                    <div class="space-y-4">
                        <img src="https://picsum.photos/id/1036/600/400" alt="大連星海広場" class="w-full h-48 object-cover rounded-lg shadow-md transform transition-transform duration-500 hover:scale-105">
                        <img src="https://picsum.photos/id/164/600/400" alt="大連沿海道路" class="w-full h-64 object-cover rounded-lg shadow-md transform transition-transform duration-500 hover:scale-105">
                    </div>
                    <div class="space-y-4 pt-8">
                        <img src="https://picsum.photos/id/158/600/400" alt="大連金石灘" class="w-full h-64 object-cover rounded-lg shadow-md transform transition-transform duration-500 hover:scale-105">
                        <img src="https://picsum.photos/id/1067/600/400" alt="大連ロシア風情街" class="w-full h-48 object-cover rounded-lg shadow-md transform transition-transform duration-500 hover:scale-105">
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 将来の夢 -->
    <section id="dreams" class="py-20 bg-gray-50 relative overflow-hidden">
        <div class="absolute inset-0 opacity-5">
            <div class="absolute inset-0 bg-[url('https://picsum.photos/id/1018/1920/1080')] bg-cover bg-center"></div>
        </div>
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <div class="text-center mb-16">
                <h2 class="text-[clamp(1.8rem,5vw,3rem)] font-bold text-primary mb-4">将来の夢</h2>
                <div class="w-24 h-1 bg-accent mx-auto rounded-full"></div>
            </div>
            <div class="grid md:grid-cols-2 gap-16 items-center">
                <div class="order-2 md:order-1">
                    <div class="space-y-8">
                        <!-- 夢1：たくさんお金を稼ぐ -->
                        <div class="bg-white p-6 rounded-xl shadow-lg transform transition-all duration-300 hover:-translate-y-1 hover:shadow-xl">
                            <div class="flex items-start">
                                <div class="w-12 h-12 bg-primary/10 rounded-full flex items-center justify-center flex-shrink-0 mr-4">
                                    <i class="fa fa-money text-primary text-xl"></i>
                                </div>
                                <div>
                                    <h3 class="text-xl font-semibold text-primary mb-3">たくさんお金を稼ぐ</h3>
                                    <p class="text-gray-600">
                                        私は自分の努力と才能を通じて、安定した経済的収入を築きたいと考えています。これによって快適な生活を送るだけでなく、家族により良い条件を提供し、より多くの可能性を実現することができます。
                                    </p>
                                </div>
                            </div>
                        </div>

                        <!-- 夢2：世界一周旅行 -->
                        <div class="bg-white p-6 rounded-xl shadow-lg transform transition-all duration-300 hover:-translate-y-1 hover:shadow-xl">
                            <div class="flex items-start">
                                <div class="w-12 h-12 bg-primary/10 rounded-full flex items-center justify-center flex-shrink-0 mr-4">
                                    <i class="fa fa-globe text-primary text-xl"></i>
                                </div>
                                <div>
                                    <h3 class="text-xl font-semibold text-primary mb-3">世界一周旅行</h3>
                                    <p class="text-gray-600">
                                        世界はとても広く、私はそれを見て回りたいです。いつか世界一周旅行ができる夢を持っています。異なる国や地域の文化、風景、料理を体験し、世界中の友達と出会い、人生の経験を豊かにしたいです。
                                    </p>
                                </div>
                            </div>
                        </div>

                        <!-- 夢3：自己成長 -->
                        <div class="bg-white p-6 rounded-xl shadow-lg transform transition-all duration-300 hover:-translate-y-1 hover:shadow-xl">
                            <div class="flex items-start">
                                <div class="w-12 h-12 bg-primary/10 rounded-full flex items-center justify-center flex-shrink-0 mr-4">
                                    <i class="fa fa-graduation-cap text-primary text-xl"></i>
                                </div>
                                <div>
                                    <h3 class="text-xl font-semibold text-primary mb-3">自己成長</h3>
                                    <p class="text-gray-600">
                                        不断に学び成長することは私の人生において重要な目標です。専門分野で成果を上げると同時に、幅広い趣味を養い、内面が豊かで見識のある責任感の強い人間になりたいです。
                                    </p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="order-1 md:order-2">
                    <div class="relative">
                        <div class="absolute -top-6 -right-6 w-32 h-32 bg-gray-200 rounded-lg -z-10"></div>
                        <div class="absolute -bottom-6 -left-6 w-32 h-32 bg-gray-200 rounded-lg -z-10"></div>
                        <img src="https://picsum.photos/id/1039/600/800" alt="未来の夢" class="w-full h-auto rounded-lg shadow-xl object-cover transform transition-transform duration-500 hover:scale-[1.02]">
                        <div class="absolute -bottom-6 -right-6 bg-white p-4 rounded-lg shadow-lg max-w-xs">
                            <p class="text-primary font-medium italic">"人生は勤勉にあり、求めざれば何を得るか。"</p>
                            <p class="text-gray-500 text-sm mt-1">—— 張衡</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- フッター -->
    <footer class="bg-primary text-white py-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid md:grid-cols-2 gap-8">
                <div>
                    <h3 class="text-xl font-bold mb-4">盧暁文</h3>
                    <p class="text-gray-300 mb-6">
                        第一工科大学学生、生活を愛し、夢を追い求める。
                    </p>
                    <div class="flex space-x-4">
                        <a href="#" class="text-gray-300 hover:text-white transition-colors duration-200">
                            <i class="fa fa-weixin text-xl"></i>
                        </a>
                        <a href="#" class="text-gray-300 hover:text-white transition-colors duration-200">
                            <i class="fa fa-qq text-xl"></i>
                        </a>
                        <a href="#" class="text-gray-300 hover:text-white transition-colors duration-200">
                            <i class="fa fa-weibo text-xl"></i>
                        </a>
                    </div>
                </div>
                <div>
                    <h3 class="text-xl font-bold mb-4">クイックリンク</h3>
                    <ul class="space-y-2">
                        <li>
                            <a href="#about" class="text-gray-300 hover:text-white transition-colors duration-200">自己紹介</a>
                        </li>
                        <li>
                            <a href="#interests" class="text-gray-300 hover:text-white transition-colors duration-200">趣味</a>
                        </li>
                        <li>
                            <a href="#hometown" class="text-gray-300 hover:text-white transition-colors duration-200">故郷</a>
                        </li>
                        <li>
                            <a href="#dreams" class="text-gray-300 hover:text-white transition-colors duration-200">将来の夢</a>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="border-t border-gray-700 mt-10 pt-6 text-center text-gray-400">
                <p>© 2023 盧暁文. 全著作権所有.</p>
            </div>
        </div>
    </footer>

    <!-- トップに戻るボタン -->
    <button id="back-to-top" class="fixed bottom-6 right-6 bg-accent text-white w-12 h-12 rounded-full flex items-center justify-center shadow-lg transform transition-all duration-300 opacity-0 translate-y-10">
        <i class="fa fa-arrow-up"></i>
    </button>

    <!-- JavaScript -->
    <script>
        // ナビゲーションバーのスクロール効果
        const navbar = document.getElementById('navbar');
        const backToTop = document.getElementById('back-to-top');

        window.addEventListener('scroll', function() {
            if (window.scrollY > 50) {
                navbar.classList.add('bg-primary');
                navbar.classList.remove('bg-primary/90');
                navbar.classList.add('shadow-lg');
                
                backToTop.classList.remove('opacity-0', 'translate-y-10');
                backToTop.classList.add('opacity-100', 'translate-y-0');
            } else {
                navbar.classList.remove('bg-primary');
                navbar.classList.add('bg-primary/90');
                navbar.classList.remove('shadow-lg');
                
                backToTop.classList.add('opacity-0', 'translate-y-10');
                backToTop.classList.remove('opacity-100', 'translate-y-0');
            }
        });

        // モバイルメニュー
        const mobileMenuButton = document.getElementById('mobile-menu-button');
        const mobileMenu = document.getElementById('mobile-menu');

        mobileMenuButton.addEventListener('click', function() {
            mobileMenu.classList.toggle('hidden');
            if (mobileMenu.classList.contains('hidden')) {
                mobileMenuButton.innerHTML = '<i class="fa fa-bars text-xl"></i>';
            } else {
                mobileMenuButton.innerHTML = '<i class="fa fa-times text-xl"></i>';
            }
        });

        // スムーズスクロール
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                
                // モバイルメニューを閉じる
                if (!mobileMenu.classList.contains('hidden')) {
                    mobileMenu.classList.add('hidden');
                    mobileMenuButton.innerHTML = '<i class="fa fa-bars text-xl"></i>';
                }
                
                const targetId = this.getAttribute('href');
                const targetElement = document.querySelector(targetId);
                
                if (targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                }
            });
        });

        // トップに戻る
        backToTop.addEventListener('click', function() {
            window.scrollTo({
                top: 0,
                behavior: 'smooth'
            });
        });

        // 画像の遅延読み込み
        document.addEventListener("DOMContentLoaded", function() {
            const lazyImages = [].slice.call(document.querySelectorAll("img"));
            
            if ("IntersectionObserver" in window) {
                let lazyImageObserver = new IntersectionObserver(function(entries, observer) {
                    entries.forEach(function(entry) {
                        if (entry.isIntersecting) {
                            let lazyImage = entry.target;
                            lazyImage.src = lazyImage.dataset.src || lazyImage.src;
                            lazyImageObserver.unobserve(lazyImage);
                        }
                    });
                });
                
                lazyImages.forEach(function(lazyImage) {
                    lazyImageObserver.observe(lazyImage);
                });
            }
        });

        // ページ読み込みアニメーション
        window.addEventListener('load', function() {
            document.body.classList.add('loaded');
        });
    </script>


</body></html>
