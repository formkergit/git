# Mini guide Git

## Configuration

-   Définir le nom d’utilisateur :
    `git config --global user.name "Votre Nom"`
-   Définir l’email :
    `git config --global user.email "votre.email@exemple.com"`
-   Branche par défaut definit à `main` :
    `git config --global init.defaultBranch main`

## Démarrage

-   Initialiser un dépôt, espace(répertoire) de travail : `git init`
-   Cloner un dépôt : `git clone <url_repo>`

## Gitignore

Utilisez un fichier `.gitignore` pour exclure des fichiers ou des
répertoires du suivi.

    .env
    node_modules/

    *.log

## Ajout et Commit

-   Toujouts vérifier l’état du dépôt : `git status`
-   Ajouter des fichiers à la zone de staging : `git add .` (ou fichier
    spécifique : `git add nom_fichier`)
-   Valider les modifications : `git commit -m "Message de commit"`

## Journaux & Historique

-   Voir l’historique des commits : `git log`
-   Afficher un commit spécifique : `git show <commit_hash>`
-   Annuler des modifications :
    -   Réinitialisation douce : `git reset <commit_hash>` (garde les
        modifications dans le répertoire de travail)
    -   Réinitialisation dure : `git reset --hard <commit_hash>`
        (supprime les modifications)

## Branches & Fusion

-   Créer une branche : `git checkout -b <nom-branche>`
-   Changer de branche : `git checkout <nom-branche>`
-   Fusionner une branche : `git merge <nom-branche>`
-   Supprimer une branche :
    -   Localement : `git branch -d <nom-branche>`
    -   À distance : `git push origin --delete <nom-branche>`

## Travailler avec des dépôts distants

-   Ajouter un dépôt distant : `git remote add origin <url_repo>`
-   Pousser les modifications vers une dépôt distant de la branche main
    : `git push -u origin main`
-   Rapatrier les modifications du dépôt distant :
    `git pull origin main`

## Travail avec un hébergeur git (Github,Gitlab,...)

## Ce qu’on peut faire chez un hébergeur git

-   **Sauvegarder** votre travail avec **git** en local chez l’hébergeur
-   **Pull Request**: demander à fusionner vos chamgements dans le dépôt
    (travail collaboratif)
-   **Issues**: Retour de **bug,amélioration,tâche à faire**
-   **Actions,Pipelines**: Automatiser les déployements **CI/CD**

## Configuration SSH

([Docuemntation
Github](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent))

([Documentation Gitalb](https://docs.gitlab.com/user/ssh/))
