# Interviews Hysope II


* Présentation (nom métier, organisme, formation universitaire)
<span class="user-answer">
Cesbio: recherche avec tutelle (UPS, INRA, etc...)
early adopter
suivi de la végétation, étude de la biodiversité
fait partie du segment observation, pour alimenter le segment modélisation
Travaille sur les séries temporelles de données spatiales à haute-résolution
Ingé telecom
</span>
  * Plutôt opérationnel? Scientifique? Archi / bureau d'étude?
<span class="user-answer">
Scientifique
Volet OP (cartographie d'occupation des sols): fait tourner / développe / qualifie IOTA2
Produit des traitements à destination des opérationnels
</span>
* Quel tâche métier principale? 
<span class="user-answer">
développement, traitement 50%
encadrement de thésard, travail de labo 50%
</span>
  * Pour quel résultat?
<span class="user-answer">
Code dans un dépôt GIT: algorithmes
Quelques Go de donnée produite
</span>
  * Pour qui?
<span class="user-answer">
Ca dépend: 
1. datascience: code pour générer des résultats de publication (autre scientifique). Stat + donnée + algo => étude thématique
2. engineering: produire de la donnée et de la méthode pour d'autres utilisateurs
</span>
  * Comment?
<span class="user-answer">
1. notebook => analyse via code scripté (sans excell)  et commentaires. Python
2. IDE (EMACS). connait des gens qui utilisent JUPITER (C / C++ parfois, Python en général)
</span>
  * Etapes?
<span class="user-answer">
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
* EMacs (IDE)
* Environnement CONDA (Python)
* Git
* GitLab
* MatPlotLib (Python)
* Images: plutôt QGis
* Travaille avec HAL (datalake / espace projet). Pas de gestion de conf pour les données moins volumineuses. Cesbio a une BD GIS (ses collègues l'utilisent mais pas lui)
</span>
  * Quels points forts?
<span class="user-answer">
* "composabilité" (indépendant mais travaillent bien ensemble), peu contraignant
* Flexibilité / souplesse
* Polyvalence
</span>
  * Quels points d'amélioration?
<span class="user-answer">
* Learning curve (nécessairement, mais pas un vrai inconvénient)
* collaboration externe plus compliquée (se sont les habitudes de son équipe)
* obsolescence des libs / versions. 
  * Gestion des dépendances de Conda
  * Maintenabilité / obsolescence des libs choisies par ses utilisateurs
</span>
  * Quels points d'intégration?
<span class="user-answer">
peu, bien standardisé, bien géré par les libs
Stack "fragile" (pb de versions), demande du temps
</span>
* Quelles données? 
<span class="user-answer">
plutôt producteur, n'utilise pas ces variables
</span>
  * Neige (couverture / prduits dérivés)
<span class="user-answer">

</span>
  * SWE (volume eau / neige)
<span class="user-answer">

</span>
  * Surface d'eau (pixel eau)
<span class="user-answer">

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
produit occupation des sols
pourrait utiliser des humidités de surface
BD terrain ou mesure terrain (variable catégorielle / quantatif comme indice "foliaire", variables biophysiques => points ou polygones, shape / sqlite).
</span>
* Quelles méthodes
  * d'exploitation
<span class="user-answer">
* pour la production
</span>
  * de comparaison
<span class="user-answer">
* Calcul de métriques ponctuel: calcul d'erreur, pas de visu
* Code de comparaison, overall accuracy (CAPA)
peu de visualisation, juste pour la validation qualitative et l'illustration, "pattern bizarres"
</span>
  * d'extrapolation
<span class="user-answer">
* Extrapolation: Forecast d'analyse (algo spécifiques, expertise humaine)
* Interpolation: données à trous => paramétrage d'interpolation à faire à chaque fois (algos connus: **TODO obtenir la liste des algo et paramètres**) De base approche naïve: réplication de la dernière valeur connue
</span>
* Tâche métier actuellement bien outillée?
<span class="user-answer">
Oui
</span>
  * Totalement couverte?
<span class="user-answer">
Il y travaille
</span>
* Quels points pénibles (outils / données / volumétrie / format / etc...)
<span class="user-answer">
* gestion des dépendances (côté très dev)
* accès à distance peu performants (bastion / cluster GRRRRRR, trop complexe et lent)
* VRE n'est pas bien pour lui (voudrait travailler sur son poste, pas de mode minitel, ne déporter que ce qui est nécessaire. Ils ont bricolé des solutions)
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
* feedback et priorisation
Via Theia ils ont déjà un embryon de communauté -> contactés par email
Sur leurs outils, plus simple (contact direct)
</span>
* Que souhaiteriez-vous apporter à la communauté?
<span class="user-answer">
acteurs historiques Theia, n'est pas trop dans cette démarche
</span>

## Ouverture

* Disponible peu (1/2 journée mois) pour participer à la conception
<span class="user-answer">
Non pour lui, demande à ses collègues (early adopters???). **TODO: trouver des membres de son équipe pour la conception, @lionel**
</span>
* Qu'est ce qui vous ferait gagner du temps?
<span class="user-answer">
* Meilleur accès aux ressources
</span>
* POST: Quelles solutions dans un monde idéal?
<span class="user-answer">
Tout local, API déport de traitement
</span>


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


<style>
.user-answer {
  color: darkcyan;  
}
</style>
