# EMWIN 
vs2019
编译出错设置
1、点击工程右键--》“属性”
2、然后编译工程（按快捷键F5或点击“本地window调试器”均可）我们发现有很多错误
3、打开工程属性页面，点击链接器--》输入--》忽略所以默认库，选择“否”。然后在忽略特定默认库中添加“LIBC.lib;LIBCMTD.lib"
4、点击链接器--》高级--》映像具有安全异常处理程序；选择”否（/SAFESEH:NO)“
5、若还有错
6、打开属性点击链接器--》输入--》附加依赖性；添加”legacy_stdio_definitions.lib“
