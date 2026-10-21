# L’Outil complet de l’évangéliste : page de vente

Version française de la page de vente de **L’Outil complet de l’évangéliste**, conçue d’abord pour le téléphone.
C’est du HTML et du CSS simples, sans JavaScript ni bibliothèque externe.
La version anglaise se trouve dans le dépôt [The-evangelist-complete-toolkit-](https://github.com/salem-ask/The-evangelist-complete-toolkit-).

## Fichiers

| Chemin | Contenu |
| --- | --- |
| `index.html` | Toute la page (textes, styles et icônes) |
| `images/` | Les affiches en français, en AVIF, WebP et JPEG à plusieurs tailles, et `share-image.jpg` pour les aperçus de lien |
| `fonts/montserrat-800.woff2` | Police des titres (Montserrat ExtraBold, caractères latins et français), avec sa licence `OFL.txt` |
| `.htaccess` | Réglages pour Hostinger : types de fichiers, compression et cache |
| `deploy/outil-complet-de-l-evangeliste-site.zip` | Les fichiers du site ci-dessus en un seul zip, utilisé pour le déploiement sur Hostinger |

## Liens utilisés

- **Paiement :** `https://livresenligne.mychariow.shop/prd_89tf5ibz/checkout` (produit « Outils complets de l’évangéliste » de la boutique Library Online). Il fonctionnera une fois le produit publié sur Chariow.
- **WhatsApp :** `https://wa.me/243823226790?...` avec un message prérempli en français, dans la FAQ et le pied de page.
- **Site :** `https://bookline.digital`, dans le pied de page.

## À modifier dans `index.html`

- **Prix (facultatif) :** cherchez `PRIX (facultatif)`. Écrivez votre prix et supprimez le mot `hidden`. Sinon, la page indique que le prix s’affiche sur la page de paiement.
- **Adresse de la page :** si la page change d’adresse, mettez à jour `og:url`, `og:image` et le lien `canonical` en haut du fichier, pour que les aperçus WhatsApp et Facebook continuent de fonctionner.
- **Affiches :** pour changer une affiche, remplacez ses fichiers dans `images/` en gardant les mêmes noms, les mêmes tailles et un format carré.

## Où la page est en ligne

**https://outil-complet-de-l-evangeliste.bookline.digital**, sur Hostinger (compte `u977986808`) :

- C’est un site à part sur l’hébergement, séparé de l’application Node.js de `bookline.digital`.
- DNS : un enregistrement `A` `outil-complet-de-l-evangeliste` → `92.113.24.54` dans la zone `bookline.digital`.
- SSL actif, avec redirection automatique vers HTTPS.

## Mettre à jour la page en ligne

1. Modifiez les fichiers, reconstruisez `deploy/outil-complet-de-l-evangeliste-site.zip` avec `index.html`, `.htaccess`, `images/` et `fonts/` à la racine du zip, puis poussez sur `main`.
2. Sur Hostinger, récupérez ce dépôt dans un dossier temporaire `_deploy` du site (déploiement Git).
3. Déployez `_deploy/deploy/outil-complet-de-l-evangeliste-site.zip` comme archive de site statique. Les fichiers du site sont remplacés par ceux du zip, et `_deploy` est supprimé.

À la main, vous pouvez aussi envoyer le zip dans le `public_html` du site avec le Gestionnaire de fichiers, puis utiliser **Extraire** en remplaçant les anciens fichiers.

## Crédits

- Police des titres : [Montserrat](https://github.com/JulietaUla/Montserrat), SIL Open Font License 1.1 (`fonts/OFL.txt`)
- Icônes : [Lucide](https://lucide.dev) (licence ISC)
- Écriture : Matthieu 9:37 et 2 Timothée 4:5, Bible Louis Segond 1910 (domaine public)
