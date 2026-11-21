# Conseil communal Ecublens — Alternative pour un formulaire officiel d’intervention

Page statique réservée aux membres du Conseil communal d’Ecublens : une alternative simple et directe pour préparer une intervention sur le formulaire officiel et télécharger le document en PDF, Word (`.docx`) ou LibreOffice (`.odt`).

## Utilisation

Publiez la page sur GitHub Pages ou servez le dossier avec un serveur HTTP local (par exemple `python3 -m http.server 8000`, puis ouvrez `http://localhost:8000`). L’ouverture directe de `index.html` avec `file://` ne permet pas au navigateur de charger le modèle PDF.

La taille du texte se choisit dans la liste 10, 11, 12 ou 13 pt. L’éditeur accepte le gras, l’italique, le souligné et le barré (⌘B/⌘I/⌘U sur Mac, Ctrl+B/Ctrl+I/Ctrl+U sur Windows/Linux, ⌘⇧X ou Ctrl+Shift+X pour barrer). Le nom, la date et la signature sont facultatifs.

Le nom des fichiers est proposé au format `type-nom-date`, par exemple `amendement-sage-daniel-2026-11-21`. Il peut être personnalisé dans le champ dédié ; le suffixe de signature et l’extension sont ajoutés automatiquement.

Les six cases correspondent aux formats Word, PDF et ODT, chacun avec ou sans signature. Utilisez « Upload signature » pour choisir une image PNG/JPEG et activer les cases « Avec signature ». Cliquez sur l’unique bouton « Télécharger » pour obtenir séparément chaque fichier sélectionné (aucun ZIP n’est créé). Le navigateur peut demander l’autorisation des téléchargements multiples.

« Prepare Email » ouvre un brouillon destiné à Silvana DellaVecchia. Le bouton ne peut pas joindre automatiquement les fichiers : ajoutez les documents téléchargés en pièces jointes.

Les informations et l’image de signature restent dans le navigateur : aucun formulaire n’est envoyé ni enregistré sur un serveur.

Le PDF est rempli directement à partir du modèle `Ecublens_Formulaire_PDF_Interventions.pdf`. Les exports Word et ODT utilisent une copie visuelle de ce PDF comme fond de page ; les éléments saisis sont superposés en texte éditable. L’image de fond `template-formulaire.png`, générée depuis le PDF officiel, doit rester à la racine avec `index.html` et le PDF modèle. Les choix Vœu et Autre utilisent la case « Autre » du modèle, avec leur précision dans le champ correspondant.

## Publication sur GitHub Pages

Dans les paramètres du dépôt, activez GitHub Pages pour la branche `main` et le dossier `/ (root)`. Vérifiez que `index.html`, le PDF modèle et `template-formulaire.png` sont présents à la racine de cette branche.

La génération des documents s’effectue dans le navigateur avec des bibliothèques chargées depuis jsDelivr. Une connexion Internet est donc nécessaire pour ouvrir la page et générer les fichiers.
