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

## intent: bonus_history    <!--分红记录-->
- 这只基金的有[分红]()吗
- 基金的[分红]()记录

## intent: bonus_rule      <!--分红规则-->
- 为什么该[基金]()不[分红]()？
- [分红]是分自己的本金吗?


# intent: fee_rule          <!--手续费规则-->
- 问一下[超级转换]()有[手续费]()吗？

 
# intent: trade_rule    <!--交易规则-->
- 昨天15点之前卖的，今天[涨跌]()和我有关系吗？
- [今天](date)买点，计算当天的收益吗
- [周六，日](date)有收益吗？[节假日](date)哪？

# intent: trade_advice    <!--交易建议-->
- 今天可以[上车]()吗？
- 你好，请问[购买]()哪只[基金]()好？
- 我应该[买]()哪个[基金]()？
- 有好的[基金]()推荐吗？


# intent: regular_purchase_rule  <!-- 定投规则 -->
- 现在是不是[基金定投]()[卖出]()的好时机？还会继续[涨]()吗
- 现在这个点可以开始[定投]()吗？



# intent: regular_purchase_fund  <!-- 定投品种 -->
- 推荐几个[定投]()的[基金]()呗？

## intent: order_fail
- 买入，卖出失败
- 交易执行超时关单，这是什么意思？

## intent: search_buy_rule
- 为什么还是不能买？
- 我就想问什么时候才能买？
- 不能加仓，玩锤子
- 快开门，我要把A里的血输进来

## intent: search_sell_rule
- 啥时候能卖呢？
- 可以卖吗？

## intent: current_info
- 到站下车
- 今天下车了
- 今天不应该跌吗？