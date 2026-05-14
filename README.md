# Les Carnets du son de l’éternel

Notes critiques, archives et études autour de Joy Division.

Ce dépôt est le dépôt public de publication du projet **Les Carnets du son de l’éternel**. Il ne remplace pas le dépôt principal **Joy Division AI Writing Studio**. Il en constitue l’espace éditorial dérivé : ici sont publiés des articles finis, issus d’un travail documentaire réalisé ailleurs.

Le principe est simple :

```text
repo RAG principal → forge documentaire
repo Carnets → publication publique
```

Le dépôt principal conserve les sources, les atomes, les relations, les registres, les exports et les documents maîtres. Le dépôt `joy-division-carnets` ne contient que les textes publiables, les brouillons éditoriaux, les pages du site et les éléments nécessaires à la diffusion.

---

## 1. Fonction du dépôt

Ce dépôt a quatre fonctions.

Premièrement, il accueille des articles courts ou moyens sur Joy Division, Manchester, Factory Records, le post-punk, les bootlegs, les objets discographiques, les mythes historiographiques et les controverses documentaires.

Deuxièmement, il sert de vitrine publique au travail critique conduit dans le dépôt RAG principal. Il rend lisible une partie du travail sans exposer l’ensemble de l’infrastructure documentaire.

Troisièmement, il permet de tester publiquement certains angles du futur livre : hypothèses, scènes fondatrices, objets, concepts, prudences, contre-mythes.

Quatrièmement, il conserve une archive éditoriale propre, stable, versionnée, compatible avec une publication GitHub Pages ou tout autre générateur statique.

---

## 2. Ce que ce dépôt n’est pas

Ce dépôt n’est pas le dépôt de sources.

Il ne doit pas accueillir :

- les scans ou OCR d’ouvrages ;
- les sources primaires complètes ;
- les atomes historiographiques complets ;
- les registres internes du RAG ;
- les documents maîtres générés par chapitre ;
- les exports bruts du dépôt principal ;
- les notes privées de lecture non stabilisées ;
- les citations non vérifiées.

Il ne doit pas devenir un second RAG, ni un double affaibli du dépôt principal. Toute preuve, toute relation documentaire, toute contradiction de sources et toute citation sensible restent gérées dans le dépôt principal.

---

## 3. Articulation avec le dépôt RAG principal

Le dépôt principal est la forge.

Il contient la chaîne documentaire :

```text
sources
→ atomes
→ registres
→ exports générés
→ audit / diagnostics
→ documents maîtres
→ RAG Studio
→ prompts autonomes
→ rédaction IA
→ manuscrit ou articles
```

Le dépôt Carnets intervient uniquement à la fin de cette chaîne :

```text
RAG Studio
→ dossier documentaire RAG 3
→ prompt autonome RAG 4
→ brouillon d’article
→ vérification humaine
→ fichier Markdown dans ce dépôt
→ publication
```

Le dépôt principal sert donc à produire une matière contrôlée. Le dépôt Carnets reçoit seulement la forme éditoriale validée.

---

## 4. Règle de séparation des fonctions

La règle de séparation est impérative.

```text
repo principal = preuve, relations, méthode, contrôle
repo Carnets = articles, pages publiques, brouillons éditoriaux
```

Un article peut naître du RAG, mais il ne remplace jamais les sources qui l’ont produit.

Un article peut révéler une lacune ou une relation nouvelle. Dans ce cas, l’information ne reste pas seulement dans le dépôt Carnets : elle doit être réinjectée dans le dépôt principal sous la forme appropriée.

Exemples :

- une citation à stabiliser → registre des citations vérifiées ;
- une contradiction entre deux témoignages → atome ou relation ;
- un mythe à déconstruire → registre des mythes ;
- une source nouvelle → registre canonique des sources ;
- un concept récurrent → registre des concepts ;
- une prudence interprétative → atome enrichi ou note de vigilance.

---

## 5. Chaîne de production d’un article

Chaque article doit suivre une chaîne courte et contrôlable.

### Étape 1 — Choisir un angle

Un article doit répondre à une question limitée.

Exemples :

- Le concert des Sex Pistols du 4 juin 1976 est-il un fait historique ou un mythe fondateur ?
- Comment la contrainte technique invente-t-elle le jeu de basse de Peter Hook ?
- Pourquoi les sessions RCA fonctionnent-elles comme un anti-récit ?
- Comment *Unknown Pleasures* transforme-t-il une image scientifique en icône pop ?
- Que montrent vraiment les bootlegs de Joy Division ?

