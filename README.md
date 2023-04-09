# `Windows 10 LSTC 2021`安装指引

## 下载

- [x] [edk2下载地址](ed2k://|file|SW_DVD9_WIN_ENT_LTSC_2021_64BIT_ChnSimp_MLF_X22-84402.ISO|5044211712|1555B7DCA052B5958EE68DB58A42408D|/)
- [x] [MSDN I tell you](https://next.itellyou.cn/)

## 安装和激活系统  
1. `win+R`来打开`cmd`（管理员身份运行） 

2. 运行以下激活代码（需要依次逐行回车运行，不能一次性全部拷贝执行） 
    ```cmd
    slmgr -upk
    slmgr -ipk M7XTQ-FN8P6-TTKYV-9D4CC-J462D
    slmgr -skms kms.03k.org
    slmgr -ato
    slmgr -dlv
    ``` 

3. 若密钥提示无效，请在[py-kms](https://py-kms.readthedocs.io/en/latest/Keys.html)查找对应版本

## 安装`Microsoft Store`
1. 打开网站 [store.rg-adguard.net](https://store.rg-adguard.net/) 
2. 搜索栏中输入`Microsoft Store`的应用链接，也即`https://apps.microsoft.com/store/detail/microsoft-store/9WZDNCRFJBMP` 
3. 点击右侧按钮，会列示`Microsoft Store`及依赖库的安装包，根据操作系统版本下载即可（如点击无反应，可复制链接到迅雷下载，链接具备有效期，访问被拒绝时需要重新生成），扩展名为`appx`或`msixbundle` 
4. 将所下载的文件置于同一目录下并全部安装，执行`Add-AppxPackage *` 
5. 此外，如果希望`msixbundle`能够双击安装，还需要安装 [App Installer](https://apps.microsoft.com/store/detail/app-installer/9NBLGGH4NNS1?hl=en-us)
