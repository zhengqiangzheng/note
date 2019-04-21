#### 安装 ：

​	`pip install scrapy`

`	windows 要安装 pypiwin32` 

#### 创建 scrapy项目：

​	`scrapy startproject 项目名`

#### 创建自己的spider ：

​	`scapy genspider 爬虫名  爬取的网页`

​	`scrapy genspider demo zimuku.net`

#### 设置settings.py

1. 查找headers 设置请求头

2. ```python
   下面的设置为false
   # Obey robots.txt rules
   ROBOTSTXT_OBEY = False
   ```

#### 启动爬虫

`scrapy crawl 爬虫名字 name的值`

在pycharm中启动爬虫，创建一个启动类：

```python
from scrapy import cmdline
cmdline.execute('scrapy crawl qsbks'.split())
```





