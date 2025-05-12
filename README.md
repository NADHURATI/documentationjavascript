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

let jour = "mardi"; // valeur
// les instructions
switch (jour) {
    case "lundi":
        console.log("c'est le début de la semaine !");
        break; // arrête l'exécution du switch après ce cas
    case "mardi":
        console.log("C'est mardi, encore du boulot !");
        break;
    case "samedi":
        break;
    case "dimanche":
        console.log("C'est le week-end !");
        break;
    default: // Si 'jour' ne correspond à aucun des cas précédents, on exécute par défaut
        console.log("Jour inconnu");                
}
```

```

Fonction avec retour de valeur :

function addition(a,b) {
    return a + b;
}
// fonction anonyme 
const add = function(a,b) {
  return a + b;
}
// fonction fléché
const add = (a, b) => {
  return a + b;
}
// exemple
const add = (a, b) => a + b;
// appel de la fonction
let resultat = add(2,2);

```

```
## 6. Objet littéral

### Qu’est-ce qu’un objet littéral en JavaScript ?

Un **objet littéral** est un moyen simple de créer un objet avec des **paires clé/valeur**. Il permet de **stocker et organiser des données**.

```jsx
const personne = {
  prenom: "Ali",
  nom: "Mansour",
  age: 30,
  estActif: true
};
```

### 🔍 Explication :

- `prenom`, `nom`, `age`, `estActif` sont les **clés** (ou propriétés).
- `"Ali"`, `"Mansour"`, `30`, `true` sont les **valeurs** associées.

```jsx
console.log(personne.prenom); // Ali
console.log(personne["nom"]); // Mansour
```

## ✍️ Modifier une propriété

```jsx
personne.age = 31;
personne["estActif"] = false;
```

## ➕ Ajouter une nouvelle propriété

```jsx

personne.profession = "Développeur";
```

---

## ❌ Supprimer une propriété

```jsx
delete personne.estActif;
```

---

## ✅ Exemple complet

```jsx
const voiture = {
  marque: "Toyota",
  modele: "Yaris",
  annee: 2020
};

console.log(voiture.modele); // Yaris

voiture.couleur = "Rouge";
console.log(voiture); // Ajout de la couleur

delete voiture.annee;
console.log(voiture); // Année supprimée
```

---

## ⚙️ Ajouter une méthode à un objet

Une **méthode** est une **fonction à l'intérieur d'un objet**.

```jsx
const utilisateur = {
  nom: "Sarah",
  saluer: function () {
    console.log("Bonjour, je m'appelle " + this.nom);
  }
};

utilisateur.saluer(); // Bonjour, je m'appelle Sarah
```

---

## les classes

- Une classe est patron de création d’objet
- la première lettre du nom de la classe doit être en majuscule
- une classe possède des propriétés qui sont dans le constructor
- une classe possède des méthodes

```
jsx
    // déclarer une class
class Personnage {
	constructor(nom, sante, force){
		this.nom = nom;
		this.sante = sante;
		this.force = force;
	}
	
	decrire(){
		return this.nom;
	}
}

// instancier
let aura = new Personnage("aurora", 150, 30);
let gla = new Personnage("gladius", 120, 50);

console.log(gla.sante); // 120
```

Les class (Exercice)
```
class Voiture {
    constructor(vitesse,marque) {
        this.vitesse = vitesse;
        this.marque = marque;
    }
    accelerer(vitesse) {
        this.vitesse = vitesse;
    }

    freiner(vitessedefreinage) {
        this.vitesse = vitessedefreinage;
    }
}

let bmw  = new Voiture(0, "bmw"); // instancier : c'est creer un objet à partir d'une class

bmw.accelerer(100);
console.log(bmw.vitesse);

bmw.freiner(50);
console.log(bmw.vitesse);
```

