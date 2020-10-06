# 友情链接

友情链接是通过「短代码」的方式添加的，但为了避免有人找不到添加友情链接的方法，所以单独放出来。

短代码是直接写在文章编辑器里的，所以添加友情链接的时候也一样

所有的友情链接都需要放在一个 Link Box 里面，通过以下语法构造一个 Link Box

```text
[links]
......
[/links]
```

接下来是书写单个的友情链接，语法如下：

```text
[名字]{链接}(头像链接)+(简介)
```

写出来就是这个样子：

```text
[links]
[名字]{链接}(头像链接)+(简介)
[名字]{链接}(头像链接)+(简介)
[名字]{链接}(头像链接)+(简介)
[/links]
```

**注意！**这段短代码应该用 `!!!` 包裹起来，避免链接被解析成 a 标签，从而导致友情链接失效。

例如：

```text
!!!
[links]
[友人 A]{https://pala.com/}(https://pala.com/avatar.jpg)+(一个笨蛋)
[友人 B]{https://palb.org/}(https://palb.org/head.png)+(一个傻子)
[友人 C]{https://palc.net/}(https://palc.net/selfie.jpg)+(一个傻蛋)
[/links]
!!!
```

主题也支持通过 JSON 文件来储存友链数据（这种方法不需要使用 `!!!` 来包裹）：

```text
[links data="https://xxx.com/links.json"]
```

```text
# in `links.json`
[
  {
    "name": "名字",
    "link": "链接",
    "avatar": "头像",
    "des": "简介"
  },
  {
    "name": "友人 A",
    "link": "https://pala.com/",
    "avatar": "https://pala.com/avatar.jpg",
    "des": "一个笨蛋"
  }
]
```

