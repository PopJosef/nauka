<!DOCTYPE html>
<html lang="cs">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Učení je mučení</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            min-height: 100vh;
            flex-direction: column;
        }

        header {
            background-color: #f0f0f0;
            padding: 1em;
            text-align: center;
        }

        .main-content {
            flex-grow: 1;
            display: flex;
            padding: 20px;
        }

        .article-section {
            flex-grow: 1;
            padding-right: 20px;
            overflow-y: auto; /* Zajistí srolování hlavní části */
        }

        .sidebar {
            width: 200px;
            padding: 20px;
            background-color: #e0e0e0;
        }

        .sidebar ul {
            list-style: none;
            padding: 0;
        }

        .sidebar li {
            margin-bottom: 10px;
        }

        .sidebar li a {
            text-decoration: none; /* Odstraní podtržení odkazů */
            color: #333; /* Nastaví barvu textu odkazu */
        }

        .sidebar li a:hover {
            color: blue; /* Změní barvu při najetí myší */
        }

        /* Pro dva boční panely */
        .left-sidebar {
            margin-right: 20px;
        }

        /* Pro rozložení se dvěma bočními panely */
        .main-content.two-sidebars {
            padding-left: 0;
            padding-right: 0;
        }

        .article-section.with-two-sidebars {
            padding-left: 20px;
            padding-right: 20px;
        }
    </style>
</head>
<body>
    <header>
        <h1>Učení je mučení</h1>
    </header>

    <div class="main-content two-sidebars">
        <div class="left-sidebar sidebar">
            <h2>Odkazy vlevo</h2>
            <ul>
                <li><a href="https://www.example.com/jarda">Jarda</a></li>
                <li><a href="https://www.example.com/petr">Petr</a></li>
                <li><a href="https://www.example.com/karel">Karel</a></li>
                <li><a href="https://www.example.com/eva">Eva</a></li>
                <li><a href="https://www.example.com/jana">Jana</a></li>
                <li><a href="https://www.example.com/michaela">Michaela</a></li>
            </ul>
        </div>

        <div class="article-section with-two-sidebars">
            <h2>Hlavní obsah - Články</h2>
            <article>
                <h3>Článek 1</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
            </article>
            <article>
                <h3>Článek 2</h3>
                <p>Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
            </article>
            <article>
                <h3>Článek 3</h3>
                <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.</p>
            </article>
            <article>
                <h3>Článek 4</h3>
                <p>Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione voluptatem sequi nesciunt.</p>
            </article>
            <article>
                <h3>Článek 5</h3>
                <p>Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia non numquam eius modi tempora incidunt ut labore et dolore magnam aliquam quaerat voluptatem.</p>
            </article>
            <article>
                <h3>Článek 6</h3>
                <p>Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat.</p>
            </article>
        </div>

        <div class="right-sidebar sidebar">
            <h2>Odkazy vpravo</h2>
            <ul>
                <li><a href="https://www.example.com/alpha">Alfa</a></li>
                <li><a href="https://www.example.com/beta">Beta</a></li>
                <li><a href="https://www.example.com/gamma">Gama</a></li>
                <li><a href="https://www.example.com/delta">Delta</a></li>
                <li><a href="https://www.example.com/epsilon">Epsilon</a></li>
                <li><a href="https://www.example.com/zeta">Zeta</a></li>
            </ul>
        </div>
    </div>

    <footer>
        <p>&copy; 2023 Moje stránka</p>
    </footer>
</body>
</html>
