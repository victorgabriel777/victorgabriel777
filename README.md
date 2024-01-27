<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #121212; /* Cor de fundo escuro */
            color: #fff; /* Cor do texto */
            transition: background-color 0.3s ease, color 0.3s ease;
            text-align: center;
        }

        .dark-mode body {
            background-color: #fff; /* Cor de fundo claro no modo escuro */
            color: #333; /* Cor do texto no modo escuro */
        }

        header {
            background-color: #333;
            color: #fff;
            padding: 10px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.5em;
            font-weight: bold;
        }

        nav ul {
            list-style: none;
            display: flex;
        }

        nav ul li {
            margin-right: 20px;
        }

        nav a {
            text-decoration: none;
            color: #fff;
            font-weight: bold;
            transition: color 0.3s ease;
        }

        nav a:hover {
            color: #ffd700;
        }

        .carousel,
        .latest-news {
            margin: 20px;
            background-color: #333; /* Cor de fundo escuro para as seções */
            padding: 15px;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            transition: background-color 0.3s ease;
        }

        .dark-mode .carousel,
        .dark-mode .latest-news {
            background-color: #fff; /* Cor de fundo claro para as seções no modo escuro */
            color: #333; /* Cor do texto para as seções no modo escuro */
        }

        footer {
            background-color: #333;
            color: #fff;
            padding: 10px;
            text-align: center;
            position: fixed;
            bottom: 0;
            width: 100%;
        }

        .dark-mode-btn {
            cursor: pointer;
            background-color: #333;
            color: #fff;
            padding: 8px;
            border: none;
            border-radius: 4px;
            font-weight: bold;
            transition: background-color 0.3s ease, color 0.3s ease;
        }

        .dark-mode-btn:hover {
            background-color: #555;
        }
    </style>
    <title>PixelInsider</title>
</head>
<body>

    <header>
        <div class="logo">PixelInsider</div>
        <nav>
            <ul>
                <li><a href="#">Início</a></li>
                <li><a href="#">Notícias</a></li>
                <li><a href="https://twitter.com/seuusuario" target="_blank">Contato</a></li>
            </ul>
        </nav>
        <button class="dark-mode-btn" onclick="toggleDarkMode()">Modo Escuro</button>
    </header>