FUNCTION FLECHE (Revision)
```
function verification (age) {
    if (age >= 22) {
        return "majeur";
    }else{
        return "mineur";
    }
}

const resultat = verification(30);
console.log(verification);
```

Les listes (REVISION)
```
let nom;
/*console.log(nom);*/

const CLE = "Mayotte";

let fruit = ["ananas", "fraise", "poire"];
fruit.push("orange"); 
console.log(fruit);

let ordinateur = {
    nom : "Lenono",
    annee : 2025,
    fonctionnalitees : ["camera" , "micro"],
    voirfonctionnalitees() {
        for (let i = 0; i < this.fonctionnalitees.length; i++) {
            console.log(this.fonctionnalitees[i]);
        }
    }
};
```

Mini Exercice
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=, initial-scale=1.0">
    <title>Document</title>
</head>

<body>

    <h1> Mini exercice </h1>

    <script>
    
    let livre = {
        titre : "Pitchou",
        auteur : "Patrick",
        nombrePage : 50
    };
    
    console.log(livre.titre , livre.auteur , livre.nombrePage);

    </script>

</body>

</html>
```

Exercce de connexion
```
<!DOCTYPE html>
<html lang="fr">
    <head>
        <meta charset="utf-8">
        <link href="connexion.css" rel="stylesheet"/>
    </head>

    <body>

        <div>
        
        <h1>Connexion agent </h1>

        <h2>Connectez-vous afin d'avoir accès à la gestion du test OISIA .</h2>

        

            <label> Email :</label>
            <input type="text" name="Votre email" placeholder="email"/> <br> <br>
            <label> Mot de passe :</label>
            <input type="text" name="Votre mot de passe" placeholder="mot de passe"/> <br> <br>

        <input type="submit"> <br><br>



        <h3> Pas de compte agent,Connectez-vous</h3> <br><br>
        
    </div>


        <footer>
            <p>&copy; Tous droits réserveés - CARIF OREF Mayotte</p>
        </footer>



    </body>
</html>
```

CSS
```
div {
    background-color: #fff; 
    padding: 20px; 
    width: 350px; 
    margin: 40px auto; 
    border-radius: 10px; 
}

body {
    background-color: #FFEFE5;
}

h1 {
    font-weight: bold; 
    color: black; 
    text-align: center; 
}

h2 {
    font-weight: bold;
    color: black;
    text-align: center;
    font-size: 10px;
}

h3 {
    color: black;
    font-size: 15px;
    text-align: center;
}

input[type="submit"] {
    background-color: #FFD8C0;
    color: black; 
    border: none; 
    padding: 15px; 
    width: 100%; 
    border-radius: 5px; 
    font-size: 16px; 
}

footer {
    text-align: center;
}
```

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Connexion</title>
    <link href="connexioncandidat.css" rel="stylesheet"/>
</head>
<body>

    <div class="connexion">

        <h1>Connexion Candidat</h1>
        
        <p>Renseignez votre identifiant unique pour accéder au test OISIA</p> <br> <br>

        <input type="text" name="Votre identifiant unique" placeholder="identifiant unique"/> <br> <br>

        <button>S'identifier</button>

    </div>
    
</body>
</html>
```

CSS
```
div {
    background-color: #fff;
    padding: 20px;
    width: 440px;
    margin: 40px auto;
    border-radius: 12px; 
}

p {
    color: black;
    text-align: center;
    font-size: 13px;
}

body {
    background-color: #FFEFE5;
}

h1 {
    font-weight: bold; 
    color: black; 
    text-align: center; 
}

button {
    background-color: #FFD8C0; 
    color: black; 
    border: none; 
    padding: 15px; 
    width: 100%; 
    border-radius: 5px; 
    font-size: 16px; 
    text-align: center; 
    
}
```

Revision sur le SERVER
```
const express = require("express");
const app = express();

const PORT = 3000;

app.get('/', (req, res) => {
    res.send('Hello, Express !');
});

app.listen(PORT, () => {
    console.log('Serveur lancé');
});
```

