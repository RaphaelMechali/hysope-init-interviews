# Interviews Hysope II

## Volet général

* Présentation (nom métier, organisme, formation universitaire)
<span class="user-answer">
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
</span>
  * Plutôt opérationnel? Scientifique? Archi / bureau d'étude?
<span class="user-answer">
Bureau d'étude / Opérationnel pour donner un coup de main
scientifique = utilisateur (lui est fabricant de la donnée). Ils leur fournissent leurs réponses / besoin.
Il est côté Radar plus qu'hydro (modèle et calcul)
</span>
* Quel tâche métier principale? 
<span class="user-answer">
* Faire tourner des algo, trouver ce qui ne va pas (debug, donnée, similaires), etoffer les fonctionnalités, capter les retours utilisateurs. Expertise (support).
* CALVAL: comparer des images et trouver les problèmes
  * Bugs algo?
  * PB d'instruments? et similaires
</span>
  * Pour quel résultat?
<span class="user-answer">
* produire des images simulées, puis par métrique, comparaison, trouver le problème (nécessite données d'entrée pour repérer les problèmes)
--> outillage partiellement similaire entre cette tâche et la CALVAL (sauf pour les produits bas niveau: produits NetCDF != SWOT). Le simu (netcdf) ne tient pas compte dans les produits de niveau 0 de certaines spécificités physiques (ex antenne). 
</span>
  * Pour qui?
<span class="user-answer">
* Pour lui même (FloodPlain Dem, simu => proto, rebouclage, échange avec des personnes liées par thématiques)
* Simu grande échelle (mis en commun), pour les scientifiques (MAJ soft, partage GIT, fournit des données qui correspondent à une étude plus ou moins spécifique), support en général
</span>
  * Comment?
<span class="user-answer">
Travaille sur le cluster CNES. Toujours dans des projets GitLab (mais parfois d'une seule personne). 
* Sessions MobaXTerm et scripts Pyhton pour la simu / QGis ouvert constamment pour visualiser les résultats (nuages de points / shapefile)
* Fenêtre Jupiter notebook (pour travailler sur RADAR, utilise MatPlotLib en Python dans ce cas)
</span>
  * Etapes?
<span class="user-answer">
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
* Visualisation: QGis, un peu de soft spec (Panoply, NCView => visualisation du netCDF et dimensions associées)
* Dev: Jupiter Notebook, éditeur (Geany? à peine moins moche que Gedit)
* Skype
</span>
  * Quels points forts?
<span class="user-answer">
* Outils maîtrisé 
  * Python: gratuit et très utilisé
  * Jupiter Hub: facilité de travail ENORME
* QGis: BIEN (mais gratuité et habitude justifient). Autonomie pour développer des plugins
</span>
  * Quels points d'amélioration?
<span class="user-answer">
Non pas trop. Actuellement en mode dégradé (situation réseau actuelle, état sanitaire, globalement problème de la VRE -> affichage déporté)
Besoins de mémoire pour les grosses simulations (jusqu'à 184Go de mémoire), peut le bloquer
</span>
  * Quels points d'intégration?
<span class="user-answer">

</span>
* Quelles données? 
<span class="user-answer">

</span>
  * Neige (couverture / prduits dérivés)
<span class="user-answer">
Non, pas dans un premier temps (peut permettre de répondre à certaines anomalies, donc oui quand même)
</span>
  * SWE (volume eau / neige)
<span class="user-answer">
Pas trop, très indirect
</span>
  * Surface d'eau (pixel eau)
<span class="user-answer">
Oui, sa deuxième métrique (validation perfo SWOT niveau L2)
</span>
  * Hauteur d'eau
<span class="user-answer">
OUI, sa première métrique (indicateur perfo). La compare
</span>
  * Débit d'eau
<span class="user-answer">
N'intervient pas dessus (éventuellement en support avec Kévin)
</span>
  * Température
<span class="user-answer">
Non (pas en première intention, en cas de phénomènes inexpliqués)
</span>
  * Turbidité
<span class="user-answer">
Non (pas en première intention, en cas de phénomènes inexpliqués)
</span>
  * Autres?
<span class="user-answer">
en cas de phénomènes inexpliqués: carte de végétation, occupation du sol. MNT
</span>
* Quelles méthodes
  * d'exploitation
<span class="user-answer">
La plupart du temps fabrique un "pseudo produit" (pré CALVAL, produit en CALVAL), et la superpose à une donnée entrante: 
1. Premier niveau: comparaison visuelle: par exemple décalage de rivière par rapport à une référence externe.
2. Deuxième niveau: calcul d'indicateurs. Calcul d'étendue et comparaison avec la donnée d'entrée ou externe si CALVAL. Moyenne / écart-type hauteur sur une zone (par cours d'eau, par lac)
3. A] tout colle, chouette. B] retraiter / resimuler pour comprendre ce qu'il se passe (le phénomène apparaît à la simulation? Nouveau phénomène?)
Importance de la vérification à l'oeil: "En général ce qu'on voit à l'oeil se voit en auto aussi. Mais l'avantage c'est d'identifier les cas les plus problématiques (ex typique: grosse erreur de déroulement de phase => toute l'eau est décalée de 700m, superposition par rapport à la référence 0%, lien direct avec l'algorithme pour lui)"
</span>
  * de comparaison
