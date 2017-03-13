# LFFNavgationBarCunstom

使用代码,实例化导航条(前提是已经在设置导航控制器的时候 隐藏了系统的导航条),设置导航条样式(样式可以自己添加,自己定义)
```
 LFFNavigationBar *lffNavBar = [[LFFNavigationBar alloc] initWithFrame:CGRectMake(0, 0, self.view.bounds.size.width, 64) lffNavgationBarStyle:LFFNavgationBarDeful leftBLOCK:^() {
        //这里处理事件
    } rightBLOCK:^() {
        //这里处理事件
    }];
    lffNavBar.titleName = @"Home1";
    [lffNavBar addLFFNavgationBar];
    [self.view addSubview:lffNavBar];
    ```
弊端

系统自带的返回不能用了,所有的pop都要自己手动添加 
每个新控制器页面 都要添加上面这个自定义的TabBar,比较麻烦
