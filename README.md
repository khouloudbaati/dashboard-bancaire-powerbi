# Tableau de Bord — Pilotage Bancaire (Power BI)

Un tableau de bord interactif de pilotage pour une banque tunisienne, construit avec Power BI. Projet de démonstration réalisé pour illustrer des compétences en modélisation de données, DAX et data visualization appliquées au secteur bancaire.

⚠️ **Toutes les données utilisées sont 100% synthétiques** (générées aléatoirement), calibrées sur des ordres de grandeur réalistes du secteur bancaire tunisien (BCT, INS). Aucune donnée réelle ou confidentielle n'est utilisée.

---

## 📊 Aperçu

Le tableau de bord comprend 4 pages :

| Page | Contenu |
|---|---|
| **Vue d'ensemble** | KPIs généraux (clients actifs, encours crédits, dépôts, adoption digitale), évolution mensuelle des transactions, répartition géographique par gouvernorat |
| **Clientèle** | Répartition par âge, statut (actif/perdu), segment, profession ; taux de churn, solde moyen client |
| **Crédits et risque** | Taux d'impayés (NPL), taux de risque, répartition des crédits par type, top gouvernorats à risque, évolution de l'encours |
| **Canaux digitaux** | Taux d'adoption digitale, répartition des transactions par canal (Mobile, E-banking, Agence, Carte/DAB), évolution dans le temps |

## 🗂️ Modèle de données

Le modèle suit un schéma en étoile autour de la table **Clients** :

- **Clients** (5 000 lignes) — profil démographique, segment, statut
- **Comptes** (~7 400 lignes) — comptes courants et épargne
- **Credits** (~1 500 lignes) — crédits immobilier, consommation, auto, PME
- **Transactions** (60 000 lignes) — transactions 2025-2026 par canal
- **Gouvernorats** (24 lignes) — dimension géographique
- **Calendrier** — table de dates pour l'analyse temporelle

## 🧮 Mesures DAX

Le projet comprend une vingtaine de mesures DAX, notamment :
- KPIs de base (clients actifs, encours, dépôts)
- Taux d'impayés et de risque crédit
- Taux de churn
- Taux d'adoption digitale
- Mesures d'évolution temporelle (comparaisons année sur année via `USERELATIONSHIP`)

## 🛠️ Compétences démontrées

- Modélisation de données en étoile
- Écriture de mesures DAX (y compris relations inactives et `USERELATIONSHIP`)
- Data visualization et storytelling avec les données
- Design d'interface (charte graphique cohérente, navigation entre pages)

## 📁 Contenu du dépôt

- `banque_powerbi.pbix` — fichier Power BI Desktop du projet
- `Donnees_Banque_Tunisie_Synthetiques.xlsx` — jeu de données source (synthétique)

## 📬 Contact

N'hésitez pas à me contacter sur [LinkedIn](#) pour toute question sur ce projet.

---

*Projet réalisé à des fins de démonstration et de portfolio.*
