<html>
<head>
    <meta charset="UTF-8">
    <title>Bijoux en ligne</title>
    <style>
        /* Style des onglets */
        .tab {
            display: none;
        }

        /* Style du bouton des onglets */
        .tab-button {
            background-color: #4CAF50;
            color: white;
            padding: 10px 20px;
            border: none;
            cursor: pointer;
        }

        /* Style actif du bouton des onglets */
        .active {
            background-color: #45a049;
        }
    </style>
</head>
<body>
    <h1>Bijoux en ligne</h1>

    <!-- Boutons des onglets -->
    <button class="tab-button" onclick="openTab('colliers')">Colliers</button>
    <button class="tab-button" onclick="openTab('boucles-oreilles')">Boucles d'oreilles</button>
    <button class="tab-button" onclick="openTab('bagues')">Bagues</button>

    <!-- Contenu des onglets -->
    <div id="colliers" class="tab">
        <h2>Colliers</h2>
        <p>Découvrez notre collection de magnifiques colliers.</p>
        <!-- Ajoutez ici des images et des descriptions de vos colliers -->
    </div>

    <div id="boucles-oreilles" class="tab">
        <h2>Boucles d'oreilles</h2>
        <p>Explorez notre gamme de boucles d'oreilles élégantes.</p>
        <!-- Ajoutez ici des images et des descriptions de vos boucles d'oreilles -->
    </div>

    <div id="bagues" class="tab">
        <h2>Bagues</h2>
        <p>Des bagues exceptionnelles pour chaque occasion.</p>
        <!-- Ajoutez ici des images et des descriptions de vos bagues -->
    </div>

    <script>
        // Fonction pour afficher l'onglet sélectionné
        function openTab(tabName) {
            var i, tabContent, tabButtons;
            tabContent = document.getElementsByClassName("tab");
            for (i = 0; i < tabContent.length; i++) {
                tabContent[i].style.display = "none";
            }
            tabButtons = document.getElementsByClassName("tab-button");
            for (i = 0; i < tabButtons.length; i++) {
                tabButtons[i].classList.remove("active");
            }
            document.getElementById(tabName).style.display = "block";
            event.currentTarget.classList.add("active");
        }
        
        // Par défaut, afficher le premier onglet
        openTab('colliers');
    </script>
</body>
</html>
