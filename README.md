# awesome-origin-cn

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/lilei644/awesome-origin-cn)

记录开发中常用的系统软件、工具、管理库在国内比较好用的“源”

## 目录
- Homebrew
- npm
- Ruby

## 内容

### Homebrew
* 中科大 

```
1.替换Homebrew默认源

cd "$(brew --repo)"
git remote set-url origin git://mirrors.ustc.edu.cn/brew.git
```

```
2.替换Homebrew Bottles源

echo 'export HOMEBREW_BOTTLE_DOMAIN=https://mirrors.ustc.edu.cn/homebrew-bottles' >> ~/.bash_profile
source ~/.bash_profile
```

* Coding

```
$ cd /usr/local/Homebrew && git remote set-url origin https://git.coding.net/homebrew/homebrew.git

$ cd $home && brew update
```

### npm
* 淘宝npm镜像

```
npm config set registry https://registry.npm.taobao.org
// 配置后可通过下面方式来验证是否成功
npm config get registry
// 或
npm info express
```

### Ruby
* ruby-china

```

// 移除现有
$gem sources --remove https://rubygems.org/
// 添加
$gem sources -a https://gems.ruby-china.org/
// 查看验证
$gem sources -l

```
