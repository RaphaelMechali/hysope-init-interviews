# Interviews Hysope II

## Volet général

* Présentation (nom métier, organisme, formation universitaire)
<span class="user-answer">Département DSO SITR, depuis 7 ans (30 ans de CNES). Intervient sur SWOT (et en parrallèle activités avales). S'estime techniquement moins fort que Roger. A fait beaucoup d'activité opérationnelles (méca spatiale). Craint une pression importante lors de la CALVAL SWOT</span>
  * Plutôt opérationnel? Scientifique? Archi / bureau d'étude?
  <span class="user-answer">OP / scientifique</span>
* Quel tâche métier principale? 
<span class="user-answer">
* Traiter la données au fil de l'eau = Données SWOT => L1, L2 (hauteur rivière lac / reach (noeud de changement marqué ~= évènement) / lieu etc)
* Comparer à l'existant, fourni par les utilisateurs (genre mesures in situ) => faire coller les deux!
* Produire pour des résultats pour les scientifiques et les utilisateurs. Discussions à prévoir pour voir ce qu'ils attendent de ces données (rebouclage)

données brute (traitement)> Pixel Cloud (traitement)> Rivières / masse d'eau OU (traitement)> données lac. Fichiers de confs à mettre en place au cas par cas, au départ (mais devrait l'être après)
</span>
  * Pour quel résultat?
  <span class="user-answer">PixelCloud (en NetCDF et shapefile=QGIS.vectoriel) de hauteur de rivières (bruit) puis traitement pour redéfinir la rivière</span>
  * Pour qui?
  <span class="user-answer"></span>
  * Comment?
  <span class="user-answer"></span>
  * Etapes?
  <span class="user-answer"></span>
* Quelles tâches métiers secondaire? (sous-tâches ou tâches parallèles?)
<span class="user-answer">Communication avec les utilisateurs / scientifiques à prévoir (mais non mis au point)</span>
  * Pour quel résultat?
  <span class="user-answer"></span>
  * Pour qui? (lui-même ?)
  <span class="user-answer"></span>
  * Comment?
  <span class="user-answer"></span>
* Quels outils actuels?
<span class="user-answer">QGis (déporté sur HPC), outils de simulation / calcul (simu JPL: SWOT-hydrology-toolbox, par le JPL, RiverOps, par le JPL, et dernier outil à voir avec Claire Pottier)</span>
  * Quels points forts?
  <span class="user-answer">NA, ils ont le mérite d'exister</span>
  * Quels points d'amélioration?
  <span class="user-answer">Mise à jour des outils JPL trop fréquentes, impacte les format de données et paramètres! (on est content quand ça marche!) Attend la stabilité des outils JPL (et s'en inquiète) --> Point intéressant pour le centre d'expertise SWOT (ou STYX / HYMOTEP)</span>
  * Quels points d'intégration?
  <span class="user-answer"></span>
* Quelles données? 
<span class="user-answer">NA pour cet utilisateur</span>
  * Neige (couverture / prduits dérivés)
  <span class="user-answer">Oui</span>
  * SWE (volume eau / neige)
  <span class="user-answer">Non</span>
  * Surface d'eau (pixel eau)
  <span class="user-answer">Oui</span>
  * Hauteur d'eau
  <span class="user-answer">Oui</span>
  * Débit d'eau
  <span class="user-answer">Non (indirectement)</span>
  * Température
  <span class="user-answer">Non</span>
  * Turbidité
  <span class="user-answer">Non</span>
  * Autres?
  <span class="user-answer">
    -> dates des produits <span color="red">? </span>
    -> conditions météo (vent)
  </span>
* Quelles méthodes
  * d'exploitation
  <span class="user-answer"></span>
  * de comparaison
  <span class="user-answer"></span>
  * d'extrapolation
  <span class="user-answer"></span>
* Tâche métier actuellement bien outillée?
<span class="user-answer">Moyennement</span>
  * Totalement couverte?
  <span class="user-answer">Non</span>
* Quels points pénibles (outils / données / volumétrie / format / etc...)
<span class="user-answer">NetCDF un peu lourd en manip</span>
* Illustrer tâche métier durant l'interview? (si moins de 20 minutes)
<span class="user-answer"></span>

## Volet intégration HI2

* Etes vous familiers avec les services Theia?
<span class="user-answer">Pas vraiment (a un peu utilisé)</span>
* Utilisez-vous des données Theia régulièrement?
<span class="user-answer">Non</span>
* Accédez-vous régulièrement à des produits CNES (peps / cdpp / hydroweb / theia similaires...)
<span class="user-answer">Peps: oui (pour d'autres projets), utilise également les données Sentinel1.</span>

## Communauté

* Que pourrait vous apporter la communauté?
<span class="user-answer">
* Echanges rapide (qualité des produits et mesures)
</span>
* Que souhaiteriez-vous apporter à la communauté?
<span class="user-answer">
* Du support autour des produits
</span>

## Ouverture

* Disponible peu (1/2 journée mois) pour participer à la conception
<span class="user-answer">Intéressé par les aspects ergo / fonctions</span>
* Qu'est ce qui vous ferait gagner du temps?
<span class="user-answer">Des outils rapides. Par exemple: QGis utilise des gros fichiers, c'est long (5 minutes d'affichage pour une rivière). A essayé de remplacer des traitement QGis par photoshop</span>
* POST: Quelles solutions dans un monde idéal?
<span class="user-answer">Rapidité d'application des prétraitements et traitements de visu et graphiques (autant calibration qu'exploitation). La taille dispo des volumes doit être visible (pour anticiper et être zen!) --> Point intéressant pour le centre d'expertise SWOT (ou STYX / HYMOTEP) </span>

<style>
.user-answer {
  color: darkcyan;  
}
</style>
