## chitchat
* ask_weather OR ask_builder OR ask_howdoing OR ask_languagesbot OR ask_howold OR ask_restaurant OR ask_time OR ask_wherefrom OR ask_whoami OR handleinsult OR telljoke OR ask_whatismyname OR marry_me OR compliment
    - action_chitchat

## greet
* greet
  - utter_greet

## sad path 1
* greet
  - utter_greet
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* affirm
  - utter_happy

## sad path 2
* greet
  - utter_greet
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* deny
  - utter_goodbye

## say goodbye
* goodbye
  - utter_goodbye

## bot challenge
* bot_challenge
  - utter_iamabot

## emergency path police
* help
    - utter_emergency_service
* police
    - utter_areyouindanger
* affirm
    - utter_what_is_problem_danger
* police_matter_danger
    - utter_thanks
    - utter_location_type
* location_type{"location_type":"house"}
    - slot{"location_type":"house"}
    - utter_thanks
    - utter_street
* street{"street":"123 Grove Street"}
    - slot{"street":"123 Grove Street"}
    - utter_thanks
    - utter_police
    - utter_ask_for_person
* person{"person":"Tom"}
    - slot{"person":"Tom"}
    - utter_console
* thanks
    - utter_welcome

## non emergency path police
* help
    - utter_emergency_service
* police
    - utter_areyouindanger
* deny
    - utter_ask_for_person
* person{"person":"Tom"}
    - slot{"person":"Tom"}
    - utter_thanks_person
    - utter_what_is_problem
* police_matter
    - utter_police_dispatch
* affirm
    - utter_location_type
* location_type{"location_type":"house"}
    - slot{"location_type":"house"}
    - utter_street
* street{"street":"123 Grove Street"}
    - slot{"street":"123 Grove Street"}
    - utter_thanks
    - utter_police_person
* thanks
    - utter_welcome

## chitchat_quit_police_noE
* help
    - utter_emergency_service
* police
    - utter_areyouindanger
* deny
    - utter_ask_for_person
* person{"person":"Tom"}
    - slot{"person":"Tom"}
    - utter_thanks_person
    - utter_what_is_problem
* ask_weather OR ask_builder OR ask_howdoing OR ask_languagesbot OR ask_howold OR ask_restaurant OR ask_time OR ask_wherefrom OR ask_whoami OR handleinsult OR telljoke OR ask_whatismyname OR marry_me OR compliment
    - action_chitchat
    - utter_what_is_problem
* ask_weather OR ask_builder OR ask_howdoing OR ask_languagesbot OR ask_howold OR ask_restaurant OR ask_time OR ask_wherefrom OR ask_whoami OR handleinsult OR telljoke OR ask_whatismyname OR marry_me OR compliment
    - utter_continue
* deny
    - utter_thanks
    - utter_goodbye

## emergency path fire
* help
    - utter_emergency_service
* fire
    - utter_areyouindanger
* affirm
    - utter_what_is_problem_danger
* fire_matter_danger
    - utter_thanks
    - utter_location_type
* location_type{"location_type":"house"}
    - slot{"location_type":"house"}
    - utter_thanks
    - utter_street
* street{"street":"123 Grove Street"}
    - slot{"street":"123 Grove Street"}
    - utter_thanks
    - utter_fire
    - utter_ask_for_person
* person{"person":"Tom"}
    - slot{"person":"Tom"}
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
* person{"person":"Tom"}
    - slot{"person":"Tom"}
    - utter_thanks_person
    - utter_what_is_problem
* fire_matter
    - utter_fire_dispatch
* affirm
    - utter_location_type
* location_type{"location_type":"house"}
    - slot{"location_type":"house"}
    - utter_street
* street{"street":"123 Grove Street"}
    - slot{"street":"123 Grove Street"}
    - utter_thanks
    - utter_fire_person
* thanks
    - utter_welcome

## emergency path ems
* help
    - utter_emergency_service
* ems
    - utter_areyouindanger
* affirm
    - utter_what_is_problem_danger
* ems_matter_danger
    - utter_thanks
    - utter_location_type
* location_type{"location_type":"house"}
    - slot{"location_type":"house"}
    - utter_street
* street{"street":"123 Grove Street"}
    - slot{"street":"123 Grove Street"}
    - utter_thanks
    - utter_ems
    - utter_ask_for_person
* person{"person":"Tom"}
    - slot{"person":"Tom"}
    - utter_console
* thanks
    - utter_welcome

## non emergency ems
* help
    - utter_emergency_service
* ems
    - utter_areyouindanger
* deny
    - utter_ask_for_person
* person{"person":"Tom"}
    - slot{"person":"Tom"}
    - utter_thanks_person
    - utter_what_is_problem
* ems_matter
    - utter_ems_dispatch
* affirm
    - utter_location_type
* location_type{"location_type":"house"}
    - slot{"location_type":"house"}
    - utter_street
* street{"street":"123 Grove Street"}
    - slot{"street":"123 Grove Street"}
    - utter_thanks
    - utter_ems_person
* thanks
    - utter_welcome

## New Story
* help
    - utter_emergency_service
* police
    - utter_areyouindanger
* affirm
    - utter_what_is_problem_danger
* police_matter_danger
    - utter_thanks
    - utter_location_type
* location_type
    - utter_thanks
    - utter_street
    - slot{"street":"123 Grove Street"}
* street{"street":"123 Grove Street"}
    - slot{"street":"123 Grove Street"}
    - utter_thanks
    - utter_police
    - utter_ask_for_person
* person{"person":"Kit"}
    - slot{"person":"Kit"}
    - utter_console
* thanks
    - utter_welcome

## New Story

* help
    - utter_emergency_service
* police
    - utter_areyouindanger
* affirm
    - utter_what_is_problem_danger
* police_matter_danger
    - utter_thanks
    - utter_location_type
* location_type{"location_type":"office"}
    - slot{"location_type":"office"}
    - utter_thanks
    - utter_street
* street{"street":"123 Grove Street"}
    - slot{"street":"123 Grove Street"}
    - utter_thanks
    - utter_police
    - utter_ask_for_person
* person{"person":"Kit"}
    - slot{"person":"Kit"}
    - utter_console
* thanks
    - utter_welcome
