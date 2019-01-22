### 关闭应用程序 \(**app\.close**\)


#### 声明
```lua
app.close(应用程序包名 或 进程号)
```


#### 参数及返回值
- 应用程序包名
    - 文本型，需要关闭的应用的 bundle identifier  
    应用包标识符，可在 **XXT 应用程序\-\-更多\-\-应用列表** 中查看  
- 进程号
    - 整数型，需要关闭的应用的 process identifier \(进程标识符\) 


#### 说明
> 关闭应用程序，参数可以是 应用程序包名 也可以是 进程号，如果应用不在运行则什么都不发生，该操作不会失败  
> 这个关闭应用是不可拒绝的强杀，目标应用在被关闭的时候不会收到任何通知  
> iOS 8 及以上系统版本推荐使用 [`app.quit`](/Handbook/app/app.quit.md) 来代替本函数  

#### 示例  
[`参考 app.run 示例`](/Handbook/app/app.run.md)  
[`参考 app.bundles 示例`](/Handbook/app/app.bundles.md)  

