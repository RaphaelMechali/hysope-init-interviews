# Interviews Hysope II

## Volet général

* Présentation (nom métier, organisme, formation universitaire)
<span class="user-answer">
Master recherche histoire (politique env. haute montagnes).
License pro 
CDI chargée d'études (socio éco) et chargée de clientèle
télédétection et cartographie
</span>
  * Plutôt opérationnel? Scientifique? Archi / bureau d'étude?
<span class="user-answer">
Opérationnelle (la recherche est en amont ou en partenariat)
But: rendre la science accessible (gratuit / libre / service à coût)
</span>
* Quel tâche métier principale? 
<span class="user-answer">
Ilôts de chaleur
Zone à risque d'érosion
</span>
  * Pour quel résultat?
<span class="user-answer">
Faire un rendu carto: sensibiliser, étude d'impact, analyse de risque, cerner les zones inondées, analyse et rendu statistique.
Suivre l'évolution par zone (couverture végétale, stats). 
</span>
  * Pour qui?
<span class="user-answer">
Collectivités locales, agglo, syndicats des eaux, réseaux sociaux, TF1 (a demandé les fichiers brutes pour respecter leur mise en forme), presse
</span>
  * Comment?
<span class="user-answer">
Utilisent Envy pour les analyses (payant) et QGis carto
</span>
  * Etapes?
<span class="user-answer">
Téléchargement de l'image, traitée sur SNAP (dont graphbuilder)
Travail d'image (Envi pour support, MathLab clusterisé), découpage, seuil, classification
Mise en forme carto: QGis
</span>
* Quelles tâches métiers secondaire? (sous-tâches ou tâches parallèles?)
<span class="user-answer">
Chargée de clientèle : exemples de carto. Chargée de comm ==> carte pédagogiques
</span>
  * Pour quel résultat?
<span class="user-answer">
nouveau site internet acmg.asso.net? 
* Clientèle
  * carto hors norme (échelle variante)
  * trombinoscope cartographié
* Comm
  * Carte répartition eau (année agricole, octobre -> octobre)
  * Carte répartition climat
  * Carte attirante, peu de logos, beaucoup de couleur, du bâti. Adaptée Viridis (bleu au vert, pour daltoniens)
Peuvent être A3 (poster) ou A4 (powerpoint)
</span>
  * Pour qui? (lui-même ?)
<span class="user-answer">

</span>
  * Comment?
<span class="user-answer">
Téléchargement:
* image Théia / Peps / Copernicus (Sci-Hub) / Landsat (usgs earth explorer)
* carto pure: IGN
* données de l'eau: téléchargée CSV / WMS (BD Carthage) => croisement de données pour les compléter
* routes et similaires sur OpenStreetMap (pas complet mais quand même très bien)
* Utilisent peu LandCover: trop daté
* occupation des sols: Cesbio **TODO compléter avec Lionel**
* IDGéo? Bâti / cadastre
* Datagouv et autres pour les départements

toujours QGis.
</span>
* Quels outils actuels?
<span class="user-answer">
* QGis
* Snap
* Envi: image de température
* PostGIS
* Excell, fichier CSV, c'est ce qu'elle préfère pour travailler
* Facebook (agricole), Twitter, LinkedIn, Vidéos Youtube
* a un serveur distant pour travailler

</span>
  * Quels points forts?
