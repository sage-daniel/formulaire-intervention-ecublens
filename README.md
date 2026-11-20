# Outil non officiel de préparation des interventions — Ecublens

Page statique non officielle, réservée aux membres du Conseil communal d’Ecublens, pour préparer une intervention sur le modèle officiel et télécharger le document en PDF, Word (`.docx`) ou LibreOffice (`.odt`).

## Utilisation

Publiez la page sur GitHub Pages ou servez le dossier avec un serveur HTTP local (par exemple `python3 -m http.server 8000`, puis ouvrez `http://localhost:8000`). L’ouverture directe de `index.html` avec `file://` ne permet pas au navigateur de charger le modèle PDF.

La taille du texte se choisit dans la liste 10, 11, 12 ou 13 pt. L’éditeur accepte le gras, l’italique, le souligné et le barré (⌘B/⌘I/⌘U sur Mac, Ctrl+B/Ctrl+I/Ctrl+U sur Windows/Linux, ⌘⇧X ou Ctrl+Shift+X pour barrer). Le nom, la date et la signature sont facultatifs.

Les six cases correspondent aux formats Word, PDF et ODT, chacun avec ou sans signature. Téléversez une image PNG/JPEG pour activer les cases « Avec signature ». Cliquez sur l’unique bouton « Télécharger » pour obtenir séparément chaque fichier sélectionné (aucun ZIP n’est créé). Le navigateur peut demander l’autorisation des téléchargements multiples.

« Prepare Email » ouvre un brouillon destiné à Silvana DellaVecchia. Le bouton ne peut pas joindre automatiquement les fichiers : ajoutez les documents téléchargés en pièces jointes.

Les informations et l’image de signature restent dans le navigateur : aucun formulaire n’est envoyé ni enregistré sur un serveur.

Le PDF est rempli à partir du modèle `Ecublens_Formulaire_PDF_Interventions.pdf`. Les exports Word et ODT reprennent son en-tête, ses cases et son cadre avec du texte éditable. Le modèle PDF et le logo `ecublens-logo.png` doivent rester à la racine du site et être inclus dans le dépôt publié. Les choix Vœu et Autre utilisent la case « Autre » du modèle, avec leur précision dans le champ correspondant.

## Publication sur GitHub Pages

Dans les paramètres du dépôt, activez GitHub Pages pour la branche `main` et le dossier `/ (root)`. Vérifiez que `index.html`, le PDF modèle et `ecublens-logo.png` sont présents à la racine de cette branche.

La génération des documents s’effectue dans le navigateur avec des bibliothèques chargées depuis jsDelivr. Une connexion Internet est donc nécessaire pour ouvrir la page et générer les fichiers.
