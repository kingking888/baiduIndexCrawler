# 百度指数（百度热搜）爬虫
两种方式爬取百度指数：
百度指数爬虫，两种模式运行。周期性爬取（输入日期>0或<31月最后几天拿不准可以用-1）或一次性爬取（输入日期周期）

## auto_run.py（要配置每天运行，自行用schedual模块实现或者用系统的任务计划实现）
每天读取setting.py中的download_days里的日期并判断是否为爬取日期，一个一个时间段地爬取数据。

## run_by_hand
读取setting.py中run_date的开始结束日期，手动一次性爬取数据。
