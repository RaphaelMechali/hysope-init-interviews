# Interviews Hysope II

## Volet général

* Présentation (nom métier, organisme, formation universitaire)
<font color="darkcyan">
CALVAL, algo produits lacs. Aggège les nuages de points par entités observés (stockage en eau, hauteur...).
2 structures de prod (Observation et aggregation par cycle)
aggregation par cycle: 3 cas différents (moyenne, observé par cycle ~21j => puzzle / synthèse, observé en partie => puzzle amélioré)
Travaille beaucoup avec CS Group
</font>
  * Plutôt opérationnel? Scientifique? Archi / bureau d'étude?
<font color="darkcyan">
Opérationnel et scientifique
</font>
* Quel tâche métier principale? 
<font color="darkcyan">
Développer en python, algorithmie ==> codeuse
</font>
  * Pour quel résultat?
<font color="darkcyan">
Evolution de codes , bugs corrigés dans les traitements lacs. Algo embarqués dans le centre de mission, en deux étapes (elle fait SAS):
1. Elle code le prototype (noyau fonctionnel). Elles ajoutent les tests fonctionnels
2. Cédric corrige les pb qualité / perfo puis envoit au centre de mission (pb multi thread et similaires). Il ajoute les TUs, wrap en éxécutable PGE
</font>
  * Pour qui?
<font color="darkcyan">
De nous d'abord, du segment sol (Charlotte Garcia), du JPL et en OpenSource (utilisés par d'autres scientifiques).
Lib de stockages en eau réutilisables (par le centre d'expertise)
</font>
  * Comment?
<font color="darkcyan">

</font>
  * Etapes?
<font color="darkcyan">
* input: besoin identifié (sur GitLab). Ano / Veo
* Implémente en local (env spider / anaconda)
* Teste sur un petit set en local sur son PC (le cluster rame trop)
  * Visu / qualitatif (vérifie les contour du shapefile, les attributs correspondent à l'entrée)
  * Outils de comparaison de deux shapefiles et similaires (plus ajout d'une vérité terrain / simulée)
* Push git
* Test de grande échelle (cluster)
* Merge
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
* Dev
  * Python
  * env spider / anaconda
* Visu
  * QGis
  * Panoply
  * Google Earth (moins lourd que QGis pour les fonds de carte)
* Moins usine logicielle (deuxième phase du SAS, concerne plus Cédric)
  Moins familière de jupiter notebook (aime moins).
  Aime mieux faire du plugin confluence sur le cluster pour produire des résultats (aide à la CALVAL)
</font>
  * Quels points forts?
<font color="darkcyan">
* Pratique à utiliser
* Léger
</font>
  * Quels points d'amélioration?
<font color="darkcyan">
Fonctionnement justifié par la lenteur du travail sur le cluster (pénible à ouvrir/ multi log etc...). Cluster trop lent (pas le calcul, mais la partie visu très lente)
</font>
  * Quels points d'intégration?
<font color="darkcyan">
passage à la CALVAL: plus de donnée in situ et similaire mais la tâche reste sensiblement la même.
</font>
* Quelles données? 
<font color="darkcyan">

</font>
  * Neige (couverture / prduits dérivés)
<font color="darkcyan">
Aggreg / interprêtation. Vraiment pas trop (et autres données)
</font>
  * SWE (volume eau / neige)
<font color="darkcyan">

</font>
  * Surface d'eau (pixel eau)
<font color="darkcyan">
Oui
</font>
  * Hauteur d'eau
<font color="darkcyan">
Oui
</font>
  * Débit d'eau
<font color="darkcyan">
pour les lacs pas trop mais peut-être rivières
</font>
  * Température
<font color="darkcyan">
Non
</font>
  * Turbidité
<font color="darkcyan">
Non
</font>
  * Autres?
<font color="darkcyan">
Stockage en haut. 
Le MNT:
* Pour l'instant, en entrée de la simu
* A terme,  en comparaison par rapport aux surfaces de lac qui ont "beaucoup d'errer" (pas son use cas, plus celui de Damien).

lacs: 3 fichiers:
* svg: def des lavs
* prior: donnée connues à priori
* unassigned: lac vides / secs
On peut voir le "storage change" en multi temporel (différence par rapport aux observation précédentes)? (feature request) 
mono: 1pixel cloud -> 1 produit
multi: stocker les fichier par lac pour retrouver l'historique
</font>
* Quelles méthodes
  * d'exploitation
<font color="darkcyan">

</font>
  * de comparaison
<font color="darkcyan">
comparaison statistique avec la base de donnée à priori: première levée des erreurs (comparaison de hauteur à la référence par exemple). Outils programmatiques
fonctions de comparaison entre 2 produits (cycle précédent ou vérité terrain):
* surface
* hauteur (- storage change, car c'est une donnée déduite de surface et hauteur)
</font>
  * d'extrapolation
<font color="darkcyan">
Interpolation: autour du stockage. Prévu pour hauteur et surface (basse priorité): lac observé partiellement mais une partie de l'info est dispo (estimation de la surface manquant) => courbe ipsométriques (impossible si SWOT est trop bruité)
</font>
* Tâche métier actuellement bien outillée?
<font color="darkcyan">
Pas mal (arrive à faire ce qu'elle veut avec ce qu'elle a)
</font>
  * Totalement couverte?
<font color="darkcyan">
Visualisation et historique mal couvert (historique des lacs notamment, sur courbe)
</font>
* Quels points pénibles (outils / données / volumétrie / format / etc...)
<font color="darkcyan">
* Rédaction de documents
* Visualisation sur le Cluster (mieux depuis qu'elle a la fibre, lui permet de bosser en local)
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
* Récupération / partage / centralisation des données in situ
* Feedback produit par les utilisateurs (lac manquant > ajout, lac inexistant) > espace d'échange en lien direct (feedback terrain aussi)
* Partage d'outils ponctuels
</font>
* Que souhaiteriez-vous apporter à la communauté?
<font color="darkcyan">
* Pourrait proposer leurs outils (ex plugin d'affichage nuage de points dans QGis)
</font>

## Ouverture

* Disponible peu (1/2 journée mois) pour participer à la conception
<font color="darkcyan">
Carrément (adore)
</font>
* Qu'est ce qui vous ferait gagner du temps?
<font color="darkcyan">
* Un scribe
* Zone de test / travail qui correspondent à ses zones de perfo, pour compiler sa donnée (type google earth)
* Prise de recul grâce à d'autres utilisateurs / pro (feedback externe)
</font>
* POST: Quelles solutions dans un monde idéal?
<font color="darkcyan">

</font>


