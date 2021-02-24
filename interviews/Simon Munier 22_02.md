# Interviews Hysope II

## Volet général

* Présentation (nom métier, organisme, formation universitaire)
<span class="user-answer">
Formation ingé ENSEEIHT, thèse INRAE à Mtp sur couplage hydraulique hydrologique (écoulements rvières)
Postdocs pendant 8 ans sur le spatial sur la thématique de l'hydrologie grande échelle avec GRACE, altimétrie, SAR Sentinel-1 
Depuis 3-4 ans : chargé de recherche au CNRM sur modélisation de tout le cycle hydrologique, impliqué dans SWOT, WISA, SMASH : assimilation de données spatiales, porter le besoin météo.
Lacs avec Patrick Lemoigne, Simon sur fleuves
</span>
  * Plutôt opérationnel? Scientifique? Archi / bureau d'étude?
<span class="user-answer">
Scientifique Chercheur mais opérationnel sous-tend le contexte général
</span>
* Quel tâche métier principale? 
<span class="user-answer">
Recherche : dévelopemment de modèles hydrauliques/hydrologiques.
Plus porté sur hydraulique mais hydrologique
</span>
  * Pour quel résultat?
<span class="user-answer">
Développer des modèles les plus réalistes possibles, prenant en compte le plus de processus possibles pour mieux comprendre la dynamique dyu cycle de l'eau dans le passé et le futur
Travail à échelle globale, grands bassins versants (10aine km, journalier)
Activités plus sur la France métropolitaine, petits bassins versants Français : km, h. Ne va pas jusqu'à la prévision de crues éclair

</span>
  * Pour qui?
<span class="user-answer">
Echelle globale, Pour la science, 
Echelle Française, pour les gestionnaires de l'eau (DREAL, DRIEE, agences de l'eau pour gestion ressource sur saison)
</span>
  * Comment?
<span class="user-answer">
Processus de long-terme. Amélioration de la partie routage (rivières et eaux souterraines et interaction) avec TRIP ou C-TRIP.
C-TRIP utilisé pour simus GIEC, amélioration de la résolution (1/12° global)
Contraintes portées par l'approche orientée passage à l'échelle globale pour des simus. Prototype le modèle sur des bassins tests mais la finalité n'est pas dd'avoir un modèle spécifiquement calibré pour le bassin local. L'idée est de pouvoir généraliser l'approche automatiquement sur d'autres bassins pour faire à terme du global.

			 

</span>
  * Etapes?
<span class="user-answer">
    * Partir d'un réseau MNT corrigé pour l'hydro, choix sur base de la littérature avec MERIT-Hydro
		  * Dév d'algos pour upscaler de 90m à 1/12° sur réseau hydro MERIT-DEM, MERIT-Hydro
		  * Ajout d'autres composantes sur eaux souterraines avec des BDD globales sur composition des sols, …etc. Recherche biblio pour trade-off hydro-géo
		  * Ajout modélisation barrages réservoirs en cours : 
		  	 * Choix d'un bassin test (territoire espagnol car Espagne a mis à disposition une grosse BDD pour arriver à comprendre le fonctionnement des barrages)
		  	 * Analyse de la donnée dispo 
		  	 * Téléchargement de la donnée dispo
		  	 * Croiser les différentes BDD pour catégoriser les différents barrages (hydro-elec, soutien étiage…)
		  	 * Pre-processing de la donnée (e.g. GRDC et bases nationales) : conversion dans un format homogène (globalement netcdf, parfois format binaire)
		  	 * Biblio pour regarder les modèles existants pour la gesiton des barrages car pas possible de calibrer pour passage en global
		  	 * Confronte approche à bassin test : analyse de sensibilité des paramètres avec modèle pour voir les valeurs typiques
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
	 * Programmation en Fortran pour les codes de simulation pour gérer les ressources de calcul
	 * Pre-processing, Post-processing en python (carte, plots…etc)
	 * Git pour des projets et dev de modules python 
	 * Ponctuellement des outils de SIG : GRASS et QGIS pour de la visu rapide (e.g. réseau rivières)
	 * IDE : éditeurs de code simples kate, vim et une console ouverte (PC perso pour post-proc)
