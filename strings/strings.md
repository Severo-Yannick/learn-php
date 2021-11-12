Strings

Les strings sont des variables qui contiennent du texte. 

Par exemple, une chaine qui contient un nom est définie comme suit :

```php
$name = "Jean";
echo $name;
```
Nous pouvons facilement formatter des chaînes en utilisant des variables. Par exemple :

```php
$name = "Jean";
$introduction = "Salut $name";
echo $introduction;
```
Nous pouvons aussi concaténer des chaînes en utilisant l'opérateur point .. Par exemple :

```php
$first_name = "Jean";
$last_name = "Bon";
$name = $first_name . " " . $last_name;
echo $name;
```
Pour mesurer la longueur d'une chaîne, on utilise la fonction strlen :

```php
$string = "La longueur de cette phrase est 43 lettres.";
echo strlen($string);
```
Pour découper un morceau d'une chaîne et le renvoyer comme nouvelle chaîne, nous pouvons utiliser la fonction substr :

```php
$filename = "image.png";
$extension = substr($filename, strlen($filename) - 3);
echo "L'extension du fichier est $extension";
```
Coller et séparer
On peut coller des tableaux pour former des chaînes, ou séparer des chaînes en tableaux de chaînes.

Par exemple, pour séparer une chaîne avec une liste de fruits séparés par une virgule, on utilise la fonction explode :
```php
$fruits = "pomme,banane,orange";
$fruit_list = explode(",", $fruits);
echo "Le second fruit dans la liste est $fruit_list[1]";
```
Pour recoller un tableau en une seule chaîne séparée par des virgules, on utilise la fonction implode :

```php
$fruit_list = ["pomme","banane","orange"];
$fruits = implode(",", $fruit_list);
echo "Les fruits sont $fruits";
```
Exercice

Séparez la chaîne qui contient la liste des nombres en un nouveau tableau appelé number_list.