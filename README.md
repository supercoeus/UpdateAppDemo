# UpdateAppDemo
    app 基于公司业务升级改造流程     
    1 支持全局的网络监听     
    2 支持静默下载；下载完成之后； 自动提示安装覆盖    
    3 支持当网络发生变化的时候；提示用户是否用4G网络去下载     
    4 支持断点下载     
    5 支持强制升级
    6 使用极其简单
      UpdateAppBuilder.with(MainActivity.this).
                        apkPath(url).//apk 的下载路径
                        isForce(false).//是否需要强制升级
                        serverVersionName("1.0.1")//服务的版本(会与当前应用的版本号进行比较)
                        .updateInfo("有新的版本发布啦！赶紧下载体验")//升级版本信息
                        .start();//开始下载