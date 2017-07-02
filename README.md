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
* github.com účet (nebo jakýkoli git hosting)
* Drupal 8 + Composer using https://github.com/drupal-composer/drupal-project
* Funkční příkazovou řádku (lokálně)
* Připravené SSH klíče ( https://help.github.com/articles/connecting-to-github-with-ssh/ )

## Založení projektu
* Vytvořit nový *prázdný* git repozitář https://github.com/new ideálně nazvaný stejně jako složka na hostingu v `~/www`, tedy `nazevprojektu.cz`
* lokálně:
  * `composer create-project drupal-composer/drupal-project:8.x-dev nazevprojektu.cz --stability dev --no-interaction`
  * `cd nazevprojektucz`
  * `git init`
  * `git add .`
  * `git commit -m "Thanks @radimklaska :)"`
  * `git remote add origin git@github.com:tvojejmeno/nazevprojektu.cz.git`
  * `git push -u origin master`

## Inicializace
* V administraci hostingu přidat 2 subdomény `dev` a `stage`.
* Nastavit přístup bez hesla na `ssh nazevprojektucz@access.snackhost.eu` (viz GitHub help)
* Pokud je git repozitář projektu privátní, je třeba na hostingu vygenerovat ssh klíč a autorirovat ho na git hostingu ("Deploy keys" na GitHubu).
* Na hostingu:
  * `git clone https://github.com/radimklaska/snackhost_drupal_workflow.git ~/snackhost_drupal_workflow`
  * `ToDo`


## Použití
* ToDo
