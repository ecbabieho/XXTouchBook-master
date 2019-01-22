### 给对话框加上一个数值选择器 \(**:add\_range**\)


#### 声明
```lua
对话框对象 = 对话框对象:add_range(范围选择器标签, 范围选择器参数 [, 默认位置 ])
```


#### 参数及返回值
- 范围选择器标签
    - 文本型，数值选择器标题标签显示的文本
- 范围选择器参数
    - 表型，用于描述范围以及步进的一个表，格式为 \{最小值, 最大值, 步进值\}
        - 最小值
            实数型，为数值选择条最左边的位置
        - 最大值
            实数型，为数值选择条最右边的位置
        - 步进值
            实数型，可选参数，为选择条拖动的最小单位，默认为 1
- 默认位置
    - 实数型，可选参数，默认值，默认为最小值
- 对话框对象
    - 对话框，返回对话框本身
- 使用 :show\(\) 返回类型
    - 实数型，返回所选择的数字


#### 说明
> **这个方法在 1\.1\.1\-1 版以上方可使用**  
> 给对话框加上一个数值选择器  


#### 示例  
```lua
local c, s = dialog():add_range('一个数值', {222, 666, 1}, 333):show()
sys.alert('数值是：'..s['一个数值'])
```
**注**：上述代码中使用了非本章函数 [`sys.alert`](/Handbook/sys/sys.alert.md)  


#### 完整示例
[`本章结尾 :show() `](/Handbook/dialog/_show.md)  
