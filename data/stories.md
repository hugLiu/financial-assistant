## happy path
* greet
  - utter_greet

## say goodbye
* goodbye
  - utter_goodbye

## bot challenge
* bot_challenge
  - utter_iamabot

## request what fund
* greet
  - utter_greet
* request_fund_what
  - utter_what_is_fund

## fund buy advice
*greet
  - utter_greet
* request_buy_advice
  - utter_fund_advice
* thanks
  - utter_did_that_help
* deny
  - utter_goodbye

## request index info 1
* greet
  - utter_greet
* request_market_info{"index": "上证指数"}
  - action_index_search
* thanks
  - utter_did_that_help
* deny
  - utter_goodbye


