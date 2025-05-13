
# Java Katas – Boîte à outils rapide (README)

## I. Chaînes de caractères (`String`)

| Action                        | Code                                      |
|------------------------------|-------------------------------------------|
| Longueur                     | `mot.length()`                            |
| Caractère à l'index `i`        | `mot.charAt(i)`                           |
| Sous-chaîne de `a` à `b`        | `mot.substring(a, b)`                     |
| Minuscules                   | `mot.toLowerCase()`                       |
| Majuscules                   | `mot.toUpperCase()`                       |
| Position de "o"              | `mot.indexOf("o")`                        |
| Contient "jour" ?           | `mot.contains("jour")`                    |
| Égalité exacte             | `mot.equals("Bonjour")`                  |
| Remplacer "o" par "a"        | `mot.replace("o", "a")`                  |
| Séparer par espace          | `mot.split(" ")`                          |
| Enlever espaces autour       | `mot.trim()`                              |
| Inverser la chaîne          | `new StringBuilder(mot).reverse().toString();` |

## II. Tableaux (`int[]`, `String[]`)

| Action                        | Code                                           |
|------------------------------|------------------------------------------------|
| Taille                       | `arr.length`                                   |
| Trier                        | `Arrays.sort(arr)`                             |
| Afficher                     | `Arrays.toString(arr)`                         |
| Copier                       | `Arrays.copyOf(arr, taille)`                   |
| Inverser (manuel)            | Boucle avec swap `i <-> j`                    |

## III. Listes (`ArrayList`)

| Action                        | Code                                     |
|------------------------------|------------------------------------------|
| Créer une liste              | `List<T> list = new ArrayList<>();`      |
| Ajouter un élément          | `list.add(val)`                         |
| Accéder à un élément       | `list.get(i)`                           |
| Modifier un élément        | `list.set(i, val)`                       |
| Taille                       | `list.size()`                            |
| Supprimer un élément       | `list.remove(i)`                         |
| Vider la liste               | `list.clear()`                            |
| Contient "a" ?              | `list.contains("a")`                      |
| Liste vide ?                | `list.isEmpty()`                          |
| Trier                       | `Collections.sort(list)`                 |
| Inverser                    | `Collections.reverse(list)`              |
| Max / Min                   | `Collections.max(list)` / `min(list)`    |

## IV. Dictionnaires (`HashMap`)

| Action                        | Code                                           |
|------------------------------|------------------------------------------------|
| Créer une map                | `Map<K, V> map = new HashMap<>();`            |
| Ajouter une paire            | `map.put(clef, valeur)`                       |
| Récupérer une valeur         | `map.get(clef)`                              |
| Clé présente ?              | `map.containsKey("clé")`                    |
| Ensemble des clés           | `map.keySet()`                                |
| Valeurs                     | `map.values()`                               |
| Supprimer une clé           | `map.remove("clé")`                          |
| Parcourir toutes les entrées | `for (Map.Entry<K, V> e : map.entrySet())`   |

## V. Conversions rapides

| Conversion                   | Code                                                              |
|-----------------------------|-------------------------------------------------------------------|
| `String` → `int`            | `Integer.parseInt("42")`                                         |
| `int` → `String`            | `String.valueOf(42)`                                              |
| `String` → `char[]`         | `"mot".toCharArray()`                                            |
| `char[]` → `String`         | `new String(tab)`                                                |
| `List<String>` → `String[]`| `list.toArray(new String[0])`                                    |
| `int[]` → `List<Integer>`   | `Arrays.stream(tab).boxed().collect(Collectors.toList())`        |

## VI. Boucles utiles

| Type de boucle         | Code exemple                                      |
|------------------------|---------------------------------------------------|
| For classique          | `for (int i = 0; i < n; i++)`                    |
| For-each               | `for (String mot : liste)`                       |
| While                  | `while (i < n)`                                  |

## VII. Astuces katas utiles

| Tâche                             | Code                                                                           |
|----------------------------------|--------------------------------------------------------------------------------|
| Minimum d’un tableau             | `Arrays.stream(tab).min().getAsInt();`                                        |
| Compter une lettre               | `mot.chars().filter(c -> c == 'a').count();`                                  |
| Trier une liste                  | `Collections.sort(liste);`                                                    |
| Fréquence des caractères         | `map.put(c, map.getOrDefault(c, 0) + 1);` dans une boucle sur `mot.toCharArray()` |

