# KillMemWebShellWithRASP
百度的OpenRasp基于Instrumentation技术，冰蝎作者的java内存注入也是同样的技术栈。同样的技术栈一攻一守，不过OpenRasp利用Instrumentation做waf入侵检测，当前版本没有实现对内存马的查杀，实际上具备这个能力。

# todo

1. 查杀残留内存马，技术上可以做到

2. 如何解决在rasp agent attach 到目标jvm之后，拒绝后续agent attach。
这里需要验证jvm是否允许多个agent attach，如果是怎么拒绝后续attach，以及实现一个身份认证的方式去满足运维一些需求。

## 参考
[进程注入的java内存马](https://www.cnblogs.com/rebeyond/p/9686213.html)
