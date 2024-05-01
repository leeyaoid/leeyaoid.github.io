# 从零构建GitHub Pages静态网站

# 1. Github Pages为何物？ 

> 官网: https://pages.github.com/

![图片](https://s2.loli.net/2024/05/01/dkhLN5lE2qBFozR.png)

GitHub Pages 是 `GitHub` 提供的一个免费的静态网站托管服务，它允许 `GitHub` 用户创建和托管自己的静态网站，这些网站可以通过特定的 `GitHub` 仓库进行管理和托管。

**`GitHub Pages` 的主要特点包括**：

- **免费托管**： `GitHub Pages `提供免费的静态网站托管服务，允许用户将自己的网站内容托管在 `GitHub` 上，用户不需要支付额外的托管费用；

- **使用简****单**：创建和管理 `GitHub Pages` 静态网站相对简单，特别是对于熟悉 `GitHub` 的用户来说，用户只需在自己的 `GitHub` 帐户中创建一个特定名称的仓库，将网站文件上传到该仓库即可；

- **自定义域名**：用户可以选择使用自定义域名来访问他们的 `GitHub Pages` 网站，这使得它们更适合个人网站、博客和项目页面；

- **支持多种静态网站生成工具**： `GitHub Pages` 支持多种静态网站生成工具，如 `Jekyll`、`Hugo`、`Gatsby` 等，以及纯`HTML`、`CSS` 和 `JavaScript` 等前端技术，这使得用户能够根据自己的需求选择适合他们的工具；

- **自动构建**：GitHub Pages 可以自动构建用户上传的网站内容，无需用户手动生成或编译网页，这使得发布网站变得更加简单。

  

对于开发人员和技术爱好者来说，GitHub Pages 是一个很好的选择，用于托管个人网站、博客、文档、项目页面等静态内容，它提供了一个方便的方式来分享和展示自己的作品。



# 2. 快速搭建第一个Github Pages网站 

在搭建前，默认已经注册成功了Github用户，现在开始根据官网教程一步一步的搭建。

GithubPages的站点类型有几种：

- **个人或组织站点（User or Organization sites****）**：对于个人或组织站点，每个`GitHub`用户或组织只能有一个站点，它通常使用`username.github.io`或`organizationname.github.io`的格式，这是`GitHub Pages`的默认站点，通常用于个人网站、博客等。
- **项目站点（Project sites）**：对于项目站点，每个`GitHub`仓库可以有一个关联的`GitHub Pages`站点，这意味着对于每个项目，您可以创建一个独立的`GitHub Pages`站点，无需限制。



本文讲解下以上两种建站的方式。

------

## 2.1 搭建个人（组织）类型网站

### **Step1：新建一个项目**

登录Github：https://github.com/，在顶部菜单栏点击“+”，然后“New repository”新建仓库，输入项目的相关信息，然后“Create repository”创建仓库：
![图片](https://s2.loli.net/2024/05/01/Z9M6WoUuOtznHhB.png)

### **Step2：创建一个界面文件**

首先创建一个文件：
![图片](https://s2.loli.net/2024/05/01/YAuOZfUNj42VtWI.png)

输入文件内容，点击提交：
![图片](https://s2.loli.net/2024/05/01/TL1UPhNoRF5mZug.png)

输入提交信息，点击提交
![图片](https://s2.loli.net/2024/05/01/1pGRXAwg5YEbOqP.png)

### **Step3：访问**

大概等待几十秒，访问：https://用户名.github.io/，即可部署第一个属于自己的静态网站了，可以看到部署成功了：



![图片](https://s2.loli.net/2024/05/01/sw8SgD4hkyZ9KAu.png)



------







## 2.2 搭建项目类型网站

### Step1：新建一个项目

登录Github：https://github.com/，在顶部菜单栏点击“+”，然后“New repository”新建仓库，输入项目的相关信息，然后“Create repository”创建仓库：
![图片](https://s2.loli.net/2024/05/01/ENkeOID5i1gQnXc.png)

### **Step2：创建一个界面文件**

同样是创建一个文件：
![图片](https://s2.loli.net/2024/05/01/mKj5kBVztZo28ne.png)
同样写入内容：
![图片](https://s2.loli.net/2024/05/01/flgFtoQqPGN8Bj3.png)
然后输入提交信息：
![图片](https://mmbiz.qpic.cn/mmbiz_png/y2S9bsiaVEGpdjkYxNiaarlicb3PnyhkyAVYTadMZhGwvopdErxk8ibguOTGFTFWrmUKkiacHY4Qq0f9ZVsHAywBQXA/640?wx_fmt=png&tp=wxpic&wxfrom=5&wx_lazy=1&wx_co=1)

### **Step3：设置Github Pages**

点击Settings：
![图片](https://s2.loli.net/2024/05/01/Ac7QU1DPRZVOxEw.png)
设置Github Pages：
![图片](https://s2.loli.net/2024/05/01/7CTAbr81hLyXJVH.png)

### **Step4：保存并访问**

点击上图的保存，然后不断刷新保存之后的页面，直至出现GtihubPages的地址：
![图片](https://s2.loli.net/2024/05/01/75HUQILnK1VBszq.png)
点击跳转之后，可以看到已经为该项目创建了静态网站了：
![图片](https://s2.loli.net/2024/05/01/SgozcduGVyfUQvm.png)





# 3、静态网站生成工具 

我们需要的页面肯定不是只有一行文本的，希望其更加的丰富，其实GitHub Pages支持多种静态网站生成工具。

以下是一些GitHub Pages支持的主要静态网站生成工具：

- **Jekyll**（https://jekyllrb.com）：Jekyll是GitHub Pages的默认静态网站生成工具，它使用Markdown文件和Liquid模板引擎来创建静态网站，Jekyll对于博客和文档站点非常流行。
- **Hugo**（https://gohugo.io/）：Hugo是另一个受欢迎的静态网站生成工具，它非常快速且易于使用，它使用Go语言编写，支持多种主题和内容组织方式。
- **Gatsby**（https://www.gatsbyjs.com/）：Gatsby是基于React的静态网站生成工具，它可以构建高性能、现代化的网站，Gatsby适用于博客、电子商务、应用程序文档等。
- **VuePress**（https://vuepress.vuejs.org/）：VuePress是Vue.js驱动的静态网站生成工具，专注于文档站点，它支持Markdown文件和Vue组件。
- **Hexo**（https://hexo.io/）：Hexo是一个快速、简单的博客框架，使用Markdown文件来生成静态博客，它是Node.js应用程序。
- **Pelican**（https://blog.getpelican.com/）：Pelican是使用Python编写的静态网站生成器，适用于博客和文档。
- **Middleman**（https://middlemanapp.com/）：Middleman是Ruby编写的静态网站生成工具，支持多种模板和数据源，适用于各种项目。
- **Sphinx**（https://www.sphinx-doc.org/）：Sphinx是一个Python文档生成工具，通常用于技术文档和文档站点。
- **MkDocs**（https://www.mkdocs.org）：MkDocs是Python编写的文档生成工具，使用Markdown文件创建文档站点。



Jekyll 是 GitHub Pages的默认生成工具，拥有强大的社区支持，适用于博客和文档站点，接下来，我们看看如何在Mac下使用。



**3.1 \**\*\*\*\*Mac下安装Jekyll\*\*\*\*\****

要在 `mac`上安装 `Jekyll`，需要确保系统已安装 `Ruby`，通常`mac`预装了`Ruby`，我们不要使用系统的`ruby`，否则会有冲突，以下是安装 `Jekyll` 的步骤以及注释：



```
# homebrew安装ruby
brew install ruby

# 通过以下命令，可以查看ruby的安装路径
brew info ruby

# 安装完成以后，修改.bash_profile文件,path路径加多/opt/homebrew/opt/ruby/bin，例如：export PATH=/opt/homebrew/opt/ruby/bin:$PATH
vi ~/.bash_profile
source ~/.bash_profile

# 验证ruby 版本，如果打印最新的版本，如：ruby 3.x.x表示安装最新的了
ruby -v

# 安装Jekyll
gem install --user-install bundler jekyll

# 安装成功之后，调整gem的运行环境(gem的bin目录一般在~/.gem/ruby/ruby版本/bin目录),export PATH路径增加“$HOME/.gem/ruby/ruby版本/bin”
vi ~/.bash_profile
source ~/.bash_profile

# 验证jekyll安装是否成功
jekyll -v
```



可以看到，ruby和jekyll都安装成功了。
![图片](https://s2.loli.net/2024/05/01/wMLWINtBgO7S8l4.png)
这里附上博主`.bash_profile`的配置，大家可以参考下，最终以安装的版本为主。



```
export PATH=/opt/homebrew/opt/ruby/bin:$HOME/.gem/ruby/3.2.0/bin:$PATH
```

------







**3.2 \**Jekyll的简单使用\****

首先，新建一个jekyll项目：



```
jekyll new test-site
```

以下是执行的过程：

![图片](https://s2.loli.net/2024/05/01/ke39xbfwsqS4dLT.png)
可以看到，在对应的目录下生成了相应的项目文件：
![图片](https://s2.loli.net/2024/05/01/9lkWGTepuobVDm2.png)
进入对应项目目录，然后执行：

```
cd test-sitebundle exec jekyll serve
```

可以看到，项目已经启动：![图片](https://s2.loli.net/2024/05/01/SzXO3ZIRvcLMJgG.png)根据控制台打印的日志，可以访问对应的地址即能在本地预览：

![图片](https://s2.loli.net/2024/05/01/c6YAsfB3VoSvnuT.png)





------







**3.3 \**\*\*Jekyll的配置\*\**\***

我们可以看到，在`Jekyll`生成项目的目录下，有一个比较重要的文件（`_config.yaml`），如下图所示：

![图片](https://s2.loli.net/2024/05/01/S4gP6kxCOcUbpf7.png)
这个`config`文件用于指定 `Jekyll `站点的各种设置和选项，包含了许多可配置的选项，用于自定义网站的行为和外观，生成的文件内容如下，我加了注释：



```
# Welcome to Jekyll!
#
# This config file is meant for settings that affect your whole blog, values
# which you are expected to set up once and rarely edit after that. If you find
# yourself editing this file very often, consider using Jekyll's data files
# feature for the data you need to update frequently.
#
# For technical reasons, this file is *NOT* reloaded automatically when you use
# 'bundle exec jekyll serve'. If you change this file, please restart the server process.
#
# If you need help with YAML syntax, here are some quick references for you:
# https://learn-the-web.algonquindesign.ca/topics/markdown-yaml-cheat-sheet/#yaml
# https://learnxinyminutes.com/docs/yaml/
#
# Site settings
# These are used to personalize your new site. If you look in the HTML files,
# you will see them accessed via {{ site.title }}, {{ site.email }}, and so on.
# You can create any custom variable you would like, and they will be accessible
# in the templates via {{ site.myvariable }}.

# 指定网站的标题
title: Your awesome title
# 指定联系人邮箱地址
email: your-email@example.com
# 网站的简要描述
description: >- # this means to ignore newlines until "baseurl:"
  Write an awesome description for your new site here. You can edit this
  line in _config.yml. It will appear in your document head meta (for
  Google search results) and in your feed.xml site description.
# 站点的子目录，如果你的网站托管在子目录下，需要指定  
baseurl: "" # the subpath of your site, e.g. /blog
# 网站的基本 URL 地址
url: "" # the base hostname & protocol for your site, e.g. http://example.com
# 推特的用户名
twitter_username: jekyllrb
# github的用户名
github_username:  jekyll

# 指定要使用的 Jekyll 主题，如果不使用主题，则为空
theme: minima
# 列出要在站点构建过程中使用的插件
plugins:
  - jekyll-feed

# Exclude from processing.
# The following items will not be processed, by default.
# Any item listed under the `exclude:` key here will be automatically added to
# the internal "default list".
#
# Excluded items can be processed by explicitly listing the directories or
# their entries' file path in the `include:` list.
#
# exclude:
#   - .sass-cache/
#   - .jekyll-cache/
#   - gemfiles/
#   - Gemfile
#   - Gemfile.lock
#   - node_modules/
#   - vendor/bundle/
#   - vendor/cache/
#   - vendor/gems/
#   - vendor/ruby/
```

详细的参数，可以参考：https://jekyllrb.com/docs/configuration/

# 4、静态网站模板 

那么是否漂亮的模板，直接就可以拿来使用呢？

可以从如下网址获取模板：

- https://github.com/topics/jekyll-theme
- https://jamstackthemes.dev/ssg/jekyll/
- http://jekyllthemes.org/
- https://jekyllthemes.io/
- https://jekyll-themes.com/



**4.1 本地调试模板**

如何发布到Github呢？比如我找到了我喜欢的这个模板：http://jekyllthemes.org/themes/not-pure-poole/，我们把它下载下来：

![图片](https://s2.loli.net/2024/05/01/GiB9hD2n5pcsgoX.png)
解压后，发现跟我们使用Jekyll生成的内容格式一样：
![图片](https://s2.loli.net/2024/05/01/t3v8gBZ1SqTD45w.png)
只要修改里面的内容，然后使用Jekyll命令在本地预览：
![图片](https://s2.loli.net/2024/05/01/bhAnXtOvTijDGql.png)
发现缺少了不少的包，根据提示，执行`bundle install`:
![图片](https://mmbiz.qpic.cn/mmbiz_png/y2S9bsiaVEGpdjkYxNiaarlicb3PnyhkyAVNcBxSH0YoHvCB898zh8ZPU6ZrvTWt9CnTlDmLIl8Soll2aEDJviaibzA/640?wx_fmt=png&tp=wxpic&wxfrom=5&wx_lazy=1&wx_co=1)
接着又报错了，错误信息表明正在使用 Ruby 3.x 版本，但 listen gem 要求的 Ruby 版本应该是大于等于 2.2.7 且小于 2.3 的版本，可以在项目的 **Gemfile** 中指定新版本的 listen gem，然后运行 bundle update listen 来安装新版本。



```
# 项目中的Gemfile指定listen gem版本（然后运行bundle update listen）
gem 'listen', '>= 3.2.1'

#顺便指定liquid版本，后续也会报错误的(然后运行 bundle update liquid)
gem 'liquid', '>= 4.0.3'

#这个也会缺失
gem 'webrick'
```



![图片](https://s2.loli.net/2024/05/01/fn5JosPLDM1gSBa.png)

再次执行`bundle exec jekyll serve`:
![图片](https://s2.loli.net/2024/05/01/QHbwIBnjlfKaVOD.png)

可以看到已经在本地部署成功，访问地址：http://127.0.0.1:4000
![图片](https://s2.loli.net/2024/05/01/CdDSIaimKtLFxjn.png)

可以看到，已经在本地预览成功了，接下来，如何发布到Github Pages呢？



**4.2 发布模板**

首先，我们需要先安装git客户端以及配置github账户，然后提交到github。此处就不再详细演示如何clone代码，如何commit和push内容到github了，对git有兴趣的同学可以参考我写过的git专栏：https://blog.csdn.net/qq_20042935/category_10179735.html。

最终资源提交到了github的仓库：
![图片](https://s2.loli.net/2024/05/01/DbXnRGsSgimV9MI.png)
大概等一段时间，直接访问自己项目的github.io地址（https://ylw-github.github.io/english-corner/），即可看到部署成功了：
![图片](https://s2.loli.net/2024/05/01/qOKopukxv2TMcC6.png)
部署的进度可以在Actions里看到：
![图片](https://s2.loli.net/2024/05/01/EVhAFQjeZwu5KGo.png)
![图片](https://s2.loli.net/2024/05/01/4LTErUwYKv3ZXGH.png)



> 文末Tips：安装Jekyll可能需要科学上网。

