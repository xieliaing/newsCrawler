# newsCrawler

这是利用下面这个博客的内容改造的使用scrapy抓取网易财经网页的python程序:

http://youngfor.me/post/spider/yong-scrapypa-wang-yi-xin-wen-jian-yi-jiao-cheng


# 主要改进有

- 1. 可以定制抓取某一天的网页
- 2. 抓取项目作为字典输出到单个文本文件，而不是输出到MongoDB，这样更简单
- 3. 一些旧的代码不适应新scrapy版本的地方进行的修改，不一一列出。
- 4. 将股票代码和新闻页码作为参数，可以灵活控制抓取内容

# 使用方法：
- 在..\newsCrawler\ 根目录下执行如下DOS命令：
--  ..\newsCrawler>scrapy crawl stocknews -a id='600000' -a page='02'

- 在..\newsCrawler\ 根目录下执行如下DOS命令来调用Python脚本执行抓取所有股票对应的历史新闻：
--  ..\newsCrawler>python PythonRun.py 

 
