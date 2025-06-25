# -<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Зачёт по информатике | Савик Виталий</title>
    <link rel="stylesheet" href="style.css">
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
            <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/5d/Maladziečna_-_Плошча_Перамогі.jpg/800px-Maladziečna_-_Плошча_Перамогі.jpg" alt="Молодечно" width="500">

            <h3>Музыкальный колледж</h3>
            <p>
                <a href="https://ru.wikipedia.org/wiki/Молодечненский_государственный_музыкальный_колледж_имени_М._К._Огинского" target="_blank">Молодечненский музыкальный колледж</a> — одно из известных учебных заведений города.
            </p>
            <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/9a/Могинского_колледж_в_Молодечно.jpg/800px-Могинского_колледж_в_Молодечно.jpg" alt="Музыкальный колледж" width="500">

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
