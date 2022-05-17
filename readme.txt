Bienvenu dans le manuel de maintenance du site ohmyfood

Les préprocesseurs sass et postcss (pour autoprefixer) ont étés utilisés pour ce projet.
L'installation de npm et de ses modules sass & autoprefixer sera necesaire en cas de revision du projet.
Sass possède un fichier principal "main.scss" pointant vers des partiels comme indiqué ci dessous:

main.scss
    |__Vendors/
    |    |__normalize.scss    //écrase les régles conflictuelles avec certains navigateurs//
    |
    |__utils/
    |    |__keyframes.scss    //Les animations.//
    |    |__variables.scss    //Les couleurs, breakpoints et delais d'anim.//
    |    |__mixins.scss       //Quelques déclarations préenregistrées.//
    |
    |__base/
    |    |__base.scss         //Les valeurs génériques pour tous le projet (body,a ..)//
    |    |__typography.scss   //Les fonts et leurs propriétées.//
    |
    |__components/
    |    |__buttons.scss      //les boutons "explorez nos restaurants", "commander" et l'icone coeur.// 
    |    |__loader.scss       //Animations à l'ouverture de l'index.//
    |    
    |__layouts/
    |     |__nav.scss          //On trouve ici les cards aux nom des restaurants qui font office//
    |     |                   // d'entrées de navigation pour ce projet.                       //
    |     |
    |     |__form.scss        // A therme, la section indiquant la localité (juste après le header) //
    |                        //  possédera une fonction permettant de choisir celle-ci, j'ai pris  //
    |                       //   les devants en incluant un formulaire dont le css ce troiuve ici.//
    |__pages/
          |__header.scss        //En-tête en commun (+liens vers accueil pour les menus).// 
          |__home.scss          //pour les régles spécifiques à l''index.//
          |__menu.scss          //pour les régles spécifiques aux pages "menus".//
          |__footer.scss        //¨Pieds de pages commun à toutes les pages.//

Sass compiles toutes les partiels puis convertis l'ensemble des régles dans le fichiers mini-css CSS/style.css 
A son tour, autoprefixer implémente les préfix necessaires dans CSS/style.css.

Voir le package.json pour les parametres de sass et postcss décris ci-dessus.
Commande pour executer ces opérations:
        npm run sass
        npm run prefix