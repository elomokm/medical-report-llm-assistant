# Micro-produit IA — Assistant de rédaction de comptes-rendus médico-sociaux

## 1. Problème terrain

Dans les structures médico-sociales (EHPAD, accompagnement handicap, protection de l’enfance), les professionnels doivent rédiger quotidiennement des observations et transmissions.

Ces écrits doivent être :

* factuels
* neutres
* structurés
* juridiquement exploitables

En pratique, ils sont souvent rédigés rapidement à partir de notes brutes par manque de temps.

Conséquences :

* hétérogénéité des écrits entre professionnels
* perte d’informations importantes
* charge mentale importante
* temps administratif au détriment de l’accompagnement humain

## 2. Hypothèse produit

Un assistant IA transforme des notes brutes en observation professionnelle structurée validable par l’humain.

L’IA n’émet jamais de diagnostic.
Elle reformule uniquement dans un cadre professionnel standardisé.

Flux d’usage :

Notes rapides → Proposition de compte-rendu → Validation humaine → Enregistrement

L’outil agit comme un accélérateur rédactionnel et non comme un remplaçant décisionnel.

## 3. Pipeline IA

### Entrée

Texte libre court (style télégraphique, imparfait, bruité)

### Traitements

1. Normalisation linguistique

   * correction grammaticale légère
   * segmentation des événements

2. Structuration sémantique
   Classification des informations :

   * comportement
   * alimentation
   * relationnel
   * traitement
   * évolution

3. Génération contrôlée
   LLM contraint par :

   * schéma de sortie fixe
   * vocabulaire encadré
   * style neutre professionnel

4. Option RAG
   Injection d’un référentiel terminologique médico-social pour uniformiser les formulations

### Sortie

Compte-rendu structuré modifiable par le professionnel

## 4. Sécurité et éthique

Contraintes intégrées :

* interdiction de diagnostic
* suppression d’interprétation psychologique
* reformulation factuelle uniquement
* traçabilité : texte original conservé
* validation humaine obligatoire avant enregistrement

Le système propose, l’humain décide.

## 5. Évaluation

### Évaluation technique

* conformité au format
* absence d’hallucination
* stabilité de génération

### Évaluation métier

Comparaison humain vs IA sur :

* neutralité
* clarté
* complétude

Validation réalisée avec professionnels terrain.

Succès = gain de temps + acceptabilité professionnelle.

## 6. Itération produit

Phase 1 : reformulation simple supervisée
Phase 2 : structuration automatique complète
Phase 3 : adaptation par structure (vocabulaire local)
Phase 4 : suggestions contextuelles non intrusives

Objectif final : réduire le temps rédactionnel sans modifier la responsabilité humaine.
