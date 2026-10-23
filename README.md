# youneselfakir0.github.io

Site public du profil professionnel de **Younes El Fakir** — technicien senior en
support informatique. Publié sur GitHub Pages.

- **En ligne :** https://youneselfakir0.github.io
- **Version sobre :** https://youneselfakir0.github.io/v1/

---

## Les deux versions

Le site propose deux présentations du **même contenu**, au mot près. Choisis selon
l'usage : la première impression, ou la lecture posée.

| Chemin | Version | Pour quoi |
|---|---|---|
| `/` (`index.html`) | **Cinématographique 3D** | Première impression, démonstration technique. Champ de nœuds en projection 3D animé, sections qui entrent en profondeur au défilement. |
| `/v1/` (`v1/index.html`) | **Sobre** | Lecture et impression. Fond clair, une colonne, mise en page mobile d'abord, feuille de style d'impression. |

Un lien discret dans le pied de chaque page permet de passer de l'une à l'autre.

## Choix techniques

- **Aucune dépendance externe.** Pas de CDN, pas de framework, pas de police
  distante. Chaque page est un fichier HTML autonome (CSS et JavaScript inclus).
  Un recruteur qui ouvre le lien sur son téléphone ne paie aucun aller-retour réseau.
- **Aucune étape de build.** Ce qui est dans le dépôt est ce qui est servi.
- **La 3D est écrite à la main** en Canvas : ~99 points avec coordonnées x/y/z,
  rotation continue, projection perspective, taille et opacité selon la profondeur,
  liens tracés entre nœuds proches. Trois nœuds « hub » plus lumineux évoquent les
  trois machines du homelab.
- **`prefers-reduced-motion` est respecté.** Si le visiteur a désactivé les
  animations, la 3D se coupe et tout le contenu reste visible et lisible.
- **Impression.** La version sobre imprime proprement ; la version 3D abandonne le
  fond animé et redevient un document lisible sur papier.

## Vérifications avant publication

Contrôles passés sur les deux pages :

- Aucune donnée privée : ni adresse civique, ni numéro de téléphone, ni l'adresse
  courriel secondaire du CV papier. Vérifié par recherche textuelle sur le fichier
  livré, pas sur les notes.
- Le titre professionnel est repris **mot pour mot**.
- Les liens externes (GitHub, LinkedIn, dépôt du homelab) répondent HTTP 200.
- Aucun débordement horizontal à 390 px ni à 1400 px.
- Détecteur de design exécuté une fois, en fin de parcours.

## Contenu

Le contenu vient d'une **source unique** : le CV de Younes El Fakir. Aucun fait
n'est inventé, aucune expérience n'est gonflée. Les éléments volontairement omis
sont listés dans `PRODUCT.md` (`Uber Eats`, et toute formation en intelligence
artificielle).

## Fichiers

| Fichier | Rôle |
|---|---|
| `index.html` | Version cinématographique (racine du site) |
| `v1/index.html` | Version sobre |
| `PRODUCT.md` | Contexte produit : audience, périmètre, contraintes, faits autorisés |
| `CHANGELOG.md` | Historique des versions |

## Modifier le site

Il n'y a rien à compiler.

```bash
git clone https://github.com/youneselfakir0/youneselfakir0.github.io.git
cd youneselfakir0.github.io
# éditer index.html ou v1/index.html
git commit -am "…" && git push
```

GitHub Pages republie automatiquement depuis la branche `main`, à la racine.

## Preuve

Le homelab TwisterLab sert de preuve de travail :
[github.com/youneselfakir0/homelab-twisterlab](https://github.com/youneselfakir0/homelab-twisterlab)
