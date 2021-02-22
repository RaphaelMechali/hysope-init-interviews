# Résumé des habitudes rencontrées

## Variables et visualisation

### Consommées

* MNT 4
* Définition des "shapes" d'entités 1
  * prior (déf à priori) 1
  * unassigned (déf "lac à sec") 1
* hauteur d'eau 7 
  * mesure par capteur de pression 1
* débit 4
* surface 7
* Volume / stockage 5
* température 2
* hygrométrie 1
* vent 1
* Neige 3
* SWE 2
* glace (et glaciers) 1
* météo actuelle 4
  * pluviométrie 4
  * température air 2
  * vent 1
* prévision météo 3
* rayonnement 1
* Humidité des sols 3
  * Par sonde capacitive 1
* Température eau 3
* Turbidité 4
* Occupation des sols 5
  * Radar (Sentinel) 2
* Pente terrain 1
* Résultats de recherches scientifiques externes 1

### Calculeés

* ETP 3
* Carte de seuil (paramétrée) 1
* Carte d'érosion 1
* Risque d'érosion 1
* Bilan hydrique 2
  * Cycle de l'eau 1

## Outils & méthodes

* Dispense formation / support 5
* In situ
  * Hydrométrie jauge 1
  * Bateaux drones 1
  * Théodolites 1
* Cartographie 6
  * ArcGis 1
  * QGis 6
  * Panoply 2
  * NCView 1
  * PostGIS 1
* Analyse mathématique 5
  * Courbe temporelle (suivi volumes, surface, débits, prélèvements, précipitations ETP, oxygènation, turbidité, hauteur + mesure) 4
  * Courbe Ipsométriques (surface x hauteur = signature lac = bathymétrie?) 3 **TODO @LZA: unifiable avec le point dessous? ~= bathymétrie**
  * Courbe multi-paramètres (corrélation météo x hydro x param trisométrique) 3
  * Multi graph 1
  * Comparaison à la moyenne / écart type 4
  * Interpolation / extrapolation polynomiale, constante optimiste, gaussienne etc... 2
    * MNT 1
    * temporelle (variable, nuage de points) 2
  * Estimation de marge d'erreur 2
  * Cartographiée 2
    * Pour corréler aval / amont (par indicateurs de propagation visuels: tronçons de rivières colorés) 1
    * Comparaison visuelle aux contours attendus 2
      * Par reconstitution de plusieurs images ou sources par entité (lac / rivières) 1
    * Comparaison automatisée aux contours attendus (image) 2
    * Pixel cloud x shapefile / Pixel cloud (analyse qualitative des surfaces) 3
  * Analyse coût / risque / bénéfice 1
  * Analyse statistique 1
    * Réseau de neurones 1
  * Simulation 2
    * SWOT-hydrology-toolbox 2
    * Jpl - RiverOps 2
