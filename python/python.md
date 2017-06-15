

# Selenium
* `自动化测试工具，支持多种浏览器，爬虫中主要用来解决JavaScript渲染的问题。`


# Flask+Redis 维护代理池
* `为什么要用代理池：许多网站有专门的饭爬虫措施，可能遇到封IP等问题；互联网上公开了大量免费代理，利用好资源；通过定时的检测维护同样可以得到多个可用代理`
* `代理池要求：多站抓取，异步检测；定时筛选，持续更新；提供接口，易于获取`


# Scrapy
* `scrapy startproject 项目名` 创建项目
* `scrapy genspider mydomain mydomin.com` 生成spider
* `scrapy genspider -t crawl mydomain mydomin.com` 根据指定模板生成spider
* `scrapy crawl 爬虫名 -o 文件名(a.json / a.jl /a.csv /a.xml /.... (或ftp保存：ftp://...))`
* `项目名 tree` 查看项目目录结构
* `scrapy:` [官方传送门](https://doc.scrapy.org/en/latest/topics/commands.html) [中文传送门](http://scrapy-chs.readthedocs.io/zh_CN/latest/topics/spiders.html)

# Redis
* 多台主机协作的关键：共享爬取队列  （分布式爬虫）
* Redis队列：Redis,非关系型数据库，key-value形式存储，结构灵活；是内存中的数据结构存储系统，处理速度快，性能好；提供队列、集合等多种存储结构，方便队列维护
* Redis提供集合数据结构，在Redis集合中存储每个Request的指纹；在向Request队列中加入Request前首先验证这个Request的指纹是否已经加入集合中，如果已存在，则不添加Request到队列，如果不存在，则将Request添加入队列并将指纹加入集合
* [Scrapy-Redis](https://github.com/rolando/scrapy-redis)实现了如上架构，改写了Scrapy的调度器，队列等组件。利用它可以方便地实现Scrapy分布式架构
* scrapyd 分布式远程部署
