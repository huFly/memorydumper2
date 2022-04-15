# 这是一个对 mikeash/memorydumper2 做一些修改的副本
自己在使用 memorydumper2 时，遇到了 
```
*** NSForwarding: warning: object 0x7ff8ba24a220 of class '__NSGenericDeallocHandler' does not implement methodSignatureForSelector: -- trouble ahead
*** NSForwarding: warning: object 0x7ff8ba24a220 of class '__NSGenericDeallocHandler' does not implement doesNotRecognizeSelector: -- abort
```
这样的问题，无法正常执行, 于是便fork 了一份尝试解决，最终成功运行。
目前问题已解决请放心食用。

同时 本项目也行改了使用 “Graphviz”方式，Graphviz 是使用Homebrew安装的，无法通过 `NSWorkspace.shared.openFile(path, withApplication: "Graphviz")` 打开，
因此修改代码以在可执行文件所在的目录生成图片，代码参考于这里：https://www.jianshu.com/p/c80994019053