Un article n’est pas un chapitre miniature. Il traite un nœud, une scène, un objet, une hypothèse ou une tension documentaire.

### Étape 2 — Interroger le RAG Studio

Dans le dépôt principal, utiliser le RAG Studio pour rechercher les atomes pertinents.

Recherches possibles :

```text
Sex Pistols Lesser Free Trade Hall mythe fondateur
Peter Hook basse ampli aigus contrainte
RCA sessions anti-récit formatage
Unknown Pleasures pulsar Saville image scientifique
bootlegs Joy Division archive sauvage
```

### Étape 3 — Produire un dossier RAG 3

Le dossier RAG 3 doit regrouper les résultats par rôle documentaire :

- faits établis ;
- scènes fondatrices ;
- témoignages directs ;
- reconstructions mémorielles ;
- lectures critiques ;
- mythes à déconstruire ;
- controverses ;
- citations disponibles ;
- concepts et motifs ;
- points de vigilance ;
- lacunes documentaires.

Ce dossier sert de base documentaire au brouillon.

### Étape 4 — Générer un prompt RAG 4

Le prompt RAG 4 doit être autonome. Il doit pouvoir être transmis à une IA de rédaction sans lui donner accès au dépôt principal.

Instruction type :

```text
À partir du dossier documentaire ci-dessous, rédige un article court pour le site « Les Carnets du son de l’éternel ».

Longueur : 1 500 à 2 500 mots.
Objet : expliquer un problème historiographique précis.
Style : essai critique accessible, sourcé, sans jargon inutile.
Contraintes :
- distinguer fait établi, témoignage, reconstruction mémorielle, interprétation critique et mythe ;
- ne pas transformer l’article en chapitre du livre ;
- ne pas introduire de fait nouveau hors dossier ;
- signaler les incertitudes ;
- vérifier les citations avant publication ;
- utiliser les guillemets français ;
- mettre les albums en italique et les chansons entre guillemets ;
- terminer par une conclusion courte.
```

### Étape 5 — Rédiger le brouillon

Le brouillon est placé dans `drafts/` tant qu’il n’est pas relu.

Il doit comporter un en-tête YAML provisoire, avec `draft: true`.

### Étape 6 — Vérifier

Avant publication, vérifier :

- la solidité factuelle ;
- les citations exactes ;
- les dates ;
- les noms ;
- les titres d’albums et de chansons ;
- la distinction entre mémoire, mythe et fait établi ;
- l’absence de reprise trop directe du manuscrit du livre ;
- l’absence d’élément privé ou non publiable issu du dépôt principal.

### Étape 7 — Publier dans `content/posts/`

Une fois validé, l’article est déplacé dans `content/posts/`.

Nom de fichier recommandé :

```text
AAAA-MM-JJ-slug-court.md
```

Exemple :

```text
2026-05-14-lesser-free-trade-hall-mythe-fondateur.md
```

### Étape 8 — Réinjecter les découvertes dans le dépôt principal

Si la rédaction de l’article révèle une relation, une contradiction, une lacune ou un concept à stabiliser, l’information doit retourner dans le dépôt RAG principal.

---

## 6. Formats éditoriaux

Le site peut accueillir trois formats.

### 6.1. Note critique

Longueur indicative : 1 000 à 1 500 mots.

Fonction : traiter une idée, une scène, une prudence ou un mythe.

Exemples :

- « Le concert qui grossit avec le temps » ;
- « Warsaw devient Joy Division : changement de nom ou bascule symbolique ? » ;
- « “Transmission” : le signal avant le slogan ».

### 6.2. Étude courte

Longueur indicative : 2 000 à 3 500 mots.

Fonction : développer un objet plus dense, avec sources croisées.

Exemples :

- « Peter Hook : la contrainte technique comme invention esthétique » ;
- « Martin Hannett et l’espace sonore : laboratoire, mythe, réalité » ;
- « *Unknown Pleasures* : comment une image scientifique devient une icône ».

### 6.3. Fiche archive

Longueur indicative : 500 à 1 000 mots.

Fonction : présenter un objet, un concert, un bootleg, une édition, un lieu ou une trace documentaire.

Exemples :

