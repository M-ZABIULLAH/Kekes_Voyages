# Dictionnaire de Données pour Kekes_Voyages

## Légende des Types de Données
- **A** : Alphanumérique texte
- **AN** : Alphanumérique numérique (identifiant)
- **D** : Date
- **T** : Timestamp (date et heure)
- **N** : Numérique
- **B** : Booléen (vrai/faux)
- **E** : Enum (liste de valeurs prédéfinies)


| Nom du champ       | Type de données | Taille | Clé | Obligation | Description                             |
|--------------------|-----------------|--------|-----|------------|-----------------------------------------|
| Id_Passager        | AN              | 36     | PK  | Obligatoire| Identifiant unique du passager          |
| nom                | A               | 50     |     | Obligatoire| Nom du passager                         |
| prenom             | A               | 50     |     | Obligatoire| Prénom du passager                      |
| email              | A               | 100    |     | Obligatoire| Adresse e-mail du passager              |
| telephone          | A               | 20     |     | Obligatoire| Numéro de téléphone du passager         |
| adresse            | A               | 255    |     | Facultatif | Adresse postale du passager             |
| date_naissance     | D               |        |     | Facultatif | Date de naissance du passager           |
| Id_Vol             | AN              | 36     | PK  | Obligatoire| Identifiant unique du vol               |
| numero_vol         | A               | 20     |     | Obligatoire| Numéro de référence du vol              |
| date_depart        | T               |        |     | Obligatoire| Date et heure de départ du vol          |
| date_arrivee       | T               |        |     | Obligatoire| Date et heure d'arrivée du vol          |
| aeroport_depart    | A               | 50     |     | Obligatoire| Nom de l'aéroport de départ             |
| aeroport_arrivee   | A               | 50     |     | Obligatoire| Nom de l'aéroport d'arrivée             |
| capacite           | N               |        |     | Obligatoire| Nombre de places disponibles            |
| prix_base          | N               | (15,2) |     | Obligatoire| Prix de base du vol                     |
| statut_vol         | E               | 20     |     | Obligatoire| Statut du vol (programmé, annulé, etc.) |
| Id_Reservation     | AN              | 36     | PK  | Obligatoire| Identifiant unique de la réservation    |
| Id_Reservation     | AN              | 36     | PK  | Obligatoire| Identifiant unique de la réservation    |
| date_reservation   | T               |        |     | Obligatoire| Date et heure de la réservation         |
| statut             | E               | 20     |     | Obligatoire| Statut (confirmé, en attente, annulé)   |
| nombre_passagers   | N               |        |     | Obligatoire| Nombre de passagers                     |
| Id_Passager        | AN              | 36     | FK  | Obligatoire| Référence au passager principal         |
| Id_Vol             | AN              | 36     | FK  | Obligatoire| Référence au vol                        |
| prix_total         | N               | (15,2) |     | Obligatoire| Prix total de la réservation            |
| Id_Reservation     | AN              | 36     | FK  | Obligatoire| Référence à la réservation              |
| Id_Billet          | AN              | 36     | PK  | Obligatoire| Identifiant unique du billet            |
| date_emission      | T               |        |     | Obligatoire| Date et heure d'émission du billet      |
| prix               | N               | (15,2) |     | Obligatoire| Prix du billet                          |
| classe             | E               | 20     |     | Obligatoire| Classe (économique, affaires, première) |
| siege              | A               | 10     |     | Facultatif | Numéro de siège                         |
| Id_Reservation     | AN              | 36     | FK  | Obligatoire| Référence à la réservation              |
| Id_Vol             | AN              | 36     | FK  | Obligatoire| Référence au vol associé                |
| Id_Passager        | AN              | 36     | FK  | Obligatoire| Référence au passager                   |

## Abréviations

- **PK** : Primary Key (Clé primaire)
- **FK** : Foreign Key (Clé étrangère)

