# Interviews Hysope II

## Volet général

* Présentation (nom métier, organisme, formation universitaire)
<span class="user-answer">
Commence chez CS, arrive au CNES en 2007 (dev segment sol mission SSALTO), 10 ans en altimétrie, puis responsable mission SWOT (archi).
2018: Labo observation de la terre (support données spatiales, adéquation donnée -> métier utilisateurs). Adresse métropole, direction départementales, entreprises (statups / SNCF, ...)
Ils réalisent des proto pour démontrer l'adéquation des données spatiales
Ils sont impliqués sur SCO, AI4Geo, aimeraient sur SWOT Aval
Utilisent beaucoup de sentinel, Pleiade, Spot 7 (images)
Ils voudraient faire du Radar mais n'ont pas de compétence interne
En altimétrie: pas trop. Leur principales demandes sont sur le domaine cotier en général, pour l'altimétrie
Détection villes endommages, XXX sur les cours d'eau. 
Les amène à Flood (détection de dommages) et FloodDam
Pas mal de sujets de batimétrie cotière (en R&T)
</span>
  * Plutôt opérationnel? Scientifique? Archi / bureau d'étude?
<span class="user-answer">
plutôt bureau d'étude (adéquation données > besoin), un peu de R&T mais très concrète
</span>
* Quel tâche métier principale? 
<span class="user-answer">
Développement: traitements, mise en place de chaînes et clusters, librairies
</span>
  * Pour quel résultat?
<span class="user-answer">
Répondre au besoin. 
* Modèle d'apprentissage qualifié (massification de traitement d'image): Transmet l'algo OU le modèle entraîné au client
* Parfois des cartes, pas de plateformes sites.
* Plugin QGis parfois (sur les modèles entraînés)
</span>
  * Pour qui?
<span class="user-answer">
* Parfois direction technique des clients, responsables innovations (Paola?)
* Souvent interlocuteurs techniques (ingénieurs / chercheur - Axa Climate)
* Direction départementale: gestionnaires ou techniques, dépend des sujet
Ils n'ont pas forcément besoin de techniques en face (le niveau de finition du produit et la ressource qui l'utilisera peuvent changer)
</span>
  * Comment?
<span class="user-answer">
</span>
  * Etapes?
