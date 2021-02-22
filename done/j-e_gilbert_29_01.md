# Interviews Hysope II

## Volet général

* Présentation (nom métier, organisme, formation universitaire)
<span class="user-answer">spécialiste chimie, problématiques polution de l'eau (en startup). Santé environnement (a dirrigé spnioff du CNRS, digicell), pertubateurs endocriniens, etc... Directeur développement chez Asquassay aujourd'hui (avec codirecteur "Stéphane" ingé gestion de l'eau). Prévoit une transition 'hydrolique' (similairement à la transition énergétique). Spécifiquement: bassin Haute-Garonne (manque à "l'étiage" important, plus impacté en France aujourd'hui). Aquassay propose des plans pour réduire consommation / pollution (qui fait quoi avec l'eau?) Difficile de connaître le consommateur (équipement) réel. </span>
  * Plutôt opérationnel? Scientifique? Archi / bureau d'étude?
  <span class="user-answer">Plutôt opérationnel, bureau d'étude</span>
* Quel tâche métier principale? 
<span class="user-answer">
* Identifier les données produites (quantité / qualité des eaux consommées / relâchées) -> nécessite une fréquence d'acquisition régulière (plusieurs fois par jours?)
* Identifie les manques dans les mesures
* Ajoute les élements manquants
* Mesurer les consommations, faire du reporting et comparer les niveaux de consommation / dispo (étude des flux, quantité + qualité - il faut que l'eau soit propre / potable / utilisable dans son contexte).
* Réalise des préconisations (une stratégie de répartition de l'eau dispo, fuites et pertes, recyclage / retraitement...), par acteur (partage réel), plan de réduction.</span>
  * Pour quel résultat?
  <span class="user-answer">stratégie de consommation de l'eau</span>
  * Pour qui?
  <span class="user-answer">Groupes industriels</span>
  * Comment?
  <span class="user-answer">(cf tâche)</span>
  * Etapes?
  <span class="user-answer">(cf tâche)</span>
* Quelles tâches métiers secondaire? (sous-tâches ou tâches parallèles?)
<span class="user-answer"></span>
  * Pour quel résultat?
  <span class="user-answer"></span>
  * Pour qui? (lui-même ?)
  <span class="user-answer"></span>
  * Comment?
  <span class="user-answer"></span>
* Quels outils actuels?
<span class="user-answer">Internes</span>
  * Quels points forts?
  <span class="user-answer">Top</span>
  * Quels points d'amélioration?
  <span class="user-answer">En cours (cf. autres points)</span>
  * Quels points d'intégration?
  <span class="user-answer">NA</span>
* Quelles données? 
<span class="user-answer"></span>
  * Neige (couverture / produits dérivés)
  <span class="user-answer">Fonction des régions (plaine Pyrénées) pour calcul de la quantité d'eau stockée. Donc plutôt Volume d'eau. Fréquence quotidienne suffisante</span>
  * SWE (volume eau / neige)
  <span class="user-answer">OUI (consommateur), aimerait bien une prévision ou un système de prévision corrélé</span>
  * Surface d'eau (pixel eau)
  <span class="user-answer">non</span>
  * Hauteur d'eau
  <span class="user-answer">non</span>
  * Débit d'eau
  <span class="user-answer">non</span>
  * Température
  <span class="user-answer">oui. Fréquence quotidienne (6h dans l'idéal, mais moyenne acceptable, si elle est bien faite) suffisante. Mesure plus fréquente en sortie d'usine (micro)</span>
  * Turbidité
  <span class="user-answer">oui</span>
  * Autres?
  <span class="user-answer">
  * matière en suspension (<= turbidité>) (Note de Lionel S2,S3)
  * analyse chimique (fréquence basse, cher techniquement)
  * conductivité
  * PH
  En général: mesures fréquentes pour pilotage (même si délai d'update est OK), mesures moins fréquentes pour éléments en entrée (pilotage temps réels VS simu / compréhension)
  </span>
* Quelles méthodes
  * d'exploitation
  <span class="user-answer">graphiques temporels</span>
  * de comparaison
  <span class="user-answer">détection des pics ou "anomalies", IA envisagée</span>
  * d'extrapolation
  <span class="user-answer">NA</span>
* Tâche métier actuellement bien outillée?
<span class="user-answer">A sa propre solution AWS (big data, données hétérogènes dans la fréquence et la localisation): OUI, mais endroits non opérationnels (les stations d'épuration ne savent pas pousser leurs données). Note: accepte une fréquence de mise à jour  </span>
  * Totalement couverte?
  <span class="user-answer">Dev en cours (data / mise à disposition). Applicatif: oui. Modèles (intelligence métier): en cours mais 90% fait (réfléchit à de l'IA, mais pour l'instant besoins basiques)</span>
* Quels points pénibles (outils / données / volumétrie / format / etc...)
<span class="user-answer">Capteurs "environnementaux" mal référencés (ils ont besoin de retrouver ce qui ce fait à côté: sondes, étaudes hydro, même études population animale, qui peuvent corroborer leur conclusions)</span>
* Illustrer tâche métier durant l'interview? (si moins de 20 minutes)
<span class="user-answer">screenshot JEG-analyse</span>

## Volet intégration HI2

* Etes vous familiers avec les services Theia?
<span class="user-answer"></span>
* Utilisez-vous des données Theia régulièrement?
<span class="user-answer"></span>
* Accédez-vous régulièrement à des produits CNES (peps / cdpp / hydroweb / theia similaires...)
<span class="user-answer"></span>

## Communauté

* Que pourrait vous apporter la communauté?
<span class="user-answer">2 aspects importants: 
* mise en commun et partage de données (nous envoi un conf qu'il a fait sur l'analyse systémique).
* Niveau faible en hydro ==> Avoir de l'aide technique des hydrologues de métier
</span>
* Que souhaiteriez-vous apporter à la communauté?
<span class="user-answer">
* Nous indique que nous pourrions aggréger les données des stations d'épuration et industriels. (Comment les y amener?)
* Leur approche opérationnel de la conso d'eau (souhaite démocratiser son approche et domaine)
</span>

## Ouverture

* Disponible peu (1/2 journée mois) pour participer à la conception
<span class="user-answer">Plutôt oui</span>
* Qu'est ce qui vous ferait gagner du temps?
<span class="user-answer"></span>
* POST: Quelles solutions dans un monde idéal?
<span class="user-answer">HI2 pourrait centraliser les données des grands groupes industriels pour eux</span>

<style>
.user-answer {
  color: darkcyan;  
}
</style>
