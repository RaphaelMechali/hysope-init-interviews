# Interviews Hysope II

## Volet général

* Présentation (nom métier, organisme, formation universitaire)
<span class="user-answer">
Exploitation image depuis 35 ans
Géologue à la base (pas physicien / info pur, touche à tout)
Travaille au SERTIT (rattaché à un labo de Strasbourg), 20 ingé de recherche, bureau d'étude like, universitaire, né avec SPOT
labo passe de local à régional
</span>
  * Plutôt opérationnel? Scientifique? Archi / bureau d'étude?
<span class="user-answer">
* Catographie rapide pour catastrophe naturelle (BE / OP), calcul d'impact sur bassin
* volet recherche: algorithmie
* management (sélection produit)
* Produit de démonstration, définition de missions spatiales (SMASH, VISA = future SWOT + opérationnel), apporte les besoin de carto rapide.
* Support équipe SWOT 
  * mise en place BD lacs / rivières
  * supervision campagne terrain
  * manage l'équipe rapid mapping
</span>
* Quel tâche métier principale? 
<span class="user-answer">
 (a choisi la tâche): Etude petits lacs
</span>
  * Pour quel résultat?
<span class="user-answer">
* aide notamment SWOT (pré-valide)
* donnée de gestion à destination commerciale (prestataire), pour la DREAL ou la region.
</span>
  * Pour qui?
<span class="user-answer">
* SWOT
* pour la DREAL ou la region
* Agence de bassin
</span>
  * Comment?
<span class="user-answer">
Attend les éléments altimétriques (compliqué de récupérer les séries temporelles) PUIS: 
Récupération donnée
</span>
  * Etapes?
<span class="user-answer">
* Récupération donnée
* BD de variation de surface
* En cours: couplage avec de l'altimétrie (quand elle sera dispo pour petits lacs)
* Comparaison avec in situ (quand dispo, rarement! beaucoup d'interlocuteurs, c'est la galère, non centralisé sur la base hydro / vigicrue). Anecdote: l'asso de pêche lui permet d'accèder à une donnée tous les 10j. 
* Courbes, rapports et visuels (exemple: inondations décennales en Alsace)
</span>
* Quelles tâches métiers secondaire? (sous-tâches ou tâches parallèles?)
<span class="user-answer">
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
* SIG: QGis (mais ont aussi ArcGis)
* Traitement d'images: (plutôt manager, utilise SNAP, mais ils ont aussi cognition, RDAS)
* Dev maison (intégrant plus ou moins de SNAP): Python + docker
* Recours aux chaînes SAR (veut passer Orpheo dessus)
</span>
  * Quels points forts?
<span class="user-answer">
* Outils génériques / standards, mieux pour la discussion (raison au peu d'adoption de l'OTB)
</span>
  * Quels points d'amélioration?
<span class="user-answer">
* pas assez validés (acuité des traitements trop souvent négocié). Notamment sur SurfWater (mais aussi en interne: optimisation contre qualité / vérification)
</span>
  * Quels points d'intégration?
<span class="user-answer">

</span>
* Quelles données? 
<span class="user-answer">

</span>
  * Neige (couverture / produits dérivés)
<span class="user-answer">
Occasionnellement (pas fou, testé au cours d'un travail avec le SHAPI)
</span>
  * SWE (volume eau / neige)
<span class="user-answer">
même réponse (mais quand même utile parfois lors des grands épisodes neigeux!)
</span>
  * Surface d'eau (pixel eau)
<span class="user-answer">
Oui
</span>
  * Hauteur d'eau
<span class="user-answer">
Oui
</span>
  * Débit d'eau
<span class="user-answer">
Non
</span>
  * Température
<span class="user-answer">
Oui
</span>
  * Turbidité
<span class="user-answer">
Oui
</span>
  * Autres?
<span class="user-answer">
Couverture en glace (pourquoi pas épaisseur)
</span>
* Quelles méthodes
  * d'exploitation
<span class="user-answer">
PPT et présentation classique / diffusion via plateformes
statistiques classiques avec Excell (pas Mathlab):
(série de surface) 
(série de hauteur)
Y a t il du bruit? débruiter (si ça marche) > identifier les cycles > 
A. c'est le résultat final
B. recherche de correlation (origine météo / autres)
C. etude faune flore (correlation avec la température et la turbidité, permanence de l'eau, étendue des systèmes inondés)
====> application (absence / présence de parasites dans l'eau, etc..)
</span>
  * de comparaison
<span class="user-answer">

</span>
  * d'extrapolation
<span class="user-answer">
extrapolation / interpolation pour caler la donnée
</span>
* Tâche métier actuellement bien outillée?
<span class="user-answer">
Non.
Surface: OK en interne.
Hauteur: KO, altimétrie indisponible pour les petits lacs
</span>
  * Totalement couverte?
<span class="user-answer">

</span>
* Quels points pénibles (outils / données / volumétrie / format / etc...)
<span class="user-answer">
* Pas de ressources pour aller chercher les séries altimétriques et les traiter pour lui (et ne peut pas cliquer dessus).
* notion de température "délicate" (bases physiques complexes). Comparaison entre capteurs complexes. Même remarque pour la turbidité (trop de modèles, compliquer à génériciser)
</span>
* Illustrer tâche métier durant l'interview? (si moins de 20 minutes)
<span class="user-answer">

</span>

## Volet intégration HI2

* Etes vous familiers avec les services Theia?
<span class="user-answer">
OUI Hydroweb (s'en sert régulièrement)
récupère aussi les feux de forêts chez le CNES
</span>
* Utilisez-vous des données Theia régulièrement?
<span class="user-answer">

</span>
* Accédez-vous régulièrement à des produits CNES (peps / cdpp / hydroweb / theia similaires...)
<span class="user-answer">
Consomme des données:
* Sentinels (PEPS/Hub Esa, chez l'ESA c'est lourd, Google earth engine): lourdeur ESA: obligé de récupérer les images stockées sur bandes magnétiques depuis quelques jours (== SciHub)
* RUS
* utilise RADARS classiques SPOT Pleiades (donnée payante HR, dans le cadre du rapid mapping, payé par leurs clients)
</span>

## Communauté

* Que pourrait vous apporter la communauté?
<span class="user-answer">
Aurait voulu intégrer la communauté Trishna, eaux continentales, pour représenter son segment utilisateur (lacs / zones inondées), pour concevoir les requirements des produits ==> le produit EST ce dont ils se servent.
Manque de vision globale, n'y retrouve pas ses priorités 
N'a pas pu intégrer cette communauté
</span>
* Que souhaiteriez-vous apporter à la communauté?
<span class="user-answer">

</span>

## Ouverture

* Disponible peu (1/2 journée mois) pour participer à la conception
<span class="user-answer">
Oui
</span>
* Qu'est ce qui vous ferait gagner du temps?
<span class="user-answer">
La vitesse d'accès à la donnée (ex accès in situ avec des tas de contacts différents).
La qualification du type de travail réalisable par donnée
Marketplace data
</span>
* POST: Quelles solutions dans un monde idéal?
<span class="user-answer">
plus de traces (toutes?) exploitées (pas comme S3!)
Disponibilité de hauteur et variations des hauteurs multi-missions, si possible, fréquence journalière!
PLUS DE DONNEES (il n'y a pas les lacs de 6/7km² aujourd'hui)
</span>

<style>
.user-answer {
  color: darkcyan;  
}
</style>
