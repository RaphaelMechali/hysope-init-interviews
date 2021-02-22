# Interviews Hysope II

## Volet général

* Présentation (nom métier, organisme, formation universitaire)
<span class="user-answer">
Ingénieur généraliste (Les mines St Etienne), Compagnie Nationale du Rhone, travaille en modélisation hydro (concessionaire du fleuve Rhone => en 1930 l'état leur procure le contrat de gestion et d'exploitation => navigation, irrigation, electricité, 1/4 prod hydro elec française, 14 écluses...). Travaille à la direction de l'ingénierie, autres missions ==> projet spatial bassin du Congo et altimétrie spatiale (membre de SWOT).
Peu d'outils universitaires encore utilisés (hors stats)
</span>
  * Plutôt opérationnel? Scientifique? Archi / bureau d'étude?
<span class="user-answer">
Interne: appui exploitation (opérationnel)
Externe: bureau d'étude
</span>
* Quel tâche métier principale? 
<span class="user-answer">
gestion de projet
récupération de jeux en hydro, analyse et critique, mise au propre (données manquantes, aberrantes, conversion éventuelle), puis caler un modèle (souvent décider en amont) => calage / validation
Modèles GR ou autres en fonction du besoin (échelle Grand BV, par ex Congo 150 000 km², Rhône découpé en 22 affluents)
</span>
  * Pour quel résultat?
<span class="user-answer">
Modèle pertinent répondant au besoin du client (prévision de débit notamment)
</span>
  * Pour qui?
<span class="user-answer">
client ou lui même. Raccrocher le modèle au système info et décision
</span>
  * Comment?
<span class="user-answer">
Critère de validation.
Modèle de chroniques comparés à l'observés. Route Min Square Error (erreur quadra), MAE (Min Absolute Error) ~MAD (précision Lionel la nomenclature) critères de bilan (bilan bien retrouvé sur une année), Critère de persistence (pour prédictif) => quantifié l'apport du modèle par rapport à un modèle "naïf"
</span>
  * Etapes?
<span class="user-answer">
* Récupérer des jeux: Ex au Congo (hauteur Sanga, affluent) ==> Ne savait pas où il y avait des données. N'a pas trouvé dans Hydroweb. CLS / IRD Legos, mis en contact par le groupe de travail hydro spatial, lui ont traité des données brutes (ici exceptionnellement non fourni par le client / in situ, d'habitude in Situ, mesuré par eux-mêmes - Rhône - ou leur client). Cas un peu exceptionnel 
* Analyser et critiquer: fréquence importante (vérification de la donnée dispo / manquant), tracer débit / temps (détecter les comportements anormaux, type ruptures, données aberrantes), comparaison avec d'autres données (débit VS hauteur par exemple, débit VS débit autres sources, choisit par crédibilité de la source via les exploitants de terrain)
* Mettre au propre
* Caler: donner de précipitation (prévi ou mesure, ça dépend, utilise terrain et données de réanalyse, prévision pour d'autres tâches prévision). Partenariat Météo France. tâche sur plusieurs années
* Valider
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
* BD interne, pour stocker les données hydro
* R (travail de calage). Résultats tableaux et graphiques (R Studio)
</span>
  * Quels points forts?
<span class="user-answer">
* R => Très utilisé en hydro, possibilité de se partager les libs (AIRGR contient les modèles de l'INRAE en OpenSource, déjà codé) 
* BD: Répond à son besoin précisément, acquisition à fréquence < heure. Recherche par nom station, carto
</span>
  * Quels points d'amélioration?
<span class="user-answer">
Nop
</span>
  * Quels points d'intégration?
<span class="user-answer">
X
</span>
* Quelles données? 
<span class="user-answer">

</span>
  * Neige (couverture / produits dérivés)
<span class="user-answer">
OUI, ils ont un outil utilisant Caméra et Modis (satellite Aqua & Terra) pour faire le suivi du manteau neigeux
</span>
  * SWE (volume eau / neige)
<span class="user-answer">
OUI (ils travaillent dessus): le plus intéressant pour eux (par rapport à la couverture)
</span>
  * Surface d'eau (pixel eau)
<span class="user-answer">
Oui (info sup pour eux là où c'est géré par d'autres), à voir
</span>
  * Hauteur d'eau
<span class="user-answer">
Oui, moins intéressant / pertinent que le débit, intéressant pour le déduire
</span>
  * Débit d'eau
<span class="user-answer">
Oui (max)
</span>
  * Température
<span class="user-answer">
Pas trop (n'utilisent pas vraiment), content de savoir que ça existe
</span>
  * Turbidité
<span class="user-answer">
Même réponse
</span>
  * Autres?
<span class="user-answer">
* Donnée météo (précipitations)
* ETP
* vent
* humidité du sol (pourrait, pour de l'étiage par exemple, mais pas utilisé aujourd'hui)
* rayonnement (à creuser): éolien, photovoltaïque?
* nébulosité (à creuser): éolien, photovoltaïque?
</span>
* Quelles méthodes
  * d'exploitation
<span class="user-answer">

</span>
  * de comparaison
<span class="user-answer">

</span>
  * d'extrapolation
<span class="user-answer">

</span>
* Tâche métier actuellement bien outillée?
<span class="user-answer">
* Manque de données (tous types, hydro (débit), météo, MNT). Ils s'en sortent sur les précitation
</span>
  * Totalement couverte?
<span class="user-answer">
Oui
</span>
* Quels points pénibles (outils / données / volumétrie / format / etc...)
<span class="user-answer">
* Mauvaise qualité des données: lacunes, incohérence, imprécision, période mesurée trop courte. Temps de travail liés important.
* La prévision requiert une mise à disposition rapide (attente sous quelques minutes, moins d'1h). Les données de calage doivent être disponibles **après le calage**.
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
Il y en a et ils sont dans certaines:
* Principalement EDA méthodes et techniques requises (hydro et modélisation, spatial)
* Comparaisons aux problématiques et solutions des autres
* Retraitement des données satellitaires parfois
**Indispendable**
</span>
* Que souhaiteriez-vous apporter à la communauté?
<span class="user-answer">
La même chose! Progression mutuelle.
Reverse aujourd'hui des données à la banque hydro.
</span>

## Ouverture

* Disponible peu (1/2 journée mois) pour participer à la conception
<span class="user-answer">
A rediscuter en interne. Reviens vers nous.
</span>
* Qu'est ce qui vous ferait gagner du temps?
<span class="user-answer">
* Temps de calcul
* Faciliter la récupération des données sur une interface et mise en forme des données adaptée
</span>
* POST: Quelles solutions dans un monde idéal?
<span class="user-answer">

</span>

<style>
.user-answer {
  color: darkcyan;  
}
</style>