calculateur météo-France pour les simus
</span>
  * Quels points forts?
<span class="user-answer">
Performance (temps d'exec et gestion de la donnée, mémoire, r/w sur ces grosses simus)
</span>
  * Quels points d'amélioration?
<span class="user-answer">
Du mal à faire du partage de code en interne/externe. Mal à faire converger les gens sur une façon de coder, de partager de la donnée.		
Sur la donnée : gros travail d'uniformisation dans les formats, les dépôts, les façons de récupérer la donnée. 
Savoir au moins que la donnée existe avec le lien vers le site distributeur si pas possible de la centraliser
</span>
  * Quels points d'intégration?
<span class="user-answer">

</span>
* Quelles données? 
<span class="user-answer">

</span>
  * Neige (couverture / prduits dérivés)
<span class="user-answer">
Non mais des collègues CNRM oui pour la couverture en eau

</span>
  * SWE (volume eau / neige)
<span class="user-answer">
SWE ils préfèrent recalculer eux-même depuis épaisseur/densité pour avoir un modèle mathématique cohérent avec les forçages et le modèle hydro
</span>
  * Surface d'eau (pixel eau)
<span class="user-answer">
Plutôt largeur de rivière (pour l'instant plus ou moins fixes dans modèle)
e.g. GRAWL largeurs moyenne issues de landsat autour du débit moyen
		
Mais aussi détection d'eau et bathy/hypso
</span>
  * Hauteur d'eau
<span class="user-answer">
Oui!
</span>
  * Débit d'eau
<span class="user-answer">
Oui!
</span>
  * Température
<span class="user-answer">
Oui va commencer
</span>
  * Turbidité
<span class="user-answer">
Non
</span>
  * Autres?
<span class="user-answer">
Réseau hydro (HYDROSHED historiquement, MERIT bien amélioré et la ref aujourd'hui) : faire un fond de carte de rivière adapté au zoom et cohérent avec MERIT-DEM, MERIT-Hydro même juste pour un fond de carte
</span>
* Quelles méthodes
  * d'exploitation
<span class="user-answer">
pas abordé
</span>
  * de comparaison
<span class="user-answer">
pas abordé
</span>
  * d'extrapolation
<span class="user-answer">
pas abordé
</span>
* Tâche métier actuellement bien outillée?
<span class="user-answer">
oui
</span>
  * Totalement couverte?
<span class="user-answer">
Non : problématique de gestion des formats, des BDD
</span>
* Quels points pénibles (outils / données / volumétrie / format / etc...)
<span class="user-answer">
Eparpillement, diversité des formats
Volumétrie : mix entre données distantes et données internes volumineuses
</span>
* Illustrer tâche métier durant l'interview? (si moins de 20 minutes)
<span class="user-answer">

</span>

## Volet intégration HI2

* Etes vous familiers avec les services Theia?
<span class="user-answer">
pas abordé
</span>
* Utilisez-vous des données Theia régulièrement?
<span class="user-answer">
pas abordé
</span>
* Accédez-vous régulièrement à des produits CNES (peps / cdpp / hydroweb / theia similaires...)
<span class="user-answer">
pas abordé
</span>

## Communauté

* Que pourrait vous apporter la communauté?
<span class="user-answer">
Partage de code, données post-traitées 
Wiki/forum/git avec un certain nombre de modules bien compartimentés
</span>
* Que souhaiteriez-vous apporter à la communauté?
<span class="user-answer">
Partage de code, données post-traitées 
</span>

## Ouverture

* Disponible peu (1/2 journée mois) pour participer à la conception
<span class="user-answer">
Oui (suivant les mois)
</span>
* Qu'est ce qui vous ferait gagner du temps?
<span class="user-answer">
  * Tout le monde sur le même serveur: architecture informatique pour éviter les transferts
	 * ou plus simplement un serveur distant pour pré-traiter des données et rassembler des données ne pouvoir télécharger que le minimum avec une interface de visualisation
</span>
* POST: Quelles solutions dans un monde idéal?
<span class="user-answer">

</span>


<style>
.user-answer {
  color: darkcyan;  
}
</style>
