## happy path
* greet
  - utter_greet

## say goodbye
* goodbye
  - utter_goodbye

## bot challenge
* bot_challenge
  - utter_iamabot

## story 1 <!-- 询问什么基金 -->
* greet
  - utter_greet
* concept_explain
  - action_concept_explain

## story 2  <!-- 询问购买建议 -->
*greet
  - utter_greet
* trade_advice
  - utter_fund_advice
* thanks
  - utter_did_that_help
* deny
  - utter_goodbye

## story 3   <!-- 请求指数多少点 -->
* greet
  - utter_greet
* market_info{"index": "上证指数"}
  - action_index_search
* thanks
  - utter_did_that_help
* deny
  - utter_goodbye

## story 4   <!-- 询问手续费 -->
* greet
  - utter_greet
* fee_rule{"fee": "手续费"}
  - action_fee_search
* thanks
  - utter_did_that_help
* deny
  - utter_goodbye
