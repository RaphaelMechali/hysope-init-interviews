# Interviews Hysope II

## Volet général

* Présentation (nom métier, organisme, formation universitaire)
<span class="user-answer">
CALVAL, algo produits lacs. Aggège les nuages de points par entités observés (stockage en eau, hauteur...).
2 structures de prod (Observation et aggregation par cycle)
aggregation par cycle: 3 cas différents (moyenne, observé par cycle ~21j => puzzle / synthèse, observé en partie => puzzle amélioré)
Travaille beaucoup avec CS Group
</span>
  * Plutôt opérationnel? Scientifique? Archi / bureau d'étude?
<span class="user-answer">
Opérationnel et scientifique
</span>
* Quel tâche métier principale? 
<span class="user-answer">
Développer en python, algorithmie ==> codeuse
</span>
  * Pour quel résultat?
<span class="user-answer">
Evolution de codes , bugs corrigés dans les traitements lacs. Algo embarqués dans le centre de mission, en deux étapes (elle fait SAS):
1. Elle code le prototype (noyau fonctionnel). Elles ajoutent les tests fonctionnels
2. Cédric corrige les pb qualité / perfo puis envoit au centre de mission (pb multi thread et similaires). Il ajoute les TUs, wrap en éxécutable PGE
</span>
  * Pour qui?
<span class="user-answer">
De nous d'abord, du segment sol (Charlotte Garcia), du JPL et en OpenSource (utilisés par d'autres scientifiques).
Lib de stockages en eau réutilisables (par le centre d'expertise)
</span>
  * Comment?
<span class="user-answer">

</span>
  * Etapes?
<span class="user-answer">
* input: besoin identifié (sur GitLab). Ano / Veo
* Implémente en local (env spider / anaconda)
* Teste sur un petit set en local sur son PC (le cluster rame trop)
  * Visu / qualitatif (vérifie les contour du shapefile, les attributs correspondent à l'entrée)
  * Outils de comparaison de deux shapefiles et similaires (plus ajout d'une vérité terrain / simulée)
* Push git
* Test de grande échelle (cluster)
* Merge
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
</span>
  * Quels points forts?
<span class="user-answer">
* Pratique à utiliser
* Léger
</span>
  * Quels points d'amélioration?
<span class="user-answer">
Fonctionnement justifié par la lenteur du travail sur le cluster (pénible à ouvrir/ multi log etc...). Cluster trop lent (pas le calcul, mais la partie visu très lente)
</span>
  * Quels points d'intégration?
<span class="user-answer">
passage à la CALVAL: plus de donnée in situ et similaire mais la tâche reste sensiblement la même.
</span>
* Quelles données? 
<span class="user-answer">

</span>
  * Neige (couverture / prduits dérivés)
<span class="user-answer">
Aggreg / interprêtation. Vraiment pas trop (et autres données)
</span>
  * SWE (volume eau / neige)
<span class="user-answer">

</span>
  * Surface d'eau (pixel eau)
<span class="user-answer">
Oui
</span>
  * Hauteur d'eau
<span class="user-answer">
Oui
</span>
  * Débit d'eau
<span class="user-answer">
pour les lacs pas trop mais peut-être rivières
</span>
  * Température
<span class="user-answer">
Non
</span>
  * Turbidité
<span class="user-answer">
Non
</span>
  * Autres?
<span class="user-answer">
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
</span>
* Quelles méthodes
  * d'exploitation
<span class="user-answer">

</span>
  * de comparaison
<span class="user-answer">
comparaison statistique avec la base de donnée à priori: première levée des erreurs (comparaison de hauteur à la référence par exemple). Outils programmatiques
fonctions de comparaison entre 2 produits (cycle précédent ou vérité terrain):
* surface
* hauteur (- storage change, car c'est une donnée déduite de surface et hauteur)
</span>
  * d'extrapolation
<span class="user-answer">
Interpolation: autour du stockage. Prévu pour hauteur et surface (basse priorité): lac observé partiellement mais une partie de l'info est dispo (estimation de la surface manquant) => courbe ipsométriques (impossible si SWOT est trop bruité)
</span>
* Tâche métier actuellement bien outillée?
<span class="user-answer">
Pas mal (arrive à faire ce qu'elle veut avec ce qu'elle a)
</span>
  * Totalement couverte?
<span class="user-answer">
Visualisation et historique mal couvert (historique des lacs notamment, sur courbe)
</span>
* Quels points pénibles (outils / données / volumétrie / format / etc...)
<span class="user-answer">
* Rédaction de documents
* Visualisation sur le Cluster (mieux depuis qu'elle a la fibre, lui permet de bosser en local)
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
* Récupération / partage / centralisation des données in situ
* Feedback produit par les utilisateurs (lac manquant > ajout, lac inexistant) > espace d'échange en lien direct (feedback terrain aussi)
* Partage d'outils ponctuels
</span>
* Que souhaiteriez-vous apporter à la communauté?
<span class="user-answer">
* Pourrait proposer leurs outils (ex plugin d'affichage nuage de points dans QGis)
</span>

## Ouverture

* Disponible peu (1/2 journée mois) pour participer à la conception
<span class="user-answer">
Carrément (adore)
</span>
* Qu'est ce qui vous ferait gagner du temps?
<span class="user-answer">
* Un scribe
* Zone de test / travail qui correspondent à ses zones de perfo, pour compiler sa donnée (type google earth)
* Prise de recul grâce à d'autres utilisateurs / pro (feedback externe)
</span>
* POST: Quelles solutions dans un monde idéal?
<span class="user-answer">

</span>

<style>
.user-answer {
  color: darkcyan;  
}
</style>
