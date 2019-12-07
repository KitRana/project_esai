## emergency path fire
* help
    - utter_emergency_service
* fire
    - utter_areyouindanger
* affirm
    - utter_what_is_problem_danger
* fire_matter_danger
    - utter_thanks
    - utter_location
* location{"location": "house"}
    - slot{"location": "house"}
    - slot{"location": "house"}
    - utter_thanks
    - utter_street
* street{"street": "123 Grove Street"}
    - slot{"street": "123 Grove Street"}
    - slot{"street": "123 Grove Street"}
    - utter_thanks
    - utter_fire   <!-- predicted: utter_police -->
    - utter_ask_for_person
* person{"person": "Tom"}
    - slot{"person": "Tom"}
    - slot{"person": "Tom"}
    - utter_console
* thanks
    - utter_welcome


## non emergency path fire
* help
    - utter_emergency_service
* fire
    - utter_areyouindanger
* deny
    - utter_ask_for_person
* person{"person": "Tom"}
    - slot{"person": "Tom"}
    - slot{"person": "Tom"}
    - utter_thanks_person
    - utter_what_is_problem
* fire_matter
    - utter_fire_dispatch
* affirm
    - utter_location
* location{"location": "house"}
    - slot{"location": "house"}
    - slot{"location": "house"}
    - utter_street
* street{"street": "123 Grove Street"}
    - slot{"street": "123 Grove Street"}
    - slot{"street": "123 Grove Street"}
    - utter_thanks
    - utter_fire_person   <!-- predicted: utter_police_person -->
* thanks
    - utter_welcome


## non emergency ems
* help
    - utter_emergency_service
* ems
    - utter_areyouindanger
* deny
    - utter_ask_for_person
* person{"person": "Tom"}
    - slot{"person": "Tom"}
    - slot{"person": "Tom"}
    - utter_thanks_person
    - utter_what_is_problem
* ems_matter
    - utter_ems_dispatch
* affirm
    - utter_location
* location{"location": "house"}
    - slot{"location": "house"}
    - slot{"location": "house"}
    - utter_street
* street{"street": "123 Grove Street"}
    - slot{"street": "123 Grove Street"}
    - slot{"street": "123 Grove Street"}
    - utter_thanks
    - utter_ems_person   <!-- predicted: utter_police_person -->
* thanks
    - utter_welcome


