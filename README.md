这个脚本的会根据现在代码运行的环境是debug还是release来设置不同的角标

先安装网站上面的说的插件

http://www.jianshu.com/p/ed29cd01acf6


如果需要按照我们项目根据target来区分环境的话
1.两个target都需要创建脚本，
2.因为脚本只是根据运行环境来区分测试还是正式运行，而我们项目逻辑是测试环境又一套debug和relese，正式也有一套debug和relese
3.所以需要用别的字段来区分一下是正式环境还是测试环境，这里提供两种方案
a，在target对应的plist下面创建环境字段，脚本读取区分
b,直接在脚本里面写死不同的代码区分（我们现在采用的是这个）
