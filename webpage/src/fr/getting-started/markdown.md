# Réduction

Cette feuille de triche Markdown est conçue comme une référence rapide et une vitrine de la syntaxe de Markdown dans QOwnNotes.

## En-têtes

Utilisez des titres pour structurer vos textes.

```markdown
# H1
## H2
### H3
#### H4
##### H5
###### H6
```

::: tip
Le **panneau de navigation** montre la structure de vos en-têtes.
:::

Alternativement, pour H1 et H2, un style souligné:

```markdown
Alt-H1
======

Alt-H2
------
```

::: tip
Par défaut, QOwnNotes crée le nom de fichier **d'une note** à partir de l'en-tête **1** (h1).
:::

## Accentuation

```markdown
Accentuation, aka italique, avec *astérisques*.

Emphase forte, aka gras, avec **astérisques**.
```

::: tip
Vous pouvez utiliser le [raccourci](./shortcuts.md) <kbd>Ctrl + B</kbd> pour mettre le texte en gras et <kbd>Ctrl + I</kbd> pour le mettre en italique.
:::

## Souligné

Il existe également un paramètre facultatif pour activer le rendu souligné dans les *Paramètres d'aperçu*.

```markdown
_souligner_
```

::: tip
Vous pouvez utiliser le [raccourci](./shortcuts.md) <kbd>Ctrl + U</kbd> pour souligner un texte.
:::

## Rayer

```markdown
~~biffer~~
```

::: tip
Vous pouvez utiliser le [raccourci](./shortcuts.md) <kbd>Alt + Maj + S</kbd> pour biffer un texte.
:::

## Listes

Il existe de nombreuses façons de créer des listes.

```markdown
1. Premier élément de liste commandé
2. Un autre article
   * Sous-liste non ordonnée.
1. Les chiffres réels n'ont pas d'importance, juste que c'est un nombre
   1. Sous-liste ordonnée (ne fonctionne que dans l'éditeur, pas dans l'aperçu)
4. Et un autre article.

* La liste non ordonnée peut utiliser des astérisques
- Ou moins
+ Ou avantages
```

::: tip
Si vous appuyez sur <kbd>Entrée</kbd> à la fin d'une liste, un nouvel élément de liste sera créé.
:::

## Liens

Il existe plusieurs façons de créer des liens.

```markdown
[Je suis un lien de style en ligne] (https://www.google.com)

[Je suis un lien de style en ligne avec titre] (https://www.google.com "Page d'accueil de Google")

[Vous pouvez utiliser des nombres pour les définitions de liens de style référence][1]

Les URL et URL entre crochets angulaires seront automatiquement transformées en liens dans l'aperçu. 
http://www.example.com ou <http://www.example.com>

[1]: https://www.qownnotes.org
```

::: tip
Vous pouvez utiliser le [raccourci](./shortcuts.md) <kbd> Ctrl + L</kbd> pour **créer des liens vers des pages Web ou d’autres notes**.

L'utilisation de <kbd>Ctrl + Maj + X</kbd> fera apparaître une boîte de dialogue qui vous aidera à **insérer des pièces jointes** dans votre note.

Vous pouvez appuyer sur <kbd>Ctrl + Espace</kbd> pendant que le curseur se trouve sur un lien dans l'édition de note pour suivre le lien.
:::

### Signets

