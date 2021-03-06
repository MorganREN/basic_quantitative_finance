# 量化策略与分析

## Tushare-金融数据接口包

- Tushare是一个免费的、开源的python财经数据接口包

- 网址：http://tushare.org/index.html

- 安装tushare，注册pro用户

- 获取token，导入tushare然后设置token，再初始化pro接口
    - import tushare as ts
    - ts.set_token('your token here')
    - pro = ts.pro_api() *or* pro = ts.pro_api('your token')[如果上一步骤ts.set_token('your token')无效或不想保存token到本地，也可以在初始化接口里直接设置token]
    
### 练习1-股票数据分析
- 使用tushare包获取某股票的历史行情数据

- 输出该股票所有收盘比开盘上涨3%以上的日期

- 输出该股票所有开盘比前日收盘跌幅超过2%的日期

- 加入我从2020年11月开始，每月第一个交易日买入1手股票，每年最后一个交易日卖出所有股票，到今天为止，我的收益如何？

### 练习2-查找历史金叉死叉日期
- 均线：对于每一个交易日，都可以计算出前N天的移动平均值，然后把这些移动平均值连起来，成为一条线，就叫做N日移动平均线。移动平均线常用线有5天、10天、30天、60天、120天和240天的指标
    - 5天和10天的是短线操作的参考指标，称作日均线指标
    
    - 30天和60天的是中期均线指标，称作季均线指标
    
    - 120天和240天的是长期均线指标，称作年均线指标
    
- 金叉：短期均线上穿长期均线，买入信号

- 死叉：短期均线下穿长期均线，卖出信号

#### 任务：
- 使用tushare包过去某股票的历史行情数据

- 使用pandas包计算该股票历史数据的5日均线和30日均线

- 使用matplotlib包可视化历史数据的收盘价和两条均线

- 分析输出所有金叉日期和死叉日期

- 如果我从2012年1月1日开始，初始资金为100000元，金叉尽量买入，死叉全部卖出，则到今天为止，我的炒股收益率如何？



















