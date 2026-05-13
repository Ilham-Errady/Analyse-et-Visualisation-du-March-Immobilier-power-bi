# Analyse-et-Visualisation-du-March-Immobilier-power-bi



Ce projet a pour objectif de concevoir une solution complète de Business Intelligence permettant d’analyser le marché immobilier marocain à partir des données collectées depuis la plateforme Avito.ma.

Dans une première étape, un pipeline ETL a été développé afin de scraper, nettoyer, transformer et charger les données immobilières dans un Data Warehouse PostgreSQL. Ce pipeline a été réalisé avec Python, PostgreSQL, Docker et Docker Compose.

Après la construction du Data Warehouse, les données ont été organisées en deux schémas distincts :

bi_schema : destiné à l’analyse décisionnelle avec Power BI
ml_schema : réservé aux futurs modèles de Machine Learning

Dans ce projet, seule la couche bi_schema a été utilisée afin de développer une solution analytique performante avec Power BI.

🔍 Exploitation des Données avec Power BI

Power BI a été connecté directement au Data Warehouse PostgreSQL afin d’importer uniquement les tables du schéma bi_schema.

Le modèle relationnel a ensuite été vérifié afin d’assurer la cohérence entre :

les tables de dimensions
la table de faits
les relations analytiques

Cette étape permet de garantir un modèle BI optimisé et performant pour les analyses interactives.

🧹 Préparation des Données avec Power Query

Avant la création des dashboards, plusieurs opérations de transformation et de nettoyage ont été réalisées avec Power Query :

correction des incohérences mineures
gestion des valeurs nulles
vérification des types de données
suppression des valeurs aberrantes
optimisation des tables pour améliorer les performances
création de colonnes calculées comme le prix par m²

Cette phase permet d’obtenir des données fiables et prêtes pour l’analyse décisionnelle.

📐 Création des KPIs et Mesures avec DAX

Plusieurs mesures et indicateurs métiers ont été développés avec DAX afin de permettre une analyse dynamique du marché immobilier marocain.

Les principaux KPIs réalisés sont :

nombre total d’annonces
prix moyen des biens immobiliers
prix moyen par ville
prix moyen par m²
évolution des annonces dans le temps
taux de croissance des annonces
répartition des types de biens immobiliers
indicateurs de tendance du marché

Ces mesures permettent de produire des analyses interactives et des visualisations avancées dans Power BI.

📊 Dashboards Réalisés

Le projet comprend plusieurs dashboards interactifs permettant d’explorer le marché immobilier sous différents angles.

📈 Dashboard 1 — Vue Globale du Marché

Ce dashboard fournit une vue d’ensemble du marché immobilier marocain avec :

le nombre total d’annonces
le prix moyen du marché
l’évolution des annonces dans le temps
la répartition des annonces par ville
les principaux KPIs
💰 Dashboard 2 — Analyse des Prix

Ce dashboard permet d’étudier les variations des prix immobiliers :

distribution des prix
prix moyen par m²
comparaison des segments immobiliers
comparaison des prix selon les villes
🗺️ Dashboard 3 — Analyse Géographique

Ce dashboard met en avant la dimension géographique du marché :

répartition des annonces par ville
visualisation cartographique des prix
classement des villes les plus chères
analyse régionale du marché immobilier
📉 Dashboard 4 — Analyse des Tendances

Ce dashboard permet de suivre l’évolution du marché immobilier dans le temps :

évolution des prix
évolution du volume des annonces
tendances du marché
analyse saisonnière
🎛️ Filtres Interactifs

Afin de rendre les dashboards dynamiques et interactifs, plusieurs filtres ont été intégrés :

ville
type de bien
surface
période
plage de prix

Tous les graphiques et indicateurs se mettent automatiquement à jour selon les filtres sélectionnés.

🛠️ Technologies Utilisées

Le projet a été réalisé avec plusieurs technologies et outils :

Power BI
Power Query
DAX
PostgreSQL
Python
Docker
Docker Compose
🔗 Projet Scraping & Pipeline ETL

Le projet repose également sur un pipeline ETL développé séparément pour :

scraper les données immobilières depuis Avito.ma
nettoyer et transformer les données
charger les données dans PostgreSQL
construire le Data Warehouse

GitHub du projet Scraping & ETL :

👉 Ajouter ici le lien GitHub de votre repository

🎯 Résultats du Projet

Cette solution permet :

d’analyser efficacement le marché immobilier marocain
d’identifier les tendances des prix
de comparer les villes et segments immobiliers
d’aider à la prise de décision grâce à des dashboards interactifs
de transformer des données brutes en informations exploitables et visuelles
