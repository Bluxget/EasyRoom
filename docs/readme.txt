Base de données :
USERS:
- id
- username
- firstname
- lastname
- password
- birthdate
- email
- roles

PROPERTY:
- id
- name
- description
- numbePersonsProperty
- postalCode
- region
- country
- typeProperty (home, flat)
- pictures
- surface
- maxNumberPeople
- #idUser
    FULL PROPERTY:
- numberRoom

ONE ROOM:

EQUIPMENTS:
- id
- name
- description

PROPOSALS:
- id
- price
- date
- #idProperty

RESERVATIONS:
- dateStart
- dateEnd
- numberPersons
- finalPrice
- approuved



Le but de notre projet était de créer une application web en PHP en utilisant le framework Symfony. Nous avons environ 3 jours pour ce projet, il a donc fallu prendre des décisions afin d’avoir un développement rapide sur les fonctions principales et les plus importantes.

Nous avons commencé par développer le système de création de comptes et de connexion afin d’avoir une gestion des rôles qui nous permet de gérer les autorisations.

Nous avons décidé de donner de gérer les droits des internautes de cette façon :
- Tous les visiteurs peuvent voir les propositions.
- Lorsque qu’un visiteur créer un compte, son compte passe en tant qu’utilisateur.
- Lorsque qu’un utilisateur créer un bien, son compte passe en tant que propriétaire.

**** Visiteur :
    Voir les propositions (/)

**** Utilisateur :
    Voir les propositions (/)
    Demander réservation pour une proposition
    Créer un bien (/property/create)

**** Propriétaire :
    Voir les propositions (/)
    Demander réservation pour une proposition
    Créer un bien (/property/create)
    Voir ses biens (/properties/user)
    Créer une proposition

Pour ce qui est de la partie esthétique, nous avons utilisé Bootstrap car nous avons quelques soucis avec Materialize.

Pour sauvegarder notre projet et gérer les différentes versions, nous utilisons un outil de versionning nommé Git (également GitHub) qui permet de travailler facilement sur un même projet.

