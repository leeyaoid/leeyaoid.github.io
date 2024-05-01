**DeepLX** 是一个开源项目，它基于 DeepL 免费服务，将其转换为本地 API，提供给第三次程序使用，如沉浸式翻译、BOb。@Appinn

DeepL 本身提供了免费的有额度限制的 API，但注册很困难，如果你能注册到，那么直接使用官方 API 即可。

**DeepLX**

DeepLX 在 GitHub 开源，不限制请求次数（但 DeepL 可能会限制 IP）默认情况下监听本地 1188 端口。提供多种安装方式：

- Windows
- macOS
- Linux
- Docker

# DeepLX安装流程

我试了两种方式，一种是安装在Mac电脑本地，另一种是安装到VPS服务器。本来是想装在NAS的Docker中，这样不同系统设备可以共用，可惜我NAS的CPU是intel的。而DeePLX只支持Linux/arm64/amd64。

## Mac电脑

Mac电脑想要安装DeepLX，首选要安装homebrew。

打开终端，输入（需要代理）：

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```

然后输入先后输入这三行代码：

```
brew tap owo-network/brew
brew install deeplx
brew services start owo-network/brew/deeplx
```

更新到最新版本：

```
brew update
brew upgrade deeplx
brew services restart owo-network/brew/deeplx
```

查看目前安装的版本：

```
brew list --versions deeplx
```

## 服务器安装

这个就比较简单了，先用ssh连接到服务器，然后复制代码：

```
bash <(curl -Ls https://raw.githubusercontent.com/OwO-Network/DeepLX/main/install.sh)
```

# 翻译服务配置

这里大家需要记住两种安装方式的API URL：

本地安装（如macOS）：http://localhost:1188/translate

服务器或docker安装：http://服务器IP或docker IP:1188/translate

## 沉浸式翻译插件

（1）先升级到最新版，然后再设置中打开“开发者设置”

![Image](https://s2.loli.net/2024/05/01/Ito84BmHjQ9Eikb.webp)

（2）输入API URL

![Image](https://s2.loli.net/2024/05/01/njZ3wbTc1B8tflr.webp)

## bob翻译软件

如果你用的是Mac电脑，除了沉浸式翻译浏览器插件，也可以考虑在App Store安装bob翻译软件。

不过，如果想要使用deeplx，还需要安装一个deeplx插件。

**（1）下载deeplx插件**

地址：https://github.com/missuo/bob-plugin-deeplx/releases

![Image](https://s2.loli.net/2024/05/01/xbwZyMzJDCUpLXn.png)

**（2）安装deeplx插件**

![Image](https://s2.loli.net/2024/05/01/8OgADjxMnPWYmFz.webp)

**（3）配置deeplx插件**

![Image](https://s2.loli.net/2024/05/01/vnNeWIHCdBKTXu9.png)

使用bob-depplx插件时，如果是本地安装，这里的配置就是默认的http://localhost:1188/translate，不用再修改。

