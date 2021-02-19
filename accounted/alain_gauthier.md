# Interviews Hysope II

## Volet général

* Présentation (nom métier, organisme, formation universitaire)
<font color="darkcyan">Bureau d'étude Eaucéa (environnement / gestion de l'eau) - petite équipe: modélise, développe (scripts de traitement de donnée), accès à la donnée hydro. Formation initiale: mathématique puis reconversion ENSEIT (1 an). 
Eaucéa:
* travaillent beaucoup sur l'étiage (réserve, partage, ressources, retenues collinaires)
* activité travaux MAO barrages hydro
* étude d'impact débit / qualité des milieux aquatiques (+autorisation de prélèvement)
* bathymétrie (mesure du bassin)
</font>
  * Plutôt opérationnel? Scientifique? Archi / bureau d'étude?
  <font color="darkcyan">OP / BE (mais exploitation de résultats issus de la recherche scientifique "hydrologie naturelle" des bassins, ie l'usage / l'impact OU enjeux de changements climatiques)</font>
* Quel tâche métier principale? 
<font color="darkcyan">
En fonction des périodes: 
* prévision hydrologique (6 mois année): anticiper "soutien d'étiage" (de la Garonne, répond aux normes d'usage et d'environnement):
  * résultat: outil d'aide à la gestion en ligne e-tiage (service).
  * Comment: données observées et prévisions météo + modèle GR4J (adapté et semi-distribué en sous bassin versant) + intégration usages => prévision à 3/4j ou 8-10j bassin Charente. Les lâchers hydro-électriques viennent perturber les précisions.
    * Données observées: fonction des bassins. 
      * Données hydrométriques (stations temps-réels ou proche)
      * API Hubeau (moins privilégiée)
      * Géoportail IGN
      * L'"adreal"??, de la CACG, etc. ont tous des conventions différentes.
      * Station spécifique pour l'ETP (par météofrance). 
      * lame d'eau Antilope par exemple (par contrat avec meteoFrance).
      * Prévision et relevés météo
* développement (scripting python): modèles implémentés en Python. Automatisation de la récupération des données (pour étude ponctuelle ou flux pour la chaîne de prévision du premier point ou analyse statistique scripté, recodage modèle hydro)
* Modélisation hydro et support modélisation (même données qie soutien d'étiage + données SIG + données SIE (Système d'Information de l'Eau, service publique): scripts de fonctionnalités mis à disposition)
</font>
  * Pour quel résultat?
  <font color="darkcyan">service</font>
  * Pour qui?
  <font color="darkcyan">EPTB (Etablissement Public Territorial de Bassin). Syndicat mixte d'aménagement de la Garonne, EPTB de la Charente</font>
  * Comment?
  <font color="darkcyan">
modèle hydrologique GR4J (INRAE) --> modèle semi-distribué (sous-bassins) sur amont vers aval avec usage --> anticiper les besoins et les usages --> soutien à l'étiage sur 3-4j, jusqu'à 8-10j suivant les bassins. Les lâchers hydro-électriques perturbe le système et complexifie la prévision
Données observées = stations hydrométriques temps réel/quasi-réelle (API Hub'eau, et convention des clients avec les producteurs de données CACGascogne, EDF, DREAL); achats méteo-France pour la prévi (lame d'eau ANTILOPE cumuls de précipitations, ETP de stations, prévi météorologiques). Résultats bruts meteo-France open data</font>
  * Etapes?
  <font color="darkcyan"></font>
* Quelles tâches métiers secondaire? (sous-tâches ou tâches parallèles?)
<font color="darkcyan">
* admin système
* RAO: peu de données, appréciation plutôt technique. Travaille sur des sujets connexes aux sujets passés.
* Gestion projet
</font>
  * Pour quel résultat?
  <font color="darkcyan"></font>
  * Pour qui? (lui-même ?)
  <font color="darkcyan"></font>
  * Comment?
  <font color="darkcyan"></font>
* Quels outils actuels?
<font color="darkcyan">
* Scripts Python
* Logiciel de modélisation: GR4J, Mart (BRGM, hydrogéologie souterraine), Telemac (hydraulique)
* Hydrométrie (jauge + bateaux drones)
* utilise les théodolites (pour mesurer les niveaux d'eau)
* SIG et QGis
* Webservices (geoportail, Sentinel HUB, service Sandre, banque hydro)
* Outil de recherche de données (SearchEveryThing, leur permet de rechercher dans leurs fichiers/données)
* pack office
* Ils n'ont pas de serveur big data (stockage mais pas de pérennisation formatée systématique, parfois excell, parfois couche formatée...)
</font>
  * Quels points forts?
  <font color="darkcyan">
  Centré projet (pragmatique et efficace). Pas d'obligation à connaître toutes les fonctionnalités / parties
  </font>
  * Quels points d'amélioration?
  <font color="darkcyan">
  * serveur carto Postgre / postgis
  * rationalisation de l'accès aux données: ne sais pas les données disponibles en un point à un moment donnée (centralisation pour l'utilisateur, par meta par exemple)
  </font>
  * Quels points d'intégration?
  <font color="darkcyan"></font>
* Quelles données? 
<font color="darkcyan"></font>
  * Neige (couverture / produits dérivés)
  <font color="darkcyan">pas directement (à cause des territoires étudiés) </font>
  * SWE (équivalent volume eau / neige)
  <font color="darkcyan">même remarques</font>
  * Surface d'eau (pixel eau)
  <font color="darkcyan">oui</font>
  * Hauteur d'eau
  <font color="darkcyan">oui</font>
  * Débit d'eau
  <font color="darkcyan">OUI (principal)</font>
  * Température
  <font color="darkcyan">oui</font>
  * Turbidité
  <font color="darkcyan">oui</font>
  * Autres?
  <font color="darkcyan">
  * volume si possible
  * analyse d'indicateur hydrique du sol (usage de l'eau) = humidité des sols, occupation sol x usage de l'eau. Plutôt pour le soutien d'étiage. Suivi du stock disponible
  * précipitations
  * température de l'air
  * ETP
  </font>
