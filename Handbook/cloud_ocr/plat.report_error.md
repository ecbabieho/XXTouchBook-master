### 提交错误的识别 \(**plat\.report\_error**\)


#### 声明
```lua
提交成败, 状态信息 = plat.report_error([ 结果标签 ])
```


#### 参数及返回值
- plat
    - 表型，云打码平台对象，可以使用 [初始化一个云打码平台](/Handbook/cloud_ocr/cloud_ocr.ocr.md) 来获得
- **结果标签**
    - 文本型，可选参数，对应打码返回的 **结果标签**，默认提交上次成功的 **结果标签**
- 提交成败
    - 布尔型，返回是否提交成功
- 状态信息
    - 文本型 或 nil，正确返回状态信息 (可不判断) ，错误返回 nil


#### 说明
> 提交错误的识别到打码平台  


#### 示例  
[`本章最后`](/Handbook/cloud_ocr/samples.md)  
