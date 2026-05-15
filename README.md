# Les Carnets du son de l’éternel

Notes critiques, archives et études autour de Joy Division.

Ce dépôt est le dépôt public de publication du projet **Les Carnets du son de l’éternel**. Il ne remplace pas le dépôt principal **Joy Division AI Writing Studio**. Il en constitue l’espace éditorial dérivé : ici sont publiés des articles finis, issus d’un travail documentaire réalisé ailleurs.

Le principe directeur est simple :

```text
repo RAG principal + manuscrit en cours → forge documentaire et argumentative
repo Carnets → publication publique
```

Le dépôt principal conserve les sources, les atomes, les relations, les registres, les exports et les documents maîtres. Le manuscrit en cours conserve les formulations, progressions et concepts déjà stabilisés dans les 14 chapitres du livre. Le dépôt `joy-division-carnets` ne contient que les textes publiables, les brouillons éditoriaux, les pages du site et les éléments nécessaires à la diffusion.

---

## Doctrine éditoriale des Carnets

Les Carnets ne fonctionnent pas comme un blog d’actualité. Ils constituent un carnet public de notes et d’études préparatoires en amont de la publication du livre *Joy Division, le son de l’éternel*.

Chaque billet doit rester autonome, lisible, argumenté et relativement bref. Il ne doit jamais devenir un fragment brut du manuscrit.

### Sources mobilisables

Les billets peuvent mobiliser deux ensembles complémentaires :

```text
1. Le RAG principal : sources, atomes, relations, registres, citations et prudences documentaires.
2. Les 14 chapitres du manuscrit en cours : formulations stabilisées, concepts, structures argumentatives, motifs et continuités stylistiques.
```

Le RAG demeure la source principale de preuve documentaire. Le manuscrit en cours sert de source de cohérence argumentative et stylistique. Les billets peuvent donc condenser, reformuler ou prolonger des analyses déjà présentes dans les chapitres, mais ils ne doivent jamais copier mécaniquement une section entière du livre ni en publier des fragments longs.

### Longueur

La longueur cible est désormais :

```text
Environ 7 500 caractères espaces compris par langue.
```

Chaque billet existe idéalement en français et en anglais.

### Structure

Les billets doivent comporter :

- une ouverture courte ;
- entre 1 et 3 intertitres maximum ;
- une conclusion brève et forte.

Les intertitres servent à structurer une progression argumentative. Ils ne doivent jamais fragmenter artificiellement le texte.

### Production bilingue

Le prompt de rédaction doit générer systématiquement les deux versions dans une seule sortie, selon l’ordre suivant :

```text
1. Front matter français
2. Texte français
3. Front matter anglais
4. Texte anglais
```

La version française est la version principale indexée. La version anglaise est masquée de l’index principal et reliée par le champ `translation_url`.

Front matter français :

```yaml
layout: post
lang: fr
index: true
primary_lang: true
```

Front matter anglais :

```yaml
layout: post
lang: en
index: false
```

### Références et notes

Les références ne doivent jamais apparaître dans le corps du texte.

Règle impérative :

```text
Toutes les références apparaissent uniquement en notes de bas de page.
```

Exemple :

```markdown
[^1]: Peter Hook, *Unknown Pleasures: Inside Joy Division*, Londres, Simon & Schuster, 2012.
```

Sont interdits dans le corps du texte :

```text
(S41-A014)
(RAG 3)
(source fragile)
(citation à vérifier)
```

### Prudences historiographiques

Les billets ne doivent jamais exposer les mécanismes internes de validation documentaire du projet.

Le lecteur ne doit jamais voir :

- les identifiants RAG ;
- les niveaux de preuve ;
- les commentaires de vérification ;
- les remarques techniques sur les sources.

Les réserves historiographiques doivent être reformulées naturellement dans la prose critique.

Mauvais exemple :

```text
« Source à vérifier. »
« Témoignage non corroboré. »
```

Bon exemple :

```text
« Les récits divergent légèrement sur ce point. »
« La mémoire de scène tend ensuite à amplifier l’événement. »
```

### Style

Les billets doivent :

- être rédigés au présent ;
- utiliser les guillemets français dans les textes français ;
- mettre les albums en italique ;
- mettre les chansons entre guillemets ;
- alterner phrases courtes et longues ;
- éviter les tricolons mécaniques ;
- éviter les formulations journalistiques ou sensationnalistes ;
- conserver une prose académique, nerveuse et lisible.

### Règles historiographiques

Les billets doivent :

- distinguer fait établi, témoignage rétrospectif, reconstruction mémorielle, interprétation critique et mythe ;
- éviter toute téléologie morbide ;
- éviter toute psychologisation simpliste de Ian Curtis ;
- éviter toute causalité simplifiée ;
- éviter de transformer un souvenir de musicien en fait brut.

---

## Fonction du dépôt

Ce dépôt accueille des articles courts ou moyens sur Joy Division, Manchester, Factory Records, le post-punk, les bootlegs, les objets discographiques, les mythes historiographiques et les controverses documentaires.

Il sert de vitrine publique au travail critique conduit dans le dépôt RAG principal et dans le manuscrit en cours. Il rend lisible une partie du travail sans exposer l’ensemble de l’infrastructure documentaire.

Il permet aussi de tester publiquement certains angles du futur livre : hypothèses, scènes fondatrices, objets, concepts, prudences, contre-mythes.

Enfin, il conserve une archive éditoriale propre, stable, versionnée, compatible avec GitHub Pages ou tout autre générateur statique.
