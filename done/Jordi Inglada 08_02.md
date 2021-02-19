# Interviews Hysope II


* Présentation (nom métier, organisme, formation universitaire)
<font color="darkcyan">
Cesbio: recherche avec tutelle (UPS, INRA, etc...)
early adopter
suivi de la végétation, étude de la biodiversité
fait partie du segment observation, pour alimenter le segment modélisation
Travaille sur les séries temporelles de données spatiales à haute-résolution
Ingé telecom
</font>
  * Plutôt opérationnel? Scientifique? Archi / bureau d'étude?
<font color="darkcyan">
Scientifique
Volet OP (cartographie d'occupation des sols): fait tourner / développe / qualifie IOTA2
Produit des traitements à destination des opérationnels
</font>
* Quel tâche métier principale? 
<font color="darkcyan">
développement, traitement 50%
encadrement de thésard, travail de labo 50%
</font>
  * Pour quel résultat?
<font color="darkcyan">
Code dans un dépôt GIT: algorithmes
Quelques Go de donnée produite
</font>
  * Pour qui?
<font color="darkcyan">
Ca dépend: 
1. datascience: code pour générer des résultats de publication (autre scientifique). Stat + donnée + algo => étude thématique
2. engineering: produire de la donnée et de la méthode pour d'autres utilisateurs
</font>
  * Comment?
<font color="darkcyan">
1. notebook => analyse via code scripté (sans excell)  et commentaires. Python
2. IDE (EMACS). connait des gens qui utilisent JUPITER (C / C++ parfois, Python en général)
</font>
  * Etapes?
<font color="darkcyan">
1. datascience
  1. collecte des données (images, mesures terrains, etc...)
  1. exploration en code (lignes de commande => stats)
  1. outils plus spécifiques pour de la représentation adaptée (données tabulées)
  1. tracer de courbes
  1. conclusion. Document(s) de quelques pages généré par les scripts. Sortie Latex / PDF
1. engineering: [pré] idée précise de ce que l'on souhaite produire
  1. Découpe en tâche
  1. Mise en place Forge
  1. Réparti les tâche, code, test intégration et regression, commit en GIT (GitFlow)
  1. L'algorithme / la chaîne est intégré 
    * A| dans leur soft 
    * OU B| par l'équipe de production du CNES - Théia (ou autre collaborateur)
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
* EMacs (IDE)
* Environnement CONDA (Python)
* Git
* GitLab
* MatPlotLib (Python)
* Images: plutôt QGis
* Travaille avec HAL (datalake / espace projet). Pas de gestion de conf pour les données moins volumineuses. Cesbio a une BD GIS (ses collègues l'utilisent mais pas lui)
</font>
  * Quels points forts?
<font color="darkcyan">
* "composabilité" (indépendant mais travaillent bien ensemble), peu contraignant
* Flexibilité / souplesse
* Polyvalence
</font>
  * Quels points d'amélioration?
<font color="darkcyan">
* Learning curve (nécessairement, mais pas un vrai inconvénient)
* collaboration externe plus compliquée (se sont les habitudes de son équipe)
* obsolescence des libs / versions. 
  * Gestion des dépendances de Conda
  * Maintenabilité / obsolescence des libs choisies par ses utilisateurs
</font>
  * Quels points d'intégration?
<font color="darkcyan">
peu, bien standardisé, bien géré par les libs
Stack "fragile" (pb de versions), demande du temps
</font>
* Quelles données? 
<font color="darkcyan">
plutôt producteur, n'utilise pas ces variables
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
produit occupation des sols
pourrait utiliser des humidités de surface
BD terrain ou mesure terrain (variable catégorielle / quantatif comme indice "foliaire", variables biophysiques => points ou polygones, shape / sqlite).
</font>
* Quelles méthodes
  * d'exploitation
<font color="darkcyan">
* pour la production
</font>
  * de comparaison
<font color="darkcyan">
* Calcul de métriques ponctuel: calcul d'erreur, pas de visu
* Code de comparaison, overall accuracy (CAPA)
peu de visualisation, juste pour la validation qualitative et l'illustration, "pattern bizarres"
</font>
  * d'extrapolation
<font color="darkcyan">
* Extrapolation: Forecast d'analyse (algo spécifiques, expertise humaine)
* Interpolation: données à trous => paramétrage d'interpolation à faire à chaque fois (algos connus: **TODO obtenir la liste des algo et paramètres**) De base approche naïve: réplication de la dernière valeur connue
</font>
* Tâche métier actuellement bien outillée?
<font color="darkcyan">
Oui
</font>
  * Totalement couverte?
<font color="darkcyan">
Il y travaille
</font>
* Quels points pénibles (outils / données / volumétrie / format / etc...)
<font color="darkcyan">
* gestion des dépendances (côté très dev)
* accès à distance peu performants (bastion / cluster GRRRRRR, trop complexe et lent)
* VRE n'est pas bien pour lui (voudrait travailler sur son poste, pas de mode minitel, ne déporter que ce qui est nécessaire. Ils ont bricolé des solutions)
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
* feedback et priorisation
Via Theia ils ont déjà un embryon de communauté -> contactés par email
Sur leurs outils, plus simple (contact direct)
</font>
* Que souhaiteriez-vous apporter à la communauté?
<font color="darkcyan">
acteurs historiques Theia, n'est pas trop dans cette démarche
</font>

## Ouverture

* Disponible peu (1/2 journée mois) pour participer à la conception
<font color="darkcyan">
Non pour lui, demande à ses collègues (early adopters???). **TODO: trouver des membres de son équipe pour la conception, @lionel**
</font>
* Qu'est ce qui vous ferait gagner du temps?
<font color="darkcyan">
* Meilleur accès aux ressources
</font>
* POST: Quelles solutions dans un monde idéal?
<font color="darkcyan">
Tout local, API déport de traitement
</font>


## Note: Solution élaborée avec Jordi (par Lionel)
Issu de mes échanges par mail avec Jordi pour archive dans l'entretien. Voici une maquette des API pythons qu'il voudrait : 

Import hysope2 as h2

### Je donne mes informations de connexion ou une page web s’ouvre comme pour google…
h2.connect(params_hal)

### Je cherche une serie de produits MAJA sur ma Region Of Interest (ROI)
search_results = h2.search(‘MAJA’, roi=(lonmin, latmin, lonmax, latmax), time=datetime(2020,12,8,14,56))

### Je prepare le datacube correspondant (il reste hébergé sur le HPC et je ne le load pas dans ma RAM, c’est juste une instance)
my_h2_datacube = search_results.prepare_datacube()

### J’applique une fonction à moi au datacube (ça tourne toujours sur HAL en distant)
my_h2_output = my_h2_datacube.apply(function_quelconque, params_function)

### Je récupère le résultat en local
my_h2_output.load()
