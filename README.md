# Une histoire de l'informatique

Site statique retraçant l'histoire de l'informatique, réalisé en équipe dans le module « Versionnage et intégration continue ».

## Présentation

- **Équipe** : ROGET Elora, SOULIER Rémi, PATRIGOT Elysabeth, BROCHETTA Aurélien
- **Responsable du dépôt** : SOULIER Rémi
- **Contenu** : une page d'accueil qui présente Ada Lovelace et qui redirige vers les pages suivantes : 
- Page de sa jeunesse et de sa formation
- Page de sa création de la machine analytique et le premier algorithme
- Page de sa fin de vie et de son héritage moderne

## Installation

Aucun outil de build n'est nécessaire : le site est en HTML et CSS.

```shell
git clone git@github.com:<organisation>/<depot>.git
cd <depot>
```

Ouvrez ensuite `index.html` dans votre navigateur.

## Contribuer

### Modèle de branches

Nous utilisons **Git Flow** :

- `main` : la version en production, uniquement mise à jour par les releases et les hotfixes
- `develop` : la version de recette, où arrivent les fonctionnalités
- `feature/<numéro-issue>-<sujet>` : une branche par fonctionnalité, créée depuis `develop`

Personne ne pousse directement sur `main` ou `develop`.

### Convention de commit

Conventional Commits : `feat: ajoute la page Turing`.

### Relecture

Toute modification passe par une **Pull Request** vers `develop`, qui :

- référence son issue (`Closes #3`)
- est relue par au moins un autre membre de l'équipe

### Ajouter sa page

1. Créez une issue pour votre page et assignez-la vous
2. Créez votre branche depuis `develop` : `git switch -c feature/<numéro>-<sujet> develop`
3. Copiez `pages/exemple.html` sous un nouveau nom et remplissez-la
4. Ajoutez votre page à la frise dans `index.html`, à sa place chronologique
5. Ouvrez une Pull Request vers `develop`

## Déploiement

À compléter : comment le site est déployé en recette et en production, et comment vérifier la version déployée.
