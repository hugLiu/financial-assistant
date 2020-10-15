## intent:greet
- hey
- hello
- hi
- 你好！
- 您好
- 机器人，你好
- 你好，机器人

## intent:goodbye
- bye
- 再见

## intent:affirm
- 是的
- 可以
- 嗯！！！
- 好的
- 行！

## intent:deny
- 不行
- 不！！！
- No
- 没有了

## intent:thanks
- 感谢
- 谢谢
- 非常感谢
- 好的，谢谢再见

## intent:bot_challenge
- 你是机器人还是人工客服？
- 你是机器人吗？
- 你是人工客服吗?

## intent:request_fund_what
- 什么是基金？
- 你好，请问什么是基金?
- 基金是什么？
- 基金

# intent: request_buy_advice
- 你好，请问购买那只基金好？
- 我应该买哪个基金？
- 有好的基金推荐吗？

## intent:request_market_info
- [上证指数](index)
- [上证综指](index)
- [519674](fundname)
- [上证50](index)
- [今天](date)[上证指数](index)是多少？
- [昨天](date)[上证指数](index)是多少？
- [上证50](index)多少？
- [今天](date)[中证500](index)指数是多少？
- [今天](date)[中证500](index)是多少
- [502056](fundname)[今天](date)涨多少？
- [银河创新成长混合](fundname)这只基金怎样？

## regex:fundname
- [0-9]{6}

## lookup:fundname
data/lookup_tables/fundname.txt

## lookup:index
data/lookup_tables/index.txt