[Uploading in<!DOCTYPE html>
<html lang="zh-CN">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>设计师个人作品集</title>
    <style>
        /* 全局样式 */
        body {
            background: linear-gradient(to bottom, #121212, #000);
            color: #fff;
            font-family: -apple-system, BlinkMacSystemFont, 'SF Pro', 'Hiragino Sans GB', 'Microsoft YaHei', 'WenQuanYi Zen Hei', sans-serif;
            margin: 0;
            padding: 0;
        }

        /* 头图样式 */
        .hero {
            background-image: url('https://p9-flow-imagex-sign.byteimg.com/ocean-cloud-tos/image_generation/eccdf8c573aadd06e328d8851ab0c00f_1741676810548865596.jpeg~tplv-a9rns2rl98-image.jpeg?rk3s=25bff839&x-expires=1773212810&x-signature=2IFyOmdqAXYpcj9n%2F8KfWze%2BW6c%3D');
            background-size: cover;
            background-position: center;
            height: 400px;
            position: relative;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .hero::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.5);
        }

        .hero h1 {
            font-family: 'SF Pro', sans-serif;
            font-size: 3rem;
            z-index: 1;
        }

        /* 导航栏样式 */
        nav {
            display: flex;
            justify-content: center;
            gap: 15px;
            padding: 15px;
        }

        nav a {
            text-decoration: none;
            color: #fff;
            padding: 10px 20px;
            border: 2px solid #fff;
            border-radius: 20px;
            transition: border-color 0.3s ease;
        }

        nav a:hover {
            border-color: hsl(210, 100%, 50%);
        }

        nav a:active {
            background-color: hsl(210, 100%, 20%);
        }

        /* 作品分类展示区样式 */
        .portfolio {
            padding: 15px;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 15px;
        }

        .portfolio-card {
            background: rgba(255, 255, 255, 0.1);
            border-radius: 15px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            transition: transform 0.3s cubic-bezier(0.25, 0.46, 0.45, 0.94), box-shadow 0.3s ease;
        }

        .portfolio-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
        }

        .portfolio-card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            transition: transform 0.5s ease;
        }

        .portfolio-card:hover img {
            transform: scale(1.05);
        }

        .portfolio-card h3 {
            padding: 15px;
            margin: 0;
            font-family: 'Hiragino Sans GB', 'Microsoft YaHei', 'WenQuanYi Zen Hei', sans-serif;
        }

        /* 创作过程样式 */
        .creative-process {
            padding: 30px 15px;
            max-width: 1000px;
            margin: 0 auto;
        }

        .process-step {
            margin-bottom: 30px;
            opacity: 0;
            transform: translateY(20px);
            transition: opacity 0.6s ease, transform 0.6s ease;
        }

        .process-step.active {
            opacity: 1;
            transform: translateY(0);
        }

        .step-number {
            font-size: 24px;
            color: hsl(210, 100%, 50%);
            margin-bottom: 10px;
        }

        .step-content {
            display: flex;
            flex-direction: column;
            gap: 15px;
        }

        .step-image {
            width: 100%;
            height: 300px;
            background-size: cover;
            background-position: center;
            border-radius: 10px;
            overflow: hidden;
            position: relative;
        }

        .step-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s ease;
        }

        .step-image:hover img {
            transform: scale(1.05);
        }

        /* 动态图片轮播样式 */
        .slider {
            width: 100%;
            max-width: 1000px;
            margin: 30px auto;
            overflow: hidden;
            position: relative;
            border-radius: 15px;
        }

        .slider-container {
            display: flex;
            transition: transform 0.5s ease-in-out;
        }

        .slider-image {
            min-width: 100%;
            height: 400px;
            background-size: cover;
            background-position: center;
        }

        .slider-controls {
            position: absolute;
            bottom: 20px;
            left: 50%;
            transform: translateX(-50%);
            display: flex;
            gap: 10px;
        }

        .slider-dot {
            width: 10px;
            height: 10px;
            border-radius: 50%;
            background-color: rgba(255, 255, 255, 0.5);
            cursor: pointer;
            transition: background-color 0.3s ease;
        }

        .slider-dot.active {
            background-color: hsl(210, 100%, 50%);
        }
    </style>
</head>

