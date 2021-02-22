# Interviews Hysope II

## Volet général

* Présentation (nom métier, organisme, formation universitaire)
<font color="darkcyan">Département DSO SITR, depuis 7 ans (30 ans de CNES). Intervient sur SWOT (et en parrallèle activités avales). S'estime techniquement moins fort que Roger. A fait beaucoup d'activité opérationnelles (méca spatiale). Craint une pression importante lors de la CALVAL SWOT</font>
  * Plutôt opérationnel? Scientifique? Archi / bureau d'étude?
  <font color="darkcyan">OP / scientifique</font>
* Quel tâche métier principale? 
<font color="darkcyan">
* Traiter la données au fil de l'eau = Données SWOT => L1, L2 (hauteur rivière lac / reach (noeud de changement marqué ~= évènement) / lieu etc)
* Comparer à l'existant, fourni par les utilisateurs (genre mesures in situ) => faire coller les deux!
* Produire pour des résultats pour les scientifiques et les utilisateurs. Discussions à prévoir pour voir ce qu'ils attendent de ces données (rebouclage)

données brute (traitement)> Pixel Cloud (traitement)> Rivières / masse d'eau OU (traitement)> données lac. Fichiers de confs à mettre en place au cas par cas, au départ (mais devrait l'être après)
</font>
  * Pour quel résultat?
  <font color="darkcyan">PixelCloud (en NetCDF et shapefile=QGIS.vectoriel) de hauteur de rivières (bruit) puis traitement pour redéfinir la rivière</font>
  * Pour qui?
  <font color="darkcyan"></font>
  * Comment?
  <font color="darkcyan"></font>
  * Etapes?
  <font color="darkcyan"></font>
* Quelles tâches métiers secondaire? (sous-tâches ou tâches parallèles?)
<font color="darkcyan">Communication avec les utilisateurs / scientifiques à prévoir (mais non mis au point)</font>
  * Pour quel résultat?
  <font color="darkcyan"></font>
  * Pour qui? (lui-même ?)
  <font color="darkcyan"></font>
  * Comment?
  <font color="darkcyan"></font>
* Quels outils actuels?
<font color="darkcyan">QGis (déporté sur HPC), outils de simulation / calcul (simu JPL: SWOT-hydrology-toolbox, par le JPL, RiverOps, par le JPL, et dernier outil à voir avec Claire Pottier)</font>
  * Quels points forts?
  <font color="darkcyan">NA, ils ont le mérite d'exister</font>
  * Quels points d'amélioration?
  <font color="darkcyan">Mise à jour des outils JPL trop fréquentes, impacte les format de données et paramètres! (on est content quand ça marche!) Attend la stabilité des outils JPL (et s'en inquiète) --> Point intéressant pour le centre d'expertise SWOT (ou STYX / HYMOTEP)</font>
  * Quels points d'intégration?
  <font color="darkcyan"></font>
* Quelles données? 
<font color="darkcyan">NA pour cet utilisateur</font>
  * Neige (couverture / prduits dérivés)
  <font color="darkcyan">Oui</font>
  * SWE (volume eau / neige)
  <font color="darkcyan">Non</font>
  * Surface d'eau (pixel eau)
  <font color="darkcyan">Oui</font>
  * Hauteur d'eau
  <font color="darkcyan">Oui</font>
  * Débit d'eau
  <font color="darkcyan">Non (indirectement)</font>
  * Température
  <font color="darkcyan">Non</font>
  * Turbidité
  <font color="darkcyan">Non</font>
  * Autres?
  <font color="darkcyan">
    -> dates des produits <span color="red">? </span>
    -> conditions météo (vent)
  </font>
* Quelles méthodes
  * d'exploitation
  <font color="darkcyan"></font>
  * de comparaison
  <font color="darkcyan"></font>
  * d'extrapolation
  <font color="darkcyan"></font>
* Tâche métier actuellement bien outillée?
<font color="darkcyan">Moyennement</font>
  * Totalement couverte?
  <font color="darkcyan">Non</font>
* Quels points pénibles (outils / données / volumétrie / format / etc...)
<font color="darkcyan">NetCDF un peu lourd en manip</font>
* Illustrer tâche métier durant l'interview? (si moins de 20 minutes)
<font color="darkcyan"></font>

## Volet intégration HI2

* Etes vous familiers avec les services Theia?
<font color="darkcyan">Pas vraiment (a un peu utilisé)</font>
* Utilisez-vous des données Theia régulièrement?
<font color="darkcyan">Non</font>
* Accédez-vous régulièrement à des produits CNES (peps / cdpp / hydroweb / theia similaires...)
<font color="darkcyan">Peps: oui (pour d'autres projets), utilise également les données Sentinel1.</font>

## Communauté

* Que pourrait vous apporter la communauté?
<font color="darkcyan">
* Echanges rapide (qualité des produits et mesures)
</font>
* Que souhaiteriez-vous apporter à la communauté?
<font color="darkcyan">
* Du support autour des produits
</font>

## Ouverture

* Disponible peu (1/2 journée mois) pour participer à la conception
<font color="darkcyan">Intéressé par les aspects ergo / fonctions</font>
* Qu'est ce qui vous ferait gagner du temps?
<font color="darkcyan">Des outils rapides. Par exemple: QGis utilise des gros fichiers, c'est long (5 minutes d'affichage pour une rivière). A essayé de remplacer des traitement QGis par photoshop</font>
* POST: Quelles solutions dans un monde idéal?
<font color="darkcyan">Rapidité d'application des prétraitements et traitements de visu et graphiques (autant calibration qu'exploitation). La taille dispo des volumes doit être visible (pour anticiper et être zen!) --> Point intéressant pour le centre d'expertise SWOT (ou STYX / HYMOTEP) </font>


