# Cahier des charges

## Membres de l'équipe

- Maureen Gaudard
- Jennifer Froidevaux
- Tess Triponez

## Thème

### Biologie marine

Le projet consiste à créer un site web consacré à la **biologie marine**.

Le site permettra de consulter un catalogue regroupant différentes espèces marines, classées par catégories.

Une partie privée sera accessible aux utilisateurs connectés. Elle leur permettra de prendre des notes personnelles, à la manière d'un **journal de plongée ou d'étude de la biologie marine**.

---

# Fonctionnalités principales de l'application

## Gestion multilingue

- Le site est disponible en **français et en anglais**.
- L'utilisateur peut changer la langue de l'interface.

## Gestion des e-mails

- Envoyer un e-mail de confirmation ou d'information lors de certaines actions.

---

# Partie publique

## Page d'accueil

La page d'accueil permet de :

- Présenter le projet et son objectif.
- Présenter brièvement la biologie marine.
- Permettre d'accéder au catalogue des espèces.
- Permettre d'accéder à la connexion et à l'inscription.

## Catalogue des espèces

Le catalogue permet de :

- Afficher les espèces disponibles et classer les espèces par catégories.
- Rechercher une espèce.
- Sélectionner une espèce afin de consulter sa fiche.

## Fiche d'une espèce

La fiche d'une espèce affiche notamment :

- **Nom commun**
- **Nom scientifique**
- **Description**
- **Habitat**
- **Alimentation**
- **Image**
- **Autres informations pertinentes**

---

# Partie utilisateur

## Créer un compte

L'utilisateur peut :

- Créer un compte avec son adresse e-mail.
- Définir un mot de passe.
- Recevoir les e-mails prévus par l'application.

## Authentification

L'utilisateur peut :

- Se connecter.
- Se déconnecter.

## Gestion du profil

L'utilisateur peut :

- Consulter son profil.
- Modifier ses informations personnelles.
- Se déconnecter.

## Journal personnel

L'utilisateur peut :

- Consulter ses notes.
- Voir ses notes classées par date.
- Consulter le détail d'une note.

## Créer une note d'observation

Une note contient notamment :

- **Titre**
- **Date**
- **Lieu**
- **Profondeur**
- **Description**
- **Espèces observées**

Les espèces observées peuvent être sélectionnées parmi celles présentes dans le catalogue.

## Modifier une note

L'utilisateur peut modifier ses propres notes.

## Supprimer une note

L'utilisateur peut supprimer ses propres notes.

---

# Partie administrateur

## Gestion des espèces

L'administrateur peut :

- Ajouter une espèce.
- Modifier une espèce.
- Supprimer une espèce.

## Gestion des utilisateurs

L'administrateur peut :

- Consulter la liste des utilisateurs.
- Consulter les informations nécessaires à leur gestion.

---

# Fonctionnalités optionnelles

Les fonctionnalités suivantes pourront être développées **si le temps le permet**.

## Gestion de la langue

- La langue choisie par l'utilisateur peut être mémorisée à l'aide d'un cookie.

## Partie utilisateur connecté

- Ajouter une espèce au catalogue.
- Modifier uniquement les espèces ajoutées par l'utilisateur.
- Ajouter une page d'accueil privée avec un tableau de bord basé sur les entrées du journal.

### Exemple de statistiques

Le tableau de bord pourrait afficher :

- **32 espèces observées**
- **3 plongées enregistrées**
- **Dernières observations :** Loutre de mer, Oursin violet

## Partie administrateur

- Valider les espèces ajoutées par les utilisateurs.
- Désactiver un compte utilisateur.
- Tableau de bord administrateur

Le tableau de bord permet d'avoir une vue générale de l'application, notamment : Le nombre d'utilisateurs et le nombre d'espèces.

---

# Partie technique

## Base de données

La base de données contiendra notamment les tables suivantes :

- `users`
- `species`
- `journal_entries`
- `journal_species`

La table `journal_species` sera une **table de liaison** entre les entrées du journal et les espèces observées.
