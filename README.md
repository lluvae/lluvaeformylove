
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Для айдиночки</title>
<style>
body {
background: linear-gradient(to right, #f9c2ff, #ffebcd);
font-family: 'Arial', sans-serif;
text-align: center;
color: #FF69B4;
}

h2 {
font-size: 30px;
margin-top: 40px;
animation: move 3s infinite alternate;
}

@keyframes move {
0% { transform: translateY(0); }
100% { transform: translateY(-10px); }
}

.heart {
width: 150px;
height: 150px;
margin: 20px auto;
animation: heartbeat 1s infinite;
}

@keyframes heartbeat {
0%, 100% { transform: scale(1); }
50% { transform: scale(1.1); }
}

.message {
font-family: Arial, sans-serif;
font-size: 20px;
margin: 20px 0;
opacity: 0;
animation: fadeIn 2s forwards;
animation-delay: 1s;
}

@keyframes fadeIn {
to { opacity: 1; }
}

.envelope {
width: 200px;
height: 120px;
border: 2px solid #ff69b4;
border-radius: 10px;
position: relative;
margin: 20px auto;
background-color: white;
cursor: pointer;
transition: transform 0.4s;
}

.envelope:hover {
transform: scale(1.05);
}

.envelope:before {
content: '';
position: absolute;
top: -10px;
left: 0;
width: 100%;
height: 20px;
background-color: #ff69b4;
border-radius: 10px 10px 0 0;
}

.letter {
display: none;
font-size: 22px;
margin: 20px;
opacity: 0;
transition: opacity 0.4s;
}

button {
padding: 10px 20px;
font-size: 20px;
cursor: pointer;
background-color: #FF69B4;
border: none;
border-radius: 5px;
color: white;
transition: background-color 0.3s;
}

button:hover {
background-color: #ff1493;
}

.arrow-button {
position: fixed;
bottom: 20px;
right: 20px;
background-color: pink;
color: white;
border: none;
padding: 10px 15px;
border-radius: 5px;
font-size: 16px;
cursor: pointer;
display: flex;
align-items: center;
}

.arrow {
margin-left: 5px;
display: inline-block;
width: 0;
height: 0;
border-top: 5px solid transparent;
border-bottom: 5px solid transparent;
border-left: 10px solid white;
}
</style>
</head>
<body>
<h2>В этот замечательный день ты появилась в моей жизни</h2>
<img src="heart.png" class="heart" alt="Сердце" />
<div class="message">
<p><i>Любимая, мы познакомились ровно 6 лет назад.</i></p>
<p><i>Ты — свет в моей жизни, мое солнышко.</i></p>
<p><i>Спасибо тебе за твою любовь!!</i></p>
<button onclick="alert('Люблю тебя, айдинка!!')">Напоминание</button>
</div>

<br>
<video align="center" width="350" height="350" autoplay muted loop controls>
<source src="love.mp4" type="video/mp4">
Ваш браузер не поддерживает видео тег.
</video>

<a href="time.html">
<button class="arrow-button">
Тыкай сюда
<span class="arrow"></span>
</button>
</a>
</body>
</html>
