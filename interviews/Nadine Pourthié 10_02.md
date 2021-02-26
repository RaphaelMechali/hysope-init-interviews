# Interviews Hysope II

## Volet général

* Présentation (nom métier, organisme, formation universitaire)
<span class="user-answer">
CNES depuis 40 ans. Traitement d'image Radar. Formation initiale en informatique (apprend le radar sur le tas). Un peu d'imagerie optique
En ce moment support SWOT, dans l'équipe CALVAL (ou future équipe), en particulier simulation d'imagerie radar (donnée brute). A une expérience d'autres types de données (S1 copernicus...)
A été responsable axe R&T CNES (altimétrie et imagerie Radar).
Fin de carrière quelques mois avant retraite.
</span>
  * Plutôt opérationnel? Scientifique? Archi / bureau d'étude?
<span class="user-answer">
Bureau d'étude (def amont), en support de toutes ces catégories
</span>
* Quel tâche métier principale? 
<span class="user-answer">
* En ce moment: simulation donnée RADAR et première partie du segment sol (fournit par le JPL - avant c'était SWOT Proto par CLS. Donne les RAW DATA, proches instruments sat, avant le pixel cloud). Un peu de bêta test. Ne programme pas. Est obligé de simuler un peu la suite pour vérifier la validité de la simulation
* Simu JPL / Simu SWOT de Damien
* Test les simulateurs
</span>
  * Pour quel résultat?
<span class="user-answer">
* Retour: cas non fonctionnels avec le simulateur
</span>
  * Pour qui?
<span class="user-answer">
si broken: pour Damien
si donnée produites: pour Claire (pré-analyse les abérrations puisse laisse la recherche spécifique erreur / typique)
</span>
  * Comment?
<span class="user-answer">
Si le teste passe (avec résultats des simu), visualise dans QGis la diff à la donnée attendue (de référence, ne creuse pas plus)
</span>
  * Etapes?
<span class="user-answer">
* Demande de Damien: file nous un coup de main sur la validation Simu
* Reçoit une nouvelle version
* Teste et valide
  * si broken: pour Damien
  * si donnée produites: pour Claire (pré-analyse les abérrations puisse laisse la recherche spécifique erreur / typique)
</span>
* Quelles tâches métiers secondaire? (sous-tâches ou tâches parallèles?)
<span class="user-answer">
L1B océano != L1B hydro (sérieux?!)
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
* QGis: Visuliser et superposer images et informations (données de ref, données google earth, NetCDF, shapefile, raster vecteur)
* Monteverdi (IHM pour l'OTB, manip d'image). DiapOTB pour le radar (remote module OTB pour le radar et l'interférométrie).
* Jupiter notebook (un peu, plus ses collègues)
Aimait bien l'outil Envi. 
</span>
  * Quels points forts?
<span class="user-answer">
* Facilité d'utilisation (par très convaincu)
</span>
  * Quels points d'amélioration?
<span class="user-answer">
* Mais pas toujours facile (prise en compte des format types NetCDF complexe), conversions pénibles
* Affichage compliqué mais requis (info orbite, trace, prise de tuiles, localisation), projections RADAR optique différences, certitude complexes
* Temps de réaction et volumes élevés
</span>
  * Quels points d'intégration?
<span class="user-answer">

</span>
* Quelles données? 
<span class="user-answer">

</span>
  * Neige (couverture / prduits dérivés)
<span class="user-answer">

</span>
  * SWE (volume eau / neige)
<span class="user-answer">

</span>
  * Surface d'eau (pixel eau)
<span class="user-answer">
https://www.notion.so/A-Beginner-s-Guide-to-Getting-Started-in-UX-Research-1e3e0567b4944c938ae8d1a4f0a21c56#4f2962643a3444d88b2bcb69438cbf47
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
* mesure et localisation du pixel, info pixel
* extraction de région de donnée
--> exploitation visuelle, valoriser la donnée pour par exemple comparer la hauteur sur la couche de reférence et la hauteur de la donnée produite.
--> Agrégation sur quelques point, sur un petit lac, sur une zone d'intérêt custom. (le sigma 0 => réflectivité)
</span>
  * de comparaison
<span class="user-answer">

</span>
  * d'extrapolation
<span class="user-answer">

</span>
* Tâche métier actuellement bien outillée?
<span class="user-answer">
Moyens du bord, bof. Pas d'outil parfaitement adéquat
</span>
  * Totalement couverte?
<span class="user-answer">

</span>
* Quels points pénibles (outils / données / volumétrie / format / etc...)
<span class="user-answer">
cf points d'amélioration
QGIs (expérience courte avec): formation requise, aide manquante (grosse réflexion pour elle). Ex: multi-sélection des layer en en retirant 1/3 (ne connaissait pas les groupes de layers). Manque de guidance
</span>
* Illustrer tâche métier durant l'interview? (si moins de 20 minutes)
<span class="user-answer">

</span>

## Volet intégration HI2

* Etes vous familiers avec les services Theia?
<span class="user-answer">

</span>
* Utilisez-vous des données Theia régulièrement?
<span class="user-answer">

</span>
* Accédez-vous régulièrement à des produits CNES (peps / cdpp / hydroweb / theia similaires...)
<span class="user-answer">

</span>

## Communauté

* Que pourrait vous apporter la communauté?
<span class="user-answer">
* Présentation de résultats partageables entre utilisateurs / avec le public (gobal / local, avec timeline, facile à créer)
* Echanges (feedback):
  * Truc et astuces
  * Besoins et évo du besoin
</span>
* Que souhaiteriez-vous apporter à la communauté?
<span class="user-answer">
* Interfaçage dev / utilisateur
</span>

## Ouverture

* Disponible peu (1/2 journée mois) pour participer à la conception
<span class="user-answer">
Oui, si elle n'est pas encore partie en retraite
</span>
* Qu'est ce qui vous ferait gagner du temps?
<span class="user-answer">
Outil
* Superposition des couches / données (complexes à cause du multi résolution / multi orbite)
* Localisation précise (coordonnée géo, carto, système de proj lat/lon ou en tout cas le plus standard --> rassurant). Mais en fait ça correspond au préférences de chacun (OK vérifier avec Lionel qui a l'air sceptique). Certains utilisateurs leur donnent des coordonnées issues d'autres systèmes de proj (exemple côte, grille océano intersection avec la zone estuaire en lat lon pour les hydro)
* Facile à utiliser
</span>
* POST: Quelles solutions dans un monde idéal?
<span class="user-answer">
cf. précédent
</span>

<style>
.user-answer {
  color: darkcyan;  
}
</style>
