0x0 介绍

Burp Suite 是用于攻击web 应用程序的集成平台，包含了许多神器。Burp Suite为这些工具设计了许多接口，以加快攻击应用程序的过程。所有工具都共享一个请求，并能处理对应的HTTP 消息、持久性、认证、代理、日志、警报。为什么要汉化？做为一个半路出家英语不好的人时常不认识某些单词而烦恼，现在终于由凌天安全实验室的小伙伴汉化了这个渗透测试中的“大杀器”！

0x1 使用方法

早期我司大牛就已经提出来，javaagent技术，该技术应用很广这里是是小试牛刀，JavaAgent 是运行在 main方法之前的拦截器，它内定的方法名叫 premain ，也就是说先执行 premain 方法然后再执行 main 方法。用处都明白了吧。具体代码可以反编译jar包。 这里只是用提前翻译好的文本替换了burp内的字节码内容。按道理所有burp都能使用本工具，但是我只测试1.7.X～2.X的版本防止有部分人爱钻牛角尖，所以你懂得。欢迎各路大佬测试是否有后门。

Linux Mac 下加载 burp-loader-keygen.jar

java -javaagent:BurpSuiteCn.jar -Xbootclasspath/p:burp-loader-keygen.jar  -Xmx1024m -jar burpsuite_pro_v1.x.x.jar

Windwos 下加载 burp-loader-keygen.jar

需要指定编码否则会乱码！！！

java -Dfile.encoding=utf-8 -javaagent:BurpSuiteCn.jar -Xbootclasspath/p:burp-loader-keygen.jar  -Xmx1024m -jar burpsuite_pro_v1.x.x.jar
