# Interviews Hysope II

## Volet général

* Présentation (nom métier, organisme, formation universitaire)
<font color="darkcyan">
Master recherhce histoire (politique env. haute montagnes).
License pro 
CDI chargée d'études (socio éco) et chargée de clientèle
télédétection et cartographie
</font>
  * Plutôt opérationnel? Scientifique? Archi / bureau d'étude?
<font color="darkcyan">
Opérationnelle (la recherche est en amont ou en partenariat)
But: rendre la science accessible (gratuit / libre / service à coût)
</font>
* Quel tâche métier principale? 
<font color="darkcyan">
Ilôts de chaleur
Zone à risque d'érosion
</font>
  * Pour quel résultat?
<font color="darkcyan">
Faire un rendu carto: sensibiliser, étude d'impact, analyse de risque, cerner les zones inondées, analyse et rendu statistique.
Suivre l'évolution par zone (couverture végétale, stats). 
</font>
  * Pour qui?
<font color="darkcyan">
Collectivités locales, agglo, syndicats des eaux, réseaux sociaux, TF1 (a demandé les fichiers brutes pour respecter leur mise en forme), presse
</font>
  * Comment?
<font color="darkcyan">
Utilisent Envy pour les analyses (payant) et QGis carto
</font>
  * Etapes?
<font color="darkcyan">
Téléchargement de l'image, traitée sur SNAP (dont graphbuilder)
Travail d'image (Envy pour support, MathLab clusterisé), découpage, seuil, classification
Mise en forme carto: QGis
</font>
* Quelles tâches métiers secondaire? (sous-tâches ou tâches parallèles?)
<font color="darkcyan">
Chargée de clientèle : exemples de carto. Chargée de comm ==> carte pédagogiques
</font>
  * Pour quel résultat?
<font color="darkcyan">
nouveau site internet acmg.asso.net? 
* Clientèle
  * carto hors norme (échelle variante)
  * trombinoscope cartographié
* Comm
  * Carte répartion eau (année agricole, octobre -> octobre)
  * Carte répartion climat
  * Carte attirante, peu de logs, beaucoup de couleur, du bâti. Adaptée Viridis (bleu au vert, pour daltoniens)
Peuvent être A3 (poster) ou A4 (powerpoint)
</font>
  * Pour qui? (lui-même ?)
<font color="darkcyan">

</font>
  * Comment?
<font color="darkcyan">
Téléchargement:
* image Théia / Peps / Copernicus (Sci-Hub) / Landsat (usgs earth explorer)
* carto pure: IGN
* données de l'eau: téléchargée / WMS (BD Carthage) => croisement de données pour les compléter
* routes et similaires
Utilisent peu LandCover: trop daté
* occupation des sols: Cesbio **TODO compléter avec Lionel**
* IDGéo? Bâti / cadastre
* Datagouv et autres pour les départements

toujours QGis.
</font>
* Quels outils actuels?
<font color="darkcyan">
* QGis
* Snap
* Envi: image de température
* PostGIS
* Excell, fichier CSV, c'est ce qu'elle préfère pour travailler
* Facebook (agricole), Twitter, LinkedIn, Vidéos Youtube
* a un serveur distant pour travailler

</font>
  * Quels points forts?
