# Midterm Elections 2026 : l'atlas des élections américaines du 3 novembre 2026

Application web autonome, en français, qui raconte et analyse les élections de mi-mandat américaines du mardi 3 novembre 2026 : Sénat, Chambre des représentants, gouverneurs, référendums, sortie des urnes, premières historiques et 80 ans d'histoire des midterms.

**Ouvrir l'application : https://abdoulhamiddiallo.github.io/midterm-elections-2026/**

Un seul fichier `index.html`, sans dépendance réseau : il s'ouvre sur téléphone, tablette et ordinateur, en mode jour ou en mode nuit.

## 🖥️ Aperçu

| Ordinateur | Téléphone |
|---|---|
| ![Vue d'ensemble](docs/capture-app.png) | ![Format téléphone](docs/capture-mobile.png) |

## 🏆 Résultats clés

- **Sénat** : 54 démocrates, 44 républicains, 2 sièges en attente (Alaska, Mississippi). Sept bascules démocrates : Caroline du Nord, Caroline du Sud, Texas, Ohio, Kansas, Iowa, Maine.
- **Chambre** : 240 sièges démocrates attribués contre 135 au 4 novembre ; estimation finale d'au moins 258 sièges, la plus large majorité depuis 1992.
- **Gouverneurs** : 28 démocrates, 20 républicains, 2 en attente. Cinq bascules : Géorgie, Iowa, Nevada, Ohio, Texas.
- **Référendums** : 145 mesures dans 39 États ; le droit à l'avortement l'emporte dans 3 États sur 4, la carte d'électeur est inscrite dans 3 constitutions.
- **Participation** : 61 millions de votes anticipés, un record pour un midterm.

## 📊 Ce que l'application permet

- **Carte géographique des 50 États** (projection Albers) : Sénat, gouverneurs, bascules par rapport à la présidentielle 2024, marge de victoire ; survol, clic, plein écran.
- **Revivre la soirée** : la carte se colore État par État dans l'ordre réel des annonces, avec l'horloge de Washington et le compteur de sièges.
- **Hémicycles siège par siège** : 100 sénateurs, 435 représentants, 50 gouverneurs.
- **Fiches de course** : candidats, photos, parcours, scores, écart, taux de dépouillement, glissement par rapport à 2024 ; filtres et recherche.
- **Tiroir par État** : présidentielle 2024, Sénat et gouvernorat réunis en un écran.
- **Duels tête d'affiche** : 14 face-à-face qui ont fait la nuit.
- **Sortie des urnes** : motivations de vote, approbation du président, coût de la vie, vote anticipé.
- **Premières historiques** et **index des 150 personnes** de A à Z.
- **Histoire** : sièges gagnés ou perdus par le parti du président à chaque midterm depuis 1946.
- **Labo** : simulateur de majorité au Sénat, comparateur de deux États, quiz de 10 questions.
- **Navigation** : trois familles (Résultats, Analyse, Outils), sommaire visuel, recherche globale, fil d'Ariane, pagination, sommaire latéral, raccourcis clavier, partage, impression.

## 🧭 Organisation

| Famille | Sections |
|---|---|
| Résultats | Accueil, Carte, Sénat, Chambre, Gouverneurs, Référendums, États et villes |
| Analyse | Duels, Sortie des urnes, Premières, Personnes, Histoire |
| Outils | Labo (simulateur, comparateur, quiz) |

## 🧱 Architecture

- Page HTML unique : HTML, CSS et JavaScript dans un seul fichier.
- Données intégrées sous forme de tableaux JavaScript (35 courses au Sénat, 36 gouvernorats, 20 référendums, 150 personnes, présidentielle 2024 par État, historique 1946-2026).
- Fond de carte vectoriel des 50 États embarqué (U.S. Census Bureau, projection Albers USA, simplifié).
- Graphiques dessinés avec Chart.js, inclus dans le fichier.
- Photos, sceaux, icônes et logo embarqués en base64 : aucun chargement externe hormis les polices.
- Thème jour / nuit mémorisé sur l'appareil.

## 🧰 Technologies

HTML5, CSS3, JavaScript, SVG, Chart.js 4, projection cartographique Albers USA (d3-geo, TopoJSON).

## 📚 Sources

- Résultats : Associated Press, Fox News, NBC News Decision Desk, CNN, CBS News, CNBC, MS NOW, Poliwave.
- Sortie des urnes : NBC News Exit Poll, AP Voter Poll, CBS News Exit Poll, Rutgers University.
- Référendums : NBC News, Ballotpedia, CalMatters, KTAR, Idaho Capital Sun.
- Premières historiques : Axios, Newsweek, Fast Company.
- Vote anticipé : University of Florida Election Lab.
- Historique 1946-2022 : Clerk of the House, Senate Historical Office.
- Fond de carte : U.S. Census Bureau. Sceaux du Sénat et de la Chambre : domaine public.

Les résultats marqués « en attente » peuvent évoluer avec le dépouillement, les recomptages et les seconds tours.

## ✍️ Auteur

Abdoul Hamid Diallo, Data Engineer (Microsoft Fabric, Azure, Power BI, SQL Server, AI et Microsoft Foundry).
LinkedIn : https://www.linkedin.com/in/abdoul-hamid-diallo-fabric-data-engineer/
Toutes mes applications : https://abdoulhamiddiallo.github.io/
