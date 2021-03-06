# Résumé des habitudes rencontrées

Fichier source, utilisé pour extraire les autres fichiers du dossier (à consulter de préférence)

## Variables et visualisation

### Consommées

* MNT 8
* Définition des "shapes" d'entités 1
  * prior (déf à priori) 1
  * unassigned (déf "lac à sec") 1
* hauteur d'eau 14
  * mesure par capteur de pression 1
* débit 9
* surface 16
  * largeur rivière (GRAWL) 1
* réflectance 1
* Aérosol atmosphériques 2
* Volume / stockage 7
* température 5
* hygrométrie 1
* Neige 10
* SWE 6
* glace (et glaciers) 2
* météo actuelle 8
  * pluviométrie 8
  * température air 5
  * Humidité 1
  * vent 4
  * Direction du vent 1
* prévision météo 6
* rayonnement 3
* Humidité des sols 6
  * Par sonde capacitive 1
  * Humidité de surface 2
* Température eau 8
* Turbidité 8
* Mesure de Chlorophyle 1
* Occupation des sols 10
  * Radar (Sentinel) 4
  * Aménagement des berges (urbain/ végétation / habitations) 1
  * Indice foliaire 2
  * Variable catégorielle 2
  * Composition 1
* Pente terrain 1
* Résultats de recherches scientifiques externes 1
* Largeur maxi / min des micro BV 1
* "Profondeur" (fond -> berge) 1
* Analyse chimique 2
  * conductivité 1
  * PH 1
* Rapports / études à proximités du BV (qualité, biodiversité, etc...) 1
* lames d'eau 1
* masques 
  * eau 2
  * neige 1
  * nuages 2
    * nébulosité 1

### Calculeés

* ETP 4
* Carte de seuil (paramétrée, eau, climat etc...) 2
* Carte d'érosion 2
* Risque d'érosion 2
* Îlots de chaleurs 1
* Bilan hydrique 4
  * Cycle de l'eau 2
* Visualisation "grand-publique" (vulgarisation) ~ échelles non linéaires et similaires 1
* Trombinoscope cartographié 1
* Affichage du bâti 1
* Risque d'inondation 1
* eutrophisation (transport sédiments) 1

## Outils & méthodes

* Dispense formation / support 9es
* In situ
  * Hydrométrie jauge 2
  * Bateaux drones 2
  * Théodolites 1
  * Drone 1
* Cartographie
  * ArcGis 2
  * QGis 12
  * GRASS 2e
  * Panoply 2
  * NCView 1
  * PostGIS 2
  * Skyline 1
  * cognition 1
  * RDAS 1
  * rapide cartographie
* Analyse mathématique
  * Courbe temporelle (suivi volumes, surface, débits, prélèvements, précipitations ETP, oxygènation, turbidité, hauteur + mesure, comparaison source / produit ~ hauteur par exemple) 10
  * Courbe Ipsométriques (surface x hauteur = signature lac = bathymétrie?) 3 **TODO @LZA: unifiable avec le point dessous? ~= bathymétrie**
  * Courbe multi-paramètres (corrélation météo x hydro x param trisométrique) 3
  * Position fauchée x Erreur de surface || taille du lac (Y) OU Hauteur / diff hauteur (erreur) 1
  * Multi graph 1
  * Comparaison à la moyenne / écart type 4
  * Interpolation / extrapolation polynomiale, constante optimiste, gaussienne etc... 4
    * MNT 1
    * temporelle (variable, nuage de points) 3
  * Estimation de marge d'erreur 6
    * Par rapport à une autre entrée / modèle / approche 2
    * Route Min Square Error (erreur quadra), MAE (Min Absolute Error) ou MAD 1
    * écart-type ciblé (1 sigma) 1
  * Cartographiée
    * Mesure indicateur par pixel 2
    * Pour corréler aval / amont (par indicateurs de propagation visuels: tronçons de rivières colorés) 1
    * Analyse d'impact statistique cartographiées (zones et seuils) 2
    * Comparaison visuelle aux contours attendus 3
      * Par reconstitution de plusieurs images ou sources par entité (lac / rivières) 2
    * Comparaison automatisée aux contours attendus (image) 2
    * Pixel cloud x shapefile / Pixel cloud (analyse qualitative des surfaces) 4
    * "Polygonisation" (raster -> shape) 2
    * Visu MERIT (pour homogénéisation de la termino / du référentiel) 1
  * Analyse coût / risque / bénéfice 2
  * Analyse statistique 3
    * Regression statistique  2
    * Réseau de neurones / deepLearning / Machine Learning 4
  * Simulation 5
    * SWOT-hydrology-toolbox 3
    * Jpl - RiverOps 3
    * Autres 1
    * GIEC - Climatique 1