* Quelles méthodes
  * d'exploitation
  <font color="darkcyan">Visualisation en flux 
  * graphes Excell  
    * temporel. Y => suivi des volumes / débit prélèvement / précipitation (météo) / ETP (météo) / temp (météo), qualité (oxygène, turbidité)
    * multi-paramètres. Combinaison de paramètres en analyse (pour dégager une corrélation => param meteo x param hydro x param trisométrique pour évaluer un risque elever)
    * carte. Situation en plusieurs lieux (anticipation pour l'aval, en observant l'amont): visualisent des indicateurs colorés par alarmes (ex Vigicrue: tronçons de rivières colorés), ouvre plusieurs graphes en parallèles. 
  </font>
  * de comparaison
  <font color="darkcyan"></font>
  * d'extrapolation
  <font color="darkcyan">
  * modèles hydro
  * ajout de modèles de propagation (pour du très court terme)
  </font>
* Tâche métier actuellement bien outillée?
<font color="darkcyan">Oui</font>
  * Totalement couverte?
  <font color="darkcyan">(vise justement à ce point particulier)</font>
* Quels points pénibles (outils / données / volumétrie / format / etc...)
<font color="darkcyan">
* Multi-producteur / multi-format, absence de format homogène (manque de convention, traitement des dates infernal, par exemple) => préparation des données (outils Python en général). Craint le fichier PDF ou donnée manuscrite.
* Récolte des données
</font>
* Illustrer tâche métier durant l'interview? (si moins de 20 minutes)
<font color="darkcyan"></font>

## Volet intégration HI2

* Etes vous familiers avec les services Theia?
<font color="darkcyan">A survolé plus fois, n'a pas eu le temps de s'y mettre. A plus d'expérience avec les services de la NASA - earthdata aujoud'hui (pour la Guyanne, programme terminé depuis)</font>
* Utilisez-vous des données Theia régulièrement?
<font color="darkcyan"></font>
* Accédez-vous régulièrement à des produits CNES (peps / cdpp / hydroweb / theia similaires...)
<font color="darkcyan">Il pense à utiliser PEPS, aime google earth engine</font>

## Communauté

* Que pourrait vous apporter la communauté?
<font color="darkcyan">
* plutôt pour les territoires moins équipés / jaugés
* innovation (accès à la R&D institutionnelle)
* ressources matérielles mises à disposition
</font>
* Que souhaiteriez-vous apporter à la communauté?
<font color="darkcyan">
* représentation du besoin d'utilisation (les questions terre à terre des EPTB et agences de l'eau)
</font>

## Ouverture

* Disponible peu (1/2 journée mois) pour participer à la conception
<font color="darkcyan">OK bêta test (plus compliqué pour les RDV fixés) => peut également demander à un collègue pour les bêta tests. Indisponible de juin-octobre</font>
* Qu'est ce qui vous ferait gagner du temps?
<font color="darkcyan">Outils de visu dans les portails bien foutus (pour se débarasser d'Excell), la prévisualisation (graphe, comparaison de données, batimétrie)</font>
* POST: Quelles solutions dans un monde idéal?
<font color="darkcyan"></font>


