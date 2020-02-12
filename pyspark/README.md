## 使用说明

### 启动

1. 启动虚拟机

    ```shell script
    vagrant up
    ```

2. 配置master能登录所有node，以及master本身

3. 初始化hadoop

    ```shell script
    hdfs namenode -format
    
    $HADOOP_HOME/sbin/start-dfs.sh
    
    hdfs dfs -mkdir -p /user/spark
    ```

3. 启动spark
   
    ```shell script
    start-all.sh
    ```

### 测试

1. hadoop UI port: `50070`
2. spark UI port: `8080`
3. 均在master主机上
