# Interviews Hysope II

## Volet général

* Présentation (nom métier, organisme, formation universitaire)
<font color="darkcyan">
Ingénieur généraliste (Les mines St Etienne), Compagnie Nationale du Rhone, travaille en modélisation hydro (concessionaire du fleuve Rhone => en 1930 l'état leur procure le contrat de gestion et d'exploitation => navigation, irrigation, electricité, 1/4 prod hydro elec française, 14 écluses...). Travaille à la direction de l'ingénierie, autres missions ==> projet spatial bassin du Congo et altimétrie spatiale (membre de SWOT).
Peu d'outils universitaires encore utilisés (hors stats)
</font>
  * Plutôt opérationnel? Scientifique? Archi / bureau d'étude?
<font color="darkcyan">
Interne: appui exploitation (opérationnel)
Externe: bureau d'étude
</font>
* Quel tâche métier principale? 
<font color="darkcyan">
gestion de projet
récupération de jeux en hydro, analyse et critique, mise au propre (données manquantes, aberrantes, conversion éventuelle), puis caler un modèle (souvent décider en amont) => calage / validation
Modèles GR ou autres en fonction du besoin (échelle Grand BV, par ex Congo 150 000 km², Rhône découpé en 22 affluents)
</font>
  * Pour quel résultat?
<font color="darkcyan">
Modèle pertinent répondant au besoin du client (prévision de débit notamment)
</font>
  * Pour qui?
<font color="darkcyan">
client ou lui même. Raccrocher le modèle au système info et décision
</font>
  * Comment?
<font color="darkcyan">
Critère de validation.
Modèle de chroniques comparés à l'observés. Route Min Square Error (erreur quadra), MAE (Min Absolute Error) ~MAD (précision Lionel la nomenclature) critères de bilan (bilan bien retrouvé sur une année), Critère de persistence (pour prédictif) => quantifié l'apport du modèle par rapport à un modèle "naïf"
</font>
  * Etapes?
<font color="darkcyan">
* Récupérer des jeux: Ex au Congo (hauteur Sanga, affluent) ==> Ne savait pas où il y avait des données. N'a pas trouvé dans Hydroweb. CLS / IRD Legos, mis en contact par le groupe de travail hydro spatial, lui ont traité des données brutes (ici exceptionnellement non fourni par le client / in situ, d'habitude in Situ, mesuré par eux-mêmes - Rhône - ou leur client). Cas un peu exceptionnel 
* Analyser et critiquer: fréquence importante (vérification de la donnée dispo / manquant), tracer débit / temps (détecter les comportements anormaux, type ruptures, données aberrantes), comparaison avec d'autres données (débit VS hauteur par exemple, débit VS débit autres sources, choisit par crédibilité de la source via les exploitants de terrain)
* Mettre au propre
* Caler: donner de précipitation (prévi ou mesure, ça dépend, utilise terrain et données de réanalyse, prévision pour d'autres tâches prévision). Partenariat Météo France. tâche sur plusieurs années
* Valider
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
* BD interne, pour stocker les données hydro
* R (travail de calage). Résultats tableaux et graphiques (R Studio)
</font>
  * Quels points forts?
<font color="darkcyan">
* R => Très utilisé en hydro, possibilité de se partager les libs (AIRGR contient les modèles de l'INRAE en OpenSource, déjà codé) 
* BD: Répond à son besoin précisément, acquisition à fréquence < heure. Recherche par nom station, carto
</font>
  * Quels points d'amélioration?
<font color="darkcyan">
Nop
</font>
  * Quels points d'intégration?
<font color="darkcyan">
X
</font>
* Quelles données? 
<font color="darkcyan">

</font>
  * Neige (couverture / produits dérivés)
<font color="darkcyan">
OUI, ils ont un outil utilisant Caméra et Modis (satellite Aqua & Terra) pour faire le suivi du manteau neigeux
</font>
  * SWE (volume eau / neige)
<font color="darkcyan">
OUI (ils travaillent dessus): le plus intéressant pour eux (par rapport à la couverture)
</font>
  * Surface d'eau (pixel eau)
<font color="darkcyan">
Oui (info sup pour eux là où c'est géré par d'autres), à voir
</font>
  * Hauteur d'eau
<font color="darkcyan">
Oui, moins intéressant / pertinent que le débit, intéressant pour le déduire
</font>
  * Débit d'eau
<font color="darkcyan">
Oui (max)
</font>
  * Température
<font color="darkcyan">
Pas trop (n'utilisent pas vraiment), content de savoir que ça existe
</font>
  * Turbidité
<font color="darkcyan">
Même réponse
</font>
  * Autres?
<font color="darkcyan">
* Donnée météo (précipitations)
* ETP
* vent
* humidité du sol (pourrait, pour de l'étiage par exemple, mais pas utilisé aujourd'hui)
* rayonnement (à creuser): éolien, photovoltaïque?
* nébulosité (à creuser): éolien, photovoltaïque?
</font>
* Quelles méthodes
  * d'exploitation
<font color="darkcyan">

</font>
  * de comparaison
<font color="darkcyan">

</font>
  * d'extrapolation
<font color="darkcyan">

</font>
* Tâche métier actuellement bien outillée?
<font color="darkcyan">
* Manque de données (tous types, hydro (débit), météo, MNT). Ils s'en sortent sur les précitation
</font>
  * Totalement couverte?
<font color="darkcyan">
Oui
</font>
* Quels points pénibles (outils / données / volumétrie / format / etc...)
<font color="darkcyan">
* Mauvaise qualité des données: lacunes, incohérence, imprécision, période mesurée trop courte. Temps de travail liés important.
* La prévision requiert une mise à disposition rapide (attente sous quelques minutes, moins d'1h). Les données de calage doivent être disponibles **après le calage**.
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
Il y en a et ils sont dans certaines:
* Principalement EDA méthodes et techniques requises (hydro et modélisation, spatial)
* Comparaisons aux problématiques et solutions des autres
* Retraitement des données satellitaires parfois
**Indispendable**
</font>
* Que souhaiteriez-vous apporter à la communauté?
<font color="darkcyan">
La même chose! Progression mutuelle.
Reverse aujourd'hui des données à la banque hydro.
</font>

## Ouverture

* Disponible peu (1/2 journée mois) pour participer à la conception
<font color="darkcyan">
A rediscuter en interne. Reviens vers nous.
</font>
* Qu'est ce qui vous ferait gagner du temps?
<font color="darkcyan">
* Temps de calcul
* Faciliter la récupération des données sur une interface et mise en forme des données adaptée
</font>
* POST: Quelles solutions dans un monde idéal?
<font color="darkcyan">

</font>


