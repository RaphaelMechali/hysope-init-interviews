# Interviews Hysope II

## Volet général

* Présentation (nom métier, organisme, formation universitaire)
<span class="user-answer">
Jean François, études Toulouse et thèse ONERA (convection naturelle). Post doc Alberta et impact réchauffement climatique, très tôt.
Assoc. Agen => lutte contre la gelée, grêle, irrigation, etc... (directeur)
Dispose d'un radar météo. S'implique dans le changement climatique. Recherche appliquée (locale à Agen), Erosion
</span>
  * Plutôt opérationnel? Scientifique? Archi / bureau d'étude?
  <span class="user-answer">scientifique</span>
* Quel tâche métier principale? 
<span class="user-answer">Mesure bas coût pour les agriculteurs (+/- chaud). Carte d'érosion. Agralis commercialise leurs résultats de recherche appliquée.
depuis 3 ans Aquafox (système de ): temp, hygromé, vent, pluie, rayonnement, ==> calcul EvapoTranspiration (ETP). en + certaines stations profil d'humidité du sol (sondes capacitives marque Sentek)
système de suivi de la hauteur d'eau ==> capteurs de pression. (mais ne trouve pas pour la qualité de l'eau) -> Aujourd'hui: ils en ont implémenté une vingtaine (toujours partenariat SIGFOX oou GPRS). Projet clipalert > plateforme (niveau d'eau / prévision)
Donnée Sentinel / Radar ==> caractérise parcelles des bassins versant (sans risque avec végétal, risqué: nu / grande pente)
Vise à démocratiser des stations / solutions (moins cher)
</span>
  * Pour quel résultat?
  <span class="user-answer"></span>
  * Pour qui?
  <span class="user-answer">Monde rural (agriculteurs, entreprises, villes villages, délaissé par l'état >> surveillance de crue comprise)</span>
  * Comment?
  <span class="user-answer">plateforme www.aqualis.fr > capteurs capacitifs (Big data cloud). Les clients ont l'appli. </span>
  * Etapes?
  <span class="user-answer"></span>
* Quelles tâches métiers secondaire? (sous-tâches ou tâches parallèles?)
<span class="user-answer">
Formation à distance des techniciens, Gérer les quantités d'eau lâchées par les lacs en été avec la donnée satellitaire et forcer les débits (gestion des réserves d'eau). In situ: étallonage. Imagerie satellitaire => interpolation de donnée et fonctionnement des bassins en amont
</span>
  * Pour quel résultat?
  <span class="user-answer"></span>
  * Pour qui? (lui-même ?)
  <span class="user-answer"></span>
  * Comment?
  <span class="user-answer"></span>
* Quels outils actuels?
<span class="user-answer">QGis</span>
  * Quels points forts?
  <span class="user-answer"></span>
  * Quels points d'amélioration?
  <span class="user-answer"></span>
  * Quels points d'intégration?
  <span class="user-answer"></span>
* Quelles données? 
<span class="user-answer">Sentinel 1, Radar (cartes d'érosion).</span>
  * Neige (couverture / prduits dérivés)
  <span class="user-answer"></span>
  * SWE (volume eau / neige)
  <span class="user-answer"></span>
  * Surface d'eau (pixel eau)
  <span class="user-answer"></span>
  * Hauteur d'eau
  <span class="user-answer">Volume lac collinaires === colinne + barrage de retenue (~50k m3 jusqu'à plusieurs million ou lac amont "décanteur" + lac utilisable, refusé par les écologistes. + de 5k en Haute-Garonne) mais lac petits pas foufou! Pixel 50cm, ils sont preneurs. Petits lacs / petites rivières ne sont pas gérables comme ça</span>
  * Débit d'eau
  <span class="user-answer"></span>
  * Température
  <span class="user-answer"></span>
  * Turbidité
  <span class="user-answer">Travail en cours pour un nouveau capteur (~ qualité, là il sait pas trop encore comment mesurer, l'évolution l'intéresse)</span>
  * Autres?
  <span class="user-answer"></span>
* Quelles méthodes
  * d'exploitation: courbe temporelle, Carte d'érosion 
  <span class="user-answer"></span>
  * de comparaison 
  <span class="user-answer">comparaison à la moyenne (écart type)</span>
  * d'extrapolation
  <span class="user-answer">modèle SAFI (évolution biomasse, réserve hydrique). Sonde pour étallonage et image pour extrapoler (+bilan hydrique complexe fourni par la station aquafox, Agri Sud-Ouest Innovation)</span>
* Tâche métier actuellement bien outillée?
<span class="user-answer">en attente de ce qui est en cours avec Amazon (AWS). Utilise QGis, à la mano</span>
  * Totalement couverte?
  <span class="user-answer">Non, en cours</span>
* Quels points pénibles (outils / données / volumétrie / format / etc...)
<span class="user-answer">Climalert > quizaine d'image à traiter (sentinel) mais capacité de traitement à 3. Puissance de calcul! Automatisation. Sentinel est inconstant (été dernier: 1 jour sans image). Récupère sur Copernicus (PEPS, Theia). Harmonisation / disposition de la donnée (différence couche WMS, WMS, Cartage, ...). Certaines n'ont pas les cours d'eau. Données à trous.</span>
* Illustrer tâche métier durant l'interview? (si moins de 20 minutes)
<span class="user-answer"></span>

## Volet intégration HI2

* Etes vous familiers avec les services Theia?
<span class="user-answer">Oui (beaucoup, parce que plateforme pas) Téléchargement compliqué (nouvelle version). Copernicus beaucoup plus simple (scihub)</span>
* Utilisez-vous des données Theia régulièrement?
<span class="user-answer">Oui</span>
* Accédez-vous régulièrement à des produits CNES (peps / cdpp / hydroweb / theia similaires...) 
<span class="user-answer">non, représenté par d'autres utilisateurs</span>

## Communauté

* Que pourrait vous apporter la communauté?
<span class="user-answer">
* Discuter en toute transparence entre organismes.
* Craint la monétarisation
* Diminution des coûts
* Intégrer les anglos saxons
</span>
* Que souhaiteriez-vous apporter à la communauté?
<span class="user-answer">
* ok pour participer et **être entendu**
* ok pour partager In situ
* Souhaite éventuellement protéger certaines de ces briques de traitement (dans 3 ans) mais d'autres sont opensource (ex SAFI)
</span>

## Ouverture

* Disponible peu (1/2 journée mois) pour participer à la conception
<span class="user-answer">Oui (rotation sur le laboratoire) ==> un grand oui!</span>
* Qu'est ce qui vous ferait gagner du temps?
<span class="user-answer">
* Systèmes automates pour générer les cartes d'érosion ==> et partageable.
* Accès à des données déjà travaillées.
* Rivières: satellite geostationnaire avec pixel à moins de 10m ou flotte de satellites qui se relaient pour suivre les évènement d'inondation.
* Chaînes de traitement plus simples à faire (graph builder plus simple)
</span>
* POST: Quelles solutions dans un monde idéal?
<span class="user-answer">
* Chaînes de traitements faciles à trouver / partager
* EUMETSAT envoie du pixel à moins de 10m et pas de temps de l'heure
* Envoie du pixel à 50cm tous les 6 jours (suffisant pour certaines applications)
</span>

<style>
.user-answer {
  color: darkcyan;  
}
</style>
