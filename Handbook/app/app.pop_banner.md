### 弹出一个应用通知 \(**app\.pop\_banner**\)


#### 声明
```lua
app.pop_banner(应用程序包名, 标题, 内容)
```


#### 参数及返回值  
- 应用程序包名
    - 文本型，应用的 bundle identifier  
    应用包标识符，可在 **XXT 应用程序\-\-更多\-\-应用列表** 中查看   
- 标题
    - 文本型，通知的标题
- 内容
    - 文本型，通知的内容


#### 说明
> **软件版本在 1\.1\.3\-1 或以上方可使用**  


#### 示例  
```lua
app.pop_banner('com.tencent.mqq', 'QQ', '[QQ红包]您收到一个假红包')
```

