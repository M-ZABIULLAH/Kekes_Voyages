# Dictionnaire de Données


## Structure des Tables

Les tables sont décrites avec les détails suivants :

| Nom du champ   | Type de données | Taille  |   |   | Description  |
|----------------|-----------------|---------|------|--------------|--------------|
| ...            | ...             | ...     |   |           | ...          |







| Nom du champ  | Type de données | Taille |   |      | Description                      |
|---------------|-----------------|--------|------|-----------------|----------------------------------|
| Id_Passager   | AN              |        |        |   | Identifiant unique du passager  |
| nom           | A               | 50     |      |          | Nom du passager                 |
| email         | A               | 50     |      |                 | Adresse e-mail du passager      |
| téléphone     | A               | 50     |      |                 | Numéro de téléphone du passager |
| Id_Vol            | AN              |        |  | | Identifiant du vol                     |
| date_depart       | D               |        |      |               | Date de départ du vol                  |
| aeroport_arrivee  | A               | 50     |      |               | Nom de l’aéroport d’arrivée            |
| Id_Paiement   | AN              |           |    | | Identifiant du paiement            |
| montant       | AN              | (15,2)    |      |               | Montant payé                        |
| date_paiement | D               |           |      |               | Date du paiement                    |
| Id_Réservation    | AN              |        |    |                      | Identifiant de la réservation       |
| date_resevation   | D               |        |      |                                     | Date de la réservation              |
| statut            | B              |        |      |                                     | Statut (confirmé, annulé, etc.)     |
| Numebre_passager  | A               | 50     |      |                                     | Nombre de passagers                 |
| Id_Passager       | AN              |        |    |     | Référence au passager               |
| Id_Paiement       | AN              |        |    |  | Référence au paiement               |
| Id_Billet        | AN              |        |    |                     | Identifiant du billet                |
| date_achat       | D               |        |      |                                       | Date d'achat du billet               |
| prix             | A               | 50     |      |                                       | Prix du billet                       |
| Id_Réservation   | AN              |        |    | | Référence à la réservation        |
| Id_Vol           | AN              |        |    |                 | Référence au vol associé             |

