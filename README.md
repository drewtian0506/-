<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>專業視覺作品集 | Portfolio</title>
    <style>
        /* 全域樣式設定 */
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: "Helvetica Neue", Arial, "Noto Sans TC", sans-serif;
        }

        body {
            background-color: #121212;
            color: #f5f5f5;
            line-height: 1.6;
        }

        /* 導覽列 */
        header {
            position: fixed;
            top: 0;
            width: 100%;
            background-color: rgba(18, 18, 18, 0.95);
            padding: 20px 40px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            z-index: 1000;
            border-bottom: 1px solid #2a2a2a;
        }

        .logo {
            font-size: 20px;
            font-weight: bold;
            letter-spacing: 2px;
            color: #fff;
        }

        nav a {
            color: #a0a0a0;
            text-decoration: none;
            margin-left: 30px;
            font-size: 14px;
            transition: color 0.3s;
        }

        nav a:hover {
            color: #fff;
        }

        /* 主視覺區 */
        .hero {
            height: 60vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 0 20px;
            margin-top: 80px;
            background: linear-gradient(rgba(18,18,18,0.6), #121212);
        }

        .hero h1 {
            font-size: 42px;
            font-weight: 300;
            letter-spacing: 4px;
            margin-bottom: 15px;
            color: #fff;
        }

        .hero p {
            color: #888;
            font-size: 16px;
            max-width: 600px;
        }

        /* 作品網格區 */
        .portfolio-container {
            padding: 40px;
            max-width: 1200px;
            margin: 0 auto;
        }

        .section-title {
            font-size: 22px;
            font-weight: 400;
            margin-bottom: 30px;
            letter-spacing: 2px;
            position: relative;
            padding-left: 10px;
            border-left: 3px solid #fff;
        }

        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-bottom: 60px;
        }

        .card {
            background-color: #1e1e1e;
            border-radius: 4px;
            overflow: hidden;
            transition: transform 0.3s, box-shadow 0.3s;
            border: 1px solid #2a2a2a;
        }

        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.5);
        }

        .card-image {
            height: 240px;
            background-color: #2a2a2a;
            display: flex;
            justify-content: center;
            align-items: center;
            color: #555;
            font-size: 14px;
            position: relative;
        }

        /* 模擬圖片的漸層佔位符 */
        .img-placeholder-1 { background: linear-gradient(45deg, #2c3e50, #3498db); }
        .img-placeholder-2 { background: linear-gradient(45deg, #111, #555); }
        .img-placeholder-3 { background: linear-gradient(45deg, #a8ff78, #78ffd6); }

        .card-info {
            padding: 20px;
        }

        .card-info h3 {
            font-size: 18px;
            margin-bottom: 8px;
            font-weight: 500;
            color: #fff;
        }

        .card-info p {
            color: #888;
            font-size: 14px;
        }

        /* 頁尾 */
        footer {
            text-align: center;
            padding: 40px 20px;
            color: #555;
            font-size: 12px;
            border-top: 1px solid #2a2a2a;
            background-color: #0a0a0a;
        }

        /* 響應式調整 */
        @media (max-width: 768px) {
            header { padding: 20px; }
            nav a { margin-left: 15px; }
            .hero h1 { font-size: 32px; }
            .portfolio-container { padding: 20px; }
        }
    </style>
</head>
<body>

    <header>
        <div class="logo">VISUAL STUDIO</div>
        <nav>
            <a href="#works">作品展示</a>
            <a href="#about">關於我們</a>
        </nav>
    </header>

    <section class="hero">
        <h1>捕捉光影與結構的瞬間</h1>
        <p>專注於高畫質視覺呈現、空間光影紀錄與專業影像修正。透過鏡頭與精準的後製工藝，為客戶留住最具張力的畫面。</p>
    </section>

    <main class="portfolio-container" id="works">
        <h2 class="section-title">精選專案</h2>
        
        <div class="grid">
            <div class="card">
                <div class="card-image img-placeholder-1">
                    <span>[ 現場光影紀實影像 ]</span>
                </div>
                <div class="card-info">
                    <h3>都會光影專案</h3>
                    <p>利用黃昏自然光與高動態範圍後製，展現建築物與環境的強烈對比。</p>
                </div>
            </div>

            <div class="card">
                <div class="card-image img-placeholder-2">
                    <span>[ 人像與細節修正 ]</span>
                </div>
                <div class="card-info">
                    <h3>細緻質感肖像</h3>
                    <p>針對商業客戶進行的高精細度皮膚調和與色彩優化作品。</p>
                </div>
            </div>

            <div class="card">
                <div class="card-image img-placeholder-3">
                    <span>[ 環境與結構安全紀錄 ]</span>
                </div>
                <div class="card-info">
                    <h3>工業與空間紀錄</h3>
                    <p>精準紀錄線條、結構與明暗分佈，適用於工程與空間設計發表。</p>
                </div>
            </div>
        </div>
    </main>

    <footer>
        <p>&copy; 2026 Visual Studio. All Rights Reserved. 網頁已成功部署上線。</p>
    </footer>

</body>
</html>
