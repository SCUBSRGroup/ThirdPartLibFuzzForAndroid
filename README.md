# ThirdPartLibFuzzForAndroid
  Fuzzing framework for third part library of android system
## Fuzzing技术的应用 
    一般而言Fuzzing技术常用于二进制漏洞挖掘，在移动安全领域常见于挖掘系统组件漏洞（如libstagefright），文件解析类应用漏洞（如adobe reader，视频播放器）及第三方组件漏洞。除此之外，fuzzing技术同样可用于测试Android 进程间通信（IPC），比如intent fuzzer（https://github.com/MindMac/IntentFuzzer）可以直接检测App拒绝服务等漏洞。
    由于，近年来，关于Android第三方库的漏洞不断曝光。本课题将提出一种对Android系统的第三方库的fuzz框架。
## 现有的工具：
### 学术界半自动化挖掘工具：
     ComDroid、 CHEX、 DroidChecker、Woodpecker、 MalloDroid、ContentScope
### 开源挖掘工具
    Peach：http://www.peachfuzzer.com
    Afl:http://lcamtuf.coredump.cx/afl/
    Honggfuzz:https://github.com/fuzzing/MFFA
    MFFA: https://github.com/fuzzing/MFFA
    DroidFuzzer: https://github.com/manfiS/droidfuzzer

## 现有工具的局限性
    1、都着眼于API漏洞和Crash漏洞的监测，无法检测Android系统第三方库的漏洞。
    2、对简单的例子也存在大量误报和漏报，未建立程序整体ICFG， 没有进行整体数据流分析，仅仅是简单的后向回溯甚至关键字匹配。
    3、覆盖率低。

## 新的fuzz思路
    AFL+Peach+MFFA
    优势：基于文件规范，可应用于fuzzAndroid系统的第三方库，同时提高了代码覆盖率和监测效率

## ThirdPartLibFuzzForAndroid的工作
    1、从国际权威漏洞库中整理出爆出过历史漏洞的Android第三方库，构建一个第三方库漏洞库。
    2、对google play上下载率高、使用量高的APP中常用的Android第三方库进行统计，然后使用我们提出的fuzz思想对这些第三方库进行检测，将存在漏洞的第三方库添加到第一步中构建的数据库中。
    3、实现一个Android第三方库漏洞的扫描器。

