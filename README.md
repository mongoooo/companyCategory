# companyCategory
根据企业名称对企业类型进行分类

## 基本描述
主要需求是根据企业名字对企业进行分类。最开始的一个Idea，就是通过爬虫和机器学习进行结合。

## 主要实现方式
* 输入企业名字
* 系统带着企业名字去天眼查查看企业的主要经营范围
* 根据企业经营范围，通过多项式朴素贝叶斯算法实现分类
* 返回分类结果
## 在使用之前需要进行
* 建立Sample文件夹，并且在文件里面建立若干分类文件夹
* 在若干分类的文件夹中（Sample的子文件夹）建立如果txt文档，并写入该分类的train内容
* 为了保证效果，尽量保证每个分类中的train的内容个数一致

* 注意：自行在相关地方修改代理ip的接口

## 运行结果
test_run.py运行结果：
Loading model from cache /var/folders/c2/gknx155x20n18hp4njybsr7r0000gn/T/jieba.cache
Loading model cost 0.944 seconds.
Prefix dict has been built succesfully.
中国移动通信集团四川有限公司 Counter({'信息传输、软件和信息技术服务业': 4, '电力、热力、燃气及水生产和供应业': 1, '水利、环境和公共设施管理业': 1, '文化、体育和娱乐业': 1})
吉林市群龙科技有限公司 Counter({'信息传输、软件和信息技术服务业': 1})
北京大成律师事务所武汉分所 无法分类
大连万达集团商业管理有限公司 Counter({'房地产业': 2, '住宿和餐饮业': 1, '建筑业': 1, '农、林、牧、渔业': 1})
腾冲恒益矿产实业有限公司 Counter({'交通运输、仓储和邮政业': 2, '采矿业': 2, '住宿和餐饮业': 1})
四川智博联想物流有限公司 Counter({'交通运输、仓储和邮政业': 1, '水利、环境和公共设施管理业': 1})
北京百度网讯科技有限公司 Counter({'金融业': 4, '信息传输、软件和信息技术服务业': 3, '文化、体育和娱乐业': 3, '居民服务、修理和其他服务业': 2, '交通运输、仓储和邮政业': 2, '科学研究和技术服务业': 2, '教育': 1, '卫生和社会工作': 1, '租赁和商务服务业': 1})
北京摩拜科技有限公司 Counter({'信息传输、软件和信息技术服务业': 6, '金融业': 5, '文化、体育和娱乐业': 4, '房地产业': 1, '科学研究和技术服务业': 1, '居民服务、修理和其他服务业': 1, '租赁和商务服务业': 1, '教育': 1, '采矿业': 1})
天津一汽丰田汽车有限公司 Counter({'信息传输、软件和信息技术服务业': 1, '科学研究和技术服务业': 1})

## More
如果您在使用的过程中有任何疑问，请与我取得联系：service@52exe.cn
