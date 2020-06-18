# SFTP远程服务器地址改变报错及解决方案

由于Dmartech系统进行了服务器迁移，在使用linux或者mac链接sftp的时候可能会报错如下：

WARNING: POSSIBLE DNS SPOOFING DETECTED!

该问题是由于远程服务器地址改变所导致的。

### 解决方案：\(适用于Linux 或者 OSX，windows系统暂时未发现此问题\)

  
**Mac系统中：在Finder菜单中找到【前往】：【前往文件夹】，然后输入地址： ~/.ssh/known\_hosts**

**Linux系统中：通过命令行 cd ~/.ssh/**

**然后编辑 known\_hosts，删除其中包含data-sftp.dmartech.cn的行并保存。**

如仍无法解决问题，请通过在线客服联系我们。感谢理解和配合！





