## Termux-QDL
Flash Qualcomm基于CPU的移动电话使用Termux''不带PC'or'（此工具仅在''arm'64''架构Termux支持的移动中运行）Root需要

##.安装 :- 

```Install``` [termux](https://f-droid.org/repo/com.termux_1021.apk)、[termux api](https://f-droid.org/repo/com.termux.api_1000.apk)、[ADBify](https://play.google.com/store/apps/details?id=com.rv882.adbify)
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
after Run this tool useg Details show in screen set your files location acording to useg details.

like this - ```sudo ./qdl --debug --storage emmc --include [flash file folder location] [prog_firhouse_xx.mbn file location] [rawprogram.xml file location] [patch.xml file location]```

不要在命令行上加上这个 ```[ ]``` .

./qdl --debug --storage emmc --include /storage/emulated/0/images /storage/emulated/0/images/prog_firhouse_lite.elf /storage/emulated/0/images/rawprogram*.xml /storage/emulated/0/images/patch*.xml 

 ./qdl --debug --storage ufs --include /storage/emulated/0/images /storage/emulated/0/images/prog_ufs_firhouse_sm8250_ddr_5.elf /storage/emulated/0/images/rawprogram*.xml /storage/emulated/0/images/patch*.xml


./qdl /storage/emulated/0/images/DevprgProgrammer2.elf /storage/emulated/0/images/rawprogram0.xml /storage/emulated/0/images/rawprogram1.xml /storage/emulated/0/images/rawprogram2.xml /storage/emulated/0/images/rawprogram3.xml /storage/emulated/0/images/rawprogram4.xml /storage/emulated/0/images/rawprogram5.xml /storage/emulated/0/images/patch0.xml /storage/emulated/0/images/patch1.xml /storage/emulated/0/images/patch2.xml /storage/emulated/0/images/patch3.xml /storage/emulated/0/images/patch4.xml /storage/emulated/0/images/patch5.xml

./qdl /storage/emulated/0/images/DevprgProgrammer2.elf /storage/emulated/0/images/rawprogram*.xml /storage/emulated/0/images/patch*.xml

after Set commands Connect Terget Device to 9008 edl mode using Otg & Data cable.
