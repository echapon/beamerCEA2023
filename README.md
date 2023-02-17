## Thème CEA pour présentation Beamer avec LaTeX (charte graphique 2023)
Le thème est défini dans `beamerthemeCEA.sty`. Il implémente les recommendations de la charte graphique en terme de couleurs, organisation
des diapositives, fonds, etc. depuis le modèle officiel PowerPoint. Un exemple est disponible dans `beamerCEA.tex`. Les images nécessaires sont dans le dossier `graphics/`.  

### Polices
Le CEA recommande d'utiliser Arial, mais il est difficile d'inclure cette police dans un ensemble cohérent de polices avec des également des équations. Nous utilisons donc la police Helvetica, du paquet `helvet`. Pour les équations, nous utilisons également Helvetica, pour une meilleure correspondance avec le texte. Les lettres grecques et les symboles utilisent la police Computer Modern sans sérif. Les majuscules ajourées utilisent la police Doublestroke sans sérif. Les lettres calligraphiques utilisent la police ITC Zapf Chancery, mise à l'échelle avec le paquet `mathalfa`.

### Utilisation
* Les commandes habituelles `\title`, `\date`, et `\author` peuvent être utilisées. Une commande additionnelle `\seminar` est disponible pour le nom de la réunion ou de la conférence. Il est également possible de fournir un sous-titre pour la présentation au moyen de la commande `\subtitle`.
* Si une image est fournie au moyen de la commande `\titlepagepicture{titleimage.jpg}`, elle sera utilisée pour la page de titre (le côté gauche de l'image étant masqué par des cubes blancs comme dans le modèle officiel).
* Deux commandes sont disponibles pour créer des pages de table des matières (à utiliser sans `\begin{frame} \end{frame}`) : `\tocframe{Slide title}` et `\toframecurrent{Slide title}`, la deuxième utilisant `\tableofcontents[current]` pour mettre en valeur la `\section` courante.
* De même, des diapositives de transition peuvent être insérées au moyen de l'une des quatre commandes suivantes (chacune correspondant à une couleur) : `\sepframewhite{Additional text}`, `\sepframered{Additional text}`, `\sepframeblack{Additional text}`, `\sepframeblue{Additional text}`. Le numéro de la section courante et son titre apparaîtront en gros, suivis de l'argument de la commande (le laisser vide si aucun texte additionnel n'est désiré).
* Dernière diapositive :
  * Elle peut être personnalisée avec les commandes `\CEAmerci`, `\CEAcenter`, `\addr`, et `\CEAemail`.
  * Pour l'insérer, utiliser
```latex
\begin{frame}[plain]
    \usebeamertemplate*{last page}
\end{frame}
```
* Les diapositives additionnelles peuvent être séparées de la présentation principale avec la commande `\appendix`. De cette manière, elles ne seront pas comptées dans le compteur principal apparaissant dans le pied-de-page.

### Remerciements

Ce modèle (non officiel) est adapté de https://gitlab.com/1a7r0ch3/CEA (qui implémente la charte graphique précédente).

## CEA theme for beamer with LaTeX (2023 style guide)
Theme is defined in `beamerthemeCEA.sty`.  It adapts the recommended colours, slide layout, backgrounds, etc. from the official PowerPoint template. Template is `beamerCEA.tex`. Required graphics are in `graphics/`.  

### Fonts
CEA recommends using Arial, but we found it hard to include it in a consistent collection of fonts also including maths. Instead, we use the Helvetica font, loaded with package `helvet`. For the math font, we also use Helvetica, for a better blending with the text. Greeks and symbols are taken from the sans-serif Computer Modern font. Blackboard letters are set to sans-serif Doublestroke font. Calligraphic letters are set as Zapf Chancery and scaled with the `mathalfa` font.  

### Usage
* The usual `\title`, `\date`, and `\author` should be defined. An additional `\seminar` is available for the name of the meeting or conference. An optional `\subtitle` for the presentation can also be set.
* If an image file is provided with `\titlepagepicture{titleimage.jpg}`, it will be used for the title page (the left side of the image being masked by white cubes as in the official template).
* Two commands are provided for outline slides: `\tocframe{Slide title}` and `\toframecurrent{Slide title}`, the latter using `\tableofcontents[current]` to highlight the current `\section`.
* Transition slides can be inserted with one of the four following commands (choose your colour): `\sepframewhite{Additional text}`, `\sepframered{Additional text}`, `\sepframeblack{Additional text}`, `\sepframeblue{Additional text}`. The number of the current section and its title will appear in big, followed by the argument for the command (leave it empty if no additional text is needed).
* Last slide:
  * It can be customised with the commands `\CEAmerci`, `\CEAcenter`, `\addr`, and `\CEAemail`.
  * To call it, use
```latex
\begin{frame}[plain]
    \usebeamertemplate*{last page}
\end{frame}
```
* Backup slides can be separated from the main slides with the command `\appendix`. In this way, they will not be included into the main page counter appearing in the footer.

### Acknowledgements

This (non official) theme is adapted from https://gitlab.com/1a7r0ch3/CEA (which implemented previous style guide).
