# Workflow

![Git Workflow](https://nvie.com/img/git-model@2x.png)

La branche `releases` sers de branche de production, où on ne merge que les versions finalisées de l'application.

Pour chaque feature en développement, on crée une branche spécifique avec un nom explicite, par exemple pour un écran de login: `login-screen`.
Chaque nouvelle feature doit être développée dans une nouvelle branche, pour ajouter un connexion par facebook à l'écran de login si son développement est "terminé", on **crée** une nouvelle branche: `facebook-login` par exemple.

La branche `master` sert de branche de développement principale. On y merge les retours branches de features, c'est-à-dire qu'**on merge d'abord `mater` dans la branche de feature** pour y résoudre les conflits avant de merge dans `mater`.
La branche master ne doit contenir **que des bugfixes**.

