Gestion des réservations de salles

## Objectifs

Créer les entités Salle, Réservation, Utilisateur, Équipement.

Faire une relation ManyToMany entre Salle et Équipement.

Tester cascade et orphanRemoval.

## Étapes

## 1️/Créer le projet Maven

Nouveau projet Maven (GroupId = com.example, ArtifactId = gestion-reservations).

Ouvrir dans ton IDE préféré.

## 2️/ Ajouter les dépendances

JPA et Hibernate pour gérer la base.

H2 pour une base en mémoire.

JUnit pour tester.

## 3️/ Configurer Hibernate

Créer persistence.xml.

Configurer H2 et Hibernate (create-drop pour créer la base à chaque lancement).

## 4️/ Créer les entités

-Utilisateur : id, nom, prenom, email

A plusieurs réservations (OneToMany, cascade + orphanRemoval).

-Réservation : id, dateDebut, dateFin, motif

Liée à un utilisateur et une salle (ManyToOne).

-Salle : id, nom, capacite, description

A plusieurs réservations (OneToMany).

A plusieurs équipements (ManyToMany).

-Équipement : id, nom, description

Lié à plusieurs salles (ManyToMany inverse).


## 5️/ Tester les relations et cascade

Persister un utilisateur avec réservation et salle.

Vérifier que la réservation se crée automatiquement grâce au cascade.

Supprimer une réservation d’un utilisateur pour voir orphanRemoval en action.

## 6️/ Tester ManyToMany

Créer des salles et équipements.

Ajouter des équipements aux salles.

Supprimer un équipement d’une salle et vérifier qu’il reste dans la base.

## Dagramme de class:

<img width="448" height="317" alt="image" src="https://github.com/user-attachments/assets/d8d9c066-d94a-4920-ab97-2eaba416f1be" />


## 7️/ Lancer le projet

Résultat:



<img width="634" height="369" alt="lab2 hibernate 1 " src="https://github.com/user-attachments/assets/697d2aca-45bd-473d-b7ce-299e95ecaac4" />


<img width="734" height="367" alt="lab2 hibernate 2 " src="https://github.com/user-attachments/assets/1a34510f-981c-4e83-9834-a8003893fa37" />


<img width="626" height="379" alt="lab2 hibernate 3 " src="https://github.com/user-attachments/assets/a1696d8a-b982-476b-80a1-354a875e5784" />



<img width="638" height="352" alt="lab2 hibernate 4 " src="https://github.com/user-attachments/assets/207e1fe7-c98b-461d-bb6b-b4e00d1cb331" />



<img width="766" height="311" alt="lab2 hibernate 5 " src="https://github.com/user-attachments/assets/6ecf3a35-6c2b-49e6-8aee-737f8324ff5e" />


<img width="717" height="365" alt="lab2 hibernate 6 " src="https://github.com/user-attachments/assets/f8993c44-913b-43e2-a86c-0a9ce14b029f" />


<img width="599" height="365" alt="lab2 hibernate 7 " src="https://github.com/user-attachments/assets/0f2794a5-e4ea-416f-8b97-12f1ace43480" />


<img width="399" height="371" alt="lab2 hibernate 8 " src="https://github.com/user-attachments/assets/6e236375-2105-4304-bb76-d7f7b96e00e0" />


<img width="397" height="359" alt="lab2 hibernate 9 " src="https://github.com/user-attachments/assets/1b396960-b8c7-47d8-bfa4-0cddf7f6a372" />


<img width="686" height="374" alt="lab2 hibernate 10 " src="https://github.com/user-attachments/assets/74026334-ce51-40b8-a838-3bc326696e75" />


<img width="325" height="368" alt="lab2 hibernate 11 " src="https://github.com/user-attachments/assets/e804f9b5-5bd6-4292-8966-d77b6fbe9a47" />



<img width="250" height="370" alt="lab2 hibernate 12 " src="https://github.com/user-attachments/assets/d52a79ae-b84f-4745-9a86-a66dc317822e" />


<img width="293" height="364" alt="lab2 hibernate 13 " src="https://github.com/user-attachments/assets/f013ee3f-0e54-48e7-bbc5-82e267ed772f" />

<img width="371" height="372" alt="lab2 hibernate 14 " src="https://github.com/user-attachments/assets/65378a7a-6a5e-4e52-90a3-476c3be3179e" />

<img width="377" height="374" alt="lab2 hibernate 15 " src="https://github.com/user-attachments/assets/a7043994-e14c-4ba7-badb-572b8d73b0af" />

<img width="387" height="365" alt="lab2 hibernate 16 " src="https://github.com/user-attachments/assets/a2a9b902-fe55-4d35-a42b-c2cb398b7d38" />

<img width="364" height="371" alt="lab2 hibernate 17 " src="https://github.com/user-attachments/assets/27779c4d-7968-47a6-9da0-a796a0e0d1fd" />

<img width="420" height="367" alt="lab2 hibernate 18 " src="https://github.com/user-attachments/assets/205729f6-5654-4c4d-9c05-265333cca04a" />

<img width="443" height="368" alt="lab2 hibernate 19 " src="https://github.com/user-attachments/assets/4049b0bd-4ec5-42fe-8fc0-cdd35313af0e" />

<img width="884" height="373" alt="lab2 hibernate 20 " src="https://github.com/user-attachments/assets/2ac4e00f-28c9-42bc-ae97-466fcf3cbcb0" />

<img width="887" height="353" alt="lab2 hibernate 21 " src="https://github.com/user-attachments/assets/df1c9b5a-08b1-460a-94c4-010dbfb27038" />



![lab3 Hibernate structure](https://github.com/user-attachments/assets/26dc06b6-6502-4fcb-a17e-2dab52a78b20)

