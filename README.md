## Termux-QDL
使用 Termux 为基于高通 CPU 的手机刷机Without PC （此工具仅适用于arm64支持 Termux 的手机架构），需要 Root 权限.

##.安装 :- 

```下载安装``` [termux](https://f-droid.org/repo/com.termux_1021.apk)、[termux api](https://f-droid.org/repo/com.termux.api_1000.apk)&[ADBify](https://play.google.com/store/apps/details?id=com.rv882.adbify)
```apk```
```console
pkg update && pkg upgrade -y
```
```console
pkg install -y termux-api
```
```console
pkg install -y git
```
```console
pkg install -y libxml2
```
```console
pkg install -y sudo
```
```console
git clone https://github.com/pcnjyz/Termux-QDL.git
```
```console
cd Termux-QDL
```
```console
chmod +x qdl
```

## 运行工具
```console
./qdl
```


## 注意 :-
运行此工具后，屏幕上会显示使用详情，请根据使用详情设置文件位置。

像这样 - ```sudo ./qdl --debug --storage emmc --include [flash file folder location] [prog_firhouse_xx.mbn file location] [rawprogram.xml file location] [patch.xml file location]```

[ ]请勿在命令行中添加此项.

./qdl --debug --storage emmc --include /storage/emulated/0/images /storage/emulated/0/images/prog_firhouse_lite.elf /storage/emulated/0/images/rawprogram*.xml /storage/emulated/0/images/patch*.xml 

##下列样式

 ./qdl --debug --storage ufs --include /storage/emulated/0/images /storage/emulated/0/images/prog_ufs_firhouse_sm8250_ddr_5.elf /storage/emulated/0/images/rawprogram*.xml /storage/emulated/0/images/patch*.xml

./qdl /storage/emulated/0/images/DevprgProgrammer2.elf /storage/emulated/0/images/rawprogram0.xml /storage/emulated/0/images/rawprogram1.xml /storage/emulated/0/images/rawprogram2.xml /storage/emulated/0/images/rawprogram3.xml /storage/emulated/0/images/rawprogram4.xml /storage/emulated/0/images/rawprogram5.xml /storage/emulated/0/images/patch0.xml /storage/emulated/0/images/patch1.xml /storage/emulated/0/images/patch2.xml /storage/emulated/0/images/patch3.xml /storage/emulated/0/images/patch4.xml /storage/emulated/0/images/patch5.xml

./qdl /storage/emulated/0/images/DevprgProgrammer2.elf /storage/emulated/0/images/rawprogram*.xml /storage/emulated/0/images/patch*.xml

设置命令后，使用 OTG 和数据线将目标设备连接到 9008 edl 模式。
