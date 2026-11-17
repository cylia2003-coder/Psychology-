# Psychologie — application mobile (PWA)

Application de révision installable sur téléphone, qui fonctionne **hors ligne**.

## Contenu du dossier (tout est à la racine, rien à classer)
| Fichier | Rôle |
|---|---|
| `index.html` | **L'application** (cours, cartes, quiz…). C'est le seul fichier à remplacer pour une mise à jour. |
| `manifest.webmanifest` | Nom « Psychologie », couleurs, logo. |
| `sw.js` | Mode hors ligne et mise à jour automatique. |
| `icon-192.png`, `icon-512.png`, `icon-maskable-512.png`, `apple-touch-icon.png`, `favicon.png` | Logo Ψ. |

## 1. Mettre en ligne sur GitHub Pages (une seule fois)
1. Sur github.com (navigateur du téléphone, en « version ordinateur » si besoin), crée un dépôt **public** nommé `psychologie`.
2. **Add file → Upload files**, sélectionne **tous les fichiers** du dossier, puis **Commit changes**.
3. **Settings → Pages** : *Source* = « Deploy from a branch », branche `main`, dossier `/ (root)`, puis **Save**.
4. Après 1 à 2 minutes, ton application est à : `https://TON-PSEUDO.github.io/psychologie/`

## 2. Installer sur le téléphone
- **Android (Chrome)** : ouvre l'adresse → menu ⋮ → **Installer l'application** (ou « Ajouter à l'écran d'accueil »).
- **iPhone (Safari)** : ouvre l'adresse → bouton Partager → **Sur l'écran d'accueil**.

L'icône « Psychologie » apparaît alors comme une vraie application, en plein écran. Après la première ouverture avec internet, elle marche sans connexion.

## 3. Mettre à jour quand tu veux
1. Dans ton dépôt GitHub, ouvre `index.html` → ✏️ ou **Add file → Upload files**, envoie la nouvelle version **avec le même nom `index.html`**, puis **Commit changes**.
2. Patiente 1 à 2 minutes. À la prochaine ouverture de l'application avec internet, la nouvelle version est chargée toute seule ; si l'ancienne s'affiche encore, ferme complètement l'application et rouvre-la.

Tu n'as rien d'autre à modifier. (Ne touche à `VERSION` dans `sw.js` que si tu changes le logo.)

## À savoir
- **Notes, surlignages, favoris, progression et mode sombre** sont enregistrés **dans ton téléphone**, pour cette adresse. Ils restent d'une mise à jour à l'autre. Ils ne sont pas partagés avec un autre appareil, et ceux faits dans l'ancien fichier HTML ne sont pas repris.
- Si tu désinstalles l'application ou effaces les données du navigateur, ces données sont perdues.
- Un dépôt **public** rend le contenu de l'application visible de tous.
