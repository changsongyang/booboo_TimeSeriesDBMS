## 分类对比

目前阿里云的TSDB和TSDB for influxdb的主要区别是什么？

|          |                | Aliyun TSDB                          | Alien TSDB For  InfluxDB                                     |
| :------- | :------------- | :----------------------------------- | ------------------------------------------------------------ |
| 协议     |                | 协议与open TSDB一致                  | TSDB for influxdb是开源influx db在阿里云上的托管版本，结合阿里内部对于内存管理、连接控制等优化 |
| 运维管控 | 服务可用性     | 99.9%                                | 根据规格和场景提供最优的参数配置，提供完善的进程恢复机制以及全自动的ECS故障转移机制。<br/>另外，具备比开源版本InfluxDB更完善的内存管理机制，实现了全自动Load Shedding，从容应对瞬时冲击。<br/>具有磁盘即将写满的自动保护机制。<br/>还可以升级双（节点）写模式，将可用性再提高一个数量级（待上线）。 |
|          | 数据可靠性     | 99.9999%                             | 基于高效云盘的99.9999999%可靠性。                            |
| 功能     | 数据模型       | 同时支持多值模型和单值模型           | 同时支持多值模型和单值模型                                   |
|          | 数据类型多样性 | 支持数值，布尔，字符串等多种数据类型 | 支持数值，布尔，字符串等多种数据类型                         |
|          | SQL查询能力    | 支持SQL的分析查询                    | SQL的分析查询能力更强                                        |
| 生态     |                | 支持较弱                             | 结合TICK生态，可视化、采集都有开源的配套组件                 |

# 总结

* 阿里云的TSDB的协议与open TSDB一致；TSDB for influxdb是开源influx db在阿里云上的托管版本，结合阿里内部对于内存管理、连接控制等优化。

* TSDB for influxdb的SQL查询能力比较强，结合TICK生态，可视化、采集都有开源的配套组件。

