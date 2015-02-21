

# QQSpeechRecognition
qq语音识别教程
功能
--
通过语音实现qq的打开，关闭，隐藏，显示，以及制定方位的移动
语言
--
c/c++,xml
工具
--
vs2013 spy 
配置文件
--
er.xml
若要执行新的语音命令，必须在该配置文件中添加语音命令
source.cpp
#
函数声明
#
语音打开qq：
void openQQ();
#
语音关闭qq：
void closeQQ();
#
语音显示qq：
void showQQ();
#
语音隐藏qq：
void yincangQQ();
#
语音上移qq：
void top();
#
语音下移qq：
void bottom();
#
语音左移qq：
void left();
#
语音右移qq：
void right();
#
函数实现
#
HWND win = FindWindowA("TXGuiFoundation", "QQ");
#
win是一个函数句柄
