# MLD : Script : 

- Personnes (**id_Personne**, nom, prenom, dateNaiss, genre, nationalite)
- Clients (**id_Client**; #id_Personne, email, mdp, adresse_facturation)
- Passagers (**num_passeport**, #id_Personne, #id_client)
- Vol (**id_vol**, date_dep, date_arrivee, details, #id_aeroport_depart, #id_aeroport_arrivee)
- Reservations (**#(id_client, id_vol, #id_passager**), num_reservation)
- Organsiations_vol_Aeroport (**#(id_vol, id_Compagnie)**)
- Escales (**id_escale**, #id-vol,#id_aeroport, date_depart_esc, date_arrivee_esc)
- Aeroports (**id_aeroport**, nom, ville, pays)
- Compagnies (**id_compagnie**, nom, num_siret)
- Avions (**id_avion**, #id_compagnie, modele, classe, capacite)

FK : **#**  
PK : **pk**

# MLD Schéma 
![Modèle Logique de Données (MLD)](notes/mld.jpg)
- Personnes (**id_personne**, nom, prenom, dateNaiss, email, genre, nationalite)
- Clients (**id_Client**; #id_personne, email, mdp, adresse_facturation)
- Passagers (**num_passeport**, #id_personne, #id_client)
- Vol (**id_vol**, date_dep, date_arriver, details)
- Reservations (**#(id_client, id_vol, #id_passager**), num_reservation)
- Organsiations_vol_Aeroport (**#(id_vol, oaci)**)
- Escales (**id_escale**, #id-vol, date_depart_esc, date_arriver_esc)
- Aeroports (**oaci**, nom, ville, pays)
- Compagnies (**iata**, nom, num_siret)
- Avion (**id_avion**, #iata, modele, classe, capacite)
FK : **#**  
PK : **pk**
