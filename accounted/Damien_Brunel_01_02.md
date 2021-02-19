# Interviews Hysope II

## Volet général

* Présentation (nom métier, organisme, formation universitaire)
<font color="darkcyan">
Hydrologue (école de Grenoble) => a fait carrière chez BRL (Maroc, Congo, vit actuellement en France) un peu de R&D (spatial, métrologie ~= l'hydrométrie)
</font>
  * Plutôt opérationnel? Scientifique? Archi / bureau d'étude?
  Bureau d'étude (stratégie échelle région / groupe de pays, et opération d'installation de station) et opérationnel
<font color="darkcyan">
</font>
* Quel tâche métier principale? 
<font color="darkcyan">
Crues et alertes de crues
Gestion de ressources
L'irrigation
</font>
  * Pour quel résultat?
<font color="darkcyan">
Système d'alerte, outillage de bassin versants, études de dimenssionnement amont, ça dépend des projets. Même plateformes informatiques (customisation Wimes)
</font>
  * Pour qui?
<font color="darkcyan">
Acteurs étatiques (Congo: direction Meteo, en France similaire, ministères et collectivités locales)
</font>
  * Comment?
<font color="darkcyan">
Diagnostique préalable > propositions (le détail dépend). On utilise souvent de la modélisation.
Anedocte => a numérisé des données de 1930 ("boule cristal)
Utilise de la donnée in situ et complète avec du spatial. Ou spatial pur si aucun in situ, mais rétiscences, mais la pluie c'est pas foufou > collègues développent des algo en R pour recalibrer les images (demande et consommes ces algorithmes)
</font>
  * Etapes?
<font color="darkcyan">
* Diagnotisque
  * recueil d'un maximum de données (et critiquer ==> jauge de fiabilité). Ont des outils pour évaluer la données
  * décide des jeux de données retenus
  * extrapoler et spatialiser (appui dur le bassin versant)
  * recherche d'études existantes sur le BV
* Préconisations (ici cru)
  * développement de modèles (modèles pluie+(évaporation||débit)+param physiques, calibré avec les observations in situ, pour compenser l'absence de mesure de débit --> extrapoler le débit)
  * statistiques (pluie ou débit pour déterminer les plus gros évènements possibles -> aménagement / coût-bénéfice / répartition des ressources)
  * considération de délai
  * développement de système d'alertes 
  Les données sont souvent très extrapolées (durant les évènements crues / étiage les données sont moins fiables). 
  Tâche: Regarder les niveaux acceptables de prélèvements d'eau (barrage), changement de mode de culture, assainissement de l'eau, etc...
</font>
* Quelles tâches métiers secondaire? (sous-tâches ou tâches parallèles?)
<font color="darkcyan">
* gestion de projet
* relation clients / partenaires
* R&D spatiale / métrologie (station low cost de mesure in situ)
* Veille sur les données dispo à fournir à leur système (ils sont notamment SWOT early adopters)
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
* Excell + macro => modèles de gestion de barrage
* R (algo)
  * Diagramme sur les données in situ (vision d'ensemble et automatisation)
  * Spatial un peu
  * Modèle GR (2m,4j,3j,D) / RGR (2m,4j,3j, D) si beaucoup de choses à faire
* APIs (Wimes <-> leur plateforme)
  * Recueillir des données in situ et spatial
  * Réaliser des traitements et appliquer des modèles (hydrologiques, pluie sur BV)
  * Carte par seuil
* SIG (Arcgis pre / post traitement), visu dans leur outil Wimes
* Utilise un peu google earth
</font>
  * Quels points forts?
<font color="darkcyan">
* Outil intégrateur: donnée -> traitement -> alertes
  * Ingère de la donnée
  * Lance des modèles
  * Gère bien les séries temporelles
* Permet une interface dédiée au projet (indicateurs simples et visuels)
* Aime Excell pour trifouiller et R pour jouer avec: on en fait ce qu'on en veut
</font>
  * Quels points d'amélioration?
<font color="darkcyan">
* Donnée d'entrée à améliorer: données payantes, manque de données
prétraitrement: combler les trous de données (homogénéiser, rendre continue)
postraitement: quantil de pluie, 
</font>
  * Quels points d'intégration?
<font color="darkcyan">
recueil données et métier client
</font>
* Quelles données? 
<font color="darkcyan">

</font>
  * Neige (couverture / produits dérivés)
<font color="darkcyan">
Oui (pour le modèle GRXX). Sur certains bassin c'est un critère prépondérant (Alpes/Amazonie)
</font>
  * SWE (volume eau / neige)
<font color="darkcyan">
Oui
</font>
  * Surface d'eau (pixel eau)
<font color="darkcyan">
Oui (utilisé récemment pour la CEAC - 11 pays d'Afrique)
</font>
  * Hauteur d'eau
<font color="darkcyan">
Oui (altimétrie spatial, ils sont moteurs dessus) --> c'est l'entrée de base en hydrologie, pour déduire, avec la pluie, le débit. Sert également à la navigation (a été utilisé pour le fleuve Congo notamment, basé sur Hydroweb puis sur une BD IRD)
</font>
  * Débit d'eau
<font color="darkcyan">
Oui (donnée la plus compliqué, demande des courbes de tarage)
</font>
  * Température
<font color="darkcyan">
Peu. Lié à ses projets
</font>
  * Turbidité
<font color="darkcyan">
Pas. Lié à ses projets. Si l'eau n'est pas turbide, on peut faire du LIDAR aérien (ce qui permet de faire la batimétrie), sinon on est obligé de recourir à un bateau
</font>
  * Autres?
<font color="darkcyan">
* température sol / air
* pluie
* pluie prévue (prévisions européennes payantes pour les privés, remplacent par le GFS)
* occupation du sol
* humidité des sols
* MNT (fondamental): SRTM (30m), HALOS (plus précis mais à trou), Hydroshed (30m) <=== gratuits
  * Idéal: MNT payants type Copernicus (regrets liés à leur accès), plus fin que le 30m
---> Ils retopographient quand ils ont besoin
---> Calent le modèles la où ils ont l'information, puis "régionalisent" le modèle. Utilisent parfois des réseau de neurones dans ce procédé
Il veut bien des données approximatives rapidement puis des données qualitatives plus tard
</font>
* Quelles méthodes
  * d'exploitation
<font color="darkcyan">
*
* 
</font>
  * de comparaison
<font color="darkcyan">

</font>
  * d'extrapolation
<font color="darkcyan">

</font>
* Tâche métier actuellement bien outillée?
<font color="darkcyan">
* Oui parce qu'on palie les manques (lié à un effort sur leur outil interne)
</font>
  * Totalement couverte?
<font color="darkcyan">
* Non parce que R&D et veille
</font>
* Quels points pénibles (outils / données / volumétrie / format / etc...)
<font color="darkcyan">
* Pérénité (projet fini, suite peu péreine)
* Pression des projets (contrainte délai / budget)
* Plus compliqué pour les privés, facilité pour les institutionnels
* Limite en capacités de calculs, regardent pour le cloud, limite en place sur les postes
</font>
* Illustrer tâche métier durant l'interview? (si moins de 20 minutes)
<font color="darkcyan">

</font>

## Volet intégration HI2

* Etes vous familiers avec les services Theia?
<font color="darkcyan">
Oui, peu maîtrisé
</font>
* Utilisez-vous des données Theia régulièrement?
<font color="darkcyan">
Non. Eventuellement altimétrie spatiale (un collègue peut éventuellement, GFS très utilisé). Demander à Stéphane.
</font>
* Accédez-vous régulièrement à des produits CNES (peps / cdpp / hydroweb / theia similaires...)
<font color="darkcyan">
non
</font>

## Communauté

* Que pourrait vous apporter la communauté?
<font color="darkcyan">
Existe déjà (groupe) en altimétrie spatiale
"Les réseaux font partie de notre métier". Toujours intéressant
* nous permet de nous tenir informer 
* débouche sur des partenariats
* fait émerger des projets
</font>
* Que souhaiteriez-vous apporter à la communauté?
<font color="darkcyan">
* Moteur sur l'altimétrie spatiale
* Contact terrain, "vrai besoins", réalité terrain pour le spatial ==> contribution à l'amélioration des chroniques d'altimétrie
</font>

## Ouverture

* Disponible peu (1/2 journée mois) pour participer à la conception
<font color="darkcyan">
Délicat de répondre => choix de sa direction.
</font>
* Qu'est ce qui vous ferait gagner du temps?
<font color="darkcyan">
* Futurs produits SWOT >> du SWOT en continu (ils ne peuvent pas développer dessus à cause de l'arrêt à 3 ans)
* Données d'entrée de haute qualité (pluie / pluie prévue / MNT)
</font>
* POST: Quelles solutions dans un monde idéal?
<font color="darkcyan">
 --> Positionne des stations (via google earth engine). Se méfie de la carotte gratuit puis payant
 --> Déport de calcul dans le cloud (contrainte forte pour eux, fonction des sujets, mais dimensionnant pour l'alerte de crue)
</font>


