### 深拷贝一个表 \(**table\.deep\_copy**\)


#### 声明
```lua
被复制的表 = table.deep_copy(一个表)
```


#### 参数及返回值
- 一个表
    - 表型，需要拷贝的表
- 被复制的表
    - 表型，返回表的拷贝份


#### 说明
> 迭代拷贝一个表到另外一个表，表中除 function 和 userdata 以外的所有值都会拷贝  
> 拷贝出来的表中如果有循环引用，那么引用关系也会获得拷贝  


#### 示例  
```lua
local _g = table.deep_copy(_G)
```