* Analyse continue (seuils d'alertes) 3
* A essayé de remplacer des traitement QGis par photoshop 1
* Programmation
  * Bash 1
  * Fortran 2
  * Python 11
    * Orphéo toolbox 2
    * S1Tiling 1
    * Spider 1
    * Anaconda / Conda / Miniconda 4
    * Carto 2
    * Plotly 1
  * R 3
    * Recalibrer les images satellitaires 1
    * RGRxx / AIGR pour big data 2
  * C/C++ 2
  * Java 1
  * Mathlab 3
  * Snap 3
  * IDE / environnement
    * Jupiter notebook 5
    * VSCode 2
    * PyCharm 1
    * Simples (EMACS/ kates / vim) 2
  * Test 1
    * Fonctionnels 1
    * Unitaires 1
  * Plugin confluence 1
  * Docker
* Outils / IHM
  * LYXEA 1
  * Envi (traitement, deep learning, remplace du code) 2
  * Snap 1
  * OTB 2
  * Moteverdi (IHM OTB) 1
  * DiapOTB (Radar, OTB) 1
* Cloud 10
  * Serveur interne 3
  * OVH / orange 1
  * AWS (et amazon bucket) 3
  * HPC HAL cluster CNES 9
  * Cluster de simulation Météo France 1
* Modèles 4
  * SAFI (évolution biomasse, réserve hydrique) 1
  * (R)GRxx 2
  * SWAT 2
  * GFS (prévision météo) 1
  * De propagation (type non mentionné) 1
  * SNOW Model 1
* Travaille par sous BV 1
* Outils internes 2
  * Qualification 2
  * Calibrage (interpolation, échantillonage, conversion...) 3
* Plateforme Web
  * Outil interne pour distribuer les données / le résultat 8
  * Theia 5
    * Venµs 1
    * Sentinel 2A S3A 1
    * dinamis 1
  * Corpernicus 4
  * Sci-Hub 6
  * Peps 4
  * Pleïades (CNES ou GeoStore Airbus) 2
  * Hubeau 2
    * NAIADE 1
  * Géoportail IGN 3
  * OFB 1
  * BD IRD 2
  * Service Sandre 1
  * Banque Hydro / BD Carthage 2
  * CNES (Hydroweb OG, Peps, HPC, Theia...) 2
  * Landsat (usgs earth explorer) 4
  * Earth data (NASA) 1
  * oceanwf - océanographie (NASA) 1
  * nsidc - glace / neige (NASA) 1
  * Reverb (NASA  )
  * Google Earth Engine 7
  * Google Earth  1
  * CTOH 1
  * OpenStreetMap 1
  * LandCover 2
  * Sentinel Hub 1
  * IDGeo 1
  * data.gouv.fr (données cadastrales) 1
  * GeoRezo **TODO: a creuser pour la comm**
  * Modis 1
  * MERIT Hydro (Merit DEM, algo, Open Street Map)
* Calcul, reporting et recherche 7
  * Word, PowerPoint 5
  * Excell 6
  * SearchEveryThing (compense l'absence de stockage correct des projets antérieurs) 1
  * Latex 3
  * Overleaf 1
  * PDF 1
* Collaboration & communication 4
  * Git 7
  * GitLab 6
  * Confluence 2
  * skype 1
  * Facebook 2
  * Twitter 2
  * Linked 1
  * Mails 2
* Veille techno 3
* Veille donnée 2

## Projets communs

* ACMG
  * R&D -> Agralis commercialise
  * ACMG <-> Aquafox <-> SigFox || GPRS
  * Projet clipalert > plateforme (niveau d'eau / prévision)

## Buts

* érosion des sols 2
* impact changement climatique / activités humaines 6
* lutte contre les impondérables: gelée, grêle, irrigation, crue, étiages, érosion 2
* distribution de la ressource (réserve, partage, ressources, retenues collinaires, soutien d'étiage, irrigation, changement de mode de culture) 3
* étude d'impact sur les milieux aquatiques (débit / qualité) 3
* navigation / voies navigables 1
* Algo SWOT 2
  * Générer de la donnée de simulation pour les algos (vérité terrain) - JPL / Simu CLS / CNES 2
  * Comparer à l'existant (in situ) 1
  * Implémenter des algo de production d'images de qualité satisfaisante 5
* Envoie d'alerte par territoire aux usagers (plateforme admin / usager) => VigiCrue 2
* Passage à l'échelle continentale / globale 1
* algorithmie, traitement du signal (Intercomparaison) 4
* Cartographie (après traitements) 2
* Preparer mission drone 1
* étude des petits lacs 1
* étude thématiques: restoration des milieux aquatiques, coef de ruisselement, cycles miniers 1
* Préparation bâti / structures 2

## Points pénibles

* Préparation des données 2
* Satellitaire
  * Temps de téléchargement / récupération / traitement 5
  * Inconstance du type de mesure 2
  * Conversion SAT (S1Tiling) 1
  * Fréquences trop basse 3
  * Fréquence aléatoires (facteurs externes) 2
  * Ressources matérielles requises 13
    * NetCDF trop lourd en manip 1
    * NetCDF trop compliqué en manip 2
    * Volumétrie 1
  * Lenteur de mise à disposition des données sur bandes 1
  * Méconnaissance données alti 1
* Manque de données 5
  * Globalement 1
  * Manque de données sur les petits cours d'eau / micro BV 3
  * Manque de données sur Google Earth Engine 1
* Données payantes (produits spécifiques ou in situ) 2
* Cartographie
  * Manque de centralisation des sources / temps de recherche élevé 6
  * Trop de formalismes et formats différents (BDO et autres) 5
  * QGis demande trop d'étapes 1
* Mise en place 1
  * Lâchers hydro-électriques perturbants 1
* VRE / cluster: lourde / lente / surcouche de complexité inutile 3
  * Plus nuancé: pb réseau d'accès HPC / HAL / VRE (et temps de chargements d'appli / crash régulier / navigateur ne se lance pas, téléchargement compliqué / bureau virtuel ne fonctionne pas...) 5
* Analyse stat. automatique filtre les évènements extrêmes réels 2
* Visualisation historique complexe 1
* Pression des projets (temps / budget) 3
* Développement
  * problèmes de dépendances / mises à jour 4
* Mise à jour des outils (JPL) trop fréquentes 2
* Manque de personnalisation (c'est pénible de repasser pas l'équipe de dev pour rajouter) 1
* Complexité de mise à disposition des résultats pour le client final 2
* Temps de formation important (learning curve) 2
* Des Outil disparates impliquent un communication externe complexe 2
* pas de données altimétriques en representation cartographique 1
* température et turbidité complexe à modéliser / rendre générique 1
* Inadéquation / complexité / fragmentation des outils 4
  * En particulier: tracer des graphiques Python 1
  * Difficulté de transition d'un outil à l'autre (dont passage sur cluster) 2
* Mise en oeuvre des outils 2
* Manque de guidance 1
* manque de moyen pour installer des sondes 1
* communication data via satellite cher 1
* trouver des partenaires qualifiés 1
## Crainte

* Monétisation des services hydro 2
* Les fichiers non copiables (PDF, manuscrits) 1
* Âpre concurrence, intérêts divergents 1
* Rédiger des documents 1
* Coder 1
* pas assez validés (acuité des traitements trop souvent négocié). Notamment sur SurfWater (mais aussi en interne: optimisation contre qualité / vérification) 2
## Appartenance communautaire

* Business
  * SigFox 1
  * Agralis 1
  * Agri sud-ouest 1
  * DREAL 2 
  * CACG 1
  * EPTB, ministères, agences, Collectivités locales, agglo, syndicats des eaux 10
  * Industriels 2
  * Banques mondiales 1
  * Segment sol 1
  * réseaux sociaux, presses 1
* Communauté global
  * Scientifique (dont CNES, JPL...) 12
  * Theia embryon communautaire 3
* Groupes de travail 5
* Trishna 2
* Doppler 1

## Vision communautaire

* Méthodes
  * Accès à de la R&D institutionnelle 3
* Ressources
  * Partager de la donnée in situ 8
  * apport de vision satellite / drone / in situ 2
  * Partager des outils / traitements / chaînes / méthodes 12
    * Altimétrie 1
    * Qualité de l'eau et industrie 1
    * Produits spécifiques 2
    * Veille techno / biblio 2
    * Simulation météo 1
  * Mettre en place des traitements pour les autres 1
  * Consommer de la donnée 9
  * Consommer des outils / traitements / chaînes / méthodes (dont support) 12
  * Consommer des ressources matérielles (CPU, disk, RAM...) 3
  * Vendre des traitements / chaînes 1
* Discussion 3
  * Entre organismes (dont besoins ETPB, méthodes existantes...) 6
  * Entre communautés scientifiques / nationales / grand public 3
  * Emergences de contrats / partenariats de projet 6
  * Emergences d'idées 3
  * Partager le besoin / feedback terrain "terrain" 3
  * Recevoir du feedback des consommateurs 4
* Diminution des coûts 1
* MarketPlace 1
* Retour opérationnel 1
* NON, refuse cette approche 1
## Attentes

* Des données SWOT continues (par d'arrêt à 3 ans) 2
* Des données de haute qualité (à terme) 2
* Des données de qualité moyenne rapidement, puis des données qualitatives plus tard (fast mapping) 3
* Des données in situ très rapidement (quelques minutes) 1
* Des données faciles à récupérer 1
* Des données et outils centralisés / uniformisés 1
* API de déport calcul (travailler chez soi, aussi vite que sur le cluster) 4
  * pré traitement des données pour limiter les téléchargements 1
* Un super QGis 3
  * adapté à la lecture des produits SWOT 2
  * qui permettrait de sélectionner un layer sur trois 1
* Un super Google Earth Engine, transparent, éthique, sans trou de donnée et permettant des traitement "externes" 1
* Outils de visualisation graphique bien faits sur portail (drop excell) 2
* Prévisualisation bien faite sur portail (drop download -> QGis) 1
* Accès rapide aux données historiques (sur bande magnétique) 3
* Libre accès aux données COSMOS SKYMED 1
* Avoir du 3m en bande X (nota: bande permettant une meilleure classification) 1
* Satellite geostationnaire avec pixel à moins de 10m (petits lacs / petites rivières) 2
* Flotte de satellites qui se relaient pour suivre les évènement d'inondation 1
* Des projets "pérennisés" (manque de suivi de long terme) 1
* Mise à disposition d'un scribe 1
* Rapidité d'application des prétraitements et traitements de visu et graphiques (autant calibration qu'exploitation) 1
* afficher la taille dispo des volumes (voir STYX / HYMOTEP) 1
* Esprit de communauté 2
* Pas de code (notamment pour les BD types PostGIS) 1
* Export partitionné de fichier(s) Excell par seuil 1
* Récupérer les données d'acteurs actuellement éparses (stations d'épuration et industriels par exemple) 5
* toutes données openSource, intégrables, récupérables, facilité de partage(flux WMS). 4
* Des chaînes de traitement "stables" qui "tournent sans problème et sans intervention" 2
* accès rapide aux stations virtuelles / vigicrue / vortexio (affichage sur bassin versant simultanée) -> date de dernière et prochaine acquisition 2
* plus de données petits lacs / flaques 3
* Superposition des couches / données facilitée (multi résolution / multi orbite) 1
* Système de préférence de projection par préférence utilisateur 1
* Facile d'utilisation 1
* Ressources matérielles 1
* traitements à grande échelle 1
* comparaisons à grande échelle 1



**A creuser: qu'est ce qu'un SIE? (Alain Gauthier) Quelle matérialisation physique? Quel contrainte en hydrologie**
* Réponse partielle: API online, certainement SANDRE, pour l'évaluation de l'état hydro (API de bilans hydro en lignes)*

**A creuser: quels modèles de propagation? (Alain Gauthier)**

**A creuser: obtenir la liste des algo d'interpolation et paramètres correspondant (forecast et interpolation des valeurs manquantes)**

Marketplace data
**A creuser : que doit - on visualiser ***
* Visualiseur (Idéal pour promotion de données)

**A reporter: Algo de déport de calcul proposé (Jordi Inglada)**e
