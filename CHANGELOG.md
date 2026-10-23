# Changelog

Toutes les modifications notables de ce projet sont documentées dans ce fichier.
Le format s'inspire de *Keep a Changelog* ; le versionnage suit SemVer.

## [1.2.0] — 2026-10-23

### Ajouté

- Publication de **deux présentations** du même contenu : version cinématographique 3D à la racine, version sobre dans `v1/`.
- `README.md` : documentation du dépôt, des deux versions et des choix techniques.
- Liens croisés discrets entre les deux versions.

### Vérifié

- Contenu textuel identique entre les deux versions.
- Aucune donnée privée, aucun débordement horizontal, liens externes en HTTP 200.

## [1.1.0] — 2026-10-23

### Modifié

- Refonte de la présentation : le parcours est désormais présenté comme un **relevé de service**, avec une chronologie à barres sur un axe 2011–2026 (bande sombre), au lieu d'une liste de blocs datés.
- Sections numérotées (01–07) et libellés en monospace.
- Bandeau technique en tête de page.

### Inchangé

- **Contenu textuel intégralement préservé** : chaque phrase, intitulé, date et description de la version 1.0 est reprise mot pour mot (vérifié par comparaison automatique des nœuds de texte).
- Aucun fait ajouté, aucune donnée privée.

## [1.0.0] — 2026-10-23

### Ajouté

- Page publique unique (`index.html`) présentant le profil professionnel de Younes El Fakir.
- En-tête : nom, titre exact, localisation publique (Saint-Hubert, Québec) et contacts publics (courriel, GitHub, LinkedIn).
- Sections : Profil, Compétences, Expérience, Formation, Preuves, Disponibilité.
- Section **Preuves** : TwisterLab — homelab de 3 machines, orchestration d'agents vérifiée par empreinte SHA-256, avec lien vers le dépôt public.
- Feuille de style intégrée, sans dépendance externe ni étape de build ; mise en page mobile d'abord.
- Feuille de style d'impression pour la version papier.
- `PRODUCT.md` : contexte produit durable (audience, périmètre, contraintes, faits autorisés).

### Sécurité et vie privée

- Aucune adresse civique et aucun numéro de téléphone dans la page ni dans le code source (vérifié par recherche textuelle).
- Aucun secret, aucun jeton dans le dépôt ni dans l'historique Git.

### Notes

- Contenu strictement limité aux faits autorisés. Uber Eats et toute formation en intelligence artificielle sont volontairement omis.
