# Interviews Hysope II

## Volet général

* Présentation (nom métier, organisme, formation universitaire)
<font color="darkcyan">
Travaille au CNES. a commencé sur du Radar
Ingé aérospatial
Thèse CNES / CLS SWOT
Après: chez SI/TR (Roger / Denis) traitement et simu radar
Prépa mission SWOT et simu des données. Partenariat JPL. Proto jusqu'au produit L2
* simu (outils génériques, pour WISA à terme, moins SWOT, automomie sur cette thématique, face au JPL. Plus HR pour lui)
* Beaucoup de dev, essentiellement Python
* Utilise beaucoup Jupiter notebook (tuto, petits résultats)
* travaille sur Floodplain DEM (premier consommateur des archives SWOT -> altimétrie à partir de SWOT) = Hypsométrie
* Support à CLaire et son équipe
</font>
  * Plutôt opérationnel? Scientifique? Archi / bureau d'étude?
<font color="darkcyan">
Bureau d'étude / Opérationnel pour donner un coup de main
scientifique = utilisateur (lui est fabricant de la donnée). Ils leur fournissent leurs réponses / besoin.
Il est côté Radar plus qu'hydro (modèle et calcul)
</font>
* Quel tâche métier principale? 
<font color="darkcyan">
* Faire tourner des algo, trouver ce qui ne va pas (debug, donnée, similaires), etoffer les fonctionnalités, capter les retours utilisateurs. Expertise (support).
* CALVAL: comparer des images et trouver les problèmes
  * Bugs algo?
  * PB d'instruments? et similaires
</font>
  * Pour quel résultat?
