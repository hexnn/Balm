# Balm（万金油-大数据PAAS组件适配器）
## 基于Spring Boot打造，一键集成各种常用的大数据PAAS组件，简化对接成本，提升应用开发效率，让业务实现更聚焦
* [DolphinScheduler](https://github.com/apache/dolphinscheduler)（1.3.x）
* [Hadoop](https://github.com/apache/hadoop)（2.x/3.x）
* [Spark](https://github.com/apache/spark)（2.x/3.x）
* [Hive](https://github.com/apache/hive)（2.x/3.x）
* Impala（敬请期待）
* [HBase](https://github.com/apache/hbase)（1.x/2.x）
* Kafka（2024.05即将上线）
* Doris（敬请期待）
* StarRocks（敬请期待）
* ClickHouse（敬请期待）
* Presto（敬请期待）
* DataX（敬请期待）
* Neo4j（敬请期待）
* Redis（敬请期待）
* ElasticSearch（敬请期待）
* MinIO（敬请期待）
* Aliyun OSS（敬请期待）
* Aliyun ODPS/MaxCompute（敬请期待）
* More+

## 提供标准的RESTFul操作接口，基于标准的SQL语句屏蔽底层架构差异性，让数据的读/写更简单，业务开发如搭积木般丝滑
### DolphinScheudler（分布式任务调度引擎）
* 环境自检相关接口
  + DolphinScheduler组件运行环境自检
* 任务管理相关接口
  + 任务创建
  + 任务列表查询
  + 任务详情查询
  + 任务更新
  + 任务删除
* 任务运行相关接口
  + 任务单次执行
  + 任务单步执行
  + 任务调度执行
  + 任务暂停
  + 任务恢复
  + 任务停止
  + 任务执行状态查询
  + 作业执行状态查询
  + 任务执行批次查询
  + 任务执行队列信息查询
* 任务执行历史相关接口
  + 任务执行历史列表查询
  + 作业执行历史列表查询
  + 任务执行历史日志查询
* 任务执行统计相关接口
  + 任务执行耗时评估
  + 作业执行耗时评估
* 资源管理相关接口
  + 资源文件注册
  + 资源文件下载
  + 资源列表查询
  + 资源文件删除
### Hadoop（HDFS分布式文件系统 + YARN资源调度）
* 环境自检相关接口
  + Hadoop组件运行环境自检
* HDFS文件系统相关接口
  + HDFS磁盘监测
  + HDFS路径检测
  + HDFS文件类型检测
  + 创建HDFS目录
  + 拷贝HDFS目录或文件
  + 移动HDFS目录或文件
  + 删除HDFS目录或文件
  + 获取HDFS文件列表
  + 下载HDFS目录或文件
  + 创建HDFS文件
  + 压缩HDFS文件
  + 解压HDFS文件
* YARN资源调度相关接口
  + 获取yarn队列信息
  + 获取yarn任务执行列表
  + 设置yarn任务执行优先级
  + yarn队列自动分配
  + 停止yarn任务
### Hive（数据仓库）
* 环境自检相关接口
  + Hive组件运行环境自检
* 数仓操作相关接口
  + Hive数仓表探查
  + Hive表元数据探查
  + Hive表数据导入
  + Hive表数据下载
  + Hive表数据随机抽样
### Spark（大数据计算引擎）
* 环境自检相关接口
  + Spark组件运行环境自检
* Spark 操作相关接口
  + SparkSQL语法检测
  + SparkSQL语句执行
  + SparkSQL语句批量执行
  + SparkSQL自定义数据分析
### HBase（列式存储数据库）
* 环境自检相关接口
  + HBase组件运行环境自检
* 数仓操作相关接口
  + HBase数仓表探查
  + HBase表元数据探查
  + HBase表数据导入
  + HBase表数据下载
  + HBase表数据随机抽样

## 快速部署
* 点击下载最新版[balm-2024.04.08.jar](https://github.com/hexnn/balm/releases/download/balm-2024.04.08/balm-2024.04.08.jar)
* 修改application.yml文件spring.profiles.include参数，按需启用组件
* 根据需要对接组件的实际部署情况，按需修改application-xxx.yml相关配置参数
* 上传服务器，一键启动服务：nohup java -jar balm-2024.04.08.jar > balm.log 2>&1 &
* Swagger-ui地址：http://$host:11011/balm

## 问题反馈
* 详细部署手册、接口使用文档、二次开发指南请联系↓↓↓
* WeChat：xxx-hx-xxx（潇湘夜雨）
* Email：hexing_xx@163.com
* 欢迎通过[Issues](https://github.com/hexnn/balm/issues)或以上联系方式提交使用问题或者建议
