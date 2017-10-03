学习hadoop中遇到的问题

## Error ##

WARN util.NativeCodeLoader: Unable to load native-hadoop library for your platform… 
using builtin-java classes where applicable

Solve the problem

用64位lib替换32位
```
wget http://dl.bintray.com/sequenceiq/sequenceiq-bin/hadoop-native-64-2.7.0.tar
解压到 hadoop-2.7.0/lib/native/
```
Link
[Unable to load native-hadoop library （已解决）](http://www.chinahadoop.cn/classroom/5/thread/43)


## Error ##

WARN net.DNS: Unable to determine address of the host-falling back to "localhost" address

Solve the problem

If /etc/hosts doesn't containt the definition of the hostname it fails. Just add your hostname to /etc/host for example 
if your hostname is work add or modified the following line:

echo $HOSTNAME

```
127.0.0.1   <your-hostname>        localhost
```
Link

[java.net.UnknownHostException](https://stackoverflow.com/questions/4969156/java-net-unknownhostexception)

