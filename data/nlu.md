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
- 什么是[基金]{"entity": "security", "value": "fund"}？
- 你好，请问什么是[基金]{"entity": "security", "value": "fund"}?
- [基金]{"entity": "security", "value": "fund"}是什么？
- [基金]{"entity": "security", "value": "fund"}

## intent:market_info
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
- [银河创新成长混合](fundname)这只[基金]{"entity": "security", "value": "fund"}怎样？

## intent: bonus_history    <!--分红记录-->
- 这只[基金]{"entity": "security", "value": "fund"}的有[分红](bonus)吗
- 查询[基金]{"entity": "security", "value": "fund"}的[分红](bonus)记录
- [基金]{"entity": "security", "value": "fund"}的[分红](bonus)历史

## intent: bonus_rule      <!--分红规则-->
- 为什么该[基金]{"entity": "security", "value": "fund"}不[分红](bonus)？
- [分红](bonus)是分自己的本金吗?


# intent: fee_rule          <!--手续费规则-->
- 问一下[超级转换](super_convert)有[手续费](fee)吗？
- 这只基金的[手续费](fee)是怎样


# intent: trade_rule    <!--交易规则-->
- 昨天15点之前[卖]{"entity": "trade", "value": "sell"}的，今天涨跌和我有关系吗？
- [今天](date)[买]{"entity": "trade", "value": "sell"}点，计算当天的收益吗
- [周六，日](date)有收益吗？[节假日](date)哪？
- 为什么还是不能[买]{"entity": "trade", "value": "buy"}？
- 我就想问什么时候才能[买]{"entity": "trade", "value": "buy"}？
- 啥时候能[卖]{"entity": "trade", "value": "sell"}呢？
- 可以[卖]{"entity": "trade", "value": "sell"}吗？


# intent: trade_advice    <!--交易建议-->
- 今天可以[上车]{"entity": "trade", "value": "buy"}吗？
- 你好，请问[购买]{"entity": "trade", "value": "buy"}哪只[基金]{"entity": "security", "value": "fund"}好？
- 我应该[买]{"entity": "trade", "value": "buy"}哪个[基金]{"entity": "security", "value": "fund"}？
- 有好的[基金]{"entity": "security", "value": "fund"}推荐吗？
- 还会继续涨吗
- 现在是不是基金定投[卖出]{"entity": "trade", "value": "sell"}的好时机？
- 现在这个点可以开始定投吗？
- 推荐[基金]{"entity": "security", "value": "fund"}
- 推荐几个定投的[基金]{"entity": "security", "value": "fund"}呗？



## intent: order_fail
- [买入]{"entity": "trade", "value": "buy"}，[卖出]{"entity": "trade", "value": "sell"}失败
- 交易执行超时关单，这是什么意思？

# intent: complain  <!-- 抱怨 -->
- 今天不应该跌吗？
- 不能[加仓]{"entity": "trade", "value": "buy"}，玩锤子


## regex:fundname
- [0-9]{6}

## lookup:fundname
data/lookup_tables/fundname.txt

## lookup:index
data/lookup_tables/index.txt

