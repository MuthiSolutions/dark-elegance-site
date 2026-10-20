# Bal Halloween Masqué — Dark Elegance

Page de réservation statique pour la soirée du 31 octobre (Noom Hotel).
Scanner un QR → cette page → choisir un salon → ouvre WhatsApp avec le message pré-rempli.

## Contenu
- `public/index.html` — la page (tout est inline : styles, scripts, animations).
- `package.json` / `railway.json` — config pour servir le fichier statique.

## Déploiement Railway
1. Pousser ce dossier sur un dépôt GitHub (voir ci-dessous).
2. Railway → **New Project → Deploy from GitHub repo** → choisir le dépôt.
3. Railway lit `railway.json` et sert `public/` automatiquement.
4. Dans **Settings → Networking → Generate Domain** pour obtenir l'URL publique.
5. Cette URL est celle que le QR code doit viser.

## Modifier
Tout est dans `public/index.html`. Le numéro WhatsApp est la variable `PHONE`
en haut du `<script>` ; les salons sont dans le tableau `SALONS`.
