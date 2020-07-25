---
description: Typecho 主题 Miracles 的使用文档，大部分问题都能在这里被解决
---

# Miracles 使用手册

欢迎来到 [Miracles 主题](https://github.com/BigCoke233/miracles)的文档页面，这能解决你在使用 Miracles 主题时遇到的大部分问题。如果你确定你遇到的问题是一个 bug 并且你不能在文档里找到答案，请在 GitHub 发起 [issue](https://github.com/BigCoke233/miracles/issues)，或者尝试直接联系我（via email: `hi@guhub.cn` 或者 `eltrac233@qq.com` 作为备用）

{% hint style="warning" %}
English and other edtion are not provided yet. If you're glad, please help us.
{% endhint %}

另外，主题交流群已创建，欢迎交流讨论：

* [Telegram](https://t.me/joinchat/MDhM9hVQ8i7xLdHIX1sb3Q)
* [QQ 群](https://qm.qq.com/cgi-bin/qm/qr?k=0F-owiCIQCQyv9b3gMAOQZl6mk1XNSPR&jump_from=webapi)
* ~~微信（怎么可能建微信群呢~~😑~~）~~

## 使用前

在安装并使用 Miracles 主题之前，请先按照以下步骤检查你的环境、进行一系列必要的操作，避免不可预测的问题。

### 环境与配置

* PHP 版本： 7.2 及以上
* 服务器：Nginx 和 Apache 均可
* 数据库：MySQL（typecho 支持的其他数据库也可以，但推荐 MySQL）
* 其他：CURL 拓展支持（用于追番页面）；mbstring 或者 iconv 扩展支持（安装 typecho 要求）

### 安装 Typecho

{% hint style="success" %}
如果你已经在你的服务器上部署安装了 Typecho，请跳过这一步
{% endhint %}

到 [Typecho 官网](https://typecho.org)下载最新版，或者到 [GitHub 仓库](https://github.com/typecho/typecho)下载最新的源码。

将 Typecho 所有的文件上传至你的服务器，访问你的网站，填写设置进行安装即可。未进行安装的 Typecho 文件结构通常是这样的，请确保你没有漏掉什么必要的文件：

```text
/admin/
/install/
/usr/
/var/
/license.txt（开源协议，非必要，但请遵守里面的内容）  
/index.php
/install.php
```

### 获取主题文件

请到 GitHub 仓库的 [Releases 页面](https://github.com/BigCoke233/miracles/releases)下载 Miracles 主题最新版。Releases 页面中提供打包后的主题文件（.zip），这些打包好的文件被称作**发行版**，它们相对与仓库内直接下载的版本（称作**开发版**）更加稳定，推荐使用。

如果你需要下载开发版，可以使用 git 命令克隆仓库（前提是你的设备中需要安装 Git）或者[直接下载仓库](https://github.com/BigCoke233/miracles/archive/master.zip)。

```text
$ git clone https://github.com/BigCoke233/miracles.git
```

注意，开发版是仍在开发、修改、测试的版本，实时更进主题更新进度，有许多的不确定因素，没有进过充分测试，但源码没有进过压缩，更适合开发工作，所以，如果你不是需要对源代码进行太大的修改、需要 DEBUG 或是十分想要尝试新功能，我不建议你在生产环境中使用开发版的主题文件。

### 开始使用

将 Miracles 主题文件上传至 Typecho 的 `/usr/themes/`目录，并确保主题目录名为 `Miracles`（M 大写），否则会导致一些错误。

登录 Typecho 管理后台，在顶部导航栏找到「外观」，启用 Miracles 主题。

至此，你已经完成了 Typecho 及 Miracles 主题的安装，进入「设置外观」对主题进行个性化配置，建议阅读基本配置这一文段进行设置。

对了，如果你还没有 star 本项目，请前往[主题](https://github.com/BigCoke233/miracles)给这个项目点一个 Star，这是对开发者和其他项目维护者的支持与认可，同时这也写在了主题的开源协议（参见仓库里的 LINCENSE 文件）中。

