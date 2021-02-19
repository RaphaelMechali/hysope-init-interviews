# Interviews Hysope II

## Volet général

* Présentation (nom métier, organisme, formation universitaire)
<font color="darkcyan">
Exploitation image depuis 35 ans
Géologue à la base (pas physicien / info pur, touche à tout)
Travaille au SERTIT (rattaché à un labo de Strasbourg), 20 ingé de recherche, bureau d'étude like, universitaire, né avec SPOT
labo passe de local à régional
</font>
  * Plutôt opérationnel? Scientifique? Archi / bureau d'étude?
<font color="darkcyan">
* Catographie rapide pour catastrophe naturelle (BE / OP), calcul d'impact sur bassin
* volet recherche: algorithmie
* management (sélection produit)
* Produit de démonstration, définition de missions spatiales (SMASH, VISA = future SWOT + opérationnel), apporte les besoin de carto rapide.
* Support équipe SWOT 
  * mise en place BD lacs / rivières
  * supervision campagne terrain
  * manage l'équipe rapid mapping
</font>
* Quel tâche métier principale? 
<font color="darkcyan">
 (a choisi la tâche): Etude petits lacs
</font>
  * Pour quel résultat?
<font color="darkcyan">
* aide notamment SWOT (pré-valide)
* donnée de gestion à destination commerciale (prestataire), pour la DREAL ou la region.
</font>
  * Pour qui?
<font color="darkcyan">
* SWOT
* pour la DREAL ou la region
* Agence de bassin
</font>
  * Comment?
<font color="darkcyan">
Attend les éléments altimétriques (compliqué de récupérer les séries temporelles) PUIS: 
Récupération donnée
</font>
  * Etapes?
<font color="darkcyan">
* Récupération donnée
* BD de variation de surface
* En cours: couplage avec de l'altimétrie (quand elle sera dispo pour petits lacs)
* Comparaison avec in situ (quand dispo, rarement! beaucoup d'interlocuteurs, c'est la galère, non centralisé sur la base hydro / vigicrue). Anecdote: l'asso de pêche lui permet d'accèder à une donnée tous les 10j. 
* Courbes, rapports et visuels (exemple: inondations décennales en Alsace)
</font>
* Quelles tâches métiers secondaire? (sous-tâches ou tâches parallèles?)
<font color="darkcyan">
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
* SIG: QGis (mais ont aussi ArcGis)
* Traitement d'images: (plutôt manager, utilise SNAP, mais ils ont aussi cognition, RDAS)
* Dev maison (intégrant plus ou moins de SNAP): Python + docker
* Recours aux chaînes SAR (veut passer Orpheo dessus)
</font>
  * Quels points forts?
<font color="darkcyan">
* Outils génériques / standards, mieux pour la discussion (raison au peu d'adoption de l'OTB)
</font>
  * Quels points d'amélioration?
<font color="darkcyan">
* pas assez validés (acuité des traitements trop souvent négocié). Notamment sur SurfWater (mais aussi en interne: optimisation contre qualité / vérification)
</font>
  * Quels points d'intégration?
<font color="darkcyan">

</font>
* Quelles données? 
<font color="darkcyan">

</font>
  * Neige (couverture / produits dérivés)
<font color="darkcyan">
Occasionnellement (pas fou, testé au cours d'un travail avec le SHAPI)
</font>
  * SWE (volume eau / neige)
<font color="darkcyan">
même réponse (mais quand même utile parfois lors des grands épisodes neigeux!)
</font>
  * Surface d'eau (pixel eau)
<font color="darkcyan">
Oui
</font>
  * Hauteur d'eau
<font color="darkcyan">
Oui
</font>
  * Débit d'eau
<font color="darkcyan">
Non
</font>
  * Température
<font color="darkcyan">
Oui
</font>
  * Turbidité
<font color="darkcyan">
Oui
</font>
  * Autres?
<font color="darkcyan">
Couverture en glace (pourquoi pas épaisseur)
</font>
* Quelles méthodes
  * d'exploitation
<font color="darkcyan">
PPT et présentation classique / diffusion via plateformes
statistiques classiques avec Excell (pas Mathlab):
(série de surface) 
(série de hauteur)
Y a t il du bruit? débruiter (si ça marche) > identifier les cycles > 
A. c'est le résultat final
B. recherche de correlation (origine météo / autres)
C. etude faune flore (correlation avec la température et la turbidité, permanence de l'eau, étendue des systèmes inondés)
====> application (absence / présence de parasites dans l'eau, etc..)
</font>
  * de comparaison
<font color="darkcyan">

</font>
  * d'extrapolation
<font color="darkcyan">
extrapolation / interpolation pour caler la donnée
</font>
* Tâche métier actuellement bien outillée?
<font color="darkcyan">
Non.
Surface: OK en interne.
Hauteur: KO, altimétrie indisponible pour les petits lacs
</font>
  * Totalement couverte?
<font color="darkcyan">

</font>
* Quels points pénibles (outils / données / volumétrie / format / etc...)
<font color="darkcyan">
* Pas de ressources pour aller chercher les séries altimétriques et les traiter pour lui (et ne peut pas cliquer dessus).
* notion de température "délicate" (bases physiques complexes). Comparaison entre capteurs complexes. Même remarque pour la turbidité (trop de modèles, compliquer à génériciser)
</font>
* Illustrer tâche métier durant l'interview? (si moins de 20 minutes)
<font color="darkcyan">

</font>

## Volet intégration HI2

* Etes vous familiers avec les services Theia?
<font color="darkcyan">
OUI Hydroweb (s'en sert régulièrement)
récupère aussi les feux de forêts chez le CNES
</font>
* Utilisez-vous des données Theia régulièrement?
<font color="darkcyan">

</font>
* Accédez-vous régulièrement à des produits CNES (peps / cdpp / hydroweb / theia similaires...)
<font color="darkcyan">
Consomme des données:
* Sentinels (PEPS/Hub Esa, chez l'ESA c'est lourd, Google earth engine): lourdeur ESA: obligé de récupérer les images stockées sur bandes magnétiques depuis quelques jours (== SciHub)
* RUS
* utilise RADARS classiques SPOT Pleiades (donnée payante HR, dans le cadre du rapid mapping, payé par leurs clients)
</font>

## Communauté

* Que pourrait vous apporter la communauté?
<font color="darkcyan">
Aurait voulu intégrer la communauté Trishna, eaux continentales, pour représenter son segment utilisateur (lacs / zones inondées), pour concevoir les requirements des produits ==> le produit EST ce dont ils se servent.
Manque de vision globale, n'y retrouve pas ses priorités 
N'a pas pu intégrer cette communauté
</font>
* Que souhaiteriez-vous apporter à la communauté?
<font color="darkcyan">

</font>

## Ouverture

* Disponible peu (1/2 journée mois) pour participer à la conception
<font color="darkcyan">
Oui
</font>
* Qu'est ce qui vous ferait gagner du temps?
<font color="darkcyan">
La vitesse d'accès à la donnée (ex accès in situ avec des tas de contacts différents).
La qualification du type de travail réalisable par donnée
Marketplace data
</font>
* POST: Quelles solutions dans un monde idéal?
<font color="darkcyan">
plus de traces (toutes?) exploitées (pas comme S3!)
Disponibilité de hauteur et variations des hauteurs multi-missions, si possible, fréquence journalière!
PLUS DE DONNEES (il n'y a pas les lacs de 6/7km² aujourd'hui)
</font>
