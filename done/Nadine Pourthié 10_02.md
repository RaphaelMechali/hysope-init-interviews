# Interviews Hysope II

## Volet général

* Présentation (nom métier, organisme, formation universitaire)
<font color="darkcyan">
CNES depuis 40 ans. Traitement d'image Radar. Formation initiale en informatique (apprend le radar sur le tas). Un peu d'imagerie optique
En ce moment support SWOT, dans l'équipe CALVAL (ou future équipe), en particulier simulation d'imagerie radar (donnée brute). A une expérience d'autres types de données (S1 copernicus...)
A été responsable axe R&T CNES (altimétrie et imagerie Radar).
Fin de carrière quelques mois avant retraite.
</font>
  * Plutôt opérationnel? Scientifique? Archi / bureau d'étude?
<font color="darkcyan">
Bureau d'étude (def amont), en support de toutes ces catégories
</font>
* Quel tâche métier principale? 
<font color="darkcyan">
* En ce moment: simulation donnée RADAR et première partie du segment sol (fournit par le JPL - avant c'était SWOT Proto par CLS. Donne les RAW DATA, proches instruments sat, avant le pixel cloud). Un peu de bêta test. Ne programme pas. Est obligé de simuler un peu la suite pour vérifier la validité de la simulation
* Simu JPL / Simu SWOT de Damien
* Test les simulateurs
</font>
  * Pour quel résultat?
<font color="darkcyan">
* Retour: cas non fonctionnels avec le simulateur
</font>
  * Pour qui?
<font color="darkcyan">
si broken: pour Damien
si donnée produites: pour Claire (pré-analyse les abérrations puisse laisse la recherche spécifique erreur / typique)
</font>
  * Comment?
<font color="darkcyan">
Si le teste passe (avec résultats des simu), visualise dans QGis la diff à la donnée attendue (de référence, ne creuse pas plus)
</font>
  * Etapes?
<font color="darkcyan">
* Demande de Damien: file nous un coup de main sur la validation Simu
* Reçoit une nouvelle version
* Teste et valide
  * si broken: pour Damien
  * si donnée produites: pour Claire (pré-analyse les abérrations puisse laisse la recherche spécifique erreur / typique)
</font>
* Quelles tâches métiers secondaire? (sous-tâches ou tâches parallèles?)
<font color="darkcyan">
L1B océano != L1B hydro (sérieux?!)
</font>
  * Pour quel résultat?
<font color="darkcyan">

</font>
  * Pour qui? (lui-même ?)
<font color="darkcyan">

</font>
  * Comment?
<font color="darkcyan">

</font>
* Quels outils actuels?
<font color="darkcyan">
* QGis: Visuliser et superposer images et informations (données de ref, données google earth, NetCDF, shapefile, raster vecteur)
* Monteverdi (IHM pour l'OTB, manip d'image). DiapOTB pour le radar (remove module OTB pour le radar et l'interférométrie).
* Jupiter notebook (un peu, plus ses collègues)
Aimait bien l'outil Envy. 
</font>
  * Quels points forts?
<font color="darkcyan">
* Facilité d'utilisation (par très convaincu)
</font>
  * Quels points d'amélioration?
<font color="darkcyan">
* Mais pas toujours facile (prise en compte des format types NetCDF complexe), conversions pénibles
* Affichage compliqué mais requis (info orbite, trace, prise de tuiles, localisation), projections RADAR optique différences, certitude complexes
* Temps de réaction et volumes élevés
</font>
  * Quels points d'intégration?
<font color="darkcyan">

</font>
* Quelles données? 
<font color="darkcyan">

</font>
  * Neige (couverture / prduits dérivés)
<font color="darkcyan">

</font>
  * SWE (volume eau / neige)
<font color="darkcyan">

</font>
  * Surface d'eau (pixel eau)
<font color="darkcyan">

</font>
  * Hauteur d'eau
<font color="darkcyan">

</font>
  * Débit d'eau
<font color="darkcyan">

</font>
  * Température
<font color="darkcyan">

</font>
  * Turbidité
<font color="darkcyan">

</font>
  * Autres?
<font color="darkcyan">

</font>
* Quelles méthodes
  * d'exploitation
<font color="darkcyan">
* mesure et localisation du pixel, info pixel
* extraction de région de donnée
--> exploitation visuelle, valoriser la donnée pour par exemple comparer la hauteur sur la couche de reférence et la hauteur de la donnée produite.
--> Agrégation sur quelques point, sur un petit lac, sur une zone d'intérêt custom. (le sigma 0 => réflectivité)
</font>
  * de comparaison
<font color="darkcyan">

</font>
  * d'extrapolation
<font color="darkcyan">

</font>
* Tâche métier actuellement bien outillée?
<font color="darkcyan">
Moyens du bord, bof. Pas d'outil parfaitement adéquat
</font>
  * Totalement couverte?
<font color="darkcyan">

</font>
* Quels points pénibles (outils / données / volumétrie / format / etc...)
<font color="darkcyan">
cf points d'amélioration
QGIs (expérience courte avec): formation requise, aide manquante (grosse réflexion pour elle). Ex: multi-sélection des layer en en retirant 1/3 (ne connaissait pas les groupes de layers). Manque de guidance
</font>
* Illustrer tâche métier durant l'interview? (si moins de 20 minutes)
<font color="darkcyan">

</font>

## Volet intégration HI2

* Etes vous familiers avec les services Theia?
<font color="darkcyan">

</font>
* Utilisez-vous des données Theia régulièrement?
<font color="darkcyan">

</font>
* Accédez-vous régulièrement à des produits CNES (peps / cdpp / hydroweb / theia similaires...)
<font color="darkcyan">

</font>

## Communauté

* Que pourrait vous apporter la communauté?
<font color="darkcyan">
* Présentation de résultats partageables entre utilisateurs / avec le public (gobal / local, avec timeline, facile à créer)
* Echanges (feedback):
  * Truc et astuces
  * Besoins et évo du besoin
</font>
* Que souhaiteriez-vous apporter à la communauté?
<font color="darkcyan">
* Interfaçage dev / utilisateur
</font>

## Ouverture

* Disponible peu (1/2 journée mois) pour participer à la conception
<font color="darkcyan">
Oui, si elle n'est pas encore partie en retraite
</font>
* Qu'est ce qui vous ferait gagner du temps?
<font color="darkcyan">
Outil
* Superposition des couches / données (complexes à cause du multi résolution / multi orbite)
* Localisation précise (coordonnée géo, carto, système de proj lat/lon ou en tout cas le plus standard --> rassurant). Mais en fait ça correspond au préférences de chacun (OK vérifier avec Lionel qui a l'air sceptique). Certains utilisateurs leur donnent des coordonnées issues d'autres systèmes de proj (exemple côte, grille océano intersection avec la zone estuaire en lat lon pour les hydro)
* Facile à utiliser
</font>
* POST: Quelles solutions dans un monde idéal?
<font color="darkcyan">
cf. précédent
</font>


