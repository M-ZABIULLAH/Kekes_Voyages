# MLD : Script : 

- Personne (**id_personne**, nom, prenom, dateNaiss, email, genre, nationalite)
- Client (**id_client**,**#id_personne**, email, mdp, info_bancaire, adresse_facturation)
- Passager (**num_passeport**, **#id_personne**)
- Vol (**id_vol**, date_dep, date_arriver, details)
- Reservation (**#(id_client, id_vol, #id_passager**), num_reservation)
- Organsiation_vol (**#(id_vol, iata)**, nom, #**num_siret**)
- Avion (id_avion, **#iata**, classe, capacite)
- Escale (**#(id_vol, oaci), date_depart_escale, date_arriver_escale)
- Aeroport (**oaci**, nom, ville, pays)
- Compagnie (**iata**, nom, num_siret)