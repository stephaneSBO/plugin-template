# Configuration

# Intro {#_intro}

Le plugin widget est un plugin un peu particulier, car il ne permet pas
de créer des équipements mais de modifier le rendu (affichage) d’une
commande. L’objectif de ce plugin est donc de permettre de personnaliser
simplement la façon d’afficher une valeur, info, ou action en fonction
de ses goûts et désirs.

Depuis la version 1.112 de Jeedom, il est possible de personnaliser les
widgets avec des options spécifiques (créées par le développeur du
widget). On peut donc avoir un widget qui s’affichera différemment d’une
commande à l’autre.

Ainsi, on peut avoir un même widget écrit en bleu sur une commande et en
vert sur une autre.

> **Note**
>
> Widget et Tuile, à ne pas confondre.
>
> Le widget, c’est la partie qui va se charger de mettre en forme et
> afficher une info ou commande. Un widget ne doit s’occuper que d’une
> seule commande ou info.
>
> La Tuile, c’est un regroupement de widgets pour un module. C’est la
> zone dans laquelle vont s’afficher les différents widgets appliqués
> aux commandes et infos du module.

# Installation du plugin Widget

Comme pour tout plugin, le plugin Widget s’installe depuis l’interface
Jeedom, menu "Général"⇒"Plugins"

![capture001](images/capture001.png)

Cliquer sur l’icône verte pour accéder directement au Market. Dans cette
fenêtre cliquer sur "Officiel" et dans le champ de recherche mettre
"Widget".

![capture002](images/capture002.png)

Cliquer sur l’icône du plugin. Cela ouvre la fiche du plugin dans
laquelle se trouvent plusieurs informations.

![capture003](images/capture003.png)

Cliquer sur le bouton "Installer stable". Une fois installé, Jeedom vous
demande si vous souhaitez aller à la page de configuration du plugin.
Répondre oui. Sur la page de configuration du plugin widget, nous
n’avons pour ce plugin qu’une seule option : activer ou désactiver.

Par défaut le plugin est désactivé. je vous invite donc à cliquer sur le
bouton vert "activer".

Dès à présent le plugin est actif et opérationnel.

Présentation et fonction de base du Plugin Widget {#_présentation_et_fonction_de_base_du_plugin_widget}
=================================================

Afin de se rendre dans le plugin Widget, il faut aller dans le menu
"Plugins"⇒"Programmation"⇒"Widget".

![capture005](images/capture005.png)

On se trouve donc sur la page principale du plugin. Ce dernier dispose
par défaut d’un éventail de widgets dès son installation Il est possible
d’en télécharger d’autres via le market ou de créer ses propres widgets
(voir plus bas).

![capture006](images/capture006.png)

En cliquant sur l’un des widgets de la liste du menu de droite ou de
gauche vous allez ouvrir la page de configuration du widget, dans
laquelle vous pouvez modifier, voir un aperçu du widget (si Jeedom
trouve une commande compatible) et tout un tas d’infos de configuration
comme le code source du widget

![capture007](images/capture007.png)

> **Warning**
>
> Si vous modifiez un widget qui n’est pas une de vos créations, il est
> préférable de le dupliquer pour éviter de perdre vos modifs si le
> widget original est mis à jour.

Pour plus d’infos sur la configuration et création de widget voir plus
bas.

# Appliquer le widget sur une commande

Pour appliquer un widget sur une seule commande ou modifier celui
appliqué, il faut vous rendre sur la page de configuration du module. Le
chemin pour accéder au module diverge en fonction du type de ce dernier.
Voici quelques exemples :

Pour les modules Z-Wave, "Plugins"⇒"Protocole domotique"⇒"Z-wave", puis
choisir le module de la commande que vous souhaitez modifier.

![capture024](images/capture024.png)

Sur la page de configuration du module, se rendre sur la commande et
cliquer sur les roues crantées. Dans la nouvelle fenêtre, se rendre dans
l’onglet "Affichage avancé"

![capture025](images/capture025.png)

Vous pouvez ici modifier le widget appliqué pour les ordinateurs et
mobiles avec les listes déroulantes dédiées.

![capture014](images/capture014.png)

> **Note**
>
> Les listes déroulantes sont auto filtrantes. Elles ne fournissent que
> les widgets compatibles avec le type de commande.

Appliquer le widget sur plusieurs commandes {#ancre-1}
-------------------------------------------

En cliquant sur le bouton “Appliquer sur des commandes” vous ouvrez une
fenêtre qui liste toutes les commandes compatibles avec le type du
widget. Vous pouvez donc simplement appliquer ou retirer le widget à de
nombreuses commandes en une seule fois.

![capture008](images/capture008.png)

Il suffit de cocher les commandes sur lesquelles vous souhaiter
appliquer le widget

### Divers exemples pour une même commande

![Widget : badge-transparent](images/capture009.png)

![Widget : badge](images/capture010.png)

![Widget : ConsoIMG](images/capture011.png)

Options de personnalisation des widgets {#_options_de_personnalisation_des_widgets}
---------------------------------------

Depuis la version 1.112 de Jeedom, il est possible de personnaliser les
widgets avec des options spécifiques (créées par le développeur du
widget) et communes à tous les widgets. On peut donc avoir un widget qui
s’affichera différemment d’une commande à l’autre.

On peut accéder à ces options de 2 façons. Soit par l’arbre Domotique
qui se trouve dans le menu "Général" ⇒ "Résumé Domotique"

![capture012](images/capture012.png)

Sur cette page vous trouvez tous vos éléments domotiques, les objets,
les modules, les commandes. Cliquez sur la petite roue crantée pour
accèder à la page de configuration.

![capture013](images/capture013.png)

Soit depuis la page de configuration des modules.

![capture015](images/capture015.png)

### Ajouter une option personnalisée

Dans l’onglet "Affichage avancé" on trouve 2 listes déroulantes qui
permettent de changer pour la commande le widget utilisé sur un
ordinateur et l’autre pour les mobiles. Il y a aussi d’autres options,
pour afficher ou non les noms et stats, forcer le retour à la ligne
avant/après le widget s’il y a plusieurs commandes dans un module
(retours à la ligne dans la tuile). Enfin la liste des paramètres
optionnels Widget appliqués (la liste disponible se trouve sur le forum
ou Wiki, un système de doc est à l’étude)

![capture014](images/capture014.png)

![exemple 1 de valeur pour afficher un compteur
spécifique](images/capture016.png)

![exemple 2 de valeur pour afficher un autre
compteur](images/capture017.png)

> **Note**
>
> Pour ajouter une option il vous suffit de cliquer sur le bouton
> "Ajouter", de renseigner le nom de l’option avec les bonnes minuscules
> et majuscules, ainsi que la valeur à attribuer à l’option. Pour
> trouver les options, consulter le forum ou/et le Wiki

# Configuration avancée

Voir la doc sur le Résumé domotique ⇒
[ICI](/doc/documentation/core/fr_FR/doc-core-display.html)

# Création / Modification de widget

Le plugin offre 2 possibilités pour la création de Widgets, le mode
facile qui permet de faire des widgets basiques facilement avec un
assistant de création, et le mode avancé qui permet aussi la
modification par la suite de tous les widgets.

> **Note**
>
> Le mode avancé apporte 
