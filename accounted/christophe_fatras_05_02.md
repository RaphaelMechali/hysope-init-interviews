# Interviews Hysope II

## Volet général

* Présentation (nom métier, organisme, formation universitaire)
<span class="user-answer">
Ingénieur R&D hydro chez CLS (initialement traitement du signal ENSEIT, puis thèse altimétrie en Afrique), 
parcours: ONERA, enseignant universitaire en Equateur, 2018 post doc CesBio (surface inondées dans le bassin du Congo, lien surface x hauteur), octobre 2019 application Hydro chez CLS (AI4Geo, estimation des volumes / hauteur d'eau, surfaces inondées)
</span>
  * Plutôt opérationnel? Scientifique? Archi / bureau d'étude?
<span class="user-answer">
entre scientifique et bureau d'étude, devient référent R&D hydro
</span>
* Quel tâche métier principale? 
<span class="user-answer">
* Veille techno
* Développement pour différents projets
* Créer et innover (Encadre un alternant pour de nouvelles méthodes, par exemple, calcul des surface)
</span>
  * Pour quel résultat?
<span class="user-answer">
* Finalité: services de suivi et gestion de l'eau d'ici quelques années.
</span>
  * Pour qui?
<span class="user-answer">
Clients potentiels: gouvernements, banques mondiales, gestionnaires, visées internationales
</span>
  * Comment?
<span class="user-answer">
Infos sur le cycle complet de l'eau: volumes d'eau, surface en haut, puis via GPM pour la pluie, Trishna (ETP). Vise à une automatisation complète. 
</span>
  * Etapes?
<span class="user-answer">
Projet:
* RAO
* Mise en place
* Réalisation de dev (informatique, mais pas que), fonction du cadre du projet
  1. Veille techno et existant
  1. Quels manques
  1. Adapter à la contrainte (temporelle VS spatiale)
Exemple FloodDam:
Analyse de hauteur d'eau et détection de surface de différente sources
Détection d'anomalies sur les hauteurs d'eau
Mise en place d'un pipeline entre briques techniques
Listing de carte / sources existantes, qualification (critiques)
Auto-amélioration: Investigue sur les résolutions et autres, traitements (Python, utilise lib externes comme Orphéo)
  * pour diminuer les contraintes espaces disques (HPC notamment)
  * pour diminuer les contraintes temps: traitement entièrement / partiellement les fichiers
* Bosse avec du SAR (utilise S1Tiling? conf assez "pénible" outil qui prend S1 ->S2, images 110kmx110, à 10m de résolution, bientôt intégré dans Orphéo Toolbox) 
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
* QGis: visu et contexte spatial. Vectorisation, clipping (en phase recherche / test uniquement). Utilise des sorties de QGis dans python (ne développe pas de plugin)
  * Orpheo Toolbox
* modèle SWAT de plus en plus (pratique pour déterminer un bassin hydrographique), faire rapidement le lien entre MNT et hydrologie
* N'utilise pas pour l'instant le VRE (en phase de préparation). Pas forcément convaincu par le format VRE (comprend mal l'intérêt: surcouche et lourdeur, complique les échanges, trop didactif à son goût). "Autant utiliser un éditeur et travailler sur terminal" (chez moi, très pratique, ou HPC, les deux lui conviennent, souvent les codes sont sur le HPC). Edite son code avec PyCharm d'habitude mais la VRE l'en empêche récemment (pb network).
* PyCharm, mais préfère VSCode
</span>
  * Quels points forts?
<span class="user-answer">
* VSCode: très rapide à lancer et sait faire tourner des programes locaux ailleurs (exécution déportée)
* VSCode: versionement centralisé
* QGis: gratuit, rapide (face à son concurrent payant ArcGis)
* Python: rapide, gratuit, multiplateforme, grosse communautés
* Orpheo Toolbox: existe! (rend un gros service), OTB mieux que concurrents (SNAP) en approche industrielle (automatise). Bien également pour déléguer au HPC (sans lui, pb de déconnexion).
</span>
  * Quels points d'amélioration?
<span class="user-answer">
* VSCode: trop de mises à jour
* QGis: plante trop vite, gourmand en ressources
* Orpheo Toolbox: beaucoup (trop d'outil), pas assez de doc
  * Bosse avec du SAR, utilise "S1Timeline"? assez "dégueulasse", attends intégration dans OTB
* VRE: peu d'intérêt pour un expert (!), interface didactique (mieux pour les noobs)
</span>
  * Quels points d'intégration?
<span class="user-answer">
</span>
* Quelles données? 
<span class="user-answer">
</span>
  * Neige (couverture / produits dérivés)
<span class="user-answer">
moyen (sauf pour calculer SWE)
</span>
  * SWE (volume eau / neige)
<span class="user-answer">
A terme, il faudra (moins intéressant pour les pays tropicaux...)
</span>
  * Surface d'eau (pixel eau)
<span class="user-answer">
Oui
</span>
  * Hauteur d'eau
<span class="user-answer">
Oui: **sa variable principale**
</span>
  * Débit d'eau
<span class="user-answer">
Oui
</span>
  * Température
<span class="user-answer">
Oui, nécessaire pour ETP, jusqu'à 50% d'évaporation localement
</span>
  * Turbidité
<span class="user-answer">
Non (**n'y connait rien**: ils s'associent à d'autres personnes plus spécialisés pour des approches intégrés, ce qu'ils souhaitent développer à terme)
</span>
  * Autres?
<span class="user-answer">
* Volume (développe des outils autour)
* Glace (et glaciers), lié au stress hydrique notamment
Très axé satellitaire (manque d'In Situ en Afrique ou Malaisie par exemple)
</span>
* Quelles méthodes
  * d'exploitation
<span class="user-answer">
demande du client: s'il demande une série temporelle, feuille Excell, graphique, fonction du besoin
</span>
  * de comparaison
<span class="user-answer">
Courbes Ipsométriques (a travaillé avec Lionel, qui saura illustrer): ABAC surface x hauteur (correspondance)
Recroisent données In Situ et données estimées (HydroWeb) pour trouver les correlations (graphique 2D de courbes ipsométriques superposées, surface x hauteur = signature du lac)
Comparaison de hauteurs d'eaux (lac en Ouganda) => altimétrie et in situ (alti nécessite gros reprocess): courbe hauteur (alti) x temps / mesure (in situ), pour comprendre lac et retenue.
Partie géo: beaucoup travaillent avec QGis et Google Earth, vérifier que les données in situ ne sont pas trop lointaines (+ expertise humain pour cette évaluation)
</span>
  * d'extrapolation
<span class="user-answer">
En fait peu:
* Sur les MNT pour extrapoler la courbe ipsométrique dérivée (marge d'erreur trop importante)
* Essaie également sur les séries temporelles (parfois, très bonne estimations, mais les outils filtrent cet évènement extrême: très difficile de filtrer erreur et bonne info)
Grosse tâche d'estimation de marge d'erreur, si une donnée n'est pas accessible
</span>
* Tâche métier actuellement bien outillée?
<span class="user-answer">
Oui
aime bien se reposer sur des calculateurs massifs (HPC et calculateur interne)
</span>
  * Totalement couverte?
<span class="user-answer">
Pour le moment oui, en cours de dev sur d'autres points / problématiques / thématiques
</span>
* Quels points pénibles (outils / données / volumétrie / format / etc...)
<span class="user-answer">
Espace disque en quantité
Données un peu vieille (2019 -), stockées sur bandes, temps d'attente important! En cours d'amélioration
</span>
* Illustrer tâche métier durant l'interview? (si moins de 20 minutes)
<span class="user-answer">

</span>

## Volet intégration HI2

* Etes vous familiers avec les services Theia?
<span class="user-answer">
Oui & non. Sait que ça existe et ce que c'est mais s'en sert peu
</span>
* Utilisez-vous des données Theia régulièrement?
<span class="user-answer">
pas trop
</span>
* Accédez-vous régulièrement à des produits CNES (peps / cdpp / hydroweb / theia similaires...)
<span class="user-answer">
SciHub (portail Copernicus)
PEPS
Hydroweb
pour les données le long de la trace: CTOH (en thèse)
</span>

## Communauté

* Que pourrait vous apporter la communauté?
<span class="user-answer">
Question difficile, beaucoup de concurrence et d'intérêts divergent / zones de chasses gardées.
La plupart des gens veulent de l'info à 50cm prêt, il peu apporter assez peu de choses
</span>
* Que souhaiteriez-vous apporter à la communauté?
<span class="user-answer">
</span>

## Ouverture

* Disponible peu (1/2 journée mois) pour participer à la conception
<span class="user-answer">
Oui (attention disponibilité)
</span>
* Qu'est ce qui vous ferait gagner du temps?
<span class="user-answer">
* Accès rapide aux données historiques.
* Libre accès aux données COSMOS SKYMED
* Avoir du 3m en bande X (hyperfréquence entre C et Ku, moins pénétrante dans le sol, permet une meilleur classification)
</span>
* POST: Quelles solutions dans un monde idéal?
<span class="user-answer">

</span>

<style>
.user-answer {
  color: darkcyan;  
}
</style>
