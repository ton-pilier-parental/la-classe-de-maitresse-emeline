# La classe de maîtresse Emeline — mode d'emploi

## Mettre le site en ligne sur Vercel (une seule fois)

1. Aller sur https://vercel.com et se connecter avec son compte GitHub.
2. **Add New… → Project**, puis choisir le dépôt `Ton-pilier-parental` → **Import**.
3. **Project Name** : `classe-maitresse-emeline` (ce nom donne l'adresse du site :
   `https://classe-maitresse-emeline.vercel.app`).
4. **Root Directory** : cliquer sur **Edit** et choisir le dossier `classe-emeline`.
5. **Framework Preset** : `Other`. Ne rien mettre dans les commandes de build.
6. Cliquer sur **Deploy**.

L'adresse finale s'affiche à la fin (onglet **Domains** du projet). C'est **elle**
qu'on met dans le QR code : elle ne changera plus jamais.

> ⚠️ Ne donnez pas aux parents les adresses longues du type
> `classe-maitresse-emeline-abc123-xxx.vercel.app` : ce sont des copies
> temporaires de chaque mise à jour. Seule l'adresse courte reste fixe.

## Ajouter ou modifier un chant

Tous les chants sont dans **un seul fichier** : `classe-emeline/chants.js`.

1. Sur GitHub, ouvrir `classe-emeline/chants.js` sur la branche `main`, puis cliquer sur le crayon ✏️.
2. Copier un bloc `{ ... },` existant, le coller **en haut de la liste** (juste
   après `window.CHANTS = [`) et changer le titre, l'onglet (`theme`), le lien
   YouTube et les paroles.
3. Cliquer sur **Commit changes**.

Vercel met le site à jour tout seul en moins d'une minute :

- **même adresse**, rien à redonner aux parents ;
- **tous les chants déjà publiés restent** : on ajoute au fichier, on n'efface rien.

## Si une mise à jour s'est mal passée

Dans Vercel → **Deployments**, choisir une version précédente → **⋯ → Promote to
Production**. L'ancienne version revient immédiatement, à la même adresse.
