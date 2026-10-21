# L’Outil complet de l’évangéliste : page de vente

Version française de la page de vente de **L’Outil complet de l’évangéliste**, conçue d’abord pour le téléphone.
C’est du HTML et du CSS simples, sans JavaScript ni bibliothèque externe.
La version anglaise se trouve dans le dépôt [The-evangelist-complete-toolkit-](https://github.com/salem-ask/The-evangelist-complete-toolkit-).

## Fichiers

| Chemin | Contenu |
| --- | --- |
| `index.html` | Toute la page (textes, styles et icônes) |
| `images/` | Les affiches en AVIF, WebP et JPEG à plusieurs tailles, et `share-image.jpg` pour les aperçus de lien |
| `fonts/montserrat-800.woff2` | Police des titres (Montserrat ExtraBold, caractères latins et français), avec sa licence `OFL.txt` |
| `.htaccess` | Réglages pour Hostinger : types de fichiers, compression et cache |

## Liens utilisés

- **Paiement :** `https://livresenligne.mychariow.shop/prd_89tf5ibz/checkout` (produit « Outils complets de l’évangéliste » de la boutique Library Online). Il fonctionnera une fois le produit publié sur Chariow.
- **WhatsApp :** `https://wa.me/243823226790?...` avec un message prérempli en français, dans la FAQ et le pied de page.
- **Site :** `https://bookline.digital`, dans le pied de page.

## À modifier dans `index.html`

- **Prix (facultatif) :** cherchez `PRIX (facultatif)`. Écrivez votre prix et supprimez le mot `hidden`. Sinon, la page indique que le prix s’affiche sur la page de paiement.
- **Adresse de la page :** une fois la page en ligne, remplacez `images/share-image.jpg` dans la ligne `og:image` par l’adresse complète, et ajoutez `og:url` et un lien `canonical`, pour que les aperçus WhatsApp et Facebook fonctionnent.
- **Affiches :** les affiches sont celles de la version anglaise (textes en anglais). Pour utiliser des affiches en français, remplacez les fichiers de `images/` en gardant les mêmes noms et un format carré.

## Mettre la page en ligne

Envoyez `index.html`, `.htaccess` et les dossiers `images` et `fonts` sur l’hébergement, en gardant la même structure. Sur Hostinger, créez de préférence un site séparé pour le sous-domaine (comme pour la version anglaise), afin qu’il ne dépende pas de l’application Node.js de `bookline.digital`.

## Crédits

- Police des titres : [Montserrat](https://github.com/JulietaUla/Montserrat), SIL Open Font License 1.1 (`fonts/OFL.txt`)
- Icônes : [Lucide](https://lucide.dev) (licence ISC)
- Écriture : Matthieu 9:37 et 2 Timothée 4:5, Bible Louis Segond 1910 (domaine public)
