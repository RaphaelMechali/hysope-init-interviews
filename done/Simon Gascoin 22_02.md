# Interviews Hysope II

## Volet général

* Présentation (nom métier, organisme, formation universitaire)
<span class="user-answer">
Chercheur CNRS (étude spatiale de l'atmoshère)
Edtudes: hydrologie
Focus sur le manteau neigeux en montagne (télédétection)
</span>
  * Plutôt opérationnel? Scientifique? Archi / bureau d'étude?
<span class="user-answer">
recherche scientifique, en contact avec des opérationnels
</span>
* Quel tâche métier principale? 
<span class="user-answer">
Traitement de données satellitaire
</span>
  * Pour quel résultat?
<span class="user-answer">
Etude du manteau neigeux:
* Etendue (cartographie)
* Epaisseur / équivalent eau
Caractériser la ressource en eau associer au manteau neigeux
</span>
  * Pour qui?
<span class="user-answer">
Communauté scientifique
Perspective opérationnelle / application possible (usages agri / industriels / gestionnaires de l'eau)
</span>
  * Comment?
<span class="user-answer">
Articles / conférences (et produits Théia), ateliers (workshops)
Réseau sociaux (sensibilisation grand public)
</span>
  * Etapes?
<span class="user-answer">
Méthode A, travail fini (Local, HPC):
* Téléchargement 
* Traitement (scipts, partiellement repris)
Méthode B (nouvelle mais ne remplace pas toujours), travail exploratoire:
* Traitement directement dans le cloud (GEE, Sentinel Hub)
Choix expliqué par le manque de flexibilité des outils dont ils disposent
</span>
* Quelles tâches métiers secondaire? (sous-tâches ou tâches parallèles?)
<span class="user-answer">
Gestion / encadrement personnel / étudiants
Rédaction documentaire (publi, rapports)
Réunions
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
* Carto: QGis / Python / Mathlab (reproj, decoupe, extraction de bandes + traitement de données), éventuellement en bash la première partie / GEE / SentinelHub
* HPC (notebook Jupiter, très bien)
* suite Office, suite Google
* Simulateur Fortran du manteau neigeux
* Latek < Word < Overleaf
</span>
  * Quels points forts?
<span class="user-answer">
* Mathlab par exemple: expérience / expertise
* Python: HPC, collaboration facile, mieux pour la massification des traitements
</span>
  * Quels points d'amélioration?
<span class="user-answer">
* Mise à jour pénible, environnement obsolètes (perte de temps)
* HPC: pas de téléchargement facile depuis un navigateur internet, ça rame, le bureau virtuel galère (n'a jamais réussi a le faire fonctionner): l'utilise uniquement en terminal
</span>
  * Quels points d'intégration?
<span class="user-answer">

</span>
* Quelles données? 
<span class="user-answer">
* ont des stations de mesure in situ 
* utilisent des données de Météo France in situ
</span>
  * Neige (couverture / prduits dérivés)
<span class="user-answer">
Oui
</span>
  * SWE (volume eau / neige)
<span class="user-answer">
Oui
</span>
  * Surface d'eau (pixel eau)
<span class="user-answer">
Oui: a besoin d'éliminer les surfaces d'eau pour les cartes de neiges (utilisent des cartes statiques, aimeraient passer à du dynamique). Partenariat avec une équipe du CNES
</span>
  * Hauteur d'eau
<span class="user-answer">
non
</span>
  * Débit d'eau
<span class="user-answer">
non mais on devrait : validation du stock de neige à partir du débit (accord d'échange de données avec EDF complexe). Comparer les estimations de stock avec le débit des rivières
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
* Données météo in situ / modèles:
  * Précipitation
  * Température
  * Humidité
  * Vent
  * Direction du vent
  * Rayonnement
* ETP
* Aérosols atmosphériques
* Occupation des sols (algo différents en fonction de forêt / agri), couverture forestière (densité)
* MNT > topographie
</span>
* Quelles méthodes
  * d'exploitation
<span class="user-answer">
* Carte / graphique (support dépend du type): durée / surface enneigement, images satellites brutes (pédagogie: fonctionnement des algo)
* Modèle de neige SNOW MODEL: analytique. Caractérise le manteau neigeux (SWE)
</span>
  * de comparaison
<span class="user-answer">
* données hydro: comparaison visuelle de séries temporelles
* peu d'automatisation
</span>
  * d'extrapolation
<span class="user-answer">
* calcul de carte d'enneigement interpolée et extrapolée au niveau temporel (et continuité) pour comparer à des données in situ ou des sorties de modèles
</span>
* Tâche métier actuellement bien outillée?
<span class="user-answer">
* HPC très positif
* Travail collaboratif moins
  * Dispositifs différents entre les organismes
  * Manque d'uniformité
</span>
  * Totalement couverte?
<span class="user-answer">

</span>
* Quels points pénibles (outils / données / volumétrie / format / etc...)
<span class="user-answer">
* Gestion des volumes de données
* Suivi des environnement de travail (MAJ version Python et similaires), reprise ultérieures
* Gestion info (installation de soft compliquée en interne au Cesbio)
</span>
* Illustrer tâche métier durant l'interview? (si moins de 20 minutes)
<span class="user-answer">

</span>

## Volet intégration HI2

* Etes vous familiers avec les services Theia?
<span class="user-answer">
Oui
</span>
* Utilisez-vous des données Theia régulièrement?
<span class="user-answer">
Oui
</span>
* Accédez-vous régulièrement à des produits CNES (peps / cdpp / hydroweb / theia similaires...)
<span class="user-answer">
* Theia
* Peps
* HPC (notebook Jupiter HPC)
* GitLab de l'OTB pour leur chaîne de traitement de la neige
* SentinelHub
* Google Earth Engine
* Pleiade (CNES ou Geostore Airbus)
* Données climatiques (oceanwf - NASA)
* Données satellite NASA (nsidc neige et glace)
* NASA Reverb
* Landsat (USGS)
</span>

## Communauté

* Que pourrait vous apporter la communauté?
<span class="user-answer">
* Données librement accessible (notamment météo)
* Collaboration
* Veille techno
* Veille bibliographique (trop de publication pour suivre): définir ses problématiques et son travail (EDA)
</span>
* Que souhaiteriez-vous apporter à la communauté?
<span class="user-answer">
* Support à l'utilisation des données S1 et S2
</span>

## Ouverture

* Disponible peu (1/2 journée mois) pour participer à la conception
<span class="user-answer">
Oui
</span>
* Qu'est ce qui vous ferait gagner du temps?
<span class="user-answer">
Petits inconvénients quotidiens (maintenance informatique sans fin, petits bugs)
</span>
* POST: Quelles solutions dans un monde idéal?
<span class="user-answer">
GEE c'est top bien! Mais sans limitation en terme de temps calcul et plus assez flexible pour l'incorporation de code externe (et surtout indépendant des GAFA, transparent et éthique)
QGis est génial quand même
</span>

<style>
.user-answer {
  color: darkcyan;  
}
</style>
