#  BookShelf - Gestion de Bibliothèque

##  Description

**BookShelf** est une application Java permettant de gérer une bibliothèque de livres.

L’application offre plusieurs fonctionnalités :

* Ajouter des livres
* Afficher les livres enregistrés
* Trier les livres par différents critères
* Garantir l’immuabilité des données retournées
* Vérifier le bon fonctionnement grâce aux tests unitaires

---

#  Technologies utilisées

* Java 21
* JUnit 5
* IntelliJ IDEA

---

# Structure du projet

```text
src/
├── bookstoread/
│   ├── Book.java
│   ├── BookShelf.java
│   └── BookShelfSpec.java
└── README.md
```

---

# Fonctionnalités principales

## Gestion des livres

L’utilisateur peut :

* Ajouter un ou plusieurs livres dans la bibliothèque
* Consulter la liste des livres enregistrés
* Obtenir une liste immuable pour éviter toute modification externe

---

## Systèmes de tri

L’application permet plusieurs types de tri.

### Tri par titre

Les livres sont triés automatiquement par ordre alphabétique.

### Tri personnalisé

Possibilité d’utiliser un `Comparator` pour appliquer un tri spécifique.

Exemple :

* Ordre décroissant
* Tri par auteur
* Tri par nombre de pages

### Tri par date de publication

Les livres sont triés du plus ancien au plus récent.

---

# Tests unitaires

Les tests sont réalisés avec **JUnit 5**.

## Cas testés

* Vérification qu’une bibliothèque est vide à l’initialisation
* Ajout de plusieurs livres
* Vérification de l’immuabilité de la liste retournée
* Tri alphabétique des livres
* Tri personnalisé avec `Comparator`
* Tri par date de publication

---

# Exécution des tests

## Avec IntelliJ IDEA

1. Ouvrir le projet dans IntelliJ IDEA
2. Faire un clic droit sur `BookShelfSpec.java`
3. Cliquer sur **Run 'BookShelfSpec'**

---

# Exemple d’utilisation

```java
BookShelf shelf = new BookShelf();

shelf.addBook(new Book("Java Basics", 2020));
shelf.addBook(new Book("Algorithms", 2018));

System.out.println(shelf.getBooks());
```

---

# Objectif pédagogique

Ce projet permet de pratiquer :

* La programmation orientée objet en Java
* L’utilisation des collections
* Les interfaces `Comparable` et `Comparator`
* Les tests unitaires avec JUnit 5
* Les bonnes pratiques de développement

---

