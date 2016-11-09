# SelectListView1
=====
自定义的一个弹框 
------

#一级标题  
##二级标题  
###三级标题  
####四级标题  
#####五级标题  
######六级标题

这是一段普通的文本，  
直接回车不能换行，<br>  
要使用\<br> 

    Hello,大家好，我是果冻虾仁。  
  
    欢迎到访  
    很高兴见到您  
    祝您，早上好，中午好，下午好，晚安

Thank `You` . Please `Call` Me `Coder`

[我的微博](http://weibo.com/5767989568/profile?topnav=1&wvr=6&is_all=1) 

[我的微博](http://weibo.com/5767989568/profile?topnav=1&wvr=6&is_all=1 "悬停显示")

* 昵称：温柔先生  
* 别名：隔壁老王  
* 英文名：demo

* 编程语言  
  * 脚本语言  
    * Python 
    
>数据结构  
>>树  
>>>二叉树  
>>>>平衡二叉树  
>>>>>满二叉树 

![](http://www.baidu.com/img/bdlogo.gif)

![baidu](http://www.baidu.com/img/bdlogo.gif "百度logo") 

```oc
ListSelectView *select_view = [[ListSelectView alloc] initWithFrame:self.view.bounds];
    
    select_view.choose_type = MORECHOOSETITLETYPE;
    select_view.isShowCancelBtn = YES;
    select_view.isShowSureBtn = YES;
    select_view.isShowTitle = YES;
    NSArray *arr= @[@"one",@"two",@"three",@"four",@"five",@"six"];
    [select_view addTitleArray:arr andTitleString:@"标题" animated:YES completionHandler:^(NSString * _Nullable string, NSInteger index) {
        
        NSLog(@"%@------%ld",string,(long)index);
    } withSureButtonBlock:^{
        NSLog(@"sure btn");
    }];
    [self.view addSubview:select_view];
```    
    
    