<span class="user-answer">
* Discussion client pour comprendre le besoin, prévoir les aménagement
* Trouver les données (résolution, revisite, diversité spectral, radar intéressant) => les guide dans les choix (Pleiade, Sentinel...)
  * Est-ce que le spatial peut répondre à la question (par exemple, suivi de la pousse des arbres --> manipule les données, fait des tests pour voir si c'est possible, sujets 3D ==> le spatial suffit)
* Itérent régulièrement 
  * avec les utilisateurs (besoin)
  * choix des meilleurs algo (résultat)
  * présentation des résultats
</span>
* Quelles tâches métiers secondaire? (sous-tâches ou tâches parallèles?)
<span class="user-answer">
* support / conseil aux utilisateurs les utilisateurs
</span>
  * Pour quel résultat?
<span class="user-answer">

</span>
  * Pour qui? (lui-même ?)
<span class="user-answer">

</span>
  * Comment?
<span class="user-answer">

</span>
* Quels outils actuels?
<span class="user-answer">
* QGIs (local ou jupiter, aime bien jupiter). Pas un grand fan (en distanciel), mais pratique pour la visu DES RESULTATS.
* OTB
* Python (local ou jupiter, aime bien jupiter): modèles etoffés en random forest => Jupiter lab pour faire tourner l'apprentissage)
* Cluster (utilisation massive, génial pour plein de traitement, cool VSCode)
* Plotly (stats sur les décharges illégales, représentation des stats en carte)
* GitLab (du CNES)
* Google Earth Engine: accès aux données HYPER SIMPLE, grand catalogue, global. Applis google earth
  * Top pour la visu, puis télécharge les données avant traitement (exemple: a commencé un sujet en Ouganda sur GEE pour la visu, pour éviter de télécharger, puis cluster)
</span>
  * Quels points forts?
<span class="user-answer">
cf au dessus
</span>
  * Quels points d'amélioration?
<span class="user-answer">
Le tracet des graphes (mathplotlib), c'est pénible! Système d'axes complexes, peu intuitifs
GEE: certaines données manquantes
QGis: chargement (sur le cluster) long et crash régulièrement. Pas terrible en distanciel. Préfère travailler en local avec (l'outil est bien en local!).
</span>
  * Quels points d'intégration?
<span class="user-answer">

</span>
* Quelles données? 
<span class="user-answer">
Tout peu potentiellement les intéresser (ils peuvent les recouper pour leurs modèles, par exemple modèle d'écoulement). AUJOURD'HUI ILS NE LES UTILISE PAS
Ajoute au moins: MNT, précipations, nature des sols (p-e, se trouve moins qualifié pour ça, mais bien pour les modèles d'apprentissage)
Ils sont là pour valoriser la donnée spatiale, mais recourent à des vérités terrain (drones aujourd'hui, in situ p-e)
</span>
  * Neige (couverture / prduits dérivés)
<span class="user-answer">
p-e, pour certains utilisateurs
</span>
  * SWE (volume eau / neige)
<span class="user-answer">

</span>
  * Surface d'eau (pixel eau)
<span class="user-answer">

</span>
  * Hauteur d'eau
<span class="user-answer">

</span>
  * Débit d'eau
<span class="user-answer">

</span>
  * Température
<span class="user-answer">

</span>
  * Turbidité
<span class="user-answer">

</span>
  * Autres?
<span class="user-answer">

</span>
* Quelles méthodes
  * d'exploitation
<span class="user-answer">
choisit:
seuils "classiques"
machine learning (random forest): regression, classification
deep learning: classification
traitements
les acteurs fournissent des données terrain pour l'entraînement. Ils labellisent les catégories sur image.
Filtrent éventuellement par masques de nuages (nuage et ombre)
</span>
  * de comparaison
<span class="user-answer">
ils produisent cartes (classification) ou extraient des indicateurs (statistiques)
Comparent par score (rappel / précision) les vérités terrain et les données détectées (et arbitrent après sur les seuils de précision, fonction de la pertinence et des exigences du métier, jamais 100% de précision)
</span>
  * d'extrapolation
<span class="user-answer">
interpolent entre plusieurs dates (pas toujours utile), interpolation linéaire
"Superrésolution" Sentinel (via modèle d'apprentissage) => injecter le savoir Pleiades dans la geo Sentinel
</span>
* Tâche métier actuellement bien outillée?
<span class="user-answer">
Oui plutôt
</span>
  * Totalement couverte?
<span class="user-answer">

</span>
* Quels points pénibles (outils / données / volumétrie / format / etc...)
<span class="user-answer">
Passe trop de temps à chercher des données aujourd'hui (exemples, les données Pléïades, c'est la gélère, même si c'est mieux qu'avant)
Trop de serveurs, login, méthodes d'accèss et formats. Ou est la plu-value de cette approche??? GEE clarifie cette approche!
Par exemple Radar: chaîne de traitement amont requise (dispo sur Peps mais c'est lourd!)
</span>
* Illustrer tâche métier durant l'interview? (si moins de 20 minutes)
<span class="user-answer">

</span>

## Volet intégration HI2

* Etes vous familiers avec les services Theia?
<span class="user-answer">
Oui
</span>
* Utilisez-vous des données Theia régulièrement?
<span class="user-answer">
Oui (S2 2A, 3A, occupation des sols, manteau neigeux, humidité des sols) Venµs / Landsat non mais y pense
</span>
* Accédez-vous régulièrement à des produits CNES (peps / cdpp / hydroweb / theia similaires...)
<span class="user-answer">
Peps: Oui
Chpines de traitement CAR pour la 3D
N'utilise pas HydroWeb aujoud'hui (peu de demande)
externes: GEE, catalogue **INAMIS?** (compléter avec Lionel)
</span>

## Communauté

* Que pourrait vous apporter la communauté?
<span class="user-answer">
Echanges sans passer par nous. 
Montée en compétence pour eux. Ont été consulter pour la qualité de l'eau d'autres acteurs (SI2A)- Exemple ils ont un fil slack: agricole. Imagine: fil slack inondation. 
Trouver de l'information
Pourrait rediriger vers ce forum
Pourrait intéresser les caisses d'assurance, globaliser la connaissance
</span>
* Que souhaiteriez-vous apporter à la communauté?
<span class="user-answer">
Contribuer à l'identification:
* Des acteurs
* Des débouchées applicatives par thématique
Souhaite amener des question, soulever des problèmes
</span>

## Ouverture

* Disponible peu (1/2 journée mois) pour participer à la conception
<span class="user-answer">
Oui
</span>
* Qu'est ce qui vous ferait gagner du temps?
<span class="user-answer">
* accès aux données
</span>
* POST: Quelles solutions dans un monde idéal?
<span class="user-answer">
Pas si mal servi, c'est vraiment un problème d'accès / visibilité des données.
passerelles entre traitements et moyens (ex cloud GEE)
Déploiement facile de petites applications Web
</span>

<style>
.user-answer {
  color: darkcyan;  
}
</style>
