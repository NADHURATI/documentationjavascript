# documentationjavascript
```javascript
// Déclaration variable
let nom = "fatima";
const age = 22;
var commune = "chirongui";

# Initiation javascript

## Commandes

```dart
npm init

npm install nodemon

npm start
```

## Package.json

```json
 "scripts": {
    "start": "nodemon index.js"
  },
```

# Cours complet de JavaScript pour débutants

## 1. Introduction à JavaScript

JavaScript est un langage de programmation utilisé principalement pour rendre les pages web interactives. Il fonctionne dans les navigateurs et permet de manipuler les éléments HTML et CSS.

---

## 2. Les Variables

Une variable sert à stocker une valeur (nombre, texte, etc.). En JavaScript, on utilise `var`, `let` ou `const` pour déclarer une variable.

### Exemple :

```jsx
let nom = "Alice"; // Variable pouvant être modifiée
const age = 25; // Variable constante, non modifiable
var ville = "Paris"; // Ancienne façon de déclarer une variable
```

### Différences entre `var`, `let` et `const` :

- `let` : Permet de déclarer une variable modifiable.
- `const` : Valeur fixe qui ne peut pas être changée.
- `var` : Moins utilisé aujourd'hui car il peut poser des problèmes de scoping.

---

## 3. Les Conditions

Les conditions permettent d'exécuter différents blocs de code en fonction d'une situation.

### Exemple :

```jsx
let age = 18;
if (age >= 18) {
    console.log("Vous êtes majeur.");
} else {
    console.log("Vous êtes mineur.");
}
```

### Les opérateurs de comparaison :

- `===` : égalité stricte (même valeur et même type)
- `!==` : différent strictement
- `>` : supérieur
- `<` : inférieur
- `>=` : supérieur ou égal
- `<=` : inférieur ou égal

---

## 4. Les Boucles (Incrémenter et Décrémenter)

Les boucles permettent d'exécuter un bloc de code plusieurs fois.

### Boucle `for` :

```jsx
for (let i = 0; i < 5; i++) {
    console.log("Tour n°" + i);
}
```

### Boucle `while` :

```jsx
let compteur = 0;
while (compteur < 5) {
    console.log("Compteur : " + compteur);
    compteur++; // Incrémentation
}
```

---

## 5. Les Fonctions

Une fonction permet de réutiliser du code.

### Exemple :

```jsx
function direBonjour(nom) {
    console.log("Bonjour, " + nom + " !");
}

direBonjour("Alice"); // Affiche : Bonjour, Alice !
```

### Fonction avec retour de valeur :

```jsx
function addition(a, b) {
    return a + b;
}
let resultat = addition(3, 5);
console.log(resultat); // Affiche 8
```

---

## 6. Conclusion

Avec ces bases, vous pouvez déjà commencer à programmer en JavaScript. Pratiquez en réalisant des petits projets comme une calculatrice ou un compteur de clics sur une page web !

```
