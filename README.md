<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>furmenCRACK - Oyun ve Program İndir</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- Üst Menü -->
    <header>
        <h1>furmenCRACK</h1>
        <nav>
            <ul>
                <li><a href="#home">Ana Sayfa</a></li>
                <li><a href="#games">Oyunlar</a></li>
                <li><a href="#programs">Programlar</a></li>
                <li><a href="#contact">İletişim</a></li>
                <li><input type="text" id="searchInput" placeholder="Ara...">
                    <button onclick="searchSite()">Ara</button>
                </li>
            </ul>
        </nav>
    </header>

    <!-- Banner -->
    <section id="home" class="banner">
        <h2>furmenCRACK İle En İyi Oyunları İndir</h2>
        <p>Favori Oyununu Bul Ve İndir!</p>
        <button onclick="scrollToSection('games')">Oyunları İncele</button>
    </section>

    <!-- Oyunlar Bölümü -->
    <section id="games" class="content-section">
        <h3>Son Eklenen Oyunlar</h3>
        <div class="game-item">
            <h4>Oyun Adı 1</h4>
            <p>Oyun Açıklaması</p>
        </div>
        <div class="game-item">
            <h4>Oyun Adı 2</h4>
            <p>Oyun Açıklaması</p>
        </div>
    </section>

    <!-- Programlar Bölümü -->
    <section id="programs" class="content-section">
        <h3>Programlar</h3>
        <div class="program-item">
            <h4>Program Adı 1</h4>
            <p>Program Açıklaması</p>
        </div>
        <div class="program-item">
            <h4>Program Adı 2</h4>
            <p>Program Açıklaması</p>
        </div>
    </section>

    <!-- İletişim Bölümü -->
    <section id="contact" class="content-section">
        <h3>İletişim</h3>
        <p>Email: contact@furmencrack.com</p>
        <p>Telefon: +90 123 456 78 90</p>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2024 furmenCRACK. Tüm Hakları Saklıdır.</p>
    </footer>

    <!-- JavaScript -->
    <script src="script.js"></script>

    <style>
        * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
}

header {
    background-color: #222;
    color: #fff;
    padding: 15px;
    text-align: center;
}

header nav ul {
    list-style-type: none;
}

header nav ul li {
    display: inline;
    margin: 0 10px;
}

header nav ul li input {
    padding: 5px;
}

header nav ul li button {
    padding: 5px;
}

.banner {
    background-color: #333;
    color: #fff;
    padding: 50px;
    text-align: center;
}

.content-section {
    padding: 20px;
}

.game-item, .program-item {
    background-color: #f4f4f4;
    margin: 10px 0;
    padding: 15px;
}

footer {
    background-color: #222;
    color: #fff;
    text-align: center;
    padding: 10px;
    margin-top: 20px;
}
    </style>

    <script>
        // Sayfa içi bölüme kaydırma
function scrollToSection(sectionId) {
    document.getElementById(sectionId).scrollIntoView({ behavior: 'smooth' });
}

// Site içi arama
function searchSite() {
    const query = document.getElementById("searchInput").value.toLowerCase();
    const sections = document.querySelectorAll(".content-section");

    sections.forEach(section => {
        const items = section.querySelectorAll("div");
        items.forEach(item => {
            if (item.innerText.toLowerCase().includes(query)) {
                item.style.display = "block";
            } else {
                item.style.display = "none";
            }
        });
    });
}
    </script>
</body>
</html>
