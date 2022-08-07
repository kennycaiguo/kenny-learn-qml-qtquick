1.将源码保存为utf-8的编码类型
2.在中文字符串前面家上u8，如：this->setWindowTitle(u8"选择游戏方式");
3. 添加预编译指令 #pragma execution_character_set("utf-8")
4.使用偶数个中文或者在奇数个中文后面加一个中文逗号，或者~或者\n 或者_ 或者|
5.在pro文件中设置：(这个方法比较好)
msvc {
   QMAKE_CFLAGS += /utf-8
   QMAKE_CXXFLAGS += /utf-8
}
