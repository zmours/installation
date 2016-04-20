# Sublime Text 3 & Plugins

![](../images/logos-st.png)

## C’est quoi Sublime Text ?

[Sublime Text](http://www.sublimetext.com/) (ou “Sublime” pour faire court) est un **éditeur portable** (OSX, Linux, Windows) **extrêmement puissant et rapide**, qui est devenu **incontournable** dans l’univers des développeurs.

Il est techniquement payant (US$ 70 au maximum par licence), mais **utilisable librement** dans l’intervalle : il affiche juste périodiquement un *nag screen* (une boîte de dialogue invitant à l’achat) lors des sauvegardes de fichiers, sans que ça soit contraignant.  Ceci étant dit, vu le boost monstrueux de productivité, ça les vaut largement.

* :point_right: [Je vais directement aux instructions d’installation](#installer-st3) :point_left:, ou
* :point_right: [Je consulte les paquets recommandés](#paquets-recommandés) :point_left:, ou alors…
* Dites-m’en davantage, mon bon monsieur.

## Est-ce obligatoire ?

**Absolument pas.**  Mais si j’étais toi, je me jetterais dessus.  Outre qu’il permet d’avoir un seul éditeur à travers les différentes plates-formes de développement, et donc de mieux capitaliser le savoir-faire d’édition, il regorge de fonctions avancées pour l’édition pure comme pour tout un tas de syntaxes et technos spécifiques.

Grâce à un **énorme écosystème de plugins**, il offre une intégration fine avec tout un tas de technos et syntaxes, ce qui en fait un outil redoutable de productivité.  Il met une **énorme claque** aux bonnes blagues comme *Notepad++* (qui est vraiment très, très minimaliste en comparaison) ou *Ultra-Edit*, et soutient largement la comparaison avec nombre d’éditeurs et EDIs reconnus.

### Sublime vs. Atom

[Atom](http://atom.io/) est un projet très intéressant d’éditeur open-source, basé sur Electron, et piloté par GitHub.  Il mérite carrément qu’on garde un œil dessus mais pour le moment, **il est trop lent et crashe trop souvent**.

### Sublime vs. TextMate

[TextMate](https://macromates.com/) est un éditeur spécifiquement pour OSX qui a connu une énorme popularité lors de l’émergence de Ruby On Rails.  Il a clairement **servi de référence** lors de la conception de Sublime, qui a repris une grande partie de ses fonctionnalités, raccourcis claviers, et son mécanisme de plugins (la plupart des plugins TextMate sont utilisables tels quels sur ST2, parfois aussi sur ST3).

Mais son développement est **arrêté depuis OSX 10.6**, il ne marche que sur OSX et fait aujourd’hui **beaucoup moins de choses** que Sublime.  Par ailleurs, il est **nettement plus lent**, en particulier pour la navigation vers fichiers.

La quasi-totalité de ses utilisateurs ont migré vers Sublime, apparemment.

### Sublime vs. Vim ou Emacs

On retrouve les mêmes principes :

* Portabilité
* Disponibilité graphique (GVim, etc.)
* Haut niveau de personnalisation
* Fonctionnalités avancées d’édition pure
* Écosystème gigantesque de plugins

En revanche, Vim et Emacs sont open-source (donc gratuits), et sont là depuis super longtemps (donc disponibles vraiment partout).  Mais ce sont des éditeurs difficiles à apprivoiser !  **Sublime a bien davantage de chances de fédérer une équipe qui ne contient pas que des geeks développeurs ou sysadmin**.

### Sublime vs. VSCode

En 2015, Microsoft a sorti un projet dans la même veine qu’Atom : [Visual Studio Code](https://code.visualstudio.com/).  On y retrouve la base Electron, le projet en open-source, l’orientation 100% web, l’intégration étroite avec Git et le multi-plate-formes.

Comme c’est Microsoft, on y trouve aussi une **bonne intégration avec leur univers**, notamment via la **complétion et un peu de refactoring**, basé pour beaucoup sur les fichiers de typage de [DefinitelyTyped](http://definitelytyped.org/).  Un **débogueur** JS / Node est également présent, basé sur le protocole de débogage de v8.  Et depuis peu, on peut même s’en servir pour déboguer et éditer du code JS tournant dans Chrome, directement depuis VSCode !

C’est vraiment pas mal, mais ça reste **trop basique** pour nombre de besoins ; l’écosystème de plugins est loin derrière celui de Sublime, et dès qu’on sort de technos pur-web pour aller, par exemple, vers Python, Ruby, ou simplement Markdown, ça pèche un peu.

Ça reste intéressant à surveiller, mais pour le moment, **Sublime est loin devant**.

### Sublime vs. Brackets

En 2013, Adobe a lancé un projet d’éditeur 100% orienté web assez innovant : [Brackets](http://brackets.io/).  Le développement ralentit un peu depuis la mi-2015, mais on y trouve pas mal **d’UI innovantes** (édition entrelacée CSS, etc.) qui en font un bon terrain d’expérimentation en termes de fonctionnalités d’édition.

Toutefois, ça reste **trop spécialisé** et, paradoxalement, trop basique hors de l’édition pure, pour être un candidat sérieux à ce stade.

### Sublime vs. EDIs

Ah, les EDIs…  Visual Studio, NetBeans, Eclipse, la famille JetBrains (IntelliJ IDEA, WebStorm, PHPStorm, RubyMine, PyCharm…) et j’en passe…

L’avantage, c’est qu’ils **intègrent** plein de choses ensemble : gestion de sources, éditeur, complétion, refactoring, gestion de projet, documentation, voire déploiement.

L’inconvénient, outre qu’ils sont souvent payants—et **chers**—c’est qu’ils sont souvent spécialisés sur un écosystème technique précis, que leur composant éditeur **laisse à désirer en édition pure**, justement, et qu’ils sont souvent **lourds**.

Je veux dire, tu as mesuré le temps, le processeur et la mémoire de tes derniers lancements Eclipse ou NetBeans ?!

Si tu as bien l’habitude de ton EDI et que tu y trouves tous les outils de l’état de l’art (cf. liste des paquets recommandés plus bas), tant mieux !  Sinon, c’est peut-être l’occasion de **tenter autre chose**, en alternative ?

## ST2 vs. ST3

Sublime, c’est un peu comme Python : y’a une distinction entre les versions 2.x et la 3.x.

Tout le développement de ces dernières années s’est concentré sur la 3.x, qui est néanmoins toujours « en beta » (pour ce que ça veut dire…).  Tant que celle-ci ne sera pas finalisée officiellement, **les licences ST2 sont valables sur ST3**, ce qui est génial !  Il y aura un petit supplément, sans doute, pour la sortie finale, mais ça risque d’attendre encore longtemps…

En pratique, ST3 a clairement l’avantage, car :

* ST3 est **nettement plus rapide** que ST2
* ST3 est **sensiblement moins lourd** que ST2
* ST3 concentre les **développements récents de plugins**, souvent pas ou plus disponibles pour ST2
* ST3 a une architecture de plugins **plus puissante**, qui leur permet notamment de nous fournir des infobulles, des boîtes de dialogue, etc., ce qui est nettement plus pratique.

Bref, prends ST3, pas d’hésitation.

## Installer ST3

OK on est partis !

1. [Télécharge ST3](http://www.sublimetext.com/3) (pas la peine de prendre les versions « portables » sur Windows, sauf si tu n’as pas les droits d’installation).  Assure-toi de prendre la 64-bit si tu es sur un Windows ou Linux 64-bit (sur OSX, c’est d’office).
2. Lance l’installeur si besoin (ou sur OSX, déplace l’application dans *Applications*).

### Configuration de base

> **Info** Sublime offre toujours deux niveaux de configuration, et deux types de configuration d’ailleurs :
> <br/><br/>
>
> * **Niveaux** *Default* et *User* : le premier sera écrasé à chaque mise à jour, le second a priorité et persiste au travers des mises à jour.  **Fais toujours tes propres réglages au niveau *User* !**
> * **Types** *Settings* et *Key Bindings* : le premier contient les réglages et les thèmes de couleurs, le second les raccourcis claviers.  Oui, dans Sublime, on peut personnaliser tous les raccourcis, en enlever, en ajouter, etc.
>
> Dans les deux cas, il s’agit de **fichiers JSON**, c’est donc tout facile à changer.  Le simple fait de **sauver le fichier le prend en compte immédiatement**.  Nickel Michel.

Par défaut, Sublime a **quelques défauts mineurs de configuration** quant à sa gestion des espaces, des onglets, etc.  Enfin, on trouve.  On t’invite donc à ajouter certains réglages à ton niveau *User*.

* Sur OSX, comme d’hab, <kbd>Cmd+,</kbd> (oui, Commande-Virgule) ouvre les Préférences.
* Sur Linux et Windows, c’est dans le menu *Preferences > Settings - User* que ça se passe.

**À la fin du fichier JSON, ajoute une virgule** après le dernier réglage, et insère ensuite, **juste avant l’accolade fermante finale**, les réglages suivants :

```json
  "auto_complete": true,
  "auto_complete_triggers":
  [
    {
      "characters": ".",
      "selector": "source.js"
    }
  ],
  "ensure_newline_at_eof_on_save": true,
  "folder_exclude_patterns":
  [
    "node_modules",
    ".git"
  ],
  "highlight_line": true,
  "highlight_modified_tabs": true,
  "tab_size": 2,
  "translate_tabs_to_spaces": true,
  "trim_trailing_white_space_on_save": true
```

Si tu te demandes ce que font certains réglages, tu peux chercher sur Google ou nous poser la question en formation, on te répondra avec plaisir ; mais fais-nous confiance, c’est bon pour ta peau :grin:.

On t’invite aussi à décocher l’option de menu *View > Side Bar > Show Open Files*, c’est vite pénible sinon.

## Package Control

Sublime lui-même n’a qu’une prise en charge de plugins, sans système de **gestion** de plugins.  Du coup, un outil s’est développé à côté, qui est immédiatement devenu indispensable : **[Package Control](https://packagecontrol.io/)**.  C’est un référentiel de plugins Sublime (2 et 3), avec un outil intégrable à Sublime pour les installer, retirer, lister, (dés)activer, etc.

L’installation est un peu rock’n’roll : faut copier-coller du Python dans la console de Sublime, cash !

1. [Va copier le code d’installation](https://packagecontrol.io/installation) pour ST3 dans ton Presse-Papier
2. Dans ST3, ouvre la console (menu *View > Show Console*, ou clic sur le petit icône tout à gauche de la barre d’état, en bas de la fenêtre, puis clic sur *Console*)
3. Colle le code que tu viens de copier, et presse <kbd>Entrée</kbd>.
4. Au bout de quelques secondes, ça t’affiche dans la console que tu dois redémarrer Sublime pour finaliser, car il a dû installer une dépendance manquante.  Ne t’inquiète pas, ça garde tes fichiers ouverts, onglets, etc.
5. Redémarre ST3.

Tu peux vérifier que tu as Package Control de plusieurs façons :

* Vérifie la présence du menu *Preferences > Package Control* (on trouve d’ailleurs aussi désormais *Preferences > Package Settings*).
* Ouvre la *Command Palette* (<kbd>Ctrl+Maj+P</kbd> ou sur OSX <kbd>Cmd+Maj+P</kbd>) et tape `insp` : tu devrais tomber sur la commande *Package Control: Install Package*.

### Comment installer un paquet ?

On recourt à la commande *Install Package* fournie par Package Control.  Il suffit d’ouvrir la *Command Palette* (<kbd>Ctrl+Maj+P</kbd> ou sur OSX <kbd>Cmd+Maj+P</kbd>) et de taper `insp`, ça devrait suffire à sélectionner la bonne commande.

On fait <kbd>Entrée</kbd> directement, ça va chercher une liste à jour des paquets auprès de Package Control (et ça va la garder en cache un petit moment), puis on tape à nouveau (toujours en mode *fuzzy finding*[^1]) pour chercher le paquet, et à nouveau <kbd>Entrée</kbd> pour lancer l’installation.

À chaque fois, la barre d’état (la barre en bas de la fenêtre) nous indique la progression de la tâche.

Une fois installés, certains paquets ont plein de trucs à nous dire (procédures complémentaires, notes de version, etc.) : si tel est le cas, ils ajouteront leurs infos à un onglet dédié, ouvert si besoin, nommé *Package Control Messages*.

[^1] En *fuzzy finding*, il suffit de taper des lettres pour filtrer sur tout élément de liste où ces lettres apparaissent dans le bon ordre (mais sans forcément être contigües, ou même être des initiales).  Ça va super vite, c’est hyper pratique.  Sublime utilise ça dans toutes ses listes : fichiers, commandes, paquets…

## Paquets recommandés

On recommande évidemment toute une série de paquets ST3, notamment pour le développement web.  N’hésite pas à [aller fureter](https://packagecontrol.io/browse)…

### Pour commencer : une bonne fonte, un bon thème

Sublime arrive par défaut avec pas mal de thèmes, mais parfois des paquets en installeront des variations améliorées.  Parmi ceux fournis par défaut, **Monokai** (et sa version *Bright*) est sans doute un des plus fins / différenciés sur fond sombre, LAZY optant pour un fond clair plutôt.

Toutefois, le paquet [Monokai Extended](https://packagecontrol.io/packages/Monokai Extended) fournit une version encore encore améliorée (notamment pour les contextes Markdown, HTML, CSS, LESS, JavaScript et Handlebars), que je te conseille.

1. Installe-le
2. Choisis-le : *Preferences > Color Scheme > Monokai Extended > Monokai Extended*.

Côté fonte, ont ne saurait trop te recommander la merveilleuse **Source Code Pro** fournie gracieusement par Adobe : [télécharge-la ici](https://github.com/adobe-fonts/source-code-pro#readme) et installe-la sur ton système, après quoi tu peux rouvrir tes réglages utilisateur (voir plus haut) et ajouter celui-ci dans le tas :

```json
  "font_face": "Source Code Pro",
```

### Paquets utiles en général

* [SideBarEnhancements](https://packagecontrol.io/packages/SideBarEnhancements) pour passer de 5–6 pauvres options en clic droit dans la barre latérale à une **pléthore** de commandes **super cool** !  La plupart deviennent évidemment disponibles aussi *via* la *Command Palette*.
* [AdvancedNewFile](https://packagecontrol.io/packages/AdvancedNewFile) pour faciliter la **création de fichiers avec le bon nom** et la bonne syntaxe d’entrée de jeu (et les dossiers parents, **à la volée**, si besoin).
* [AutoFileName](https://packagecontrol.io/packages/AutoFileName) pour avoir une **complétion**, même si elle n’est pas toujours à propos, sur les noms de **fichiers locaux** dans plein d’endroits du code qui semblent en avoir besoin.
* [Terminal](https://packagecontrol.io/packages/Terminal) pour ouvrir facilement un terminal dans le dossier du fichier courant.
* [Origami](https://packagecontrol.io/packages/Origami) pour pouvoir **découper la fenêtre** en autant de **panneaux** qu’on veut, sur des dispositions totalement libres.
* [Color Highlighter](https://packagecontrol.io/packages/Color Highlighter) pour mettre en exergue, avec la couleur idoine, toute syntaxe CSS de couleur (ou tout nom reconnu de couleur) présente dans le texte.
* [Unicode Character Highlighter](https://packagecontrol.io/packages/Unicode Character Highlighter) pour mettre en exergue certains caractères qui peuvent être problématiques, notamment les **espaces insécables** littérales, qui bien souvent nous jouent des tours en JS et Ruby avec nos claviers OSX…
* [BracketHighlighter](https://packagecontrol.io/packages/BracketHighlighter) pour signaler à tout moment les bornes de début et de fin du segment courant (parenthèses, accolades, crochets, guillemets simples ou doubles).
* [DocBlockr](https://packagecontrol.io/packages/DocBlockr) pour faciliter **énormément** la saisie de commentaires dans le code.

### Paquets utiles pour Git

* [Git Config](https://packagecontrol.io/packages/Git Config) pour avoir une coloration syntaxique des configurations globale et locale de Git.
* [GitGutter](https://packagecontrol.io/packages/GitGutter) pour afficher dans la marge des symboles de lignes ajoutées, modifiées et supprimées, ainsi que des stats dans la barre d’état.
* [GitSyntaxes](https://packagecontrol.io/packages/GitSyntaxes) pour améliorer la coloration des fichiers de type Git (message de commit, script de *rebase* interactif, etc.).

### Paquets utiles pour le développement web

* [SublimeLinter](https://packagecontrol.io/packages/SublimeLinter) pour pour le **moteur de base** de tous les *linters* pris en charge.
* [SublimeLinter-contrib-standard](https://packagecontrol.io/packages/SublimeLinter-contrib-standard) pour utiliser **[StandardJS](http://standardjs.com/)** et en finir une bonne fois pour toutes avec le *bikeshedding* sur les réglages de [ESLint](http://eslint.org/).
* [StandardFormat](https://packagecontrol.io/packages/StandardFormat) pour aider à la **mise en conformité** de nos fichiers avec StandardJS (attention toutefois à décocher *Preferences > Package Settings > StandardFormat > Format On Save*, c’est trop pénible en automatique comme ça, et ça ralentit la sauvegarde).
* [Emmet](https://packagecontrol.io/packages/Emmet) pour des **raccourcis incroyables de saisie** HTML et CSS.
* [ChangeQuotes](https://packagecontrol.io/packages/ChangeQuotes) pour basculer facilement entre les **guillemets simples et doubles** (on aura toutefois besoin de reconfigurer le raccourci clavier sur les claviers OSX français).
* [Sass](https://packagecontrol.io/packages/Sass) ou [Stylus](https://packagecontrol.io/packages/Stylus) pour avoir une jolie coloration syntaxique avec nos **préprocesseurs CSS** chéris.
* [Babel](https://packagecontrol.io/packages/Babel) pour une coloration syntaxique haut de gamme sur **ES6+ et JSX** (React).
* [tern_for_sublime](https://packagecontrol.io/packages/tern_for_sublime) pour la **complétion intelligente sur JS** (y compris ES6+). [Voir ici](./tern.md) pour les détails de mise en œuvre, c‘est parfois un peu *tricky*.
* [Better CoffeeScript](https://packagecontrol.io/packages/Better CoffeeScript) pour une coloration syntaxique CoffeeScript (par exemple, pour la configuration de certains outils comme Brunch).

#### Un mot sur les modules basés Node

Les modules **SublimeLinter-contrib-standard** et **StandardFormat** nécessitent la présence des outils correspondants dans votre chemin d’exécution (`PATH`).  Ces outils s’installent tous *via* Node.js.

Si vous n’avez pas Node.js d’installé, [c’est par ici](./node.md).

Si vous l’avez, vous allez devoir installer les modules nécessaires en global :

```
npm install -g standard standard-format
```

Vérifiez alors que ça fonctionne en sollicitant le paquet de base, quitte à garder la console ouverte (*View > Show Console*) pour y repérer d’éventuels messages d’erreur.

Si vous utilisez NVM pour Node, ou si vous avez recours à des binaires installés par Homebrew sur OSX, il se peut que vous ayez besoin de préciser les chemins complets des commandes, si elles ne sont pas dans le `PATH` principal (mais sont étendues par votre fichier d’initialisation).  Sur OSX, un paquet qui peut aider est [Fix Mac Path](https://packagecontrol.io/packages/Fix%20Mac%20Path).

Du temps de ST2, les paquets comme **Sublime Linter** incorporaient les outils sous-jacents (tels que JSHint, par exemple), mais depuis ST3 cette approche a changé, d’où cette section.

### Paquets utiles pour Markdown

* [Markdown Preview](https://packagecontrol.io/packages/Markdown Preview) pour pouvoir produire facilement le **rendu HTML de nos fichiers Markdown**, en mode standard ou **GFM** (*GitHub-Flavored Markdown*).
* [MarkdownEditing](https://packagecontrol.io/packages/MarkdownEditing) pour rendre l’édition de fichiers Markdown **infiniment plus agréable** !

## La commande `subl` depuis le terminal

Une bonne manière d’utiliser ST3 sur un projet précis consiste à ouvrir le dossier du projet directement, avec *File > Open*.  Ça crée un « project *ad hoc* » avec sa propre fenêtre Sublime, du coup on ne navigue qu’au sein de ces fichiers-là.

On aura souvent envie d’ouvrir un fichier, ou carrément un dossier, dans Sublime depuis la ligne de commande.  Sublime fournit une petite commande pour ça, baptisée `subl`, mais encore faut-il qu’elle soit dans ton chemin d’exécution.

### Sur Windows

1. Édite tes variables d’environnement personnelles.  Ça dépend de ta version de Windows, mais généralement <kbd>Windows+Pause</kbd> ouvre les Propriétés Système, et là tu as un bouton *Variables d’Environnement…*.
2. Sélectionne la variable `PATH` (pour toi ou pour le système, comme tu veux/peux) et clique sur le bouton *Edit…* sous la liste en question.
3. Va tout à la fin de la valeur ; si elle ne se termine pas par un point-virgule (`;`), ajoutes-en un.  Finalement, ajoute le chemin de la commande `subl` fournie : `C:\Program Files\Sublime Text 3`.
4. Valide jusqu’à avoir refermé toutes les boîtes de dialogue

Pour tester, ouvre une nouvelle Invite de Commandes (`cmd`), et tape dedans :

```
subl Desktop
```

Ça devrait t’ouvrir une fenêtre Sublime Text 3 avec ton Bureau déjà prêt comme « projet *ad hoc* ».

### Sur OSX

Ouvre un terminal et fais le lien symbolique qui va bien :

```
$ sudo ln -nfs '/Applications/Sublime Text 3.app/Contents/SharedSupport/bin/subl' /usr/local/bin/subl
```

Pour tester, ouvre un Terminal, et tape dedans :

```
subl Desktop
```

Ça devrait t’ouvrir une fenêtre Sublime Text 3 avec ton Bureau déjà prêt comme « projet *ad hoc* ».

### Sur Linux

Sur Debian / Ubuntu / Mint, la commande `subl` est installée par défaut dans `/usr/bin`.

Sur les autres distros, on décompresse le tarball [fourni](https://www.sublimetext.com/3) et on le déplace ou bon nous semble (si on suit l’exemple de la version Debian & Cie, on le met dans /opt/).  Ça donnerait ceci (pensez à utiliser votre nom d’archive plutôt que celui mis ici) :

```
$ tar xjf sublime_text_3_build_xxxx_xxx.tar.bz2
$ sudo mkdir -p /opt
$ sudo mv 'Sublime Text 3' /opt/sublime_text_3
$ sudo ln -nfs /opt/sublime_text_3/sublime_text /usr/bin/sublime
$ sudo ln -nfs /opt/sublime_text_3/sublime_text /usr/bin/subl
```

Pour tester, tape ensuite dans ton shell :

```
$ subl ~/Desktop
```

Ça devrait t’ouvrir une fenêtre Sublime Text 3 avec ton Bureau déjà prêt comme « projet *ad hoc* ».

## ST3, ton éditeur par défaut ?

Si tu veux faire de Sublime ton éditeur par défaut, même pour les commandes basées terminal / shell (comme Git, par exemple), c’est possible, mais attention, comme Sublime est une application graphique, il faudra lui dire d’attendre que tu aies refermé le fichier (voire Sublime entier, sur Windows) pour qu’il rende la main dans le shell.

### Sur Windows

Pour ce qui est de l’éditeur invoqué par des commandes, c’est uniquement pertinent dans le **Git Bash** qui vient avec ton installation de Git (sinon, tu n’en as pas besoin).

Dans ton dossier utilisateur (`C:\Users\ton-compte`), tu as peut-être déjà un fichier `.bash_profile` (oui, ça démarre par un point).  Si c’est le cas, ouvre-le avec Sublime, sinon crée un fichier vide dans Sublime et sauve-le sous ce nom-là, dans ce dossier-là.

Ensuite, ajoute tout à la fin :

```
export EDITOR='subl -w'
```

N’oublie pas de sauver.  Ça sera effectif la prochaine fois que tu ouvres un **Git Bash**

Pour ce qui est **d’ouvrir certains types de fichiers avec Sublime par défaut**, tu fais comme d’habitude :

1. Trouve un fichier avec l’extension qui t’intéresse sur ton disque
2. Clique bouton droit dessus, choisis *Propriétés*
3. Dans l’onglet *Général*, dans la section *Type de fichier*, en face de *Ouvrir avec*, clique *Modifier…*
4. D’une version à l’autre de Windows, ça change de procédure mais en gros trouve le moyen de choisir une application sur la machine
5. Navigue dans `C:\Program Files\Sublime Text 3` et choisis `sublime_text.exe`.
6. Valide jusqu’à avoir fermé toutes les boîtes de dialogue

Tente de double-cliquer sur le fichier en question : ça devrait l’ouvrir dans Sublime !

Répète l’opération pour les autres types de fichier qui t’intéressent.

### Sur OSX

À la racine de ton compte (`/Users/ton-compte`), tu as peut-être déjà un fichier `.profile`, ou `.bash_profile`, ou `.bashrc`.  Si c’est le cas, ouvre-le avec Sublime, sinon crée un fichier vide dans Sublime et sauve-le sous le nom `.profile`, dans ce dossier-là.

Ensuite, ajoute tout à la fin :

```
export EDITOR='subl -w'
```

N’oublie pas de sauver.  Ça sera effectif la prochaine fois que tu ouvres un shell (nouvel onglet de Terminal, nouveau Terminal…).

Pour ce qui est **d’ouvrir certains types de fichiers avec Sublime par défaut**, tu fais comme d’habitude :

1. Trouve un fichier avec l’extension qui t’intéresse dans ton *Finder*
2. Clique bouton droit dessus, choisis *Get Info*
3. Dans la partie *Open with*, déroule la liste et choisis *Sublime Text 3 (build…)*.  Si tu ne le vois pas, choisis *Other…* et va chercher l’appli dans *Applications*
4. Clique ensuite sur le bouton *Change All…* pour en faire le choix par défaut, confirme en cliquant *Continue*.

Tente de double-cliquer sur le fichier en question : ça devrait l’ouvrir dans Sublime !

Répète l’opération pour les autres types de fichier qui t’intéressent.

### Sur Linux

À la racine de ton compte (`/home/ton-compte`), tu as peut-être déjà un fichier `.bash_profile`, ou `.bashrc` (ou `.zshrc` si tu fais du ZSH).  Si c’est le cas, ouvre-le avec Sublime, sinon crée un fichier vide dans Sublime et sauve-le sous le nom `.bash_profile`, dans ce dossier-là.

Ensuite, ajoute tout à la fin :

```
export EDITOR='subl -w'
```

N’oublie pas de sauver.  Ça sera effectif la prochaine fois que tu ouvres un shell.

Pour ce qui est **d’ouvrir certains types de fichiers avec Sublime par défaut**, ça dépend carrément de ton environnement graphique.

Côté interfaces graphiques, GNOME (la couche graphique par défaut d’Ubuntu, notamment) a un *GNOME Control Center* qui propose une partie *Default Applications* permettant ce type d’associations.  Il suffit alors d’associer le `sublime_text` de l’installation, ou un des liens symboliques `sublime` ou `subl` de `/usr/bin`, aux types souhaités.

D’une façon générale, la plupart des environnements graphiques Linux adhèrent au standard XDG, et la commande `xdg-open` est utilisée en interne, laquelle consulte entre autres `xdg-mime`.  Tu trouveras [plus de détails ici](https://wiki.archlinux.org/index.php/Xdg-open).
