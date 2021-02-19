# Interviews Hysope II

## Volet général

* Présentation (nom métier, organisme, formation universitaire)
<font color="darkcyan">spécialiste chimie, problématiques polution de l'eau (en startup). Santé environnement (a dirrigé spnioff du CNRS, digicell), pertubateurs endocriniens, etc... Directeur développement chez Asquassay aujourd'hui (avec codirecteur "Stéphane" ingé gestion de l'eau). Prévoit une transition 'hydrolique' (similairement à la transition énergétique). Spécifiquement: bassin Haute-Garonne (manque à "l'étiage" important, plus impacté en France aujourd'hui). Aquassay propose des plans pour réduire consommation / pollution (qui fait quoi avec l'eau?) Difficile de connaître le consommateur (équipement) réel. </font>
  * Plutôt opérationnel? Scientifique? Archi / bureau d'étude?
  <font color="darkcyan">Plutôt opérationnel, bureau d'étude</font>
* Quel tâche métier principale? 
<font color="darkcyan">
* Identifier les données produites (quantité / qualité des eaux consommées / relâchées) -> nécessite une fréquence d'acquisition régulière (plusieurs fois par jours?)
* Identifie les manques dans les mesures
* Ajoute les élements manquants
* Mesurer les consommations, faire du reporting et comparer les niveaux de consommation / dispo (étude des flux, quantité + qualité - il faut que l'eau soit propre / potable / utilisable dans son contexte).
* Réalise des préconisations (une stratégie de répartition de l'eau dispo, fuites et pertes, recyclage / retraitement...), par acteur (partage réel), plan de réduction.</font>
  * Pour quel résultat?
  <font color="darkcyan">stratégie de consommation de l'eau</font>
  * Pour qui?
  <font color="darkcyan">Groupes industriels</font>
  * Comment?
  <font color="darkcyan">(cf tâche)</font>
  * Etapes?
  <font color="darkcyan">(cf tâche)</font>
* Quelles tâches métiers secondaire? (sous-tâches ou tâches parallèles?)
<font color="darkcyan"></font>
  * Pour quel résultat?
  <font color="darkcyan"></font>
  * Pour qui? (lui-même ?)
  <font color="darkcyan"></font>
  * Comment?
  <font color="darkcyan"></font>
* Quels outils actuels?
<font color="darkcyan">Internes</font>
  * Quels points forts?
  <font color="darkcyan">Top</font>
  * Quels points d'amélioration?
  <font color="darkcyan">En cours (cf. autres points)</font>
  * Quels points d'intégration?
  <font color="darkcyan">NA</font>
* Quelles données? 
<font color="darkcyan"></font>
  * Neige (couverture / produits dérivés)
  <font color="darkcyan">Fonction des régions (plaine Pyrénées) pour calcul de la quantité d'eau stockée. Donc plutôt Volume d'eau. Fréquence quotidienne suffisante</font>
  * SWE (volume eau / neige)
  <font color="darkcyan">OUI (consommateur), aimerait bien une prévision ou un système de prévision corrélé</font>
  * Surface d'eau (pixel eau)
  <font color="darkcyan">non</font>
  * Hauteur d'eau
  <font color="darkcyan">non</font>
  * Débit d'eau
  <font color="darkcyan">non</font>
  * Température
  <font color="darkcyan">oui. Fréquence quotidienne (6h dans l'idéal, mais moyenne acceptable, si elle est bien faite) suffisante. Mesure plus fréquente en sortie d'usine (micro)</font>
  * Turbidité
  <font color="darkcyan">oui</font>
  * Autres?
  <font color="darkcyan">
  * matière en suspension (<= turbidité>) (Note de Lionel S2,S3)
  * analyse chimique (fréquence basse, cher techniquement)
  * conductivité
  * PH
  En général: mesures fréquentes pour pilotage (même si délai d'update est OK), mesures moins fréquentes pour éléments en entrée (pilotage temps réels VS simu / compréhension)
  </font>
* Quelles méthodes
  * d'exploitation
  <font color="darkcyan">graphiques temporels</font>
  * de comparaison
  <font color="darkcyan">détection des pics ou "anomalies", IA envisagée</font>
  * d'extrapolation
  <font color="darkcyan">NA</font>
* Tâche métier actuellement bien outillée?
<font color="darkcyan">A sa propre solution AWS (big data, données hétérogènes dans la fréquence et la localisation): OUI, mais endroits non opérationnels (les stations d'épuration ne savent pas pousser leurs données). Note: accepte une fréquence de mise à jour  </font>
  * Totalement couverte?
  <font color="darkcyan">Dev en cours (data / mise à disposition). Applicatif: oui. Modèles (intelligence métier): en cours mais 90% fait (réfléchit à de l'IA, mais pour l'instant besoins basiques)</font>
* Quels points pénibles (outils / données / volumétrie / format / etc...)
<font color="darkcyan">Capteurs "environnementaux" mal référencés (ils ont besoin de retrouver ce qui ce fait à côté: sondes, étaudes hydro, même études population animale, qui peuvent corroborer leur conclusions)</font>
* Illustrer tâche métier durant l'interview? (si moins de 20 minutes)
<font color="darkcyan">screenshot JEG-analyse</font>

## Volet intégration HI2

* Etes vous familiers avec les services Theia?
<font color="darkcyan"></font>
* Utilisez-vous des données Theia régulièrement?
<font color="darkcyan"></font>
* Accédez-vous régulièrement à des produits CNES (peps / cdpp / hydroweb / theia similaires...)
<font color="darkcyan"></font>

## Communauté

* Que pourrait vous apporter la communauté?
<font color="darkcyan">2 aspects importants: 
* mise en commun et partage de données (nous envoi un conf qu'il a fait sur l'analyse systémique).
* Niveau faible en hydro ==> Avoir de l'aide technique des hydrologues de métier
</font>
* Que souhaiteriez-vous apporter à la communauté?
<font color="darkcyan">
* Nous indique que nous pourrions aggréger les données des stations d'épuration et industriels. (Comment les y amener?)
* Leur approche opérationnel de la conso d'eau (souhaite démocratiser son approche et domaine)
</font>

## Ouverture

* Disponible peu (1/2 journée mois) pour participer à la conception
<font color="darkcyan">Plutôt oui</font>
* Qu'est ce qui vous ferait gagner du temps?
<font color="darkcyan"></font>
* POST: Quelles solutions dans un monde idéal?
<font color="darkcyan">HI2 pourrait centraliser les données des grands groupes industriels pour eux</font>


