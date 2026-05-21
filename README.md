<!DOCTYPE html>
<!-- saved from url=(0034)file:///D:/Desktop/Untitled-1.html -->
<html lang="zh-CN"><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
    
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>豪士面包 | 爆款早餐推荐</title>
    <link rel="stylesheet" href="./豪士面包 _ 爆款早餐推荐_files/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Helvetica Neue', Arial, 'Microsoft YaHei', sans-serif;
        }
        
        :root {
            --primary-color: #e63946;
            --secondary-color: #f4a261;
            --light-color: #f8f9fa;
            --dark-color: #333333;
            --gray-color: #6c757d;
        }
        
        body {
            background-color: #f9f5f0;
            color: var(--dark-color);
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* 头部样式 */
        header {
            background: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)), url('https://images.unsplash.com/photo-1567620905732-2d1ec7ab7445?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1180&q=80');
            background-size: cover;
            background-position: center;
            color: white;
            padding: 100px 0 60px;
            text-align: center;
            position: relative;
        }
        
        .logo {
            font-size: 2.8rem;
            font-weight: 800;
            margin-bottom: 10px;
            color: var(--light-color);
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        }
        
        .logo span {
            color: var(--secondary-color);
        }
        
        .tagline {
            font-size: 1.2rem;
            margin-bottom: 30px;
            opacity: 0.9;
        }
        
        /* 导航栏 */
        nav {
            background-color: white;
            box-shadow: 0 2px 15px rgba(0, 0, 0, 0.1);
            position: sticky;
            top: 0;
            z-index: 1000;
        }
        
        .nav-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 0;
        }
        
        .nav-links {
            display: flex;
            list-style: none;
        }
        
        .nav-links li {
            margin-left: 30px;
        }
        
        .nav-links a {
            text-decoration: none;
            color: var(--dark-color);
            font-weight: 600;
            transition: color 0.3s;
        }
        
        .nav-links a:hover {
            color: var(--primary-color);
        }
        
        .nav-links a.active {
            color: var(--primary-color);
        }
        
        .mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            font-size: 1.5rem;
            color: var(--dark-color);
            cursor: pointer;
        }
        
        /* 主要内容区 */
        .main-title {
            text-align: center;
            margin: 60px 0 40px;
            position: relative;
        }
        
        .main-title h1 {
            font-size: 2.8rem;
            color: var(--dark-color);
            margin-bottom: 15px;
        }
        
        .main-title h1 span {
            color: var(--primary-color);
        }
        
        .main-title p {
            color: var(--gray-color);
            font-size: 1.1rem;
            max-width: 700px;
            margin: 0 auto;
        }
        
        /* 产品网格 */
        .products-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(350px, 1fr));
            gap: 30px;
            margin-bottom: 60px;
        }
        
        .product-card {
            background-color: white;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.08);
            transition: transform 0.3s, box-shadow 0.3s;
        }
        
        .product-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.15);
        }
        
        .product-img {
            height: 250px;
            overflow: hidden;
        }
        
        .product-img img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s;
        }
        
        .product-card:hover .product-img img {
            transform: scale(1.05);
        }
        
        .product-content {
            padding: 25px;
        }
        
        .product-title {
            font-size: 1.5rem;
            margin-bottom: 10px;
            color: var(--dark-color);
        }
        
        .product-desc {
            color: var(--gray-color);
            margin-bottom: 20px;
            font-size: 0.95rem;
        }
        
        .product-tags {
            display: flex;
            flex-wrap: wrap;
            margin-bottom: 20px;
        }
        
        .tag {
            background-color: #ffe5e7;
            color: var(--primary-color);
            padding: 5px 12px;
            border-radius: 20px;
            font-size: 0.8rem;
            font-weight: 600;
            margin-right: 8px;
            margin-bottom: 8px;
        }
        
        .product-footer {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .price {
            font-size: 1.3rem;
            font-weight: 700;
            color: var(--primary-color);
        }
        
        .btn {
            background-color: var(--primary-color);
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 30px;
            font-weight: 600;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        
        .btn:hover {
            background-color: #d32f2f;
        }
        
        /* 特色推荐 */
        .featured {
            background-color: white;
            border-radius: 15px;
            padding: 40px;
            margin-bottom: 60px;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.08);
        }
        
        .featured h2 {
            text-align: center;
            margin-bottom: 30px;
            font-size: 2.2rem;
            color: var(--dark-color);
        }
        
        .featured-content {
            display: flex;
            align-items: center;
            gap: 40px;
        }
        
        .featured-img {
            flex: 1;
            border-radius: 10px;
            overflow: hidden;
        }
        
        .featured-img img {
            width: 100%;
            height: auto;
            display: block;
        }
        
        .featured-text {
            flex: 1;
        }
        
        .featured-text h3 {
            font-size: 1.8rem;
            margin-bottom: 20px;
            color: var(--dark-color);
        }
        
        .featured-text p {
            margin-bottom: 20px;
            color: var(--gray-color);
        }
        
        /* 早餐搭配建议 */
        .breakfast-tips {
            background-color: white;
            border-radius: 15px;
            padding: 40px;
            margin-bottom: 60px;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.08);
        }
        
        .breakfast-tips h2 {
            text-align: center;
            margin-bottom: 30px;
            font-size: 2.2rem;
            color: var(--dark-color);
        }
        
        .tips-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 30px;
        }
        
        .tip-item {
            text-align: center;
            padding: 20px;
        }
        
        .tip-icon {
            background-color: #ffe5e7;
            color: var(--primary-color);
            width: 70px;
            height: 70px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 20px;
            font-size: 1.8rem;
        }
        
        .tip-item h3 {
            margin-bottom: 15px;
            color: var(--dark-color);
        }
        
        /* 页脚 */
        footer {
            background-color: var(--dark-color);
            color: white;
            padding: 60px 0 30px;
        }
        
        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            margin-bottom: 40px;
        }
        
        .footer-section h3 {
            font-size: 1.3rem;
            margin-bottom: 20px;
            position: relative;
            padding-bottom: 10px;
        }
        
        .footer-section h3::after {
            content: '';
            position: absolute;
            left: 0;
            bottom: 0;
            width: 50px;
            height: 3px;
            background-color: var(--primary-color);
        }
        
        .footer-section p {
            margin-bottom: 20px;
            opacity: 0.8;
        }
        
        .social-links {
            display: flex;
            gap: 15px;
        }
        
        .social-links a {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            background-color: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            color: white;
            text-decoration: none;
            transition: background-color 0.3s;
        }
        
        .social-links a:hover {
            background-color: var(--primary-color);
        }
        
        .footer-links li {
            list-style: none;
            margin-bottom: 10px;
        }
        
        .footer-links a {
            color: rgba(255, 255, 255, 0.8);
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .footer-links a:hover {
            color: var(--primary-color);
        }
        
        .copyright {
            text-align: center;
            padding-top: 30px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            opacity: 0.7;
            font-size: 0.9rem;
        }
        
        /* 响应式设计 */
        @media (max-width: 992px) {
            .featured-content {
                flex-direction: column;
            }
            
            .nav-links {
                display: none;
            }
            
            .mobile-menu-btn {
                display: block;
            }
            
            .nav-links.active {
                display: flex;
                flex-direction: column;
                position: absolute;
                top: 100%;
                left: 0;
                width: 100%;
                background-color: white;
                box-shadow: 0 5px 10px rgba(0, 0, 0, 0.1);
                padding: 20px;
            }
            
            .nav-links.active li {
                margin: 10px 0;
            }
        }
        
        @media (max-width: 768px) {
            .main-title h1 {
                font-size: 2.2rem;
            }
            
            .products-grid {
                grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            }
            
            .product-img {
                height: 200px;
            }
            
            .featured, .breakfast-tips {
                padding: 30px 20px;
            }
        }
        
        @media (max-width: 576px) {
            header {
                padding: 80px 0 40px;
            }
            
            .logo {
                font-size: 2.2rem;
            }
            
            .main-title h1 {
                font-size: 1.8rem;
            }
            
            .products-grid {
                grid-template-columns: 1fr;
            }
            
            .featured h2, .breakfast-tips h2 {
                font-size: 1.8rem;
            }
        }
        
        /* 动画效果 */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .fade-in {
            animation: fadeIn 0.8s ease-out forwards;
        }
    </style>
</head>
<body>
    <!-- 头部区域 -->
    <header>
        <div class="container">
            <h1 class="logo">豪士<span>面包</span></h1>
            <p class="tagline">每一口都是新鲜，每一天都有好心情</p>
            <p>精选优质原料，打造您的每日美味早餐</p>
        </div>
    </header>
    
    <!-- 导航栏 -->
    <nav>
        <div class="container nav-container">
            <div class="logo">豪士<span>面包</span></div>
            <button class="mobile-menu-btn" id="mobileMenuBtn">
                <i class="fas fa-bars"></i>
            </button>
            <ul class="nav-links" id="navLinks">
                <li><a href="file:///D:/Desktop/Untitled-1.html#" class="active">爆款早餐</a></li>
                <li><a href="file:///D:/Desktop/Untitled-1.html#">产品系列</a></li>
                <li><a href="file:///D:/Desktop/Untitled-1.html#">早餐搭配</a></li>
                <li><a href="file:///D:/Desktop/Untitled-1.html#">品牌故事</a></li>
                <li><a href="file:///D:/Desktop/Untitled-1.html#">购买渠道</a></li>
            </ul>
        </div>
    </nav>
    
    <!-- 主要内容 -->
    <main class="container">
        <!-- 标题 -->
        <section class="main-title fade-in">
            <h1>豪士<span>爆款早餐</span>推荐</h1>
            <p>探索最受欢迎的豪士早餐选择，为您的一天注入满满能量。无论是匆忙的早晨还是悠闲的周末，总有一款适合您。</p>
        </section>
        
        <!-- 产品网格 -->
        <section class="products-grid">
            <!-- 产品1 -->
            <article class="product-card fade-in">
                <div class="product-img">
                    <img src="./豪士面包 _ 爆款早餐推荐_files/photo-1555507036-ab794f27d2e9" alt="豪士牛奶夹心面包">
                </div>
                <div class="product-content">
                    <h3 class="product-title">豪士牛奶夹心面包</h3>
                    <p class="product-desc">松软面包体包裹着香浓牛奶夹心，口感细腻绵密，奶香四溢，是孩子们的最爱。</p>
                    <div class="product-tags">
                        <span class="tag">畅销爆款</span>
                        <span class="tag">儿童喜爱</span>
                        <span class="tag">奶香浓郁</span>
                    </div>
                    <div class="product-footer">
                        <div class="price">¥19.9</div>
                        <button class="btn">立即购买</button>
                    </div>
                </div>
            </article>
            
            <!-- 产品2 -->
            <article class="product-card fade-in">
                <div class="product-img">
                    <img src="./豪士面包 _ 爆款早餐推荐_files/photo-1488477181946-6428a0291777" alt="豪士全麦三明治">
                </div>
                <div class="product-content">
                    <h3 class="product-title">豪士全麦三明治</h3>
                    <p class="product-desc">全麦面包搭配新鲜蔬菜、鸡蛋和火腿，低脂健康，营养均衡，适合健身早餐。</p>
                    <div class="product-tags">
                        <span class="tag">健康低脂</span>
                        <span class="tag">营养均衡</span>
                        <span class="tag">上班族必备</span>
                    </div>
                    <div class="product-footer">
                        <div class="price">¥24.9</div>
                        <button class="btn">立即购买</button>
                    </div>
                </div>
            </article>
            
            <!-- 产品3 -->
            <article class="product-card fade-in">
                <div class="product-img">
                    <img src="./豪士面包 _ 爆款早餐推荐_files/photo-1608198093002-ad4e0054842b" alt="豪士菠萝包">
                </div>
                <div class="product-content">
                    <h3 class="product-title">豪士经典菠萝包</h3>
                    <p class="product-desc">金黄酥脆的外皮，柔软香甜的内里，经典港式风味，唤醒您的味蕾记忆。</p>
                    <div class="product-tags">
                        <span class="tag">经典港式</span>
                        <span class="tag">酥脆香甜</span>
                        <span class="tag">早餐优选</span>
                    </div>
                    <div class="product-footer">
                        <div class="price">¥16.8</div>
                        <button class="btn">立即购买</button>
                    </div>
                </div>
            </article>
            
            <!-- 产品4 -->
            <article class="product-card fade-in">
                <div class="product-img">
                    <img src="./豪士面包 _ 爆款早餐推荐_files/photo-1546069901-ba9599a7e63c" alt="豪士法式可颂">
                </div>
                <div class="product-content">
                    <h3 class="product-title">豪士法式可颂</h3>
                    <p class="product-desc">酥脆金黄的外层，层次分明的内里，黄油香气浓郁，搭配咖啡绝佳。</p>
                    <div class="product-tags">
                        <span class="tag">法式经典</span>
                        <span class="tag">黄油香气</span>
                        <span class="tag">咖啡伴侣</span>
                    </div>
                    <div class="product-footer">
                        <div class="price">¥22.5</div>
                        <button class="btn">立即购买</button>
                    </div>
                </div>
            </article>
            
            <!-- 产品5 -->
            <article class="product-card fade-in">
                <div class="product-img">
                    <img src="./豪士面包 _ 爆款早餐推荐_files/photo-1565299624946-b28f40a0ae38" alt="豪士肉松小贝">
                </div>
                <div class="product-content">
                    <h3 class="product-title">豪士肉松小贝</h3>
                    <p class="product-desc">松软蛋糕体包裹着鲜美肉松，咸甜适中，口感丰富，网红早餐新选择。</p>
                    <div class="product-tags">
                        <span class="tag">网红爆款</span>
                        <span class="tag">咸甜适中</span>
                        <span class="tag">口感丰富</span>
                    </div>
                    <div class="product-footer">
                        <div class="price">¥28.8</div>
                        <button class="btn">立即购买</button>
                    </div>
                </div>
            </article>
            
            <!-- 产品6 -->
            <article class="product-card fade-in">
                <div class="product-img">
                    <img src="./豪士面包 _ 爆款早餐推荐_files/photo-1608198093002-ad4e0054842b" alt="豪士巧克力丹麦">
                </div>
                <div class="product-content">
                    <h3 class="product-title">豪士巧克力丹麦</h3>
                    <p class="product-desc">酥脆的丹麦面包搭配浓郁巧克力，每一口都是甜蜜的享受，满足您的甜食渴望。</p>
                    <div class="product-tags">
                        <span class="tag">巧克力控</span>
                        <span class="tag">甜蜜享受</span>
                        <span class="tag">下午茶优选</span>
                    </div>
                    <div class="product-footer">
                        <div class="price">¥26.9</div>
                        <button class="btn">立即购买</button>
                    </div>
                </div>
            </article>
        </section>
        
        <!-- 特色推荐 -->
        <section class="featured fade-in">
            <h2>本周<span style="color: var(--primary-color);">特色推荐</span></h2>
            <div class="featured-content">
                <div class="featured-img">
                    <img src="./豪士面包 _ 爆款早餐推荐_files/photo-1607472586893-edb57bdc0e39" alt="豪士早餐套餐">
                </div>
                <div class="featured-text">
                    <h3>豪士营养早餐套餐</h3>
                    <p>精选豪士最受欢迎的4款产品组合，包含牛奶夹心面包、全麦三明治、菠萝包和肉松小贝，满足全家人的不同口味需求。</p>
                    <p>套餐特惠价仅需 ¥89.9，比单独购买节省 15%。每天一款，一周早餐不重样！</p>
                    <p>特别适合忙碌的上班族和学生党，5分钟即可准备一份营养美味的早餐，让您精力充沛一整天。</p>
                    <button class="btn" style="margin-top: 20px; padding: 12px 30px;">查看套餐详情</button>
                </div>
            </div>
        </section>
        
        <!-- 早餐搭配建议 -->
        <section class="breakfast-tips fade-in">
            <h2>完美<span style="color: var(--primary-color);">早餐搭配</span>建议</h2>
            <div class="tips-grid">
                <div class="tip-item">
                    <div class="tip-icon">
                        <i class="fas fa-coffee"></i>
                    </div>
                    <h3>搭配饮品</h3>
                    <p>豪士面包搭配牛奶、豆浆或咖啡，既能补充蛋白质，又能带来更丰富的口感体验。</p>
                </div>
                <div class="tip-item">
                    <div class="tip-icon">
                        <i class="fas fa-apple-alt"></i>
                    </div>
                    <h3>搭配水果</h3>
                    <p>早餐搭配一份新鲜水果，如香蕉、苹果或橙子，营养更均衡，维生素更全面。</p>
                </div>
                <div class="tip-item">
                    <div class="tip-icon">
                        <i class="fas fa-egg"></i>
                    </div>
                    <h3>搭配蛋白质</h3>
                    <p>搭配水煮蛋、酸奶或少量坚果，增加优质蛋白质摄入，保持上午精力充沛。</p>
                </div>
                <div class="tip-item">
                    <div class="tip-icon">
                        <i class="fas fa-clock"></i>
                    </div>
                    <h3>最佳时间</h3>
                    <p>早餐最佳时间为早上7-9点，此时新陈代谢最旺盛，营养吸收效果最佳。</p>
                </div>
            </div>
        </section>
    </main>
    
    <!-- 页脚 -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-section">
                    <h3>豪士面包</h3>
                    <p>我们致力于为消费者提供新鲜、健康、美味的面包产品，让每一顿早餐都成为一天美好的开始。</p>
                    <div class="social-links">
                        <a href="file:///D:/Desktop/Untitled-1.html#"><i class="fab fa-weixin"></i></a>
                        <a href="file:///D:/Desktop/Untitled-1.html#"><i class="fab fa-weibo"></i></a>
                        <a href="file:///D:/Desktop/Untitled-1.html#"><i class="fab fa-tiktok"></i></a>
                        <a href="file:///D:/Desktop/Untitled-1.html#"><i class="fab fa-instagram"></i></a>
                    </div>
                </div>
                
                <div class="footer-section">
                    <h3>快速链接</h3>
                    <ul class="footer-links">
                        <li><a href="file:///D:/Desktop/Untitled-1.html#">产品系列</a></li>
                        <li><a href="file:///D:/Desktop/Untitled-1.html#">早餐搭配</a></li>
                        <li><a href="file:///D:/Desktop/Untitled-1.html#">品牌故事</a></li>
                        <li><a href="file:///D:/Desktop/Untitled-1.html#">门店查询</a></li>
                    </ul>
                </div>
                
                <div class="footer-section">
                    <h3>联系我们</h3>
                    <p><i class="fas fa-map-marker-alt"></i> 地址：上海市浦东新区豪士大厦</p>
                    <p><i class="fas fa-phone"></i> 客服热线：400-888-8888</p>
                    <p><i class="fas fa-envelope"></i> 邮箱：service@haoshi.com</p>
                </div>
            </div>
            
            <div class="copyright">
                <p>© 2023 豪士面包 版权所有 | 设计用于公众号展示</p>
            </div>
        </div>
    </footer>
    
    <script>
        // 移动端菜单切换
        const mobileMenuBtn = document.getElementById('mobileMenuBtn');
        const navLinks = document.getElementById('navLinks');
        
        mobileMenuBtn.addEventListener('click', () => {
            navLinks.classList.toggle('active');
        });
        
        // 滚动动画效果
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };
        
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('fade-in');
                }
            });
        }, observerOptions);
        
        // 观察所有需要动画的元素
        document.querySelectorAll('.product-card, .featured, .breakfast-tips').forEach(el => {
            observer.observe(el);
        });
        
        // 购买按钮点击事件
        document.querySelectorAll('.btn').forEach(button => {
            button.addEventListener('click', function() {
                const productTitle = this.closest('.product-card').querySelector('.product-title').textContent;
                alert(`您已选择购买：${productTitle}\n我们将跳转到购买页面...`);
            });
        });
    </script>


</body></html>
