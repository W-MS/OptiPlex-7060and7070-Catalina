# OptiPlex - 7060 & 7070 - Catalina


Tested on：

> * OptiPlex 7060 
> * OptiPlex 7070 

<br/><br/>
You need to run

` setup_var 0x8dc 0x2 `

in Grub to update DVMT settings first and after everytime you reset your bios.

请在放置EFI前在Grub中修改DVMT设置。默认8Bit的显存容量不足以引导系统启动。

CFG Lock 

`setup_var 0x5BE 0x0 `


**This command works FOR 7060 and 7070 ONLY!**

此命令仅对7060和7070有效，在其他电脑上运行可能会损坏BIOS。


如果运行后无效，建议通过Dell PFS Extract工具提取一下BIOS(用EXE升级程序包)，再用UEFI Tool找到包含DVMT字段PE32镜像，导出并使用Universal IFR extractor解码出txt自行就能看到地址。

You could use Dell PFS Extract to dump your bios from exe updater, then run UEFI Tool in order to find the PE32 image contains DVMT in BIOS.bin so you could use Universal IFR extractor to extract the body of the setup information.

**Use this on other model may damage your computer!**

<br/><br/>

Replace intel ac9560 to DW1560/1830 if you need to use wireless function. Or you can just disable it in BIOS settings.

如需使用无线，需要把内置intel AC9560网卡换成DW1560或DW1830.鉴于这两张卡现在非常贵，如果你不用无线，在BIOS里面关闭无线功能就行。



<br/>
<br/>

FileVault加密不可打开，开启会导致无法启动。

**NEVER** enable FileVault on a hackintosh. 




**其他机型 黑苹果Hackintosh资源 [请访问链接](https://github.com/daliansky/Hackintosh)**

