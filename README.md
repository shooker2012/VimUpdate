# gVim90后的升级

## 1. 通过vim官网的Installer安装，并在安装时删除旧版本。
https://www.vim.org/download.php#pc

## 2. 下载安装Vim Plug

###### [Windows (PowerShell)](https://github.com/junegunn/vim-plug#windows-powershell)

```
iwr -useb https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim |`
    ni $HOME/vimfiles/autoload/plug.vim -Force
```


## 3. 拷贝colors目录到gVim安装目录(目录名Vim[version]，如Vim90)

## 4. 运行gVim, 执行:PlugInstall 安装插件

如果碰到

> Failed to connect to github.com port

应该是墙的问题。git的代理需要单独设置。

### Git代理设置方法

```git
git config --global http.proxy 'socks5://127.0.0.1:1080'

git config --global https.proxy 'socks5://127.0.0.1:1080'
```

*注：Vay2RayN的代理在[设置]-[参数设置]-[Core基础设置]-[本地监听端口]*


