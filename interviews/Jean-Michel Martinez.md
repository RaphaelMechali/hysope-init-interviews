# Interviews Hysope II

## Volet général

* Présentation (nom métier, organisme, formation universitaire)
<span class="user-answer">
Physicien de formation (M2 télédétection, doctorat télédétection)
Puis surtout en hydro (couleur des eaux pour la qualité, surfaces en haut ~ optique / radar) ~ 20 ans
A utilisé capteur S3, Modis, ou HR
Métier: Dév de chaînes et exploitation (pour gestionnaires, end user, scientifiques pour études)
travaille à l'IRD
</span>
  * Plutôt opérationnel? Scientifique? Archi / bureau d'étude?
<span class="user-answer">
Scientifique, contact opérationnel
</span>
* Quel tâche métier principale? 
<span class="user-answer">
Rédaction de mails
Dév de chaînes et tests
</span>
  * Pour quel résultat?
<span class="user-answer">
* La chaîne en elle même
* Etude de cas d'évolution, études environnementales (état de la qualité de l'eau continentale, beaucoup de tropical): Impact de l'activité minière, l'eutrophisation de lac (transport de sédiment et qualité de l'eau)
Fait de la formation: master / doctorat / gestionnaires.
</span>
  * Pour qui?
<span class="user-answer">
Pour l'agence de l'eau du Brésil (transfert de chaîne de données Modis, hydrosat), pour des scientifiques
20% gestionnaires ressources et end user, 80% scientifiques
</span>
  * Comment?
<span class="user-answer">
- cf étapes
</span>
  * Etapes?
<span class="user-answer">
* identifie un besoin en partenariat avec des gestionnaires
* part de produits type Maya
* essaie d'identifier problèmes d'images et de les résoudre
* les premières chaînes: a développé, validé, puis supervisé son transfert en JAVA
* maintenant supervise le dev des chaînes (définit et porte le besoin). 
* valide les chaînes
* exploite les chaînes, produit les études (avec étudiants), les fournit au gestionnaire 
</span>
* Quelles tâches métiers secondaire? (sous-tâches ou tâches parallèles?)
<span class="user-answer">
* Observatoire conventionnel de la qualité de l'eau en Amazonie (contribue les données à Theia>Ozcar)
* Envoie des mails
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
* cluster CNES et OFB (Organisme Français pour la Biodiversité)
* S2/S3 avec leur moyens locaux
* Données terrains (drones, in situ) et satellitaire
* Données HR ==> code Python, SNAP, Java
* Données BR ==> code Java serveur
* Visu: Python (lib)
</span>
  * Quels points forts?
<span class="user-answer">
* Cluster: gère bien la masse d'information!
* Aspect dev (leur point fort)
</span>
  * Quels points d'amélioration?
<span class="user-answer">
* Aggrégation / centralisation de produits qui leur sont nécessaires (masque eau / masque neige)
* Espace nécessaire pour les calculs (pays / partie de continents)
* Facilité de mise à disposition pour la communauté et de démonstration
</span>
  * Quels points d'intégration?
<span class="user-answer">

</span>
* Quelles données? 
<span class="user-answer">
</span>
  * Neige (couverture / produits dérivés)
<span class="user-answer">
OUI
</span>
  * SWE (volume eau / neige)
<span class="user-answer">

</span>
  * Surface d'eau (pixel eau)
<span class="user-answer">
OUI
</span>
  * Hauteur d'eau
<span class="user-answer">

</span>
  * Débit d'eau
<span class="user-answer">

</span>
  * Température
<span class="user-answer">
Oui
</span>
  * Turbidité
<span class="user-answer">
Oui
</span>
  * Autres?
<span class="user-answer">
* produits de niveaux 1C
* masque eaux (SurfWater), nuages, neige (EumetSat, WaterFullResolution)
* Réflectance (Maya? 2A moins précis les intéresse)
===> produit de couleur d'eau
* A aussi besoin des aérosols (Synergy)
* Mesure de Chlorophyle
* NAIADE
</span>
* Quelles méthodes
  * d'exploitation
<span class="user-answer">
Méthodes mathématiques (MonteCarlo, Radom Forest, Machine Learning), regression statistique (R puis Machine Learning), nombre de canaux spectraux, gros jeux de données
Se dirige progressivement vers de l'analyse Big Data
</span>
  * de comparaison
<span class="user-answer">

</span>
  * d'extrapolation
<span class="user-answer">
Commence à travailler sur des problématiques d'interpolation / extrapolation par modèle
modélisation des flux d'abord, puis modélisation qualité. (utilisent SWAT, même famille que MGB mais complètement ouvert, qui modélise les flux)
Veulent passer à l'échelle continentale
Veulent à terme de développer une chaîne qui peut utiliser toutes les données de couleur disponibles (MODIS, Sentinel, …etc)
</span>
* Tâche métier actuellement bien outillée?
<span class="user-answer">
Oui
</span>
  * Totalement couverte?
<span class="user-answer">
attend HI2 pour travailler à une échelle continentale, voir globale
</span>
* Quels points pénibles (outils / données / volumétrie / format / etc...)
<span class="user-answer">
Comment récupérer les jeux de données (éclatement des sources => masques eau, neige, etc...): grosse complication d'unification, vu qu'ils mélangent un peu toutes les sources (et parfois remplacent S2 par S3 en cas d'image manquante, par exemple)
Gros calcul (mais cluster, **vérifier avec l'enregistrement**)
</span>
* Illustrer tâche métier durant l'interview? (si moins de 20 minutes)
<span class="user-answer">

</span>

## Volet intégration HI2

* Etes vous familiers avec les services Theia?
<span class="user-answer">
Oui un peu (Ozcar)
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
* Récupérer et adapter des bouts de routine pour gérer des jeux spécifiques, des codes d'exploit/big data/autres
* Apport d'idées d'utilisateurs
</span>
* Que souhaiteriez-vous apporter à la communauté?
<span class="user-answer">
* Connaissance autour de nos produits, montrer / démontrer l'intérêt
</span>

## Ouverture

* Disponible peu (1/2 journée mois) pour participer à la conception
<span class="user-answer">
Oui
</span>
* Qu'est ce qui vous ferait gagner du temps?
<span class="user-answer">
* Chaînes qui tournent sans problèmes de différentes sources (plus d'intervention humaine quotidienne), sur des volumes importants. Problème de changement de repertoires sources
</span>
* POST: Quelles solutions dans un monde idéal?
<span class="user-answer">
* Endroit unique ou accéder à toute la donnée
* stable et sans problème de dépendances
</span>

<style>
.user-answer {
  color: darkcyan;  
}
</style>