<font color="darkcyan">
* ALL instinctif
* QGis (2.18, mais utilise aussi la 3.x pour la 3D) est plus ludique que ArcGis, communauté plus intéressante
* Excell > rapide, bon support
* Snap: installation facile, intuitif, peu gourmand en ressources
* Envy: payant mais très bien! (support, facilité d'utilisation, ) Exemple: polygonisation d'une zone 35min face à 8h. Très compatible avec QGis
* Google Earth Engine avec KML et KMZ, effet WAOUH, a utilisé pour transférer des données à un client
</font>
  * Quels points d'amélioration?
<font color="darkcyan">
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
</font>
  * Quels points d'intégration?
<font color="darkcyan">

</font>
* Quelles données? 
<font color="darkcyan">

</font>
  * Neige (couverture / produits dérivés)
<font color="darkcyan">
Oui si publiée récemment (tous les 15j). Actuellement non
</font>
  * SWE (volume eau / neige)
<font color="darkcyan">
Non
</font>
  * Surface d'eau (pixel eau)
<font color="darkcyan">
Oui
</font>
  * Hauteur d'eau
<font color="darkcyan">
Oui, fonction des cours d'eau (pour le petits!)
</font>
  * Débit d'eau
<font color="darkcyan">
Oui, fonction des cours d'eau (pour le petits!)
</font>
  * Température
<font color="darkcyan">
Oui (landsat 8)
Température de surface: mesuré par eux mêmes
</font>
  * Turbidité
<font color="darkcyan">
Calculé par leur station, la veulent bien. Mal communiqué
</font>
  * Autres?
<font color="darkcyan">
Température air
Prévisions météo
micro BV: largeur maxi / mini
en plus de hauteur d'eau, hauteur entre fond et berge (pour prévision crue) ~= profondeur du lit
aménagement des berges (urbain / végétation / habitation), occupation de la zone tampon
</font>
* Quelles méthodes
  * d'exploitation
<font color="darkcyan">
demander à Maël?
système de seuil statistique
Jean François, dans Eau et Climat, utilise le résultat (modèle) => étudie le positionnement, propose des stratégies (lacs, irrigations, etc...). Ils mesurent les ilots de chaleur sur le terrain au préalable
</font>
  * de comparaison
<font color="darkcyan">
stats de répartition (% d'occupation, calcul et évo de surface, température et dégagement de corrélations)
très peu automatisé aujourd'hui (mais pourrait)
</font>
  * d'extrapolation
<font color="darkcyan">
Analyse de pixel mais sinon préfères une courbe coupée à une courbe fausse. Même raisonnement au niveau pixel (préfères le pixel "noir")
Son collègue p-e sur du Radar / de l'optique (image avant après)
Modèle interne: telle temp => batiment / ilot de chaleur, évolution connue et corrélation => interpolation de la température du bâtiment (est-ce que mes bâtiments seront menacés dans un futur)
Beaucoup de modélisation des pluies / climats, sur plusieurs scénarios (3 en général)
</font>
* Tâche métier actuellement bien outillée?
<font color="darkcyan">
Oui
</font>
  * Totalement couverte?
<font color="darkcyan">
Manque de données sinon oui
</font>
* Quels points pénibles (outils / données / volumétrie / format / etc...)
<font color="darkcyan">
QGis plante ("plantage dumpé, enregistrement dans C impossible") => toute la symbolique à refaire
Création de BD complexe (requiert Python, SQL, mais ça pourrait être graphique, pour créer des couches shapes!)
</font>
* Illustrer tâche métier durant l'interview? (si moins de 20 minutes)
<font color="darkcyan">

</font>

## Volet intégration HI2

* Etes vous familiers avec les services Theia?
<font color="darkcyan">
Oui
</font>
* Utilisez-vous des données Theia régulièrement?
<font color="darkcyan">
Oui
</font>
* Accédez-vous régulièrement à des produits CNES (peps / cdpp / hydroweb / theia similaires...)
<font color="darkcyan">
Oui (cf. au dessus)
</font>

## Communauté

* Que pourrait vous apporter la communauté?
<font color="darkcyan">
* accès à la donnée (carnet d'addresse): qui a la donnée? est-elle gratuite? Contraintes? a qui l'acheter? 
  * Annuaire des prestataires de données. Indique que c'est également un problème de l'UNESCO
mais conf, type SHF hydro, montre qu'il y a des communautés, mais peu accessibles hors université, demande trop de veille
    * trouver les BE sans passer par le site du gouvernement: nul pour les mots clefs (certains sont "mesure" quand d'autres, comme eux, sont plus "analyse / prévision")
* pro et cons des soft (quel outil / quelle version favoriser pour quelle tâche?) -> partage de méthodes et de connaissances entre utilisateurs
* présentation le travail par utilisateur (presque réseau social d'hydrologie)
</font>
* Que souhaiteriez-vous apporter à la communauté?
<font color="darkcyan">
* leur production dans le cadre des projets européens est accessibles à tout le monde (hauteur de 20 cours d'eau, ils peuvent fournir les mots de passe)
* donnée en vente ou en échange
</font>

## Ouverture

* Disponible peu (1/2 journée mois) pour participer à la conception
<font color="darkcyan">
Oui
</font>
* Qu'est ce qui vous ferait gagner du temps?
<font color="darkcyan">
pas gagner du temps
Theia plus instinctif!
</font>
* POST: Quelles solutions dans un monde idéal?
<font color="darkcyan">
Esprit de communauté (notamment pour les étudiants qui recherchent des stages ~ actuellement ils vont sur Géoréseau)
PAS DE CODE (notamment pour les BD types PostGIS)
Note: elle multi-exporte, clic par clic, tous ses fichiers Excell > pouvoir exporter plusieurs fichiers excell au format qui va bien, par seuils
</font>
