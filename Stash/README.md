# TikTok 解锁  + 换区 + 发布视频 + 直播 + 点赞评论

*感谢 [Semporia](https://github.com/Semporia/TikTok-Unlock)、[Fei](https://github.com/Infatuation-Fei/rule/tree/main/Stash/Rewrite/TikTokUnlock)、[jnlaoshu](https://github.com/jnlaoshu/MySelf/tree/main/Stash/Script/TikTokUnlock)的无私分享

> 目录

* [TikTok](#TikTok)
* [操作步骤](#操作步骤)
* [抓包降级](#抓包降级)
* [抖音無法觀看](#抖音)

---

### <a id="TikTok"> TikTok </a>

* iOS系统版本：15.5 （支持向下兼容）
* TikTok版本：v24.1.0（需要从抓包的21.1.0升级方可使用）
* TikTok TestFlight (支持)
* 下载方式：在 美区/日区/台区 App Store搜索 TikTok 并下载 （港区已停止运营）

---

### 关于换区

* 解锁并换区：将`CN`改为想看的国家/地区的2位`大写`英文简写，

    * 在`HTTP复写`中，将`CN`的替换值改为`SG`、`MO`、`TW`等即可换区

---
### 特别说明

1、为什么要先卸载TikTok，TikTok会在第一次使用时触发限制，并导致之后无法通过MiMt解密  
2、所以先配置好规则之后，然后在下载TikTok，减少重定向的请求次数，降低风险，延长规则的寿命  
3、为什么配置好之后还是无法使用，请检查软件的证书有没有安装，信任，  
4、或者是Https解密（MiMt）与重写（Rewrite）有没有开启  
5、或者是软件是不是盗版，比如用共享ID下载的Quantumult X，有设备限制，是无法使用重写脚本功能的  

---

### <a id="操作步骤"> 操作步骤 </a>

1、打开`Stash`  

2、点击`覆写`进去添加想看国家的对应模块。

**日本**
```
https://raw.githubusercontent.com/MinghaoChow/TikTok-Unlock/master/Stash/TikTok-JP.stoverride
```

**台湾**
```
https://raw.githubusercontent.com/MinghaoChow/TikTok-Unlock/master/Stash/TikTok-TW.stoverride
```

**韩国**
```
https://raw.githubusercontent.com/MinghaoChow/TikTok-Unlock/master/Stash/TikTok-KR.stoverride
```

**美国**
```
https://raw.githubusercontent.com/MinghaoChow/TikTok-Unlock/master/Stash/TikTok-US.stoverride
```

3、添加以下`分流`

```
https://raw.githubusercontent.com/MinghaoChow/TikTok-Unlock/master/Stash/TikTok.list
```
---

### <a id="抓包降级"> 抓包降级 TikTok 21.1.0 </a>
**支持系统**  
* windows 11/windows 10/windows 8/windows 7（由于使用了 Fiddler 库，所以需要.Net 环境）

**使用方法**  

**一、直接搜索方式**
* 搜索 APP，双击选择。  
* 双击选择要下载的版本。  
* 在 iTunes 中下载即可。  
![Image text](https://raw.githubusercontent.com/Semporia/TikTok-Unlock/master/iOS抓包/1.png)
![Image text](https://raw.githubusercontent.com/Semporia/TikTok-Unlock/master/iOS抓包/2.png)
![Image text](https://raw.githubusercontent.com/Semporia/TikTok-Unlock/master/iOS抓包/3.png)

**二、复制 APP 链接方式**
* 在 iTunes 下载按钮右侧下拉菜单中，选择【复制链接】。  
* 双击选择要下载的版本。  
* 在 iTunes 中下载即可。  

**常见问题**

**问：iTunes 账号无法登录成功**
* 请先关闭本工具，再进行 iTunes 登录操作。  
* 登录成功后，再打开本工具即可。  

**问：iTunes 对电脑进行授权时，授权不了，反复授权**
* 关闭本工具，再进行授权即可。  

**问：搜不到 APP 历史版本号？（以下方法 100%可解决）**
* 先不要拦截，在 iTunes 商店中下载此软件，等待下载完成。  
* 在本工具中【安装管理】下找到对应 IPA 安装包，右键选择【查找版本 ID】。  
* 即可列出软件所有历史版本 ID，版本号按新版到旧版排序。  
* PS：暂时没有通过版本 ID，查版本号的接口，所以抓下来，看吧。  

**问：iTunes 一直显示正在下载...**
* iTunes 先取消下载。  
* 抓包工具【停止拦截】，再点击 iTunes【继续下载】。  

**问：下载完 APP，安装到手机，打开闪退。**
* 先在手机中卸载该 APP。  
* 使用下载此 App 的账号，登录 App Store，在 App Store 中随便下载一个应用，不要卸载。  
* 使用同步助手，重新安装。（如果仍闪退，尝试覆盖安装）  

**问：导入伪旧版 App 后，iTunes 未检测到更新。**
* iTunes 更新列表页面下，按 F5 即可。  
* 如上述方法未解决，删除当列表所有文件，保留文件，再点击右下角检测更新按钮。  

**问：“已停止供货”的 APP 怎么抓取？（已失效）**
* 取消拦截，下载该软件最新版。  
* 本助手里切换到【安装管理】，右键 APP，选择【伪装旧版 APP】。  
* 双击【\*\_伪装版.ipa】（或右键，在文件夹中打开），将 APP 拖动到 iTunes 资料库，替换，检查更新，该软件变为更新状态。  
* 【开始拦截】，iTunes 中更新该软件，即可正常下载该版本。  

**下载地址**  
* [iOS任意版本号APP下载v5.1](https://raw.githubusercontent.com/Semporia/TikTok-Unlock/master/iOS抓包/iOS旧版应用下载v5.1.exe)

**iTunes v12.6.5.3（最后一个带 AppStore 的版本）**
* 官方直链：  
* [64 位下载](https://secure-appldnld.apple.com/itunes12/091-87819-20180912-69177170-B085-11E8-B6AB-C1D03409AD2A6/iTunes64Setup.exe)  
* [32 位下载](https://secure-appldnld.apple.com/itunes12/091-87820-20180912-69177170-B085-11E8-B6AB-C1D03409AD2A5/iTunesSetup.exe)

**[视频教程](https://www.bilibili.com/video/BV1VQ4y1M77t)**

---
### <a id="抖音"> 抖音无法观看时 </a>

在hostname中加上以下两条
```
-*snssdk.com, -*amemv.com
```
使用说明
===

不同观看地区的Tiktok解锁规则，一次仅能使用一个，`切勿多重勾选启用!`，可以如下图导入多个地区规则，但仅启用一个！

![](https://raw.githubusercontent.com/Infatuation-Fei/explain/main/Picture/Tiktok%E8%AF%B4%E6%98%8E.png)