<span class="user-answer">
* ALL instinctif
* QGis (2.18, mais utilise aussi la 3.x pour la 3D) est plus ludique que ArcGis, communauté plus intéressante
* Excell > rapide, bon support
* Snap: installation facile, intuitif, peu gourmand en ressources
* Envy: payant mais très bien! (support, facilité d'utilisation, ) Exemple: polygonisation d'une zone 35min face à 8h. Très compatible avec QGis
* Google Earth, effet WAOUH, a utilisé pour transférer des données à un client
</span>
  * Quels points d'amélioration?
<span class="user-answer">
* N'aime pas PostGIS (le délègue à son collègue qui aime faire ça)
* Données: insuffisant
* QGis: simplifier les étapes (créer un BV: trop d'étapes, mieux sur ArcGIS).  Boîte à outil trop complexe
  * Ou rendre la donnée accessible à tous
* Envy: rien à changer (passez le en français)
* Snap: des fois affichage trop rudimentaire
* Excell: ne rien changer mais:
  * Formalisme non intégrable
  * coller 35k lignes le tue
* 100 caractères de plus sur twitter
* Référencement Youtube compliqué
* LinkedIn emoticon pénibles à faire
</span>
  * Quels points d'intégration?
<span class="user-answer">

</span>
* Quelles données? 
<span class="user-answer">

</span>
  * Neige (couverture / produits dérivés)
<span class="user-answer">
Oui si publiée récemment (tous les 15j). Actuellement non
</span>
  * SWE (volume eau / neige)
<span class="user-answer">
Non mauvaise comm?
</span>
  * Surface d'eau (pixel eau)
<span class="user-answer">
Oui
</span>
  * Hauteur d'eau
<span class="user-answer">
Oui, fonction des cours d'eau (pour le petits!)
</span>
  * Débit d'eau
<span class="user-answer">
Oui, fonction des cours d'eau (pour le petits!)
</span>
  * Température
<span class="user-answer">
Oui (landsat 8)
Température de surface: mesuré par eux mêmes
</span>
  * Turbidité
<span class="user-answer">
Calculé par leur station, la veulent bien. Mal communiqué
</span>
  * Autres?
<span class="user-answer">
Température air
Prévisions météo
micro BV: largeur maxi / mini
en plus de hauteur d'eau, hauteur entre fond et berge (pour prévision crue) ~= profondeur du lit
aménagement des berges (urbain / végétation / habitation), occupation de la zone tampon
</span>
* Quelles méthodes
  * d'exploitation
<span class="user-answer">
demander à Maël?
système de seuil statistique
Jean François, dans commité Eau et Climat, utilise le résultat (modèle) => étudie le positionnement, propose des stratégies (lacs, irrigations, etc...). Ils mesurent les îlots de chaleur sur le terrain au préalable
</span>
  * de comparaison
<span class="user-answer">
stats de répartition (% d'occupation, calcul et évo de surface, température et dégagement de corrélations)
très peu automatisé aujourd'hui (mais pourrait)
</span>
  * d'extrapolation
<span class="user-answer">
Analyse de pixel mais sinon préfères une courbe coupée à une courbe fausse. Même raisonnement au niveau pixel (préfères le pixel "noir")
Son collègue p-e sur du Radar / de l'optique (image avant après)
Modèle interne: telle temp => batiment / ilot de chaleur, évolution connue et corrélation => interpolation de la température du bâtiment (est-ce que mes bâtiments seront menacés dans un futur)
Beaucoup de modélisation des pluies / climats, sur plusieurs scénarios (3 en général)
</span>
* Tâche métier actuellement bien outillée?
<span class="user-answer">
Oui
</span>
  * Totalement couverte?
<span class="user-answer">
Manque de données sinon oui
</span>
* Quels points pénibles (outils / données / volumétrie / format / etc...)
<span class="user-answer">
QGis plante ("plantage dumpé, enregistrement dans C impossible") => toute la symbolique à refaire
Création de BD complexe (requiert Python, SQL, mais ça pourrait être graphique, pour créer des couches shapes!)
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
Oui
</span>
* Accédez-vous régulièrement à des produits CNES (peps / cdpp / hydroweb / theia similaires...)
<span class="user-answer">
Oui (cf. au dessus)
</span>

## Communauté

* Que pourrait vous apporter la communauté?
<span class="user-answer">
* accès à la donnée (carnet d'addresse): qui a la donnée? est-elle gratuite? Contraintes? a qui l'acheter? 
  * Annuaire des prestataires de données. Indique que c'est également un problème de l'UNESCO
mais conf, type SHF hydro, montre qu'il y a des communautés, mais peu accessibles hors université, demande trop de veille
    * trouver les BE sans passer par le site du gouvernement ou recherche google: nul pour les mots clefs (certains sont "mesure" quand d'autres, comme eux, sont plus "analyse / prévision")
* pro et cons des soft (quel outil / quelle version favoriser pour quelle tâche?) -> partage de méthodes et de connaissances entre utilisateurs
* présentation le travail par utilisateur (presque réseau social d'hydrologie)
</span>
* Que souhaiteriez-vous apporter à la communauté?
<span class="user-answer">
* leur production dans le cadre des projets européens est accessibles à tout le monde (hauteur de 20 cours d'eau, ils peuvent fournir les mots de passe)
* donnée en vente ou en échange
</span>

## Ouverture

* Disponible peu (1/2 journée mois) pour participer à la conception
<span class="user-answer">
Oui
</span>
* Qu'est ce qui vous ferait gagner du temps?
<span class="user-answer">
pas gagner du temps
Theia plus instinctif!
</span>
* POST: Quelles solutions dans un monde idéal?
<span class="user-answer">
Esprit de communauté (notamment pour les étudiants qui recherchent des stages ~ actuellement ils vont sur GeoRezo)
PAS DE CODE (notamment pour les BD types PostGIS)
Note: elle multi-exporte, clic par clic, tous ses fichiers Excell > pouvoir exporter plusieurs fichiers excell au format qui va bien, par seuils
</span>

<style>
.user-answer {
  color: darkcyan;  
}
</style>