<body>
    <!-- 头图 -->
    <div class="hero">
        <h1>设计师个人作品集</h1>
    </div>
    <!-- 导航栏 -->
    <nav>
        <a href="#">品牌</a>
        <a href="#">海报</a>
        <a href="#">UI</a>
    </nav>
    <!-- 作品分类展示区 -->
    <div class="portfolio">
        <div class="portfolio-card">
            <img src="https://p3-flow-imagex-sign.byteimg.com/ocean-cloud-tos/image_generation/2988c3e31fe68b55e5c789859e778505_1741676608255000828.jpeg~tplv-a9rns2rl98-image.jpeg?rk3s=25bff839&x-expires=1773212608&x-signature=BGNQKzQHjCUWuP3358I1AuG8AgM%3D" alt="作品1">
            <h3>作品1</h3>
        </div>
        <div class="portfolio-card">
            <img src="https://p3-flow-imagex-sign.byteimg.com/ocean-cloud-tos/image_generation/8c36a5a4198d08486c790c08c8a89086_1741676613387820088.jpeg~tplv-a9rns2rl98-image.jpeg?rk3s=25bff839&x-expires=1773212613&x-signature=037oR%2BjN6uK1j4e8lW0%2B4gB8y3A%3D" alt="作品2">
            <h3>作品2</h3>
        </div>
        <div class="portfolio-card">
            <img src="https://p9-flow-imagex-sign.byteimg.com/ocean-cloud-tos/image_generation/b5667ae1754a29f6e069cfd812244d33_1741676780503652328.jpeg~tplv-a9rns2rl98-image.jpeg?rk3s=25bff839&x-expires=1773212780&x-signature=fiTrHsN2qhuOaAzayGVAfUfWkhg%3D" alt="作品3">
            <h3>作品3</h3>
        </div>
        <div class="portfolio-card">
            <img src="https://p3-flow-imagex-sign.byteimg.com/ocean-cloud-tos/image_generation/43e6290f18ee5bc4903d76f9717a52b6_1741676793075906318.jpeg~tplv-a9rns2rl98-image.jpeg?rk3s=25bff839&x-expires=1773212793&x-signature=VwCh7DJ6ZqoVBY1rtsp%2FDEpxoZM%3D" alt="作品4">
            <h3>作品4</h3>
        </div>
        <div class="portfolio-card">
            <img src="https://p3-flow-imagex-sign.byteimg.com/ocean-cloud-tos/image_generation/2da7068d0eccfbd948b49573a898497a_1741676796261828122.jpeg~tplv-a9rns2rl98-image.jpeg?rk3s=25bff839&x-expires=1773212796&x-signature=uIIiTkeWo8GWGoUoK4Qy4qxBunU%3D" alt="作品5">
            <h3>作品5</h3>
        </div>
        <div class="portfolio-card">
            <img src="https://p3-flow-imagex-sign.byteimg.com/ocean-cloud-tos/image_generation/6983a7f631da8bd703f55446e97fb67b_1741676814574567326.jpeg~tplv-a9rns2rl98-image.jpeg?rk3s=25bff839&x-expires=1773212814&x-signature=NAgTrIWKVBnWYFyzSO17BZZM3%2FY%3D" alt="作品6">
            <h3>作品6</h3>
        </div>
        <div class="portfolio-card">
            <img src="https://p9-flow-imagex-sign.byteimg.com/ocean-cloud-tos/image_generation/29b4f83ce72c120a37ab9c761b0db6d2_1741676819325501108.jpeg~tplv-a9rns2rl98-image.jpeg?rk3s=25bff839&x-expires=1773212819&x-signature=EsIuTJFNCHlwr9DV80%2BwpxyuqhQ%3D" alt="作品7">
            <h3>作品7</h3>
        </div>
        <div class="portfolio-card">
            <img src="https://p3-flow-imagex-sign.byteimg.com/ocean-cloud-tos/image_generation/ef992168f008e0c1a1438e57aeeffaa3_1741676842016969033.jpeg~tplv-a9rns2rl98-image.jpeg?rk3s=25bff839&x-expires=1773212842&x-signature=Mu%2BocIGzO62zBluIFGLH1n6yRmw%3D" alt="作品8">
            <h3>作品8</h3>
        </div>
        <div class="portfolio-card">
            <img src="https://p9-flow-imagex-sign.byteimg.com/ocean-cloud-tos/image_generation/0a1d13c8aa3e40b71330cf360695d22f_1741676843812404689.jpeg~tplv-a9rns2rl98-image.jpeg?rk3s=25bff839&x-expires=1773212843&x-signature=%2BzjzO2%2FxNBSr2qX0Av2dX6nBD7E%3D" alt="作品9">
            <h3>作品9</h3>
        </div>
        <div class="portfolio-card">
            <img src="https://p3-flow-imagex-sign.byteimg.com/ocean-cloud-tos/image_generation/b1f5de2f3e308e5b9d67ddbd194f510b_1741676845622130502.jpeg~tplv-a9rns2rl98-image.jpeg?rk3s=25bff839&x-expires=1773212845&x-signature=TyicEtBcta4LyPlrM8t%2Be1bZTso%3D" alt="作品10">
            <h3>作品10</h3>
        </div>
    </div>
    
    <!-- 动态图片轮播 -->
    <div class="slider">
        <div class="slider-container" id="slider-container">
            <div class="slider-image" style="background-image: url('https://picsum.photos/1000/400?random=1')"></div>
            <div class="slider-image" style="background-image: url('https://picsum.photos/1000/400?random=2')"></div>
            <div class="slider-image" style="background-image: url('https://picsum.photos/1000/400?random=3')"></div>
        </div>
        <div class="slider-controls">
            <div class="slider-dot active" data-index="0"></div>
            <div class="slider-dot" data-index="1"></div>
            <div class="slider-dot" data-index="2"></div>
        </div>
    </div>
    
    <!-- 创作过程 -->
    <div class="creative-process">
        <h2>创作灵感与过程</h2>
        
        <div class="process-step" id="step1">
            <div class="step-number">1. 灵感来源</div>
            <div class="step-content">
                <div class="step-image">
                    <img src="https://picsum.photos/1000/300?random=4" alt="灵感来源">
                </div>
                <p>每一个设计都始于一个灵感火花。我的灵感来源广泛，包括自然、艺术、文化和日常体验。我相信设计应该是有意义的，能够引起情感共鸣的。</p>
            </div>
        </div>
        
        <div class="process-step" id="step2">
            <div class="step-number">2. 概念开发</div>
            <div class="step-content">
                <div class="step-image">
                    <img src="https://picsum.photos/1000/300?random=5" alt="概念开发">
                </div>
                <p>一旦灵感闪现，我会开始收集参考资料并进行头脑风暴。这个阶段是探索可能性和定义设计方向的关键时期。我会制作草图和思维导图来组织思路。</p>
            </div>
        </div>
        
        <div class="process-step" id="step3">
            <div class="step-number">3. 原型设计</div>
            <div class="step-content">
                <div class="step-image">
                    <img src="https://picsum.photos/1000/300?random=6" alt="原型设计">
                </div>
                <p>将概念转化为视觉形式是一个迭代的过程。我会创建多个版本的原型，尝试不同的配色方案、排版和布局。这个阶段的目标是找到最能表达设计意图的视觉语言。</p>
            </div>
        </div>
        
        <div class="process-step" id="step4">
            <div class="step-number">4. 精雕细琢</div>
            <div class="step-content">
                <div class="step-image">
                    <img src="https://picsum.photos/1000/300?random=7" alt="精雕细琢">
                </div>
                <p>细节决定成败。在这个阶段，我会专注于完善每一个元素，确保设计的一致性和精致度。我会考虑排版层次、视觉节奏和交互体验等方面的细节。</p>
            </div>
        </div>
        
        <div class="process-step" id="step5">
            <div class="step-number">5. 最终呈现</div>
            <div class="step-content">
                <div class="step-image">
                    <img src="https://picsum.photos/1000/300?random=8" alt="最终呈现">
                </div>
                <p>经过多次迭代和优化，设计终于准备好与世界见面。我会确保设计在不同平台和设备上都能完美呈现，并进行最终的质量检查，确保没有任何细节被忽视。</p>
            </div>
        </div>
    </div>

    <script>
        // 动态图片轮播逻辑
        const sliderContainer = document.getElementById('slider-container');
        const sliderDots = document.querySelectorAll('.slider-dot');
        let currentSlide = 0;
        const totalSlides = sliderDots.length;
        
        // 初始化轮播
        function initSlider() {
            updateSlider();
            // 自动轮播
            setInterval(nextSlide, 5000);
            
            // 点击导航点切换图片
            sliderDots.forEach(dot => {
                dot.addEventListener('click', () => {
                    currentSlide = parseInt(dot.dataset.index);
                    updateSlider();
                });
            });
        }
        
        function nextSlide() {
            currentSlide = (currentSlide + 1) % totalSlides;
            updateSlider();
        }
        
        function updateSlider() {
            // 移动轮播容器
            sliderContainer.style.transform = `translateX(-${currentSlide * 100}%)`;
            
            // 更新导航点状态
            sliderDots.forEach((dot, index) => {
                if (index === currentSlide) {
                    dot.classList.add('active');
                } else {
                    dot.classList.remove('active');
                }
            });
        }
        
        // 滚动动画逻辑
        function checkScroll() {
            const processSteps = document.querySelectorAll('.process-step');
            
            processSteps.forEach(step => {
                const stepPosition = step.getBoundingClientRect().top;
                const screenPosition = window.innerHeight / 1.3;
                
                if (stepPosition < screenPosition) {
                    step.classList.add('active');
                }
            });
        }
        
        // 页面加载完成后初始化
        window.addEventListener('load', () => {
            initSlider();
            checkScroll(); // 初始检查
        });
        
        // 滚动时检查
        window.addEventListener('scroll', checkScroll);
    </script>
</body>

</html>
    dex.html…]()
