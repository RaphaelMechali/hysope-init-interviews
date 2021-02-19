# Interviews Hysope II

## Volet général

* Présentation (nom métier, organisme, formation universitaire)
<font color="darkcyan">
Ingénieur prédict (météo France / airbus / VRL) => gestion des risques naturels
spatial -> analyse risque inondation (estimation précipitation > estimation zones inondables)
international (assistance aux sites industriels / assurances), 95 pays
Vise à informer en temps réels les usagers des risques en cours (météo, volcano, etc...)
</font>
  * Plutôt opérationnel? Scientifique? Archi / bureau d'étude?
<font color="darkcyan">
Plutôt opérationnels
</font>
* Quel tâche métier principale? 
<font color="darkcyan">
* Sortie modèle météo (CEP, GFS) => Analyse initiale
* Recroisement avec les in situ et radar (locaux) ou estimation de pluie par satellite pour estimations des niveaux d'inondation
* Gestion des l'évènement (alerte -> suivi): Données et retour terrain
</font>
  * Pour quel résultat?
<font color="darkcyan">
Envoie d'alerte par territoire aux usagers (plateforme admin / usager). 
Plusieurs niveaux d'alerte (par ampleur):
* Soyez vigilant
* Mobilisation 
* Prise d'action
* Renforcement d'action
Les sites / territoires disposent d'estimation de vulnérabilité pour soutenir la décision des actions. Mais les actions à prendre sont sélectionnées manuellement.
</font>
  * Pour qui?
<font color="darkcyan">
  assureur des sites et industriels / collectivités en France (mais peu à l'international)
</font>
  * Comment?
<font color="darkcyan">
Contact par la plateforme
</font>
  * Etapes?
<font color="darkcyan">
cf. tâche
</font>
* Quelles tâches métiers secondaire? (sous-tâches ou tâches parallèles?)
<font color="darkcyan">
* Recherche de données (toujours en cours, déjà bien riche mais souvent complété) et estimation de fiabilité avant insertion dans la banque de donnée centrale
</font>
  * Pour quel résultat?
<font color="darkcyan">
Enrichissement de la banque de données centrales
</font>
  * Pour qui? (lui-même ?)
  <font color="darkcyan">

</font>
  * Comment?
  <font color="darkcyan">
En galérant un peu (recherche à droite à gauche)
</font>
* Quels outils actuels?
<font color="darkcyan">
* Plateforme communication (outil web évoqué précédemment)
* Globe 3D type SIG basé sur Skyline (couple vulnérabilité ~ infrastructure et l'aléa ~ précipitation ==> décisionnel) -> 3D pour relief / ruissellement. La 3D permet de visualiser les quantités de pluies à l'échelle du bassin versant
</font>
  * Quels points forts?
<font color="darkcyan">
* Adaptatifs
* Intuitifs
</font>
  * Quels points d'amélioration?
<font color="darkcyan">
* Manque de personnalisation (c'est pénible de repasser pas l'équipe de dev pour rajouter)
</font>
  * Quels points d'intégration?
<font color="darkcyan">
* Banque de données centrales
</font>
* Quelles données? 
<font color="darkcyan">
Données de suivi:
* Radar local
* Vigicru France
* hors Europe:
  * s'appuie sur Sentinel malgré les limites (nuages, petits cours d'eau) pas terrible pour les petits Bassins Versant
  * quelques mesures in situ mais gros manques. A fait une recherche sur ce qui existe en fonction des pays. A obtenu une banque de données riche (in situ, radar, modèles météo)
Ont utilisé 'Float observatory' avant Hydroweb 1 (pour calculer une tendance). La fréquence des données Hydroweb est trop faible (le temps de mise à disposition est moins grave pour les grands BV, à cause du temps de propagation des crues).  
</font>
  * Neige (couverture / produits dérivés)
<font color="darkcyan">
Oui (contexte défavorable)
</font>
  * SWE (volume eau / neige)
<font color="darkcyan">
Oui
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
Non
</font>
  * Turbidité
<font color="darkcyan">
Non
</font>
  * Autres?
<font color="darkcyan">
Exhaustif pour lui (ne s'intéresse pas autant à précipitation / vent, mais ça reste intéressant) => serait preneur vent observé
Utilise les lames d'eau (pluvio radar, recalibré avec mesure au sol)
Utilise aussi orthophotographie IGN et images Pleïades
</font>
* Quelles méthodes
  * d'exploitation
<font color="darkcyan">
95% expertise humaine (veille météo, carte de risques ==> ciblage des points chaud par la quantité de pluie OU les rafales de vent etc)
</font>
  * de comparaison
<font color="darkcyan">
* Utilise paramètres hydro (hauteur => impact) === Vigicrue
* Capitalise sur les évènements déjà survenus chez eux (y compris satellitte )
</font>
  * d'extrapolation
<font color="darkcyan">

</font>
* Tâche métier actuellement bien outillée?
<font color="darkcyan">
Oui
</font>
  * Totalement couverte?
<font color="darkcyan">
Oui, bémol ==> ajoute de l'IA pour aider à la prise de décision
</font>
* Quels points pénibles (outils / données / volumétrie / format / etc...)
<font color="darkcyan">
gros point négatif: manque de données sur lesquelles s'appuyer sur de nombreux territoires (suivi des cours d'eau à l'international, hors Amérique / Europe)
</font>
* Illustrer tâche métier durant l'interview? (si moins de 20 minutes)
<font color="darkcyan">
cf. screenshot
</font>

## Volet intégration HI2

* Etes vous familiers avec les services Theia?
<font color="darkcyan">
Non s'en sert rarement (manque de connaissance / formation). Hydroweb n'a pas été retenu (donnée peu fiable, estimée notamment pendant la crue du Niger)
</font>
* Utilisez-vous des données Theia régulièrement?
<font color="darkcyan">
Non
</font>
* Accédez-vous régulièrement à des produits CNES (peps / cdpp / hydroweb / theia similaires...)
<font color="darkcyan">
Non
</font>

## Communauté

* Que pourrait vous apporter la communauté?
<font color="darkcyan">
* Entraide
  * Utilisation des données
* Echanges notamment les locaux > qui pourrait me fournir des données
</font>
* Que souhaiteriez-vous apporter à la communauté?
<font color="darkcyan">
* Retour opérationnel
</font>

## Ouverture

* Disponible peu (1/2 journée mois) pour participer à la conception
<font color="darkcyan">
Oui carrément
</font>
* Qu'est ce qui vous ferait gagner du temps?
<font color="darkcyan">

</font>
* POST: Quelles solutions dans un monde idéal?
<font color="darkcyan">
toutes données openSource, intégrables, récupérables, facilité de partage.
Note: ils utilisent essentiellement des flux WMS
</font>


