# SnackHost Drupal 8 workflow

NOTE: Work in progress!

Podpůrné scripty pro Drupal 8 dev/stage/prod workflow na SnackHost: http://www.jdoqocy.com/2c111js0ys-FOJMOHHIFHINKNKMO (affiliate, díky)

## Background
* Mám rád best practice, ale některé projekty prostě nemají budget pro high end hosting.
* Nechci spravovat vlastní server.
* Rád bych se vyhnul dalším placeným službám.
* SnackHost mi byl doporučen na drupal.cz meetupu. Využil jsem affiliate program, jinak nemám se SnackHostem nic společného.

## Požadavky
* Aktivní Cloud Hosting (ne Cloud Server)
* Drupal 8 + Composer
* Funkční příkazovou řádku (lokálně)
* Připravené SSH klíče ( https://help.github.com/articles/connecting-to-github-with-ssh/ )

## Inicializace
* V administraci hostingu přidat 2 subdomény `dev` a `stage`.
* Nastavit přístup bez hesla na `ssh NAZEVPROJEKTU@access.snackhost.eu` (viz GitHub help)
* `git clone https://github.com/radimklaska/snackhost_drupal_workflow.git ~/snackhost_drupal_workflow`

## Použití
* ToDo
