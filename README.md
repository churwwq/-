# <!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Зачёт по информатике | Савик Виталий</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 0;
            padding: 20px;
            background-color: #f0f0f0;
        }
        .container {
            max-width: 800px;
            margin: 0 auto;
            background-color: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        h1, h2, h3 {
            color: #333;
        }
        img {
            border-radius: 8px;
            margin: 10px 0;
            max-width: 100%;
            height: auto;
        }
        button {
            padding: 10px 20px;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
            margin: 10px;
        }
        button:hover {
            background-color: #45a049;
        }
        a {
            color: #1a73e8;
            text-decoration: none;
        }
        a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Первая страница -->
        <section id="page1">
            <h1>Вас приветствует Савик Виталий</h1>
            <p>Этот сайт является его зачётом по информатике</p>
            <button onclick="nextPage()">Далее</button>
        </section>

        <!-- Вторая страница (скрыта изначально) -->
        <section id="page2" style="display: none;">
            <h2>Молодечно и Музыкальный колледж</h2>
            
            <h3>Молодечно</h3>
            <p>
                <a href="https://ru.wikipedia.org/wiki/Молодечно" target="_blank">Молодечно</a> — город в Беларуси, известный своей историей и культурой.
            </p>
            <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/5d/Maladziečna_-_Плошча_Перамогі.jpg/800px-Maladziečna_-_Плошча_Перамогі.jpg" alt="Фото Молодечно">

            <h3>Музыкальный колледж</h3>
            <p>
                <a href="https://ru.wikipedia.org/wiki/Молодечненский_государственный_музыкальный_колледж_имени_М._К._Огинского" target="_blank">Молодечненский музыкальный колледж</a> — одно из известных учебных заведений города.
            </p>
            <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/9a/Могинского_колледж_в_Молодечно.jpg/800px-Могинского_колледж_в_Молодечно.jpg" alt="Фото Музыкального колледжа">

            <button onclick="prevPage()">Назад</button>
        </section>
    </div>

    <script>
        function nextPage() {
            document.getElementById("page1").style.display = "none";
            document.getElementById("page2").style.display = "block";
        }

        function prevPage() {
            document.getElementById("page2").style.display = "none";
            document.getElementById("page1").style.display = "block";
        }
    </script>
</body>
</html>
