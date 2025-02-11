# 1.准备工作
手机下载并安装kernelSU管理器：https://github.com/tiann/KernelSU/releases

手机下载并安装devcheck或底层探测器查看当前系统位于A/B分区的哪个分区：https://github.com/imknown/AndroidLowLevelDetector/releases

电脑下载搞机助手：https://lsdy.top/gjzs

电脑下载当前的系统镜像备份boot.img https://xiaomirom.com/

# 2.下载机型对应的boot.img文件
## 在设置-全部参数与信息中查看内核版本，其格式如下

``````
Version.PatchLevel.SubLevel-AndroidRelease-KmiGeneration-suffix
w      .x         .y       -zzz           -k            -something
``````
需要w.x.*-zzz相同，KernelSU的releases中的格式为zzz-w.x.*即AndroidRelease-Version.PatchLevel.SubLevel

## releases文件格式的选择

| boot-gz.img.gz | boot-lz4.img.gz | boot.img.gz |
|----------------|-----------------|-------------|
| gz压缩格式     | lz4压缩格式     | 无压缩      |

骁龙soc一般为无压缩的格式，所以选择后缀为boot.img.gz的文件

天玑soc一般为gz的格式，所以选择后缀为boot-gz.img.gz的文件

下载完成后解压获得img文件
# 3.刷入boot.img文件
手机关机后长按电源键和音量和音量下键，进入fastboot模式

在搞机助手中点击引导模式-A/B分区设备输入Boot

连接手机，等显示连接后，选择第一步查看到的当前系统分区，选择第二部下载并解压的img文件，刷入等待完成开机即可



