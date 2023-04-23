# Configurer Git et GitHub

Configurer votre compte Git et GitHub est une étape essentielle pour une collaboration réussie sur les projets et une gestion efficace de version. Dans cette présentation, nous couvrirons les étapes pour configurer votre compte Git et GitHub.

## Configurer la clé SSH

1. Ouvrez le Terminal ou Git Bash sur votre ordinateur.
2. Tapez `ssh-keygen -t ed25519 -C "votre_email@example.com"` et appuyez sur Entrée pour générer une nouvelle paire de clés SSH.
3. Appuyez sur Entrée pour accepter le nom et l'emplacement de fichier par défaut.
4. Tapez une phrase de passe pour sécuriser votre clé SSH et appuyez sur Entrée.
5. Tapez `cat ~/.ssh/id_ed25519.pub` pour afficher le contenu de votre clé publique.
6. Copiez le contenu de la clé publique.

## Ajouter la clé SSH à votre compte GitHub

1. Connectez-vous à votre compte GitHub.
2. Cliquez sur votre photo de profil en haut à droite et sélectionnez "Settings" (Paramètres).
3. Dans le menu de gauche, sélectionnez "SSH and GPG keys".
4. Cliquez sur le bouton "New SSH key".
5. Donnez un nom à votre clé SSH et collez le contenu de la clé publique.
6. Cliquez sur "Add SSH key".

## Configurer la clé GPG

1. Ouvrez le Terminal ou Git Bash sur votre ordinateur.
2. Tapez `gpg --full-generate-key` et suivez les invites pour générer une nouvelle paire de clés GPG.
3. Tapez `gpg --list-secret-keys --keyid-format LONG` pour afficher l'identifiant de votre clé GPG.
4. Copiez l'identifiant de la clé GPG (qui ressemble à `sec rsa4096/XXXXXXXXXXXXXXXX 2021-04-01`).
5. Tapez `gpg --armor --export XXXXXXXXXXXXXXXX` (en remplaçant les X par l'identifiant de votre clé GPG) pour afficher le contenu de votre clé publique GPG.
6. Copiez le contenu de la clé publique.

## Ajouter la clé GPG à votre compte GitHub

1. Connectez-vous à votre compte GitHub.
2. Cliquez sur votre photo de profil en haut à droite et sélectionnez "Settings" (Paramètres).
3. Dans le menu de gauche, sélectionnez "SSH and GPG keys".
4. Cliquez sur le bouton "New GPG key".
5. Collez le contenu de la clé publique GPG.
6. Cliquez sur "Add GPG key".

## Configurer les paramètres globaux

1. Ouvrez le Terminal ou Git Bash sur votre ordinateur.
2. Tapez `git config --global user.name "Votre Nom"` et appuyez sur Entrée pour configurer votre nom.
3. Tapez `git config --global user.email "votre_email@example.com"` et appuyez sur Entrée pour configurer votre adresse e-mail.

En suivant ces étapes, vous pouvez configurer votre compte Git et GitHub et être prêt à collaborer avec d'autres sur des projets et à gérer efficacement

# Comment démarrer un nouveau projet avec Git

Git est un système de contrôle de version largement utilisé pour gérer les changements de code source d'un projet. GitHub est un service en ligne qui héberge des dépôts Git et facilite la collaboration entre les développeurs. Dans ce tutoriel, nous allons voir comment démarrer un nouveau projet avec Git et GitHub.

## Étape 1 : Créer un nouveau dépôt sur GitHub

1. Connectez-vous à votre compte GitHub.
2. Cliquez sur le signe plus (+) dans la barre de navigation en haut à droite.
3. Cliquez sur **New repository**.
4. Entrez un nom pour votre dépôt dans le champ **Repository name**.
5. Choisissez si vous voulez que votre dépôt soit public ou privé.
6. Cochez la case **Initialize this repository with a README** pour ajouter un fichier README à votre projet.
7. Cliquez sur le bouton **Create repository**.

## Étape 2 : Cloner votre dépôt sur votre ordinateur

1. Ouvrez votre terminal ou Git Bash.
2. Tapez `git clone url-de-votre-dépôt` dans le terminal et appuyez sur Entrée. Remplacez `url-de-votre-dépôt` par l'URL de votre dépôt GitHub. Vous pouvez trouver cette URL sur la page de votre dépôt GitHub, dans la section **Clone or download**.

## Étape 3 : Ajouter des fichiers à votre projet

1. Ouvrez votre éditeur de texte préféré et créez un nouveau fichier.
2. Ajoutez du contenu à votre fichier.
3. Enregistrez votre fichier.

## Étape 4 : Commit et push

1. Tapez `git add .` dans le terminal et appuyez sur Entrée pour ajouter tous les fichiers modifiés à l'index.
2. Tapez `git commit -m "message de votre commit"` dans le terminal et appuyez sur Entrée pour committer les modifications. Remplacez `message de votre commit` par un message décrivant les modifications que vous avez apportées.
3. Tapez `git push` dans le terminal et appuyez sur Entrée pour pousser vos modifications sur GitHub.

Maintenant que vous avez commencé un nouveau projet avec Git, vous pouvez ajouter des commits et des branches pour organiser votre travail.

## Conclusion

Dans ce tutoriel, vous avez appris comment configurer Git et GitHub, comment démarrer un nouveau projet avec Git, et comment ajouter des fichiers, des commits et des branches à votre projet. En utilisant Git et GitHub, vous pouvez travailler en collaboration avec d'autres développeurs et suivre les changements de votre projet au fil du temps.