* Analyse continue (seuils d'alertes) 2
* A essayé de remplacer des traitement QGis par photoshop 1
* Programmation 1
  * Python 4
    * Orphéo toolbox 1
    * S1Tiling 1
    * PyCharm 1
    * Spider 1
    * Anaconda /miniconda 2
  * R 1
    * Recalibrer les images satellitaires 1
    * RGRxx pour big data
  * VSCode 1
  * Test 1
    * Fonctionnels 1
    * Unitaires 1
  * Plugin confluence 1
  * Jupiter notebook 1
* Partage & comm 3
  * Git 2
  * GitLab 2
  * Confluence 1
  * skype 1
* Cloud 3
  * AWS 1
  * HPC HAL cluster CNES 4
* Modèles 3
  * SAFI (évolution biomasse, réserve hydrique) 1
  * (R)GRxx 2
  * SWAT 1
  * GFS (prévision météo)
  * De propagation (type non mentionné) 1
* Travaille par sous BV 1
* Outils internes 1
  * Qualification 1
  * Calibrage (interpolation, échantillonage, conversion...) 1
* Plateforme Web 5
  * Outil interne pour distribuer les données / le résultat 4
  * Theia 1
  * Corpernicus 2
  * Sci-Hub 3
  * Hubeau 1
  * Géoportail IGN 1
  * BD IRD 1
  * Service Sandre 1
  * Banque Hydro 1
  * CNES (Hydroweb OG, Peps, HPC, Theia...) 2
  * Earth data (NASA) 1
  * Google Earth Engine 4
  * CTOH 1
* Calcul, reporting et recherche 1
  * Word, PowerPoint 2
  * Excell 3
  * SearchEveryThing (compense l'absence de stockage correct des projets antérieurs) 1
* Veille techno 3
* Veille donnée 2

## Projets communs

* ACMG
  * R&D -> Agralis commercialise
  * ACMG <-> Aquafox <-> SigFox || GPRS
  * Projet clipalert > plateforme (niveau d'eau / prévision)

## Buts

* érosion des sols 1
* impact changement climatique 2
* lutte contre les impondérables: gelée, grêle, irrigation, crue, étiages, érosion 2
* distribution de la ressource (réserve, partage, ressources, retenues collinaires, soutien d'étiage, irrigation, changement de mode de culture) 3
* étude d'impact sur les milieux aquatiques (débit / qualité) 1
* navigation / voies navigables 1
* Algo SWOT 2
  * Générer de la donnée de simulation pour les algos (vérité terrain) 1
  * Implémenter des algo de production d'images de qualité satisfaisante 2
  * Comparer à l'existant (in situ) 1
  * Produire pour des résultats pour les scientifiques et les utilisateurs 1

## Points pénibles

* Préparation des données 1
* Satellitaire 3
  * Temps de téléchargement / récupération / traitement 3
  * Puissance / espace requis 3
  * Inconstance du type de mesure 1
  * Conversion SAT (S1Tiling) 1
  * Fréquences trop basse 1
  * Ressources matérielles requises 6
    * NetCDF trop lourd en manip 1
  * Lenteur de mise à disposition des données sur bandes 1
* Données payantes (produits spécifiques ou in situ) 2
* Cartographie 3
  * Manque d'homogénéité / continuité / uniformité (WMS, Cartage...) 4
  * Manque de centralisation des sources 1
* Mise en place 1
  * Lâchers hydro-électriques perturbants 1
* VRE / cluster: lourde / lente / surcouche de complexité inutile 2
  * Plus nuancé: pb réseau d'accès HPC / HAL / VRE 2
* Analyse stat. automatique filtre les évènements extrêmes réels 2
* Estimer la marge d'erreur 2
* Visualisation historique complexe 1
* Pression des projets (temps / budget) 2
* Mise à jour des outils JPL trop fréquentes 1

## Crainte

* Monétisation des services hydro 2
* Les fichiers non copiables (PDF, manuscrits) 1
* Âpre concurrence, intérêts divergents 1
* Rédiger des documents 1

## Appartenance communautaire

* Business 2
  * SigFox 1
  * Agralis 1
  * Agri sud-ouest 1
  * DREAL 1 
  * CACG 1
  * EPTB, ministères, agences, syndicats 5
  * Banques mondiales 1
  * CNES 4
  * Segment sol 1
* Communauté globale 1
  * Scientifique (CNES / JPL / Universités) 4
* Groupes de travail 3

## Vision communautaire

* Méthodes 1
  * Accès à de la R&D institutionnelle 2
* Ressources
  * Partager de la donnée in situ 1
  * Partager des outils / traitements / chaînes / méthodes 3
    * Altimétrie 1
  * Partager le besoin "terrain" 2
  * Mettre en place des traitements pour les autres 1
  * Consommer de la donnée 4
  * Consommer des outils / traitements / chaînes / méthodes 3
  * Consommer des ressources matérielles (CPU, disk, RAM...) 1
  * Vendre des traitements / chaînes 1
  * Emergences de contrats / partenariats de projet 1
* Discussion 3
  * Entre organismes (dont besoins ETPB, méthodes...) 3
  * Entre communautés scientifiques / nationales 1
  * Réception de feedback des consommateurs 2
* Diminution des coûts 1


## Attentes

* Des données SWOT continues (par d'arrêt à 3 ans) 1
* Des données de haute qualité (à terme) 1
* Des données de qualité moyenne rapidement, puis des données qualitatives plus tard (fast mapping) 1
* API de déport calcul (travailler chez soi, aussi vite que sur le cluster) 2
* Un super QGis adapté à la lecture des produits SWOT auxiliaires (+ calcul auto des métriques) 1
* Outils de visualisation graphique bien faits sur portail (drop excell) 1
* Prévisualisation bien faite sur portail (drop download -> QGis) 1
* Accès rapide aux données historiques (sur bande magnétique) 1
* Libre accès aux données COSMOS SKYMED 1
* Avoir du 3m en bande X (nota: bande permettant une meilleure classification) 1
* Satellite geostationnaire avec pixel à moins de 10m (petits lacs / petites rivières) 1
* Flotte de satellites qui se relaient pour suivre les évènement d'inondation 1
* Des projets "pérennisés" (manque de suivi de long terme) 1
* Mise à disposition d'un scribe 1
* Rapidité d'application des prétraitements et traitements de visu et graphiques (autant calibration qu'exploitation) 1
* afficher la taille dispo des volumes (voir STYX / HYMOTEP) 1



**A creuser: qu'est ce qu'un SIE? (Alain Gauthier) Quelle matérialisation physique? Quel contrainte en hydrologie**
*Réponse partielle: API online, certainement SANDRE, pour l'évaluation de l'état hydro (API de bilans hydro en lignes)*

**A creuser: quels modèles de propagation? (Alain Gauthier)**

