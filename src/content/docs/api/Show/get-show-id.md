---
title: Recevoir un show par id ✅
description: Route pour recevoir un show par son id
---

* **URL**

  /api/shows/{showId}

* **Méthode:**
  
  `GET`

* **Réponse de succès:**
  
  * **Code:** 200 <br />
    **Contenu:** 
    ```json
    {
      "id": 1,
      "name": "Competition 1",
        "address": {
          "street_address": "123 Main Street",
          "province": "Quebec",
          "country": "Canada",
          "city": "Quebec",
          "zip_code": "J9K1P9",
          "other_information": "Troisième porte à droite"
        },
      "organizer": {
        "id": 2,
        "name": "Mark Admio",
        "email": "mark.admio@example.com",
        "phone": "123-456-1234",
        "birthdate": "1990-01-01T00:00:00.000Z"
      },
      "can_have_late_registration": false,
      "path_logo": null,
      "nb_total_place": 100,
      "nb_free_place": 100,
      "nb_temp_stalls": 75,
      "nb_permanent_stalls": 25,
      "nb_tack_stalls": 25,
      "nb_free_temp_stalls": 75,
      "nb_free_permanent_stalls": 25,
      "nb_free_tack_stalls": 25,
      "show_fees": {
        "id": 1,
        "hay": 50,
        "shaving": 30,
        "temp_stall_per_day": 25,
        "permanent_stall_per_day": 25,
        "tack_stall_per_day": 25,
        "drug_test": 20
      },
      "administration_fee": {
        "id": 1,
        "administration": 50,
        "late_inscription": 40,
        "cancel_inscription": 25,
        "ground": 90,
        "paramedics": 120,
        "camper_ground_rental": 80
      },
      "recognized_show": false,
      "rules": "Hello I am the rules !",
      "start_date": "2024-01-01T00:00:00.000Z",
      "end_date": "2024-01-05T00:00:00.000Z",
      "inscription_start_date": "2024-01-01T00:00:00.000Z",
      "inscription_end_date": "2024-01-01T00:00:00.000Z",
      "inscription_end_late_date": "2024-01-01T00:00:00.000Z",
      "is_published": false, 
      "secretary": {
        "id": 3,
        "name": "Jo Nathan",
        "email": "jo.nathan@example.com",
        "phone": "123-456-9874",
        "birthdate": "1990-01-01T00:00:00.000Z"
      }
    }
    ```

* **Réponse d'erreur:**

  * **Code:** 404 NOT FOUND <br />
    **Contenu:** 
    ```json
    { "message": "La ressource n’existe pas." }
    ```
