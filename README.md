# OptiPlex - 7060 & 7070 - Catalina


Tested on：

> * OptiPlex 7060 
> * OptiPlex 7070 

You need to run

` setup_var 0x8dc 0x2 `

in Grub to update DVMT settings first and after everytime you reset your bios.

请在放置EFI前在Grub中修改DVMT设置。默认8Bit的显存容量不足以引导系统启动。

**This command works FOR 7060 and 7070 ONLY!**

此命令仅对7060和7070有效，在其他电脑上运行可能会损坏BIOS。

**Use this on other model may damage your computer!**


DW1560/1830 tested.

FileVault加密不可打开，开启会导致无法启动。此配置不能创建Wi-Fi诊断报告。

**NEVER** enable FileVault on a hackintosh. 

Wi-Fi Diagnostic Report can not be generated.
