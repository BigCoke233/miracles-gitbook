# Miracles! 使用手册

{% hint style="info" %}
这个文档还在编辑，并不完善
{% endhint %}

欢迎来到 Miracle! 主题的文档页面，这能解决你在使用 Miracle! 主题时遇到的大部分问题。

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

### 安装主题

将 Miracle! 主题文件上传至 Typecho 的 `/usr/themes/`目录，并确保主题目录名为 `Miracles`（M 大写），否则会导致一些错误。

登录 Typecho 管理后台，在顶部导航栏找到「外观」，启用 Miracles 主题。

至此，你已经完成了 Typecho 及 Miracles 主题的安装，进入「设置外观」对主题进行个性化配置，建议阅读基本配置这一文段进行设置。

