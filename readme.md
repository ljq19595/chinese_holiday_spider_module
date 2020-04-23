# 国家节假日解析爬虫(crawler of chinese holiday)

可用于解析获取国家节假日公布页面的节假日安排。(It can be used to analyze and obtain the holiday arrangement of the chinese national holiday announcement page)

## 使用示例(demo)

```python
from holiday import get_holiday
from datetime import datetime

# 得到当前年节假日(get holiday of this year)
current_year_holiday = get_holiday(datetime.now().year)

```

返回该年所有节假日的时间戳(return every holiday of China this year, but not included weekend)：

```json

{"holiday": [1293811200, 1293897600, 1293984000, 1296576000, 1301760000, 1301846400, 1301932800, 1304092800, 1304179200, 1304265600, 1307116800, 1307203200, 1307289600, 1315584000, 1315670400, 1315756800, 1317398400, 1317484800, 1317571200, 1317657600, 1317744000, 1317830400, 1317916800]}
```

## 注意(attention)

建议作为每年执行的脚本调用，而非实时API。(It is recommended to call every year rather than in real time)

## 主要修改点(major modify)

1. python2 -> python3(python3.5)
2. 增加了一个写入json的例子，可以看一下，同时把采集到的json文件也上传了(demo for json file)

## fork from [chinese_holiday_spider_module](https://github.com/imlinhanchao/chinese_holiday_spider_module)

## English from Construction site
