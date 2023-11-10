# influxDB-V1-Document

## 安装

#### 安装要求 <a href="#an-zhuang-yao-qiu" id="an-zhuang-yao-qiu"></a>

需要`root`用户权限进行安装。

**使用的端口**

* TCP 端口 8086 可用于使用 influxDB API 进行客户端与服务端的通信。
* TCP 端口 8080 可供 RPC 服务执行备份和恢复操作。

**网络时间协议**

InfluxDB 使用主机的本地时间（UTC）为数据分配时间戳。 使用网络时间协议（NTP）在主机之间同步时间；如果主机的时钟与 NTP 不同步，则写入 InfluxDB 的数据的时间戳可能会不准确。

#### 安装 <a href="#an-zhuang" id="an-zhuang"></a>

**Ubuntu & Debian**

安装并启动 InfluxDB 服务。sudo apt-get update && sudo apt-get install influxdbsudo service influxdb start如果系统是 Ubuntu 15.04+, Debian 8+sudo apt-get update && sudo apt-get install influxdbsudo systemctl unmask influxdb.servicesudo systemctl start influxdb