- « *An Ideal for Living* : objet discographique, malaise visuel, seuil esthétique » ;
- « RCA sessions : l’échec comme anti-modèle » ;
- « Electric Circus : lieu réel, lieu fantôme ».

---

## 7. Structure du dépôt

```text
joy-division-carnets/
  README.md
  content/
    posts/
    pages/
  drafts/
  templates/
  data/
  public/
    images/
  scripts/
```

### `content/posts/`

Articles publiés ou prêts à publier.

### `content/pages/`

Pages fixes : à propos, méthode, bibliographie, avertissement éditorial.

### `drafts/`

Brouillons issus du RAG ou de la rédaction IA. Rien dans ce dossier n’est considéré comme publié.

### `templates/`

Modèles Markdown pour les nouveaux articles.

### `data/`

Données éditoriales légères : tags, séries, statuts, catégories. Ce dossier ne doit pas accueillir les registres complets du dépôt principal.

### `public/images/`

Images publiques, libres de droits ou autorisées. Ne pas y déposer d’images protégées sans vérification.

### `scripts/`

Scripts éventuels de contrôle éditorial ou de publication. Ce dossier reste facultatif.

---

## 8. Métadonnées obligatoires d’un article

Chaque article doit commencer par un en-tête YAML.

```yaml
title: "Titre de l’article"
date: 2026-05-14
description: "Résumé court de l’article."
tags: ["Joy Division", "Manchester", "post-punk"]
format: "note critique"
source_status: "issu du RAG principal, vérifié manuellement"
draft: false
```

Champs recommandés :

```yaml
series: "Interzone Notes"
related_chapters: ["chapitre 1", "chapitre 2"]
rag_origin: "RAG 3 + RAG 4"
verification_status: "citations vérifiées"
```

---

## 9. Règles éditoriales

Les règles suivantes s’appliquent à tous les articles.

- Écrire au présent.
- Utiliser les guillemets français.
- Mettre les albums en italique.
- Mettre les titres de chansons entre guillemets.
- Distinguer clairement fait établi, témoignage, reconstruction mémorielle, interprétation critique et mythe.
- Ne jamais publier une citation non vérifiée.
- Signaler les incertitudes au lieu de les masquer.
- Éviter les listes de références décoratives.
- Éviter les articles encyclopédiques.
- Préférer un angle net à une synthèse générale.
- Ne pas publier de documents internes au dépôt principal.

---

## 10. Règle de non-cannibalisation du livre

Le site ne doit pas publier le manuscrit par fragments.

Un article peut :

- tester une hypothèse ;
- clarifier une tension documentaire ;
- isoler une scène ;
- présenter un objet ;
- déconstruire un mythe ;
- préparer une lecture.

Un article ne doit pas :

- reprendre un passage entier du livre ;
- publier une section complète du manuscrit ;
- révéler l’architecture globale d’un chapitre ;
- affaiblir la valeur éditoriale du futur ouvrage.

Le blog est une chambre d’écho. Il n’est pas une prépublication intégrale.

---

## 11. Première série recommandée

Série de lancement possible :

1. « Le concert du 4 juin 1976 : naissance d’un mythe mancunien »
2. « Peter Hook : quand une mauvaise amplification invente une basse »
3. « *An Ideal for Living* : l’objet maladroit qui annonce autre chose »
4. « RCA sessions : l’échec qui sauve Joy Division du formatage »
5. « Manchester n’explique pas tout : contre le déterminisme urbain »
6. « Martin Hannett : producteur réel, fantôme critique »
7. « *Unknown Pleasures* : une pochette devenue langage universel »
8. « Les bootlegs : mémoire sauvage de Joy Division »

---

## 12. Workflow Git recommandé

Créer un article :

```bash
git pull
cp templates/post.md drafts/AAAA-MM-JJ-slug.md
```

Après rédaction et vérification :

```bash
mv drafts/AAAA-MM-JJ-slug.md content/posts/AAAA-MM-JJ-slug.md
git add .
git commit -m "Publie l’article : titre court"
git push
```

Pour une simple mise à jour :

```bash
git pull
git add .
git commit -m "Actualise la méthode éditoriale"
git push
```

---

## 13. Principe directeur

Le dépôt principal fabrique la connaissance.

Le dépôt Carnets fabrique la lecture.

L’un doit rester dense, relationnel, probatoire.

L’autre doit rester clair, public, lisible.
