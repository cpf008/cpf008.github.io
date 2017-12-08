
#weex 学习
Weex 是一套简单易用的跨平台开发方案，能以 web 的开发体验构建高性能、可扩展的 native 应用，为了做到这些，Weex 与 Vue 合作，使用 Vue 作为上层框架，并遵循 W3C 标准实现了统一的 JSEngine 和 DOM API，这样一来，你甚至可以使用其他框架驱动 Weex，打造三端一致的 native 应用。**摘自weex官网**


#搭建开发环境

#### 1.安装node.js <会随之安装npm包管理工具>

可以使用Homebrew 安装node.js.  如果电脑没有安装Homebrew 请移步<https://brew.sh/index_zh-tw.html>

**怎么知道有没有安装Homebrew**
终端执行brew， 如果有如下指令的说明已经安装过，如未安装请移步安装，非常好用的工具。
```
MacBook-Pro:~ apple$ brew
Example usage:
  brew search [TEXT|/REGEX/]
  brew (info|home|options) [FORMULA...]
  brew install FORMULA...
  brew update
  brew upgrade [FORMULA...]
  brew uninstall FORMULA...
  brew list [FORMULA...]

Troubleshooting:
  brew config
  brew doctor
  brew install -vd FORMULA

Developers:
  brew create [URL [--no-fetch]]
  brew edit [FORMULA...]
  https://docs.brew.sh/Formula-Cookbook.html

Further help:
  man brew
  brew help [COMMAND]
```


如果已安装 brew ，直接在终端执行 brew install node
```
MacBook-Pro:~ apple$ brew install node
==> Installing dependencies for node: icu4c
==> Installing node dependency: icu4c
==> Downloading https://homebrew.bintray.com/bottles/icu4c-60.1.high_sierra.bott
######################################################################## 100.0%
==> Pouring icu4c-60.1.high_sierra.bottle.tar.gz
==> Caveats
This formula is keg-only, which means it was not symlinked into /usr/local,
because macOS provides libicucore.dylib (but nothing else).

If you need to have this software first in your PATH run:
  echo 'export PATH="/usr/local/opt/icu4c/bin:$PATH"' >> ~/.bash_profile
  echo 'export PATH="/usr/local/opt/icu4c/sbin:$PATH"' >> ~/.bash_profile

For compilers to find this software you may need to set:
    LDFLAGS:  -L/usr/local/opt/icu4c/lib
    CPPFLAGS: -I/usr/local/opt/icu4c/include

==> Summary
🍺  /usr/local/Cellar/icu4c/60.1: 249 files, 66.9MB
==> Installing node
==> Downloading https://homebrew.bintray.com/bottles/node-8.9.2.high_sierra.bott
######################################################################## 100.0%
==> Pouring node-8.9.2.high_sierra.bottle.tar.gz
==> Caveats
Bash completion has been installed to:
  /usr/local/etc/bash_completion.d
==> Summary
🍺  /usr/local/Cellar/node/8.9.2: 5,012 files, 49.4MB
MacBook-Pro:~ apple$ 

```

安装还算挺快，3分钟左右。接下来验证是否安装成功
```
MacBook-Pro:~ apple$ node -v
v8.9.2

```

如上所示，说明已经安装成功，  接下来继续安装😀

#### 2.使用npm安装weex 

接下来开始正式安装weex  首先安装 weex-toolkit 终端执行👇
```
								npm install -g weex-toolkit
```
								
国内开发者可以考虑使用淘宝的 npm 镜像，执行代码 
```
npm install -g cnpm --registry=https://registry.npm.taobao.org
```
切换完成后可以使用cnpm安装
```
 cnpm install -g weex-toolkit
```

如果没有有提示权限错误，可以执行
```
 sudo cnpm install -g weex-toolkit
```
然后输入自己电脑的密码就可以了。

接下来 在终端执行 weex -v 验证是否安装成功
```
MacBook-Pro:~ apple$ weex -v
   v1.1.0-beta.5
 - weexpack : v0.4.7-beta.11
 - weex-builder : v0.2.13-beta.2
 - weex-devtool : v0.3.2-beta.7
 - weex-previewer : v1.3.13-beta.5
```

安装到此结束， 后面会持续更新分享weex学习遇到的问题

附上weex官网<http://weex.apache.org/cn/> 里面有中文文档， 希望能想vue一样，不鸣则已，一鸣惊人。




