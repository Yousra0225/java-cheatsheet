# 📘 Guide Java Collections — Listes, Tableaux, Sets, Maps

## 🌳 Arborescence des Collections Java

        Collection (interface)
           /       |       \
      List       Set      Queue
       |          |         |

ArrayList HashSet PriorityQueue
LinkedList TreeSet ArrayDeque
Vector LinkedHashSet

### Résumé :

- `Collection` est une interface générale → regroupe les structures qui peuvent contenir plusieurs éléments.
- `List`, `Set`, et `Queue` sont des **types spécifiques** de collections :
  - **List** : avec **ordre**, éléments en **double autorisés**.
  - **Set** : **pas d’ordre**, **pas de doublon**.
  - **Queue** : utile pour la gestion **FIFO** (files).

---

## 📋 Tableaux vs Listes vs Sets vs Maps

| Structure    | Ordre ? | Doublons ?   | Accès direct (par index) | Quand l'utiliser ?             |
| ------------ | ------- | ------------ | ------------------------ | ------------------------------ |
| `Array[]`    | Oui     | Oui          | Oui                      | Taille fixe, simple et rapide  |
| `ArrayList`  | Oui     | Oui          | Oui                      | Liste dynamique                |
| `LinkedList` | Oui     | Oui          | Non (accès lent)         | Beaucoup d'ajouts/suppressions |
| `HashSet`    | Non     | Non          | Non                      | Éléments uniques, sans ordre   |
| `TreeSet`    | Oui     | Non          | Non                      | Éléments uniques, **triés**    |
| `HashMap`    | Non     | Clés uniques | Accès par clé            | Dictionnaire clé/valeur        |

---

## 🛠️ Déclaration des structures

| Type         | Déclaration                                   | Remarques                               |
| ------------ | --------------------------------------------- | --------------------------------------- |
| `Array`      | `int[] tab = new int[10];`                    | Taille fixe                             |
| `ArrayList`  | `List<String> list = new ArrayList<>();`      | Liste classique, dynamique              |
| `LinkedList` | `List<String> list = new LinkedList<>();`     | Rapide pour ajouter/enlever (FIFO/LIFO) |
| `HashSet`    | `Set<Integer> set = new HashSet<>();`         | Pas de doublon, ordre non garanti       |
| `TreeSet`    | `Set<Integer> set = new TreeSet<>();`         | Pas de doublon, trié automatiquement    |
| `HashMap`    | `Map<String, Integer> map = new HashMap<>();` | Association clé-valeur                  |

---

## 🧰 Méthodes utiles (List, Set, Map)

### ✅ Communes aux **List/Set**

| Méthode         | Description                      |
| --------------- | -------------------------------- |
| `add(elm)`      | Ajouter un élément               |
| `remove(elm)`   | Supprimer un élément             |
| `contains(elm)` | Vérifie si l’élément est présent |
| `size()`        | Taille de la collection          |
| `clear()`       | Vide la collection               |
| `isEmpty()`     | Vérifie si elle est vide         |

### 🔢 Spécifiques à **List**

| Méthode                | Description                       |
| ---------------------- | --------------------------------- |
| `get(index)`           | Accès à un élément par index      |
| `set(index, val)`      | Modifier un élément               |
| `indexOf(val)`         | Obtenir l'index d'un élément      |
| `sort()` (Collections) | Trie la liste                     |
| `add(index, val)`      | Insérer à une position spécifique |

### 🧩 Pour **Map**

| Méthode                | Description                   |
| ---------------------- | ----------------------------- |
| `put(key, value)`      | Ajouter une paire clé/valeur  |
| `get(key)`             | Accéder à la valeur d’une clé |
| `remove(key)`          | Supprimer une paire           |
| `containsKey(key)`     | Vérifie si une clé existe     |
| `containsValue(value)` | Vérifie si une valeur existe  |
| `keySet()`             | Retourne toutes les clés      |
| `values()`             | Retourne toutes les valeurs   |

---
