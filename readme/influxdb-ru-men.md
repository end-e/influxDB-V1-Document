# influxDB 入门

在本节中，我们将使用influx命令行界面（CLI），它包含在所有InfluxDB包中，并且是一种轻量级且简单的方法来与数据库交互。 CLI通过默认情况下在端口8086上向InfluxDB API发送请求直接与InfluxDB通信。

### 创建数据库

如果您已本地安装InfluxDB，则可以通过命令行访问influx命令。 执行influx将启动CLI并自动连接到本地InfluxDB实例（假设您已经通过service influxdb start或直接运行influxd启动了服务器）。 输出应如下所示：

```
influx -precision rfc3339
```

`-precision` 参数指定返回的时间戳的格式/精度。 在上面的例子中，rfc3339告诉InfluxDB以RFC3339格式（YYYY-MM-DDTHH：MM：SS.nnnnnnnnZ）返回时间戳。
