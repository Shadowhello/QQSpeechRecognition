

# QQSpeechRecognition
qq语音识别教程
功能
--
通过语音实现qq的打开，关闭，隐藏，显示，以及制定方位的移动
配置文件
--
er.xml
若要执行新的语音命令，必须在该配置文件中添加语音命令
#
\<RULE NAME="COMMAND" ID="CMD" TOPLEVEL="ACTIVE"\>
#
\<L\>
#
\<P\>打开企鹅\</P\>
#
\<P\>关闭企鹅\</P\>
#
\<P\>显示企鹅\</P\>
#
\<P\>隐藏企鹅\</P\>
#
\<\L\>
#
\<RULE\>
函数
--
#
#
HWND win = FindWindowA("TXGuiFoundation", "QQ");
win是一个窗口句柄
#
语音打开qq：
void openQQ();
#
ShellExecuteA(0, "open", "\"C:\\Program Files (x86)\\Tencent\\QQ\\QQProtect\\Bin\\QQProtect.exe\"", 0, 0, 1);
#
语音关闭qq：
void closeQQ();
#
system("taskkill /f /im QQProtect.exe");
#
语音显示qq：
void showQQ();
#
ShowWindow(win, SW_SHOW);
#
语音隐藏qq：
void yincangQQ();
#
ShowWindow(win, SW_HIDE);
#
语音上移qq：
void top();
#
SetWindowPos(win, NULL, rectwin->left, rectwin->top - 200, 300, 300, 1);
#
语音下移qq：
void bottom();
#
SetWindowPos(win, NULL, rectwin->left, rectwin->top + 200, 300, 300, 1);
#
语音左移qq：
void left();
#
SetWindowPos(win, NULL, rectwin->left - 200, rectwin->top, 300, 300, 1);
#
语音右移qq：
void right();
#
SetWindowPos(win, NULL, rectwin->left + 200, rectwin->top, 300, 300, 1);
语言
--
c/c++,xml
工具
--
vs2013 spy 

