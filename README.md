
# 图片采集工具
## initDb.pl - 数据存数据库
 数据存储在以下表内
 - t_category：目录信息
 - t_subject：帖子信息
 - t_image：图片名，url
 - t_download: 图片内容信息

##fectchxx.pl - 数据存yaml文件里
本脚本主要用于抓取图片，网站, 本程序用多个线程来抓取，本地建立
md5样本库，用于去掉重复图片，由于无法在服务器端获取md5值，目前采取下载到本地然后在
本地库内遍历，看是否已存在，若是，即删除之。

可以使用 Control + c 来停止脚本