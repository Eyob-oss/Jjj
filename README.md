<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>EOTC Hymns</title>
    <link rel="stylesheet" href="css.css">
    <script src="js.js" defer></script>
</head>
<body>
    <header>
        <button class="icon-btn" onclick="openInfo()">ℹ️</button>
        <h1>EOTC HYMNS</h1>
        <button class="icon-btn" onclick="toggleSearch()">🔍</button>
    </header>

    <div id="search-bar">
        <input type="text" id="search" placeholder="Search hymns..." onkeyup="searchHymns()">
    </div>

    <main id="home">
        <div class="logo">
            <img src="mine.png" alt="EOTC Logo">
        </div>
        <div class="categories">
            <button onclick="openCategory('English Hymns')">English Hymns</button>
            <button onclick="openCategory('Faaruwwan Afaan Oromoo')">Faaruwwan Afaan Oromoo</button>
            <button onclick="openCategory('የማህበረ ሰብ መዝሙራት')">የማህበረ ሰብ መዝሙራት</button>
            <button onclick="openCategory('Spiritual Resources')">Spiritual Resources</button>
            <button onclick="openCategory('What is Hymn?')">What is Hymn?</button>
        </div>
    </main>

    <main id="hymn-list" class="hidden">
        <button class="back-btn" onclick="goHome()">⬅ Back</button>
        <h2 id="category-title">Category</h2>
        <ul id="hymns">
            <!-- Hymns will be loaded here -->
        </ul>
    </main>
</body>
</html>