<font color="darkcyan">
* produire des images simulées, puis par métrique, comparaison, trouver le problème (nécessite données d'entrée pour repérer les problèmes)
--> outillage partiellement similaire entre cette tâche et la CALVAL (sauf pour les produits bas niveau: produits NetCDF != SWOT). Le simu (netcdf) ne tient pas compte dans les produits de niveau 0 de certaines spécificités physiques (ex antenne). 
</font>
  * Pour qui?
<font color="darkcyan">
* Pour lui même (FloodPlain Dem, simu => proto, rebouclage, échange avec des personnes liées par thématiques)
* Simu grande échelle (mis en commun), pour les scientifiques (MAJ soft, partage GIT, fournit des données qui correspondent à une étude plus ou moins spécifique), support en général
</font>
  * Comment?
<font color="darkcyan">
Travaille sur le cluster CNES. Toujours dans des projets GitLab (mais parfois d'une seule personne). 
* Sessions MobaXTerm et scripts Pyhton pour la simu / QGis ouvert constamment pour visualiser les résultats (nuages de points / shapefile)
* Fenêtre Jupiter notebook (pour travailler sur RADAR, utilise MatPlotLib en Python dans ce cas)
</font>
  * Etapes?
<font color="darkcyan">
Dépend des périodes:
* A: proto (FloodPlain Dem). 
  * a un produit intermédiaire
  * algorithmie papier
  * code
  * simule d'autres données
  * Teste avec et incrémente jusqu'à un résultat convenable
* B: nouvelle fonctionnalité
  * Reprend le code existant
  * Code
  * Vérifie la sortie
* C: Récupère un algo "partiellement implémenté" (robustesse) -> rejoint A
* D: Expertise/Support radar
  * mail / coup de fil d'un collègue
  * Investigue dans les résultats (image / refait tourner l'algo)
  * Explique les problèmes

Pas encore très carré pour lui, mais ont des issues GitLab pour tracer.
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
* Visualisation: QGis, un peu de soft spec (Panoply, NCView => visualisation du netCDF et dimensions associées)
* Dev: Jupiter Notebook, éditeur (Geany? à peine moins moche que Gedit)
* Skype
</font>
  * Quels points forts?
<font color="darkcyan">
* Outils maîtrisé 
  * Python: gratuit et très utilisé
  * Jupiter Hub: facilité de travail ENORME
* QGis: BIEN (mais gratuité et habitude justifient). Autonomie pour développer des plugins
</font>
  * Quels points d'amélioration?
<font color="darkcyan">
Non pas trop. Actuellement en mode dégradé (situation réseau actuelle, état sanitaire, globalement problème de la VRE -> affichage déporté)
Besoins de mémoire pour les grosses simulations (jusqu'à 184Go de mémoire), peu le bloquer
</font>
  * Quels points d'intégration?
<font color="darkcyan">

</font>
* Quelles données? 
<font color="darkcyan">

</font>
  * Neige (couverture / prduits dérivés)
<font color="darkcyan">
Non, pas dans un premier temps (peut permettre de répondre à certaines anomalies, donc oui quand même)
</font>
  * SWE (volume eau / neige)
<font color="darkcyan">
Pas trop, très indirect
</font>
  * Surface d'eau (pixel eau)
<font color="darkcyan">
Oui, sa deuxième métrique (validation perfo SWOT niveau L2)
</font>
  * Hauteur d'eau
<font color="darkcyan">
OUI, sa première métrique (indicateur perfo). La compare
</font>
  * Débit d'eau
<font color="darkcyan">
N'intervient pas dessus (éventuellement en support avec Kévin)
</font>
  * Température
<font color="darkcyan">
Non (pas en première intention, en cas de phénomèmes inexpliqués)
</font>
  * Turbidité
<font color="darkcyan">
Non (pas en première intention, en cas de phénomèmes inexpliqués)
</font>
  * Autres?
<font color="darkcyan">
en cas de phénomes inexpliqués: carte de végétation, occupation du sol. MNT
</font>
* Quelles méthodes
  * d'exploitation
<font color="darkcyan">
La plupart du temps fabrique un "pseudo produit" (pré CALVAL, produit en CALVAL), et la superpose à une donnée entrante: 
1. Premier niveau: comparaison visuelle: par exemple décalage de rivière par rapport à une référence externe.
2. Deuxième niveau: calcul d'indicateurs. Calcul d'étendue et comparaison avec la donnée d'entrée ou externe si CALVAL. Moyenne / écart-type hauteur sur une zone (par cours d'eau, par lac)
3. A] tout colle, chouette. B] retraiter / resimuler pour comprendre ce qu'il se passe (le phénomène apparaît à la simulation? Nouveau phénomène?)
Importance de la vérification à l'oeil: "En général ce qu'on voit à l'oeil se voit en auto aussi. Mais l'avantage c'est d'identifier les cas les plus problématiques (ex typique: grosse erreur de déroulement de phase => toute l'eau est décalée de 700m, superposition par rapport à la référence 0%, lien direct avec l'algorithme pour lui)"
</font>
  * de comparaison
<font color="darkcyan">
A initié un petit projet Git SWOT-CALVAL:
* ex typique 1: niveau 1.5 ou 2 (pixel cloud), superposé avec surfwater, ouverture des deux fichiers superposés, pour premier aperçu. Puis calcul d'étendu commune entre masque de référence et produit SWOT.
* ex typique 2 (plutôt simu mais applicable SWOT): Hauteur de ref et Moyenne sur la donnée
</font>
  * d'extrapolation
<font color="darkcyan">
* En cours d'étude pour le produit FloodPlain Dem (produit le plus compliqué de SWOT, tente de reconstituer la batimétrie).
Lignes de niveaux => batimétrie => 1er produit = points multitemporel => interpolation (premiere intention distribution Gaussienne, pas satisfaisante) ~ InverseDistanceWaiting idw.py. 
Probablement représenté dans la CALVAL pour comparer du pixel cloud
* Interpolation des RASTER pour les mettre à la même résolution
* Interpoler le pixel cloud sur une grille 
</font>
* Tâche métier actuellement bien outillée?
<font color="darkcyan">
Oui je pense.
</font>
  * Totalement couverte?
<font color="darkcyan">
Pas couvert: récupération de données externes (la galère!). Où est la BD tartempion, comment je récupère, comment modifier la donnée pour la faire correspondre à la mienne (pas son coeur de métier).
Récupérer rapidement toutes les tuiles intéressantes
</font>
* Quels points pénibles (outils / données / volumétrie / format / etc...)
<font color="darkcyan">
* Aura besoin de données externes (moins efficace que d'autres la dessus, veut bien de l'aide?)
* Gros besoin mémoires / Temps / CPU, ce qui nécessite beaucoup de méthode ("simulation bien carrée")
* Projection (UTM -> lat lon, pénible même s'il est maintenant mieux formé et le fait via QGis / script directement) ~ un peu projectif
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
Travaille très souvent avec des scientifiques:
1. A
  * Récupérer des données d'entrées (multi temporelles réaliste, ex: masque d'eau sur 1an)
  * En retour, ils sont souvent intéressés par le produit SWOT corresopndant (boucle feedback)
2. B - expertise des scientifiques (on s'éloigne, dans FloodPlain Dem du Radar). Les hydrologues peuvent l'aider dans la sélection des méthodes / algorithmie (collaboration écrite / GitLab)
* Du code (Utilise souvent stackoverflow et similaires)
</font>
* Que souhaiteriez-vous apporter à la communauté?
<font color="darkcyan">
Support aux produits SWOT et au simulateur, adaptation des produits (produit de haut niveau pas tout à fait figé au moment de la CALVAL), sélection des meilleurs produits / métriques. Support à des logiciels sans accès externe
</font>

## Ouverture

* Disponible peu (1/2 journée mois) pour participer à la conception
<font color="darkcyan">
Oui pas de souci
</font>
* Qu'est ce qui vous ferait gagner du temps?
<font color="darkcyan">
Voit pas trop
</font>
* POST: Quelles solutions dans un monde idéal?
<font color="darkcyan">
QGis est l'outil le plus complet qu'il utilise actuellement. UN SUPER QGIS ADAPTE POUR LIRE LES PRODUITS SWOT et produits auxiliaires, calculerait des métriques.
</font>


