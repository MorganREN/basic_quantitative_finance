# 量化策略与分析

## Tushare-金融数据接口包

- Tushare是一个免费的、开源的python财经数据接口包

- 网址：http://tushare.org/index.html

- 安装tushare，注册pro用户

- 获取token，导入tushare然后设置token，再初始化pro接口
    - import tushare as ts
    - ts.set_token('your token here')
    - pro = ts.pro_api() *or* pro = ts.pro_api('your token')[如果上一步骤ts.set_token('your token')无效或不想保存token到本地，也可以在初始化接口里直接设置token]