# Interviews Hysope II

## Volet général

* Présentation (nom métier, organisme, formation universitaire)
<font color="darkcyan">
Service DSO SI TR, SWOT HYDRO depuis 2008-2009
Coordinateur d'activités
Thèse au CesBio sur l'imagerie radar
</font>
  * Plutôt opérationnel? Scientifique? Archi / bureau d'étude?
<font color="darkcyan">
Scientifique, prépare
</font>
* Quel tâche métier principale? 
<font color="darkcyan">
prépare CalVal, coordonne les équipes SWOT: définition du produit, documentation, implémente les algos (proto avant).
Coopère avec SDS pour rendre les soft opérationnels et exploitables
</font>
  * Pour quel résultat?
<font color="darkcyan">
* algorithmes & évaluation de performance
* documentation produit
</font>
  * Pour qui?
<font color="darkcyan">
Consommés par la "science team" et utilisateurs des données / projets (il tient les specs => facile à utiliser, répond au besoin)
</font>
  * Comment?
<font color="darkcyan">
* GitLab synchrone avec l'équipe JPL (USA) et reviews croisées
* Confluence pour la communication avec les sous-traitants
* Pas d'outils standard
* beaucoup de code de simulation (par le JPL en C, récupère les binaires, se sont fait simu simplifié en Python)
</font>
  * Etapes?
<font color="darkcyan">
* regrouper les données nécessaires pour la simu (MNT, Landcover pour occupation des sols) et injecter des vérités terrain. **Uniquement durant le développement d'algo**
* Injecter de vraies données pour la CALVAL **uniquement CALVAL** (attentes HI2; données in situ)
* chaîne de traitements
* Produits: Niveau d'eau, étendu surface d'eau principaux. Plus haut niveau: stock, débit (moins validé aujourd'hui, donc un peu moins intéressant).
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
QGis (mais pas trop lui)
Visu qui vient de JPL (mais trop lui)
</font>
  * Quels points forts?
<font color="darkcyan">

</font>
  * Quels points d'amélioration?
<font color="darkcyan">

</font>
  * Quels points d'intégration?
<font color="darkcyan">

</font>
* Quelles données? 
<font color="darkcyan">

</font>
  * Neige (couverture / produits dérivés)
<font color="darkcyan">

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
Oui
</font>
  * Température
<font color="darkcyan">

</font>
  * Turbidité
<font color="darkcyan">

</font>
  * Autres?
<font color="darkcyan">
 Volume d'eau (stock)
</font>
* Quelles méthodes
  * d'exploitation
<font color="darkcyan">
Actuellement: Python pour générer des rapport: compare la vérité terrain avec le produit (par pixel / par image / par rivière / par lac). Par exemple, -de 15% d'erreur surface d'eau (erreur à 1 segment?). Note: écart type acceptable <= 1sigma (10cm)
Leur génère un doc Latex avec courbes.
En CALVAL: utiliseront de vraies vérités terrains, pas générées.
Courbes:
* Fonction de où on est dans la fauchée x qualité
* Erreur de surface (Y) OU Hauteur / diff hauteur, X: taille du lac, endroit de la fauchée
</font>
  * de comparaison
<font color="darkcyan">
visualisé directement (notamment pour trouver les erreurs, comparer image optique et in situ).
Même type de courbe
Méthodes du JPL éventuellement imposée, peut nécessiter des conversions pour échanges entre labos
</font>
  * d'extrapolation
<font color="darkcyan">

</font>
* Tâche métier actuellement bien outillée?
<font color="darkcyan">
Plutôt oui (des outils ajoutés en une décennie, aspect très dev., un peu partage de données aussi via le cloud amazon bucket, notamment pour les données in situ / simu)
</font>
  * Totalement couverte?
<font color="darkcyan">
Non ce n'est pas fini
simu OK
attentes:
* adaptation pour pouvoir faire l'évaluation algo / données, récupération de vraies données
* visualisation à améliorer
</font>
* Quels points pénibles (outils / données / volumétrie / format / etc...)
<font color="darkcyan">
beaucoup de travail de mise en oeuvre des outils, calculs longs
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
* En lien avec quelques personnes de la Science Team, qui amènent des mesures terrain (in situ, batimétrie, campagnes de mesures).
* Aimerait travailler avec groupes de scientifiques (feedback communautaire)
</font>
* Que souhaiteriez-vous apporter à la communauté?
<font color="darkcyan">
* La donnée SWOT, performante et fiable (hauteur / surface)
</font>

## Ouverture

* Disponible peu (1/2 journée mois) pour participer à la conception
<font color="darkcyan">
Oui, ça pourrait aller
</font>
* Qu'est ce qui vous ferait gagner du temps?
<font color="darkcyan">
Récupérer les données de référence en ligne automatiquement (à ingérer / convertir toutes les 7 minutes depuis les agences de mesures)
Visu 3D, courbes, produits différents
</font>
* POST: Quelles solutions dans un monde idéal?
<font color="darkcyan">
Outil ouvert: comm scientifique interne / externe
Récupération facile des données
diverses visu dans l'outil
traitements à grande échelle
comparaisons à grande échelle
</font>


