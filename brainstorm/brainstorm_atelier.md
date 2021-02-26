## Atelier
* data :
  * SWOT continues (par d'arrêt à 3 ans)
  * de haute qualité (à terme) 2
  * de qualité moyenne rapidement, puis des données qualitatives plus tard (fast mapping) 3
  * in situ très rapidement (quelques minutes) 1
  * faciles à récupérer 1
  * et outils centralisés / uniformisés 1
  * Accès rapide aux données historiques (sur bande magnétique) 3
  * payantes (produits spécifiques ou in situ) 2
  * pas de données altimétriques en representation cartographique 1
  * Récupérer les données d'acteurs actuellement éparses (stations d'épuration et industriels par exemple) 5
  * toutes données openSource, intégrables, récupérables, facilité de partage(flux WMS). 4
  * plus de données petits lacs / flaques 3
* cartographie
 * 
* materiel / ressources distantes

* outils 


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


