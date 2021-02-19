# Résumé des habitudes rencontrées

## Variables et visualisation

### Consommées

* MNT 3
* Définition des "shapes" d'entités 1
  * prior (déf à priori) 1
  * unassigned (déf "lac à sec") 1
* hauteur d'eau 5 
  * mesure par capteur de pression 1
* débit 3
* surface 5
* Volume / stockage 5
* température 1
* hygrométrie 1
* vent 1
* Neige 1
* SWE 1
* glace (et glaciers) 1
* météo actuelle 2
  * pluviométrie 3
  * température air 1
* prévision météo 2
  * lame d'eau Antilope par exemple 1
* rayonnement 1
* Humidité des sols 2
  * Par sonde capacitive 1
* Température 2
* Turbidité 3
* Occupation des sols 4
  * Radar (Sentinel) 2
* Pente terrain 1
* Résultats de recherches scientifiques externes 1

### Calculeés

* ETP 3
* Carte d'érosion 1
* Risque d'érosion 1
* Bilan hydrique 2
  * Cycle de l'eau 1

## Outils & méthodes

* Dispense formation / support 5
* Outil propre pour distribuer les données / le résultat 2
* In situ
  * Hydrométrie jauge 1
  * Bateaux drones 1
  * Théodolites 1
* Cartographie
  * QGis 5
  * Panoply 2
  * NCView 1
  * PostGIS 1
* Analyse mathématique 5
  * Courbe temporelle (suivi volumes, surface, débits, prélèvements, précipitations ETP, oxygènation, turbidité, hauteur + mesure) 4
  * Courbe Ipsométriques (surface x hauteur = signature lac = bathymétrie?) 3 **TODO @LZA: unifiable avec le point dessous? ~= bathymétrie**
  * Courbe multi-paramètres (corrélation météo x hydro x param trisométrique) 3
  * Multi graph 1
  * Comparaison à la moyenne / écart type 3
  * Interpolation / extrapolation polynomiale, constante optimiste, gaussienne etc... 2
    * MNT 1
    * temporelle (variable, nuage de points) 2
  * Estimation de marge d'erreur 1
  * Cartographiée 2
    * Pour corréler aval / amont (par indicateurs de propagation visuels: tronçons de rivières colorés) 1
    * Comparaison visuelle aux contours attendus 2
      * Par reconstitution de plusieurs images ou sources par entité (lac / rivières) 1
    * Comparaison automatisée aux contours attendus (image) 2
    * Pixel cloud x shapefile / Pixel cloud (analyse qualitative des surfaces) 2
* Programmation 1
  * Python 4
    * Orphéo toolbox 1
    * S1Tiling 1
    * PyCharm 1
    * Spider 1
    * Anaconda 1
  * VSCode 1
  * Test 1
    * Fonctionnels 1
    * Unitaires 1
  * Plugin confluence 1
  * Jupiter notebook 1
* Partage & comm 2
  * Git 2
  * GitLab 2
  * Confluence 1
  * skype 1
* Cloud 3
  * AWS 1
  * HPC HAL cluster CNES 3
* Modèles 2
  * SAFI (évolution biomasse, réserve hydrique) 1
  * (R)GRxx 1
  * SWAT 1
  * De propagation (type non mentionné) 1
* Travaille par sous BV 1
* Plateforme Web 2
  * Interne 1
  * Theia 1
  * Corpernicus 2
  * Sci-Hub 3
  * Hubeau 1
  * Géoportail IGN 1
  * Service Sandre 1
  * Banque Hydro 1
  * CNES (Hydroweb OG, Peps, HPC, Theia...) 1
  * Earth data (NASA) 1
  * Google Earth Engine 3
  * CTOH 1
* Calcul, reporting et recherche 1
  * Word, PowerPoint 2
  * Excell 2
  * SearchEveryThing (compense l'absence de stockage correct des projets antérieurs) 1
* Veille techno 2
* Veille donnée 1

## Projets communs

* ACMG
  * R&D -> Agralis commercialise
  * ACMG <-> Aquafox <-> SigFox || GPRS
  * Projet clipalert > plateforme (niveau d'eau / prévision)

## Buts

* érosion des sols 1
* impact changement climatique 2
* lutte contre la gelée, grêle, irrigation, 1
* distribution de la ressource (réserve, partage, ressources, retenues collinaires, soutien d'étiage) 2
* étude d'impact sur les milieux aquatiques (débit / qualité) 1

## Points pénibles

* Préparation 1
* Satellitaire 3
  * Temps de téléchargement / récupération / traitement 3
  * Puissance / espace requis 2
  * Inconstance du type de mesure 1
  * Conversion SAT (S1Tiling) 1
  * Fréquences trop basse 1
  * Ressources matérielles requises 4
  * Lenteur de mise à disposition des données sur bandes 1
* Cartographie 3
  * Manque d'homogénéité / uniformité des couches (WMS, Cartage...) 3
  * Manque de centralisation des sources 1
* Mise en place 1
  * Lâchers hydro-électriques perturbants 1
* VRE / cluster: lourde / lente / surcouche de complexité inutile 2
  * Plus nuancé: pb réseau d'accès HPC / HAL / VRE 1
* Analyse stat. automatique filtre les évènements extrêmes réels 1
* Estimer la marge d'erreur 2
* Visualisation historique complexe 1


## Crainte

* Monétisation des services hydro 1
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
  * EPTB (Etablissement Public Territorial de Bassin) 1
  * Syndicat Mixte d'Aménagement de la Garonne 1
  * Gouvernements 1
  * Banques mondiales 1
  * Gestionnaires 1
  * CNES 3
  * Segment sol 1
* Communauté globale 1
  * Scientifique (CNES / JPL / Universités) 3

## Vision communautaire

* Méthodes 1
  * Accès à de la R&D institutionnelle 1
* Ressources
  * Partager de la donnée in situ 1
  * Partager des outils / traitements / chaînes / méthodes 3
  * Mettre en place des traitements pour les autres 1
  * Consommer de la donnée 4
  * Consommer des outils / traitements / chaînes / méthodes 3
  * Consommer des ressources matérielles (CPU, disk, RAM...) 1
  * Vendre des traitements / chaînes 1
* Discussion 2
  * Entre organismes (dont besoins ETPB, méthodes...) 2
  * Entre communautés scientifiques / nationales 1
  * Réception de feedback des consommateurs 2
* Diminution des coûts 1


## Attentes

* API de déport calcul (travailler chez soi, aussi vite que sur le cluster) 1
* Un super QGis adapté à la lecture des produits SWOT auxiliaires (+ calcul auto des métriques) 1
* Outils de visualisation graphique bien faits sur portail (drop excell) 1
* Prévisualisation bien faite sur portail (drop download -> QGis) 1
* Accès rapide aux données historiques (sur bande magnétique) 1
* Libre accès aux données COSMOS SKYMED 1
* Avoir du 3m en bande X (nota: bande permettant une meilleure classification) 1
* Satellite geostationnaire avec pixel à moins de 10m (petits lacs / petites rivières) 1
* Flotte de satellites qui se relaient pour suivre les évènement d'inondation 1
* Mise à disposition d'un scribe



**A creuser: qu'est ce qu'un SIE? (Alain Gauthier) Quelle matérialisation physique? Quel contrainte en hydrologie**
*Réponse partielle: API online, certainement SANDRE, pour l'évaluation de l'état hydro (API de bilans hydro en lignes)*

** A creuser: quels modèles de propagation? (Alain Gauthier)**
