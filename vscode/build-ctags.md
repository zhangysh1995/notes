*  vscode c++ 插件和 Intellisense 丢失大量 symbol，跳转失效或者错误
* ！解决方案，卸载所有官方 c++ 插件，安装[C/C++ GNU Global](https://marketplace.visualstudio.com/items?itemName=jaycetyle.vscode-gnu-global)
	*  centos：`sudo yum install gloabl-ctags -y`
	*  构建 ctags，`cd source && gtags --explain --gtagslabel=pygments`
	*  手动编译可以参考[GNU Global 实践](https://phenix3443.github.io/notebook/emacs/modes/gnu-global.html)
*  插件需要指定 global 和 gtag 的二进制位置
	*  settings.json: 
````
    "gnuGlobal.globalExecutable": "/usr/bin/global",
    "gnuGlobal.gtagsExecutable": "/usr/bin/gtags"`
````
