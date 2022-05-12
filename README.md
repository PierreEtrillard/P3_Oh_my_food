# Bienvenu dans le dépot git du Projet Ohmyfood

Merci de consulter le readme.txt concernant l'utilisation des préprocesseurs et l'indexation des fichiers avant toute révision du code. 
 ________________________________________________________________________________________________________________________________________________________________
|                                                                                                                                                                |
|  Branch no layout                                                                                                                                              |
| Ce projet posséde une branch secondaire "nolayout" destinée aux appareils à faibles ressources.                                                                |   
|   Celle-ci différe de la branch "main" dans l'utilisation de la propriété transform: scaleX() sur le texte au survol des étiquettes des plats.                 |
|   Cette propriétée est interessante, car contrairement à la réduction de width choisie pour coller à la maquette sur la version principal, elle n'entraine pas |
|   de calcul sur la couche "layout" du navigateur et garantie donc un FPS optimal pour la fluidité de l'animation (coche verte et icone 'validate').            |
|   En contrepartie elle génére un effet écrasé que je trouve disgracieux sur le texte.                                                                          |
|                                                                                                                                                                |
| J'ai également versionné un deuxiéme loader plus ludique sur cette version, cependant, il utilise la font shrikhand qui met un peu de temps à ce charger;      |
|   ce qui pourrais nuir à l'esthétique de l'animation sur les appareils ne disposant pas d'une connexion internet rapide.                                       |
|                                                                                                                                                                |
| Le choix vous ai laissé de merger cette branch ou non (pour le loader il suffirait de décommenter le relicat de code situé dans la partielle "loader.scss" du  |
| dossier "SASS".                                                                                                                                                |
|________________________________________________________________________________________________________________________________________________________________|