<span class="user-answer">
A initié un petit projet Git SWOT-CALVAL:
* ex typique 1: niveau 1.5 ou 2 (pixel cloud), superposé avec surfwater, ouverture des deux fichiers superposés, pour premier aperçu. Puis calcul d'étendu commune entre masque de référence et produit SWOT.
* ex typique 2 (plutôt simu mais applicable SWOT): Hauteur de ref et Moyenne sur la donnée
</span>
  * d'extrapolation
<span class="user-answer">
* En cours d'étude pour le produit FloodPlain Dem (produit le plus compliqué de SWOT, tente de reconstituer la batimétrie).
Lignes de niveaux => batimétrie => 1er produit = points multitemporel => interpolation (premiere intention distribution Gaussienne, pas satisfaisante) ~ InverseDistanceWaiting idw.py. 
Probablement représenté dans la CALVAL pour comparer du pixel cloud
* Interpolation des RASTER pour les mettre à la même résolution
* Interpoler le pixel cloud sur une grille 
</span>
* Tâche métier actuellement bien outillée?
<span class="user-answer">
Oui je pense.
</span>
  * Totalement couverte?
<span class="user-answer">
Pas couvert: récupération de données externes (la galère!). Où est la BD tartempion, comment je récupère, comment modifier la donnée pour la faire correspondre à la mienne (pas son coeur de métier).
Récupérer rapidement toutes les tuiles intéressantes
</span>
* Quels points pénibles (outils / données / volumétrie / format / etc...)
<span class="user-answer">
* Aura besoin de données externes (moins efficace que d'autres la dessus, veut bien de l'aide?)
* Gros besoin mémoires / Temps / CPU, ce qui nécessite beaucoup de méthode ("simulation bien carrée")
* Projection (UTM -> lat lon, pénible même s'il est maintenant mieux formé et le fait via QGis / script directement) ~ un peu projectif
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
Travaille très souvent avec des scientifiques:
1. A
  * Récupérer des données d'entrées (multi temporelles réaliste, ex: masque d'eau sur 1an)
  * En retour, ils sont souvent intéressés par le produit SWOT corresopndant (boucle feedback)
2. B - expertise des scientifiques (on s'éloigne, dans FloodPlain Dem du Radar). Les hydrologues peuvent l'aider dans la sélection des méthodes / algorithmie (collaboration écrite / GitLab)
* Du code (Utilise souvent stackoverflow et similaires)
</span>
* Que souhaiteriez-vous apporter à la communauté?
<span class="user-answer">
Support aux produits SWOT et au simulateur, adaptation des produits (produit de haut niveau pas tout à fait figé au moment de la CALVAL), sélection des meilleurs produits / métriques. Support à des logiciels sans accès externe
</span>

## Ouverture

* Disponible peu (1/2 journée mois) pour participer à la conception
<span class="user-answer">
Oui pas de souci
</span>
* Qu'est ce qui vous ferait gagner du temps?
<span class="user-answer">
Voit pas trop
</span>
* POST: Quelles solutions dans un monde idéal?
<span class="user-answer">
QGis est l'outil le plus complet qu'il utilise actuellement. UN SUPER QGIS ADAPTE POUR LIRE LES PRODUITS SWOT et produits auxiliaires, calculerait des métriques.
</span>

<style>
.user-answer {
  color: darkcyan;  
}
</style>
