# Revue Typographie

Veille typographique libre : polices, fonderies et outils.

Site : https://olanlive.github.io/revue-typographie/ · RSS : https://olanlive.github.io/revue-typographie/feed.xml

Ajouter une entrée dans `data/discoveries.json`, puis `python3 scripts/build.py`.

## Version anglaise

Champs optionnels, à plat, à côté du français : `name_en`, `summary_en` (280 caractères maximum, même avertissement « ATTENTION » au build) et `source.label_en`. S’ils sont absents ou vides, la page anglaise (`docs/en/`) affiche le texte français dans un élément `lang="fr"`. L’ancre reste calculée sur `name` (ou `id`), jamais sur `name_en`. `date`, `url`, `tags` et `source.url` ne se traduisent pas.

`python3 scripts/build.py` écrit `docs/en/index.html`, `docs/en/tags/` et `docs/en/feed.xml`. Les pages anglaises réutilisent `docs/style.css`. Il n’y a pas de `docs/en/latest.json`.
