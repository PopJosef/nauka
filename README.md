
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
            position: relative; /* Pro umístění dropdown menu */
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

        /* Styly pro dropdown menu */
        .dropdown-content {
            display: none; /* Skryje nabídku ve výchozím stavu */
            position: absolute; /* Pro umístění nabídky */
            background-color: #f9f9f9;
            min-width: 160px;
            box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
            z-index: 1; /* Zajistí, že se nabídka zobrazí nad ostatním obsahem */
        }

        .dropdown-article:hover .dropdown-content {
            display: block; /* Zobrazí nabídku při najetí na článek */
        }

        .dropdown-content ul {
            list-style: none;
            padding: 0;
            margin: 0;
        }

        .dropdown-content li a {
            color: black;
            padding: 12px 16px;
            text-decoration: none;
            display: block;
        }

        .dropdown-content li a:hover {
            background-color: #ddd;
        }

        .dropdown-trigger {
            cursor: pointer; /* Změní kurzor myši na ukazatel */
        }
    </style>
</head>
<body>
    <header>
        <h1>Učení je mučení</h1>
    </header>

    <div class="main-content two-sidebars">
        <div class="left-sidebar sidebar">
            <h2>Matematika</h2>
            <ul>
                <li><a href="https://youtube.com/watch?v=fhe7WsRPDa0&feature=shared">Daniel</a></li>
                <li><a href="https://www.youtube.com/shorts/oLh0qNzXkMw">Zeman</a></li>
                <li><a href="https://www.example.com/karel">čeština</a></li>
                <li><a href="https://www.example.com/eva">fyzika</a></li>
                <li><a href="https://www.example.com/jana">přírodověda</a></li>
                <li><a href="https://www.example.com/michaela">zeměpis</a></li>
            </ul>
        </div>

        <div class="article-section with-two-sidebars">
            <h2>Tothle je pro tebe myšáku - Články</h2>
            <article class="dropdown-article">
                <h3 class="dropdown-trigger">Matematika</h3>
                <div class="dropdown-content">
                    <ul>
                        <li><a href="#">Poměr</a></li>
                        <li><a href="#">Zlomky</a></li>
                        <li><a href="#">Míry a váhy</a></li>
                    </ul>
                </div>
                <p>Poměr je způsob, jak porovnávat údaje lépe než jen "větší, menší, rovno". V životě se s poměrem setkáte při zápisu výsledků sportovních zápasů, v návodu, jak ředit barvy, v receptech...</p>
            </article>
            <article>
                <h3>Článek 2</h3>
                <p>Tady bude aktuální učivo ze sedmé třídy.</p>
            </article>
            <article>
                <h3>Článek 3</h3>
                <p>Tady budeš mít aktuální úkoly.</p>
            </article>
            <article>
                <h3>Článek 4</h3>
                <p>Přírodopis aktuální téma.</p>
            </article>
            <article>
                <h3>Článek 5</h3>
                <p>Němčina</p>
            </article>
            <article>
                <h3>Článek 6</h3>
                <p>Ještě nevím.</p>
            </article>
        </div>

        <div class="right-sidebar sidebar">
            <h2>Odkazy vpravo</h2>
            <ul>
                <li><a href="https://https://youtu.be/fhe7WsRPDa0?si=fO_KskV6OsiyuXOb">Alfa</a></li>
                <li><a href="https://www.example.com/beta">Beta</a></li>
                <li><a href="https://www.example.com/gamma">Gama</a></li>
                <li><a href="https://www.example.com/delta">Delta</a></li>
                <li><a href="https://www.example.com/epsilon">Epsilon</a></li>
                <li><a href="https://www.example.com/zeta">Zeta</a></li>
            </ul>
        </div>
    </div>

    <footer>
        <p>© 2023 Moje stránka</p>
    </footer>
</body>
</html>
