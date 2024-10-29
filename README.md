<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>研究テーマ「Raspberry Pi スマート時計制作」</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background-color: #ffffff;
            color: #333;
            margin: 0;
            padding: 10px; /* パディングを減らす */
        }
        .container {
            max-width: 100%; /* 最大幅を60%に設定 */
            margin: auto;
            background-color: #f7f7f7; /* 背景をやや濃いグレーに */
            border-radius: 10px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            padding: 5px; /* パディングを減らす */
        }
        h1 {
            text-align: center;
            color: #333;
            padding: 10px; /* パディングを減らす */
            margin: 0;
            border-bottom: 2px solid #bbb; /* ボーダーの色を濃く */
        }
        .task-info {
            padding: 10px; /* パディングを減らす */
            background-color: #e0e0e0; /* タスク情報の背景を濃いグレーに */
            border-bottom: 1px solid #bbb; /* ボーダーの色を濃く */
        }
        .section-header {
            background-color: #ddd; /* ヘッダーの背景を濃いグレーに */
            color: #333;
            padding: 10px; /* パディングを減らす */
            cursor: pointer;
            margin: 0;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: relative;
            transition: background-color 0.3s;
        }
        .section-header:hover {
            background-color: #ccc; /* ホバー時にさらに濃いグレーに */
        }
        .section-header .icon {
            font-size: 1.5em;
            transition: transform 0.3s;
        }
        .content {
            display: none;
            background-color: #fff;
            padding: 10px; /* パディングを減らす */
        }
        ul {
            list-style-type: disc;
            margin-left: 20px;
            padding-left: 10px;
        }

        /* モバイル用のスタイル */
        @media (max-width: 600px) {
            h1 {
                font-size: 1.5em; /* タイトルのサイズを小さく */
            }
            .section-header {
                font-size: 1.2em; /* セクションヘッダーのサイズを調整 */
            }
        }
    </style>
    <script>
        function toggleContent(header) {
            const content = header.nextElementSibling;
            const icon = header.querySelector('.icon');
            const isActive = header.classList.toggle('active');
            content.style.display = isActive ? 'block' : 'none';
            icon.textContent = isActive ? '−' : '+'; // +から−に変化
            icon.style.transform = isActive ? 'rotate(180deg)' : 'rotate(0deg)'; // アニメーション
        }
    </script>
</head>
<body>

    <div class="container">
        <h1>研究テーマ<br>「Raspberry Pi スマート時計制作」</h1>

        <div class="task-info">
            <strong>やることリスト：</strong><br>
            パワーポイントの作成：川崎・高橋<br>
            レジュメ作成：𠮷原<br>
            原稿の作成：加藤
        </div>

        <div class="section-header" onclick="toggleContent(this)">
            Raspberry Piとは
            <span class="icon">+</span>
        </div>
        <div class="content">
            <p>Raspberry Piの基本説明など</p>
        </div>

        <div class="section-header" onclick="toggleContent(this)">
            スマート時計とは
            <span class="icon">+</span>
        </div>
        <div class="content">
            <p>スマート時計の基本説明など</p>
        </div>

        <div class="section-header" onclick="toggleContent(this)">
            目的・目標・概要
            <span class="icon">+</span>
        </div>
        <div class="content">
            <ul>
                <li>どのような目的でこのテーマについて研究するのか</li>
                <li>今回の作品について</li>
                <li>どのようにして制作を進めたか</li>
                <li>なぜRaspberry Piを使用するか</li>
            </ul>
        </div>

        <div class="section-header" onclick="toggleContent(this)">
            使用器具
            <span class="icon">+</span>
        </div>
        <div class="content">
            <p>写真があれば貼る（すべて使用用途を調べる）</p>
            <ul>
                <li>Raspberry Pi4</li>
                <li>MicroSD card</li>
                <li>Display</li>
                <li>スピーカー</li>
                <li>マイク</li>
                <li>温度・湿度センサー</li>
                <li>ブレッドボード</li>
                <li>GPIOケーブル</li>
            </ul>
        </div>

        <div class="section-header" onclick="toggleContent(this)">
            制作の課程
            <span class="icon">+</span>
        </div>
        <div class="content">
            <ul>
                <li>準備したファイル</li>
                <li>Raspberry Pi 64bit OS</li>
                <li>参考にしたサイト</li>
                <li>聞きにきて</li>
                <li>デザイン</li>
                <li>追加要素</li>
            </ul>
        </div>

        <div class="section-header" onclick="toggleContent(this)">
            研究結果
            <span class="icon">+</span>
        </div>
        <div class="content">
            <ul>
                <li>どのような物ができたか</li>
                <ul>
                    <li>成果</li>
                    <li>反省点</li>
                </ul>
            </ul>
        </div>

        <div class="section-header" onclick="toggleContent(this)">
            感想
            <span class="icon">+</span>
        </div>
        <div class="content">
            <p>プロジェクトに関する感想</p>
        </div>
    </div>

</body>
</html>
