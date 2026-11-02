# Ma première contribution depuis le navigateur

Ce guide t'accompagne pas à pas pour proposer ta première modification à **mboka**, sans rien installer : uniquement un compte GitHub et ton navigateur.

**Durée estimée :** 15 à 20 minutes.

**Ce que tu vas faire :**

1. Forker le dépôt
2. Modifier un fichier dans l'éditeur web de GitHub
3. Créer une branche et un commit au bon format
4. Ouvrir la Pull Request vers le dépôt principal
5. Répondre à une demande de modification

> Pas de panique : tu ne peux rien casser. Ton travail se fait sur ta propre copie, et rien n'est fusionné sans relecture.

---

## Avant de commencer

- Un compte GitHub (gratuit) : <https://github.com/signup>
- Une issue choisie, étiquetée `good first issue` : <https://github.com/mboka-dev/core/issues>
- Commente l'issue (« Je prends celle-ci ») pour éviter que deux personnes fassent le même travail.

---

## Étape 1 : Forker le dépôt

Un *fork* est ta copie personnelle du projet, hébergée sur ton compte.

1. Ouvre <https://github.com/mboka-dev/core>.
2. Clique sur **Fork** en haut à droite.
3. Laisse le nom par défaut, puis clique sur **Create fork**.

![Bouton Fork en haut à droite du dépôt](images/01-fork-bouton.png)

Tu arrives sur `https://github.com/<ton-pseudo>/core`. Vérifie sous le titre : tu dois lire « forked from mboka-dev/core ».

![Page de ton fork](images/02-fork-cree.png)

---

## Étape 2 : Modifier un fichier dans l'éditeur web

1. Dans **ton fork**, ouvre le fichier à modifier (par exemple `README.md`).
2. Clique sur l'icône **crayon** (Edit this file) en haut à droite du fichier.
3. Fais ta modification dans l'éditeur.
4. Onglet **Preview** : relis le rendu avant de continuer.

![Icône crayon pour éditer un fichier](images/03-editer-crayon.png)

![Éditeur web de GitHub avec une modification](images/04-editeur-modification.png)

> Pour un nouveau fichier : bouton **Add file → Create new file**, puis saisis le chemin complet dans le nom (par exemple `docs/mon-fichier.md`). Taper `/` crée automatiquement le dossier.

---

## Étape 3 : Créer une branche et un commit au bon format

Un *commit* enregistre ta modification. Une *branche* la garde séparée du reste.

1. Clique sur **Commit changes…** (bouton vert en haut à droite).
2. Dans le champ **Commit message**, écris un message au format :

   ```
   type(portée): description courte à l'impératif
   ```

   Exemples :

   ```
   docs: ajouter un README en anglais
   data(phone): confirmer le plan de numérotation +242
   test(fixtures): ajouter des cas limites Unicode
   ```

   Types courants : `docs`, `feat`, `fix`, `test`, `data`, `ci`.
   La portée (entre parenthèses) est facultative.

3. Choisis **Create a new branch for this commit and start a pull request**.
4. Donne un nom clair à la branche, par exemple `docs/readme-anglais`.
5. Clique sur **Propose changes**.

![Fenêtre Commit changes avec message et nouvelle branche](images/05-commit-branche.png)

---

## Étape 4 : Ouvrir la Pull Request vers le dépôt principal

Une *Pull Request* (PR) demande aux mainteneurs d'intégrer ta modification.

1. Tu arrives sur la page **Open a pull request**. Vérifie en haut :
   - **base repository** : `mboka-dev/core`
   - **head repository** : ton fork
2. Titre : reprends le message de ton commit.
3. Description : explique brièvement ce que tu as fait et mentionne l'issue :

   ```
   Closes #4
   ```

4. Si ta modification touche des données, **cite ta source** (lien et date).
5. Clique sur **Create pull request**.

![Formulaire d'ouverture de la Pull Request](images/06-ouvrir-pr.png)

C'est fait ! Ta PR apparaît dans l'onglet **Pull requests** du dépôt principal.

---

## Étape 5 : Répondre à une demande de modification

Les mainteneurs relisent ta PR et peuvent demander des changements. C'est normal, et c'est même bon signe : ils s'intéressent à ta contribution.

1. Tu reçois une notification (e-mail ou cloche GitHub).
2. Ouvre ta PR et lis les commentaires dans l'onglet **Conversation**.
3. Pour corriger : va dans l'onglet **Files changed**, ouvre le menu **⋯** du fichier, puis **Edit file**. Tu modifies **la même branche**, et la PR se met à jour toute seule.
4. Commit sur la branche existante (**Commit directly to the `<ta-branche>` branch**).
5. Réponds au commentaire (« Corrigé ») et clique sur **Resolve conversation** si tu peux.

![Commentaire de relecture sur une PR](images/07-demande-modification.png)

Une fois la PR approuvée, un mainteneur la fusionne. Bravo, tu es contributeur·rice de mboka !

---

## Un souci ?

- Ouvre une issue ou pose ta question en commentaire sur ta PR.
- Retrouve toutes les règles dans [CONTRIBUTING.md](../CONTRIBUTING.md).
