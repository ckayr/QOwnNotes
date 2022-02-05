# Installer en tant qu'AppImage

Vous pouvez télécharger la dernière AppImage à partir de la [page des versions de QOwnNotes](https://github.com/pbek/QOwnNotes/releases). Elle devrait être nommée `QOwnNotes-x86_64.AppImage` sur cette page.

::: tip
Si [jq](https://stedolan.github.io/jq/) est installé vous pouvez également télécharger directement l'AppImage la plus récente :

```bash
# demander la version Linux la plus récente depuis l'API QOwnNotes, faire l'analyse syntaxique du JSON pour obtenir son URL et la télécharger
curl -L https://api.qownnotes.org/latest_releases/linux | jq .url | xargs curl -Lo QOwnNotes-x86_64.AppImage
```
:::

Vous pouvez ensuite modifier les autorisations d'exécution du fichier :

```bash
chmod a+x QOwnNotes-*.AppImage
```

Vous devriez ensuite être en mesure d'exécuter l'AppImage pour lancer QOwnNotes.

::: warning
Si vous souhaitez utiliser la **mise à jour automatique**, assurez-vous de placer votre AppImage à un endroit où votre compte utilisateur a un accès en écriture, par exemple quelque part dans votre répertoire personnel.
:::

::: tip
Si vous rencontrez des difficultés pour exécuter l'AppImage parce que votre version de glibc est trop ancienne vous pouvez essayer l'[AppImage d'OBS](https://download.opensuse.org/repositories/home:/pbek:/QOwnNotes/AppImage/QOwnNotes-latest-x86_64.AppImage), qui devrait avoir été constuite en utilisant glibc 2.16.
:::
