# Memory PCM — application Android

Ce dossier contient le jeu Memory PCM sous forme d'application Android.
L'APK est fabriquée gratuitement par GitHub. Rien à installer sur votre ordinateur.

## 1. Créer le dépôt
1. Connectez-vous sur https://github.com (créez un compte si besoin).
2. En haut à droite : « + » → « New repository ».
3. Nom : `memory-pcm`. Laissez le reste par défaut. Bouton « Create repository ».

## 2. Déposer les fichiers
1. Sur la page du dépôt, cliquez sur « uploading an existing file ».
2. Ouvrez le dossier `memory-pcm-android` sur votre ordinateur, sélectionnez **tout son contenu**
   et glissez-le dans la page.
3. En bas : « Commit changes ».

Vérifiez que le dépôt contient bien un dossier `.github`. Ce dossier est parfois masqué
par l'ordinateur et n'est alors pas envoyé. Dans ce cas :
1. « Add file » → « Create new file ».
2. Nom du fichier : `.github/workflows/build-apk.yml`
3. Copiez-collez le contenu du fichier `build-apk.yml` fourni, puis « Commit changes ».

## 3. Récupérer l'APK
1. Onglet « Actions » du dépôt : une tâche « Construire l'APK » démarre seule
   (sinon, cliquez dessus puis « Run workflow »).
2. Attendez la coche verte (3 à 6 minutes).
3. Cliquez sur la tâche terminée, puis en bas sur « memory-pcm-apk » : un fichier zip se télécharge.
4. Décompressez-le : il contient `app-debug.apk`.

## 4. Installer sur le téléphone
1. Envoyez `app-debug.apk` sur le téléphone (mail, WhatsApp, câble, Drive…).
2. Ouvrez-le. Android demande d'autoriser l'installation depuis cette source : acceptez.
3. L'icône « Memory PCM » apparaît.

Vous pouvez envoyer le même fichier `app-debug.apk` à d'autres personnes.

## Mettre à jour le jeu
Remplacez le fichier `app/src/main/assets/index.html` dans le dépôt par la nouvelle version :
GitHub refabrique l'APK automatiquement. Pour installer la mise à jour sur un téléphone
qui a déjà l'appli, ouvrez simplement le nouvel APK.

## Bon à savoir
- Le jeu fonctionne hors ligne. Sans internet, il utilise la police du téléphone au lieu
  de celles du jeu ; tout le reste est identique.
- La progression, les records et l'ambiance sont enregistrés dans l'appli, sur le téléphone.
- Il s'agit d'une version de test : elle n'est pas destinée au Play Store en l'état.
