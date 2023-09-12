<html>
<head>
    <meta charset="UTF-8">
    <title>Ma Boutique de Bijoux</title>
    <style>
        /* Styles CSS pour la mise en page, les onglets, etc. */
        /* ... */

        /* Styles pour les produits, les descriptions, etc. */
        /* ... */
    </style>
</head>
<body>
    <header>
        <h1>Ma Boutique de Bijoux</h1>
        <!-- Barre de navigation (menu) si nécessaire -->
        <!-- ... -->
    </header>

    <nav>
        <!-- Onglets pour les catégories de bijoux -->
        <button onclick="showCategory('colliers')">Colliers</button>
        <button onclick="showCategory('boucles-oreilles')">Boucles d'oreilles</button>
        <button onclick="showCategory('bagues')">Bagues</button>
        <!-- Ajoutez d'autres catégories si nécessaire -->
    </nav>

    <main>
        <!-- Contenu des onglets (affichage dynamique des produits) -->
        <div id="colliers">
            <!-- Liste de colliers à vendre -->
            <!-- ... -->
        </div>

        <div id="boucles-oreilles">
            <!-- Liste de boucles d'oreilles à vendre -->
            <!-- ... -->
        </div>

        <div id="bagues">
            <!-- Liste de bagues à vendre -->
            <!-- ... -->
        </div>
        <!-- Ajoutez d'autres sections pour d'autres catégories de bijoux -->
    </main>

    <footer>
        <!-- Pied de page avec des informations de contact, des liens sociaux, etc. -->
        <!-- ... -->
    </footer>

    <script>
        // Fonction pour afficher la catégorie sélectionnée
        function showCategory(category) {
            var categories = document.querySelectorAll('main > div');
            for (var i = 0; i < categories.length; i++) {
                categories[i].style.display = 'none';
            }
            document.getElementById(category).style.display = 'block';
        }

        // Par défaut, afficher la première catégorie (par exemple, "colliers")
        showCategory('colliers');
    </script>
</body>
</html>
