# Interviews Hysope II

## Volet général

* Présentation (nom métier, organisme, formation universitaire)
<span class="user-answer">
Service DSO SI TR, SWOT HYDRO depuis 2008-2009
Coordinateur d'activités
Thèse au CesBio sur l'imagerie radar
</span>
  * Plutôt opérationnel? Scientifique? Archi / bureau d'étude?
<span class="user-answer">
Scientifique, prépare
</span>
* Quel tâche métier principale? 
<span class="user-answer">
prépare CalVal, coordonne les équipes SWOT: définition du produit, documentation, implémente les algos (proto avant).
Coopère avec SDS pour rendre les soft opérationnels et exploitables
</span>
  * Pour quel résultat?
<span class="user-answer">
* algorithmes & évaluation de performance
* documentation produit
</span>
  * Pour qui?
<span class="user-answer">
Consommés par la "science team" et utilisateurs des données / projets (il tient les specs => facile à utiliser, répond au besoin)
</span>
  * Comment?
<span class="user-answer">
* GitLab synchrone avec l'équipe JPL (USA) et reviews croisées
* Confluence pour la communication avec les sous-traitants
* Pas d'outils standard
* beaucoup de code de simulation (par le JPL en C, récupère les binaires, se sont fait simu simplifié en Python)
</span>
  * Etapes?
<span class="user-answer">
* regrouper les données nécessaires pour la simu (MNT, Landcover pour occupation des sols) et injecter des vérités terrain. **Uniquement durant le développement d'algo**
* Injecter de vraies données pour la CALVAL **uniquement CALVAL** (attentes HI2; données in situ)
* chaîne de traitements
* Produits: Niveau d'eau, étendu surface d'eau principaux. Plus haut niveau: stock, débit (moins validé aujourd'hui, donc un peu moins intéressant).
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
QGis (mais pas trop lui)
Visu qui vient de JPL (mais trop lui)
</span>
  * Quels points forts?
<span class="user-answer">

</span>
  * Quels points d'amélioration?
<span class="user-answer">

</span>
  * Quels points d'intégration?
<span class="user-answer">

</span>
* Quelles données? 
<span class="user-answer">

</span>
  * Neige (couverture / produits dérivés)
<span class="user-answer">

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
Oui
</span>
  * Température
<span class="user-answer">

</span>
  * Turbidité
<span class="user-answer">

</span>
  * Autres?
<span class="user-answer">
 Volume d'eau (stock)
</span>
* Quelles méthodes
  * d'exploitation
<span class="user-answer">
Actuellement: Python pour générer des rapport: compare la vérité terrain avec le produit (par pixel / par image / par rivière / par lac). Par exemple, -de 15% d'erreur surface d'eau (erreur à 1 segment?). Note: écart type acceptable <= 1sigma (10cm)
Leur génère un doc Latex avec courbes.
En CALVAL: utiliseront de vraies vérités terrains, pas générées.
Courbes:
* Fonction de où on est dans la fauchée x qualité
* Erreur de surface (Y) OU Hauteur / diff hauteur, X: taille du lac, endroit de la fauchée
</span>
  * de comparaison
<span class="user-answer">
visualisé directement (notamment pour trouver les erreurs, comparer image optique et in situ).
Même type de courbe
Méthodes du JPL éventuellement imposée, peut nécessiter des conversions pour échanges entre labos
</span>
  * d'extrapolation
<span class="user-answer">

</span>
* Tâche métier actuellement bien outillée?
<span class="user-answer">
Plutôt oui (des outils ajoutés en une décennie, aspect très dev., un peu partage de données aussi via le cloud amazon bucket, notamment pour les données in situ / simu)
</span>
  * Totalement couverte?
<span class="user-answer">
Non ce n'est pas fini
simu OK
attentes:
* adaptation pour pouvoir faire l'évaluation algo / données, récupération de vraies données
* visualisation à améliorer
</span>
* Quels points pénibles (outils / données / volumétrie / format / etc...)
<span class="user-answer">
beaucoup de travail de mise en oeuvre des outils, calculs longs
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
* En lien avec quelques personnes de la Science Team, qui amènent des mesures terrain (in situ, batimétrie, campagnes de mesures).
* Aimerait travailler avec groupes de scientifiques (feedback communautaire)
</span>
* Que souhaiteriez-vous apporter à la communauté?
<span class="user-answer">
* La donnée SWOT, performante et fiable (hauteur / surface)
</span>

## Ouverture

* Disponible peu (1/2 journée mois) pour participer à la conception
<span class="user-answer">
Oui, ça pourrait aller
</span>
* Qu'est ce qui vous ferait gagner du temps?
<span class="user-answer">
Récupérer les données de référence en ligne automatiquement (à ingérer / convertir toutes les 7 minutes depuis les agences de mesures)
Visu 3D, courbes, produits différents
</span>
* POST: Quelles solutions dans un monde idéal?
<span class="user-answer">
Outil ouvert: comm scientifique interne / externe
Récupération facile des données
diverses visu dans l'outil
traitements à grande échelle
comparaisons à grande échelle
</span>


<style>
.user-answer {
  color: darkcyan;  
}
</style>
