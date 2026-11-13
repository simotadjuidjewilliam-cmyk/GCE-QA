GCE ANSWERS — PROJET ANDROID COMPLET POUR GITHUB ACTIONS
Powered by Tadjuidje Labs

IMPORTANT
Ce ZIP contient le PROJET SOURCE Android complet pour générer un APK avec GitHub Actions.
Ce n'est pas encore un fichier APK installable. Ne renommez pas le ZIP en .apk.

IDENTITÉ DU PROJET
- Nom affiché : GCE Answers
- Identifiant Android : com.tadjuidjelabs.gceanswers
- Interface intégrée : GCE Answers V9 (fichier HTML autonome)
- Technologie : application Android avec WebView
- Version : 1.0-demo

INVENTAIRE DES FICHIERS
- settings.gradle : configuration du projet et module app
- build.gradle : version du plugin Android
- gradle.properties : paramètres Gradle
- .gitignore : fichiers à ignorer
- app/build.gradle : configuration de l'application Android
- app/src/main/AndroidManifest.xml : déclaration Android et activité principale
- app/src/main/java/com/tadjuidjelabs/gceanswers/MainActivity.java : activité Android/WebView
- app/src/main/assets/index.html : interface GCE Answers V9 intégrée
- app/src/main/res/values/styles.xml : thème Android
- .github/workflows/build-apk.yml : compilation automatique et dépôt de l'APK
- DEMARRAGE_GITHUB_ANDROID.txt : guide simplifié pour téléphone

INSTALLATION DU CODE DANS GITHUB DEPUIS ANDROID
1. Téléchargez puis décompressez ce ZIP dans l'application Files.
2. Ouvrez le dépôt GCE-Questions-Answers sur GitHub et sélectionnez la branche main.
3. Envoyez TOUS les fichiers et dossiers extraits à la RACINE du dépôt, sans créer un dossier parent supplémentaire.
4. Vérifiez particulièrement que le dossier caché .github est présent et que le chemin complet est : .github/workflows/build-apk.yml.
5. Validez l'envoi avec Commit changes sur main.
6. Ouvrez Actions et choisissez Build GCE Answers APK.
7. Si nécessaire, appuyez sur Run workflow.
8. Attendez la coche verte, ouvrez l'exécution, puis téléchargez l'artefact GCE-Answers-debug-APK.
9. Décompressez l'artefact : le fichier à installer est app-debug.apk.

STRUCTURE ATTENDUE À LA RACINE GITHUB
.github/
app/
build.gradle
settings.gradle
gradle.properties
.gitignore

À SAVOIR
- Le workflow installe Java 17, Android SDK et Gradle 8.9 automatiquement. Un Gradle Wrapper local n'est donc pas requis pour cette compilation GitHub Actions.
- Le workflow produit un APK de débogage (debug), pas un APK signé pour publication Play Store.
- Cette livraison est un conteneur Android pour l'interface V9. Les fonctions qui nécessitent un serveur réel (comptes synchronisés, paiement, administration distante, bibliothèque hébergée ou IA distante) exigent un backend et des services séparément configurés.
- Les données de démonstration peuvent rester locales à l'appareil. Ne l'utilisez pas pour de vrais paiements ou des données sensibles de candidats.
