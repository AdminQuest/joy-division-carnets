# PROMPT AUTONOME — Les Carnets du son de l’éternel

## Fonction

Ce prompt sert à produire un billet bilingue publiable dans le dépôt `joy-division-carnets`.

Le texte peut mobiliser :

```text
1. Le dossier documentaire RAG.
2. Les 14 chapitres du manuscrit en cours de rédaction.
```

Le RAG demeure la source principale de preuve documentaire.

Le manuscrit sert de source de cohérence argumentative, stylistique et conceptuelle.

---

## Contraintes générales

### Longueur

```text
Environ 10 000 caractères espaces compris par langue.
```

### Structure

- ouverture courte ;
- entre 1 et 3 intertitres maximum ;
- conclusion brève et forte.

Les intertitres structurent l’argumentation. Ils ne doivent jamais fragmenter artificiellement le texte.

### Style

- écrire au présent ;
- prose académique, nerveuse et lisible ;
- alterner phrases courtes et longues ;
- respecter les consignes typographiques françaises dans les textes français ;
- respecter les consignes typographiques anglaises dans les textes anglais ;
- utiliser les guillemets français dans les textes français : « … » ;
- utiliser les guillemets anglais dans les textes anglais : “…” ;
- respecter les espaces typographiques françaises avant les signes doubles ;
- ne jamais appliquer ces espaces aux textes anglais ;
- mettre les titres de livres en italique ;
- mettre les titres d’albums en italique ;
- mettre les chansons entre guillemets ;
- éviter les formulations journalistiques ou sensationnalistes ;
- éviter les tricolons mécaniques.

### Règles historiographiques

Le texte doit :

- distinguer fait établi, témoignage rétrospectif, reconstruction mémorielle, interprétation critique et mythe ;
- éviter toute téléologie morbide ;
- éviter toute psychologisation simpliste de Ian Curtis ;
- éviter toute causalité simplifiée ;
- éviter de transformer un souvenir de musicien en fait brut.

### Références

- ne jamais faire apparaître les références dans le corps du texte ;
- ne jamais faire apparaître les identifiants RAG ;
- ne jamais écrire « source à vérifier », « citation fragile », « preuve faible » ou équivalent ;
- reformuler les prudences historiographiques naturellement dans la prose ;
- placer les références uniquement en notes de bas de page Markdown.

Exemple :

```markdown
[^1]: Peter Hook, *Unknown Pleasures: Inside Joy Division*, Londres, Simon & Schuster, 2012.
```

---

## Sortie obligatoire

Le prompt doit toujours produire la sortie dans l’ordre suivant :

```text
1. Front matter français
2. Texte français
3. Front matter anglais
4. Texte anglais
```

### Front matter français obligatoire

```yaml
layout: post
lang: fr
index: true
primary_lang: true
```

### Front matter anglais obligatoire

```yaml
layout: post
lang: en
index: false
```

La version anglaise doit pointer vers la version française via `translation_url`.

---

## Consigne de rédaction

À partir du dossier documentaire RAG et des chapitres déjà rédigés du manuscrit, rédige un billet bilingue publiable dans `joy-division-carnets`.

Le texte doit rester autonome. Il peut prolonger ou condenser des motifs, structures ou analyses déjà stabilisés dans le livre, mais il ne doit jamais reproduire mécaniquement une section entière du manuscrit.
