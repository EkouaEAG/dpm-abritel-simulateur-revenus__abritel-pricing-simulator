# Data Product Management : Simulateur de revenus pour Abritel

# Contexte et Problématique
Sur des plateformes comme Abritel, chaque nuitée non pourvue représente un manque à gagner direct pour l'hôte et une perte de commission pour l'entreprise.
Lors de la phase de *Discovery*, j'ai constaté que pendant les saisons basses, les propriétaires particuliers n'ajustent pas leurs tarifs, laissant leurs logements vides. La raison principale n'est pas un refus de louer, mais une paralysie décisionnelle due à l'incertitude : sans visibilité chiffrée, baisser le prix est perçu comme une dévalorisation du bien.

# L'approche centrée utilisateur (Persona)
Toute la solution a été pensée pour **Manon (52 ans)**, notre "propriétaire pragmatique". Gérant seule sa résidence secondaire, elle n'est pas experte en données et craint les systèmes algorithmiques opaques. 
L'objectif produit est donc de transformer son incertitude en une décision rationnelle grâce à la donnée.

# La Solution Data : Le Simulateur de manque à gagner
Plutôt que d'imposer un prix via un algorithme de Machine Learning ("boîte noire" rejetée par les utilisateurs méfiants), j'ai opté pour une approche **Business Intelligence (BI)** transparente.
L'outil quantifie financièrement l'impact de l'inoccupation et projette les gains d'une promotion ciblée en se basant sur le marché local. 

**Fonctionnalités clés du MVP :**
*   Alertes proactives de vacance (ex: à J-14).
*   Simulateur interactif pour visualiser le gain potentiel par rapport au marché local.
*   Bouton d'action directe pour activer une "Offre Flash" sur les créneaux vides.

*(N'oublie pas d'uploader ton Experience Map et de changer le nom du fichier ci-dessous)*
![Experience Map de Manon](experience_map.png)

# Stack Technique du MVP
*   **Data Warehouse :** Stockage de l'historique des réservations et des prix du marché local.
*   **Power BI :** Moteur de calcul et de visualisation intégré via API dans l'espace propriétaire.
*   **API Salesforce :** Gestion du profil de l'hôte (Manon).

*(N'oublie pas d'uploader l'image de ta maquette et de changer le nom du fichier ci-dessous)*
![Maquette du MVP Power BI](maquette_dashboard.png)

# KPIs et Mesure du succès
Pour s'assurer que la donnée crée de la valeur, la performance du produit s'évalue sur :
1.  **Taux de remplissage des créneaux de vacance :** Objectif de conversion de 40 % sur les "trous" de 2 à 5 nuits.
2.  **Revenu incrémentiel (N vs N-1) :** Prouver la rentabilité économique de la stratégie de prix dynamique sur la basse saison.
3.  **Indice de protection de la marge :** Un garde-fou comparant le revenu net après promotion au prix plancher défini par l'hôte, garantissant la rentabilité.
4.  **Délai moyen de réservation (Lead Time) et Taux d'acceptation des réservations "Flash".**

## Méthodologie Produit & Leçons apprises
Ce projet a été mené en méthodologie Agile, en passant par plusieurs outils de cadrage : **Business Model Canvas, Benchmark concurrentiel et Grille de priorisation**.
**L'enseignement majeur :** "Prioriser le problème avant la technologie". La valeur de ce produit data ne réside pas dans la complexité de ses calculs, mais dans sa capacité à résoudre un blocage psychologique (la charge mentale de la veille tarifaire) en redonnant le contrôle à l'utilisateur via la transparence de la Business Intelligence.

---
*Projet réalisé dans le cadre du cursus Data Product Management chez Liora.*