Les signets utilisés par [l'extension de navigateur QOwnNotes Web Companion](./browser-extension.md) utilisent des liens dans des listes.

```markdown
- [Nom de la page Web] (https://www.example.com) #tag1 #tag2 une description et des balises
```

## Images

Les images peuvent être intégrées dans QOwnNotes. Ils seront affichés dans l'aperçu.

```markdown
![alt text](media/my-image.jpg)
```

::: tip
Vous pouvez utiliser le [raccourci](./shortcuts.md) <kbd>Ctrl + Maj + I</kbd> pour insérer une image dans une note. L'image peut également être dans le presse-papiers, la boîte de dialogue la détectera et affichera un aperçu.

Vous pouvez également coller directement une image du presse-papiers dans votre note avec <kbd>Ctrl + Maj + V</kbd>.
:::


## Code en ligne et blocs de code

```markdown
Le «code» en ligne a des «back-ticks autour».
```

::: tip
Vous pouvez utiliser le [raccourci](./shortcuts.md) <kbd>Ctrl + Maj + C</kbd> sur texte en ligne sélectionné ou juste à l'intérieur du texte pour créer un bloc de code en ligne.
:::

Les blocs de code sont délimités par des lignes avec trois contre-graduations ou sont indentés avec quatre espaces.

### Clôture 4 espaces

Ajoutez quatre espaces devant votre code pour le marquer comme bloc de code.

```markdown
    s = "Code avec espace en retrait"
    print s
```

### Clôture Backtick

Vous pouvez également utiliser trois backticks pour créer un bloc de code.
~~~markdown
```
Le code va ici
Le code va ici
```
~~~

::: tip
Vous pouvez utiliser le [raccourci] (./ shortcuts.md) <kbd>Ctrl + Maj + C</kbd> sur plusieurs lignes de texte sélectionnées ou dans une ligne vide pour créer un bloc de code. 
:::

### Clôture Backtick avec mise en évidence du code

Il y a aussi une coloration syntaxique avec des blocs de code dans QOwnNotes.

~~~ markdown
``` bash
# Je suis un commentaire
cd Notes
```
~~~

Les languages (et identifiants de blocs de code) actuellement pris en charge sont :

* BASh scripting, `bash`
* C, `c`
* C++, `cpp`
* C++, `cxx`
* C++, `c++`
* C#, `c#`
* CMake, `cmake`
* C#, `csharp`
* CSS, `css`
* Go, `go`
* HTML, `html`
* INI, `ini`
* Java, `java`
* JavaScript, `javascript`
* JavaScript, `js`
* JSON, `json`
* Makefile, `make`
* PHP, `php`
* Python, `py`
* Python, `python`
* QML, `qml`
* Rust, `rust`
* Shell scripting, `sh`
* SQL, `sql`
* TypeScript, `ts`
* TypeScript, `typescript`
* V, `v`
* Vex, `vex`
* XML, `xml`
* YAML, `yml`
* YAML, `yaml`

## Tableaux

Les tableaux ne font pas partie des spécifications originales de Markdown mais le mode de prévisualisation de QOwnNotes les prend en charge. 

~~~markdown
Les double-points peuvent être utilisés pour aligner le contenu des colonnes.

| Les Tables | Sont | Chouettes |
| ------------- |: -------------: | -----: |
| col 3 est | alignée à droite | 1600 $ |
| col 2 est | centrée | 12 $ |
| rayures zébrées | sont soignées | 1 $ |

Il doit y avoir au moins 3 tirets séparant chaque cellule d'en-tête.

Vous pouvez également utiliser le Markdown en ligne.

| Markdown | Moins | Jolie |
| --- | --- | --- |
| *Encore* | `rend` | **bien** |
| 1 | 2 | 3 |
~~~

::: tip
Appuyez sur <kbd>Alt + Maj + T</kbd> pour faire apparaître une boîte de dialogue qui vous aidera à créer des tableaux. Vous pouvez même importer des fichiers CSV dans cette boîte de dialogue.

Utilisez <kbd>Ctrl + Espace</kbd> dans un tableau de démarquage pour le formater automatiquement.
:::

## Blocs de citation

```markdown
> Les blockquotes sont très pratiques dans les e-mails pour émuler le texte de réponse.
> Cette ligne fait partie du même devis.

Citation pause.

> This is a very long line that will still be quoted properly when it wraps. Oh mon garçon, continuons à écrire pour nous assurer que cela est assez long pour que tout le monde puisse en profiter. Oh, vous pouvez *mettre* **Markdown** dans un blockquote. 
```

::: tip
Vous pouvez dire à QOwnNotes de surligner entièrement les blockquotes ou juste le caractère blockquote dans les *Paramètres de l'éditeur*

Vous pouvez utiliser le [raccourci](./shortcuts.md) <kbd>Ctrl + Maj + B</kbd> pour marquer le texte comme blockquote.
:::

## Règle horizontale

Il existe trois façons d'obtenir une règle horizontale: traits d'union, astérisques ou traits de soulignement.

```markdown
Trois ou plus ...

Traits d'union

---

Astérisques

***

Soulignements

___

Traits d'union

---

Astérisques

***

Soulignements

___
```

## Sauts de ligne

- Vous pouvez construire un paragraphe comme un enchaînement de plusieurs lignes pour en faciliter l'édition, il sera tout de même affiché comme un seul paragraphe.
- Dans un paragraphe, vous pouvez forcer un retour à la ligne en insérant deux espaces à la fin d'une ligne.
- Vous pouvez définir un paragraphe distinct en le délimitant avec des sauts de ligne.

::: tip
Vous pouvez insérer deux espaces et un retour à la ligne avec <kbd>⇧ Shift</kbd> + <kbd>Entrée</kbd>.
:::

```markdown
Voici une ligne pour nous de commencer.

Cette ligne est séparée de celle ci-dessus par deux nouvelles lignes, ce sera donc un *paragraphe séparé*.

Cette ligne commence également un paragraphe séparé, mais ...
Cette ligne n'est séparée que par deux espaces de fin et un seul saut de ligne, c'est donc une ligne distincte dans le *même paragraphe*.
```

::: tip
Les espaces de fin sont mis en évidence par défaut dans l'éditeur.
:::

## Commentaires

Les commentaires ne sont pas affichés dans l'aperçu.

```markdown
[comment]: # (Ce commentaire n'apparaîtra pas dans l'aperçu)

<! - Les commentaires HTML sont également masqués ->
```

::: tip
Un bloc de commentaire HTML en tête d'une note sera également ignoré dans la génération automatique du nom de fichier de la note.
:::

## Listes de cases à cocher

Vous pouvez créer des listes de tâches simples avec des listes de cases à cocher.

```markdown
- [x] fait
- [ ] à faire
```

::: tip
Vous pouvez cocher / décocher les cases à cocher dans l'aperçu.
:::

## Frontmatter

Dans QOwnNotes, vous pouvez utiliser un « frontmatter » (par exemple YAML) pour ajouter des méta-informations supplémentaires. Cela ne sera **pas affiché dans l'aperçu** et ne perturbera **pas la génération automatique de nom de fichier de note**.

```markdown
---
title: un nom
description: une description
---

# Le titre de la note commence ici

Du texte
```

Le nom de fichier de cet exemple de note serait `L'en-tête de la note commence ici.md`.