Les CLASS (Exercice)
```
class Personnage {
    constructor(nom,sante,force) {
        this.nom = nom;
        this.sante = sante;
        this.force = force;
    }
    decrire(){
        return this.nom;
    }
}

let boubou = new Personnage("boubou",120,100);
let petitcoeur = new Personnage("petitcoeur",120,80);

let boubou1 = {
    nom : "boubou",
    sante : 120,
    force : 100,
    decrire() {
        return this.nom;
    }
};
```

Les Fetch avec les HTTP
```
class APIhttp {
    async getHttp() {
        try {
            const response = await fetch("https://www.google.fr");
            if (response.ok) {
                return response;
            }
            return "sans réponse";
        } catch (error) {
            return error;
        }
    }
}

let requete = new APIhttp();
const data = await requete.getHttp();
console.log(data);
```

Les Class avec La Voiture
```
class Voiture {
    constructor(marque, puissance) {
        this.marque = marque;
        this.puissance = puissance;
    }
    augmenter(valeur) {
        this.puissance += valeur;
    }
    augmenter(valeur) {
        this.puissance -= valeur;
    }
}

let audi = new Voiture("audi", 50);
audi.augmenter(100);
console.log(audi.puissance);
```

Les Fonction avec les retour des valeurs avec les Marque de Voitures
```
// Déclaration d'un tableau contenant des marques de voitures
let marqueVoiture = ["mercedes", "bmw", "audi"];

// Définition d'une fonction qui cherche une marque spécifique dans le tableau
function trouverMarque(marques) {
  // Boucle qui parcourt chaque élément du tableau
  for (let i = 0; i < marques.length; i++) {
    // Si la marque courante est "bmw"
    if (marques[i] === "bmw") {
      // Affiche "bmw" dans la console
      console.log(marques[i]);
      // Interrompt la boucle immédiatement après avoir trouvé "bmw"
      break;
    }
  }
}

// Appel de la fonction avec le tableau de marques
// La variable 'valeurRecuperer' vaudra 'undefined' car la fonction ne retourne rien
let valeurRecuperer = trouverMarque(marqueVoiture);

```

Exercice
```
<!DOCTYPE html>
<html lang="fr">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Icônes avec Style</title>

    <!-- Lien Font Awesome -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">

    <!-- Ton CSS externe -->
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <div class="container">
    
    <div class="logo">
        <p><i class="fas fa-at icon"></i></p>
    </div> 

    <div class="Menu">

        <div class="menu-item"><i class="fas fa-copy icon"></i> Menu item 1</div>
        <div class="menu-item"><i class="fas fa-calendar-alt icon"></i> Menu item 2</div>
        <div class="menu-item"><i class="fas fa-user icon"></i> Menu item 3</div>
        <div class="menu-item"><i class="fas fa-paperclip icon"></i> Menu item 4</div>

    </div>

    <div class="box">
        <h1><i class="fas fa-copyright title-icon"></i> Bacar Darwin</h1>
    </div>

    </div>
</body>
</html>
```

Requête HTTP
```
const axios = require("axios");

const connexion = {
    name: "anonyme",
    first_name: "anonyme",
    password: "n03dh10ra",
    status_agent: "all",
    assigned_digital_space: "Mangajou",
    email: "nadhuratiali47@gmail.com"
  };
  
  axios.post("https://backend-taarafa.onrender.com/log/signup-agent", connexion)
    .then(response => {
      console.log('✅ Inscription réussie !');
      console.log('Code de statut :', response.status); // Doit être 201
      console.log('Réponse :', response.data);
    })
    .catch(error => {
      if (error.response) {
        console.log('❌ Erreur lors de la requête');
        console.log('Code de statut :', error.response.status);
        console.log('Message :', error.response.data);
      } else {
        console.error('Erreur réseau ou autre :', error.message);
      }
    });
  ```






