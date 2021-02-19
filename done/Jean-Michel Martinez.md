# Interviews Hysope II

## Volet général

* Présentation (nom métier, organisme, formation universitaire)
<font color="darkcyan">
Physicien de formation (M2 télédétection, doctorat télédétection)
Puis surtout en hydro (couleur des eaux pour la qualité, surfaces en haut ~ optique / radar) ~ 20 ans
A utilisé capteur S3, Modis, ou HR
Métier: Dév de chaînes et exploitation (pour gestionnaires, end user, scientifiques pour études)
travaille à l'IRD
</font>
  * Plutôt opérationnel? Scientifique? Archi / bureau d'étude?
<font color="darkcyan">
Scientifique, contact opérationnel
</font>
* Quel tâche métier principale? 
<font color="darkcyan">
Rédaction de mails
Dév de chaînes et tests
</font>
  * Pour quel résultat?
<font color="darkcyan">
* La chaîne en elle même
* Etude de cas d'évolution, études environnementales (état de la qualité de l'eau continentale, beaucoup de tropical): Impact de l'activité minière, l'eutrophisation de lac (transport de sédiment et qualité de l'eau)
Fait de la formation: master / doctorat / gestionnaires.
</font>
  * Pour qui?
<font color="darkcyan">
Pour l'agence de l'eau du Brésil (transfert de chaîne de données Modis, hydrosat), pour des scientifiques
20% gestionnaires ressources et end user, 80% scientifiques
</font>
  * Comment?
<font color="darkcyan">
- cf étapes
</font>
  * Etapes?
<font color="darkcyan">
* identifie un besoin en partenariat avec des gestionnaires
* part de produits type Maya
* essaie d'identifier problèmes d'images et de les résoudre
* les premières chaînes: a développé, validé, puis supervisé son transfert en JAVA
* maintenant supervise le dev des chaînes (définit et porte le besoin). 
* valide les chaînes
* exploite les chaînes, produit les études (avec étudiants), les fournit au gestionnaire 
</font>
* Quelles tâches métiers secondaire? (sous-tâches ou tâches parallèles?)
<font color="darkcyan">
* Observatoire conventionnel de la qualité de l'eau en Amazonie (contribue les données à Theia>Ozcar)
* Envoie des mails
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
* cluster CNES et OFB (Organisme Français pour la Biodiversité)
* S2/S3 avec leur moyens locaux
* Données terrains (drones, in situ) et satellitaire
* Données HR ==> code Python, SNAP, Java
* Données BR ==> code Java serveur
* Visu: Python (lib)
</font>
  * Quels points forts?
<font color="darkcyan">
* Cluster: gère bien la masse d'information!
* Aspect dev (leur point fort)
</font>
  * Quels points d'amélioration?
<font color="darkcyan">
* Aggrégation / centralisation de produits qui leur sont nécessaire (masque eau / masque neige)
* Espace nécessaire pour les calculs (pays / partie de continents)
* Facilité de mise à disposition pour la communauté et de démonstration
</font>
  * Quels points d'intégration?
<font color="darkcyan">

</font>
* Quelles données? 
<font color="darkcyan">
</font>
  * Neige (couverture / produits dérivés)
<font color="darkcyan">
OUI
</font>
  * SWE (volume eau / neige)
<font color="darkcyan">

</font>
  * Surface d'eau (pixel eau)
<font color="darkcyan">
OUI
</font>
  * Hauteur d'eau
<font color="darkcyan">

</font>
  * Débit d'eau
<font color="darkcyan">

</font>
  * Température
<font color="darkcyan">
Oui
</font>
  * Turbidité
<font color="darkcyan">
Oui
</font>
  * Autres?
<font color="darkcyan">
* produits de niveaux 1C
* masque eaux (SurfWater), nuages, neige (EumetSat, WaterFullResolution)
* Réflectance (Maya? 2A moins précis les intéresse)
===> produit de couleur d'eau
* A aussi besoin des aérosols (Synergy)
* Mesure de Chlorophyle
* NAIADE
</font>
* Quelles méthodes
  * d'exploitation
<font color="darkcyan">
Méthodes mathématiques (MonteCarlo, Radom Forest, Machine Learning), regression statistique (R puis Machine Learning), nombre de canaux spectraux, gros jeux de données
Se dirige progressivement vers de l'analyse Big Data
</font>
  * de comparaison
<font color="darkcyan">

</font>
  * d'extrapolation
<font color="darkcyan">
Commence à travailler sur des problématiques d'interpolation / extrapolation par modèle
modélisation des flux d'abord, puis modélisation qualité. (utilisent SWAT, même famille que MGB mais complètement ouvert, qui modélise les flux)
Veulent passer à l'échelle continentale
Veulent à terme de développer une chaîne qui peut utiliser toutes les données de couleur disponibles (MODIS, Sentinel, …etc)
</font>
* Tâche métier actuellement bien outillée?
<font color="darkcyan">
Oui
</font>
  * Totalement couverte?
<font color="darkcyan">
attend HI2 pour travailler à une échelle continentale, voir globale
</font>
* Quels points pénibles (outils / données / volumétrie / format / etc...)
<font color="darkcyan">
Comment récupérer les jeux de données (éclatement des sources => masques eau, neige, etc...): grosse complication d'unification, vu qu'ils mélangent un peu toutes les sources (et parfois remplacent S2 par S3 en cas d'image manquante, par exemple)
Gros calcul (mais cluster, **vérifier avec l'enregistrement**)
</font>
* Illustrer tâche métier durant l'interview? (si moins de 20 minutes)
<font color="darkcyan">

</font>

## Volet intégration HI2

* Etes vous familiers avec les services Theia?
<font color="darkcyan">
Oui un peu (Ozcar)
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
* Récupérer et adapter des bouts de routine pour gérer des jeux spécifiques, des codes d'exploit/big data/autres
* Apport d'idées d'utilisateurs
</font>
* Que souhaiteriez-vous apporter à la communauté?
<font color="darkcyan">
* Connaissance autour de nos produits, montrer / démontrer l'intérêt
</font>

## Ouverture

* Disponible peu (1/2 journée mois) pour participer à la conception
<font color="darkcyan">
Oui
</font>
* Qu'est ce qui vous ferait gagner du temps?
<font color="darkcyan">
* Chaînes qui tournent sans problèmes de différentes sources (plus d'intervention humaine quotidienne), sur des volumes importants. Problème de changement de repertoires sources
</font>
* POST: Quelles solutions dans un monde idéal?
<font color="darkcyan">
* Endroit unique ou accéder à toute la donnée
* stable et sans problème de dépendances
</font>


