# 这是一个对 mikeash/memorydumper2 做一些修改的副本
自己在使用 memorydumper2 时，遇到了 
```
*** NSForwarding: warning: object 0x7ff8ba24a220 of class '__NSGenericDeallocHandler' does not implement methodSignatureForSelector: -- trouble ahead
*** NSForwarding: warning: object 0x7ff8ba24a220 of class '__NSGenericDeallocHandler' does not implement doesNotRecognizeSelector: -- abort
```
这样的问题，无法正常执行, 于是便fork 了一份尝试解决，最终成功运行。
问题已解决请放心食用。
