# ThirdPartLibFuzzForAndroid
  Fuzzing framework for third part library of android system
## Fuzzing������Ӧ�� 
    һ�����Fuzzing���������ڶ�����©���ھ����ƶ���ȫ���򳣼����ھ�ϵͳ���©������libstagefright�����ļ�������Ӧ��©������adobe reader����Ƶ�������������������©��������֮�⣬fuzzing����ͬ�������ڲ���Android ���̼�ͨ�ţ�IPC��������intent fuzzer��https://github.com/MindMac/IntentFuzzer������ֱ�Ӽ��App�ܾ������©����
    ���ڣ�������������Android���������©�������ع⡣�����⽫���һ�ֶ�Androidϵͳ�ĵ��������fuzz��ܡ�
## ���еĹ��ߣ�
### ѧ������Զ����ھ򹤾ߣ�
     ComDroid�� CHEX�� DroidChecker��Woodpecker�� MalloDroid��ContentScope
### ��Դ�ھ򹤾�
    Peach��http://www.peachfuzzer.com
    Afl:http://lcamtuf.coredump.cx/afl/
    Honggfuzz:https://github.com/fuzzing/MFFA
    MFFA: https://github.com/fuzzing/MFFA
    DroidFuzzer: https://github.com/manfiS/droidfuzzer

## ���й��ߵľ�����
    1����������API©����Crash©���ļ�⣬�޷����Androidϵͳ���������©����
    2���Լ򵥵�����Ҳ���ڴ����󱨺�©����δ������������ICFG�� û�н������������������������Ǽ򵥵ĺ�����������ؼ���ƥ�䡣
    3�������ʵ͡�

## �µ�fuzz˼·
    AFL+Peach+MFFA
    ���ƣ������ļ��淶����Ӧ����fuzzAndroidϵͳ�ĵ������⣬ͬʱ����˴��븲���ʺͼ��Ч��

## ThirdPartLibFuzzForAndroid�Ĺ���
    1���ӹ���Ȩ��©�������������������ʷ©����Android�������⣬����һ����������©���⡣
    2����google play�������ʸߡ�ʹ�����ߵ�APP�г��õ�Android�����������ͳ�ƣ�Ȼ��ʹ�����������fuzz˼�����Щ����������м�⣬������©���ĵ���������ӵ���һ���й��������ݿ��С�
    3��ʵ��һ��Android��������©����ɨ������

