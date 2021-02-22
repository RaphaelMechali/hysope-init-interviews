# Interviews Hysope II

## Volet général

* Présentation (nom métier, organisme, formation universitaire)
<span class="user-answer">
Ingénieur prédict (météo France / airbus / VRL) => gestion des risques naturels
spatial -> analyse risque inondation (estimation précipitation > estimation zones inondables)
international (assistance aux sites industriels / assurances), 95 pays
Vise à informer en temps réels les usagers des risques en cours (météo, volcano, etc...)
</span>
  * Plutôt opérationnel? Scientifique? Archi / bureau d'étude?
<span class="user-answer">
Plutôt opérationnels
</span>
* Quel tâche métier principale? 
<span class="user-answer">
* Sortie modèle météo (CEP, GFS) => Analyse initiale
* Recroisement avec les in situ et radar (locaux) ou estimation de pluie par satellite pour estimations des niveaux d'inondation
* Gestion des l'évènement (alerte -> suivi): Données et retour terrain
</span>
  * Pour quel résultat?
<span class="user-answer">
Envoie d'alerte par territoire aux usagers (plateforme admin / usager). 
Plusieurs niveaux d'alerte (par ampleur):
* Soyez vigilant
* Mobilisation 
* Prise d'action
* Renforcement d'action
Les sites / territoires disposent d'estimation de vulnérabilité pour soutenir la décision des actions. Mais les actions à prendre sont sélectionnées manuellement.
</span>
  * Pour qui?
<span class="user-answer">
  assureur des sites et industriels / collectivités en France (mais peu à l'international)
</span>
  * Comment?
<span class="user-answer">
Contact par la plateforme
</span>
  * Etapes?
<span class="user-answer">
cf. tâche
</span>
* Quelles tâches métiers secondaire? (sous-tâches ou tâches parallèles?)
<span class="user-answer">
* Recherche de données (toujours en cours, déjà bien riche mais souvent complété) et estimation de fiabilité avant insertion dans la banque de donnée centrale
</span>
  * Pour quel résultat?
<span class="user-answer">
Enrichissement de la banque de données centrales
</span>
  * Pour qui? (lui-même ?)
  <span class="user-answer">

</span>
  * Comment?
  <span class="user-answer">
En galérant un peu (recherche à droite à gauche)
</span>
* Quels outils actuels?
<span class="user-answer">
* Plateforme communication (outil web évoqué précédemment)
* Globe 3D type SIG basé sur Skyline (couple vulnérabilité ~ infrastructure et l'aléa ~ précipitation ==> décisionnel) -> 3D pour relief / ruissellement. La 3D permet de visualiser les quantités de pluies à l'échelle du bassin versant
</span>
  * Quels points forts?
<span class="user-answer">
* Adaptatifs
* Intuitifs
</span>
  * Quels points d'amélioration?
<span class="user-answer">
* Manque de personnalisation (c'est pénible de repasser pas l'équipe de dev pour rajouter)
</span>
  * Quels points d'intégration?
<span class="user-answer">
* Banque de données centrales
</span>
* Quelles données? 
<span class="user-answer">
Données de suivi:
* Radar local
* Vigicru France
* hors Europe:
  * s'appuie sur Sentinel malgré les limites (nuages, petits cours d'eau) pas terrible pour les petits Bassins Versant
  * quelques mesures in situ mais gros manques. A fait une recherche sur ce qui existe en fonction des pays. A obtenu une banque de données riche (in situ, radar, modèles météo)
Ont utilisé 'Float observatory' avant Hydroweb 1 (pour calculer une tendance). La fréquence des données Hydroweb est trop faible (le temps de mise à disposition est moins grave pour les grands BV, à cause du temps de propagation des crues).  
</span>
  * Neige (couverture / produits dérivés)
<span class="user-answer">
Oui (contexte défavorable)
</span>
  * SWE (volume eau / neige)
<span class="user-answer">
Oui
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
Non
</span>
  * Turbidité
<span class="user-answer">
Non
</span>
  * Autres?
<span class="user-answer">
Exhaustif pour lui (ne s'intéresse pas autant à précipitation / vent, mais ça reste intéressant) => serait preneur vent observé
Utilise les lames d'eau (pluvio radar, recalibré avec mesure au sol)
Utilise aussi orthophotographie IGN et images Pleïades
</span>
* Quelles méthodes
  * d'exploitation
<span class="user-answer">
95% expertise humaine (veille météo, carte de risques ==> ciblage des points chaud par la quantité de pluie OU les rafales de vent etc)
</span>
  * de comparaison
<span class="user-answer">
* Utilise paramètres hydro (hauteur => impact) === Vigicrue
* Capitalise sur les évènements déjà survenus chez eux (y compris satellitte )
</span>
  * d'extrapolation
<span class="user-answer">

</span>
* Tâche métier actuellement bien outillée?
<span class="user-answer">
Oui
</span>
  * Totalement couverte?
<span class="user-answer">
Oui, bémol ==> ajoute de l'IA pour aider à la prise de décision
</span>
* Quels points pénibles (outils / données / volumétrie / format / etc...)
<span class="user-answer">
gros point négatif: manque de données sur lesquelles s'appuyer sur de nombreux territoires (suivi des cours d'eau à l'international, hors Amérique / Europe)
</span>
* Illustrer tâche métier durant l'interview? (si moins de 20 minutes)
<span class="user-answer">
cf. screenshot
</span>

## Volet intégration HI2

* Etes vous familiers avec les services Theia?
<span class="user-answer">
Non s'en sert rarement (manque de connaissance / formation). Hydroweb n'a pas été retenu (donnée peu fiable, estimée notamment pendant la crue du Niger)
</span>
* Utilisez-vous des données Theia régulièrement?
<span class="user-answer">
Non
</span>
* Accédez-vous régulièrement à des produits CNES (peps / cdpp / hydroweb / theia similaires...)
<span class="user-answer">
Non
</span>

## Communauté

* Que pourrait vous apporter la communauté?
<span class="user-answer">
* Entraide
  * Utilisation des données
* Echanges notamment les locaux > qui pourrait me fournir des données
</span>
* Que souhaiteriez-vous apporter à la communauté?
<span class="user-answer">
* Retour opérationnel
</span>

## Ouverture

* Disponible peu (1/2 journée mois) pour participer à la conception
<span class="user-answer">
Oui carrément
</span>
* Qu'est ce qui vous ferait gagner du temps?
<span class="user-answer">

</span>
* POST: Quelles solutions dans un monde idéal?
<span class="user-answer">
toutes données openSource, intégrables, récupérables, facilité de partage.
Note: ils utilisent essentiellement des flux WMS
</span>

<style>
.user-answer {
  color: darkcyan;  
}
</style>
