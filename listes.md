# 📘 Guide Java Collections — Listes, Tableaux, Sets, Maps

## 🌳 Arborescence des Collections Java

        Collection (interface)
           /       |       \
      List       Set      Queue
       |          |         |
ArrayList      HashSet   PriorityQueue
LinkedList     TreeSet   ArrayDeque
Vector         LinkedHashSet


### Résumé :
- `Collection` est une interface générale → regroupe les structures qui peuvent contenir plusieurs éléments.
- `List`, `Set`, et `Queue` sont des **types spécifiques** de collections :
  - **List** : avec **ordre**, éléments en **double autorisés**.
  - **Set** : **pas d’ordre**, **pas de doublon**.
  - **Queue** : utile pour la gestion **FIFO** (files).

---

## 📋 Tableaux vs Listes vs Sets vs Maps

| Structure        | Ordre ? | Doublons ? | Accès direct (par index) | Quand l'utiliser ?                    |
|------------------|--------|------------|---------------------------|----------------------------------------|
| `Array[]`        | Oui    | Oui        | Oui                       | Taille fixe, simple et rapide          |
| `ArrayList`      | Oui    | Oui        | Oui                       | Liste dynamique                        |
| `LinkedList`     | Oui    | Oui        | Non (accès lent)          | Beaucoup d'ajouts/suppressions        |
| `HashSet`        | Non    | Non        | Non                       | Éléments uniques, sans ordre           |
| `TreeSet`        | Oui    | Non        | Non                       | Éléments uniques, **triés**            |
| `HashMap`        | Non    | Clés uniques| Accès par clé            | Dictionnaire clé/valeur                |

---

