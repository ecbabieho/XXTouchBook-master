### touch 示例代码


#### 示例  
```lua
-- 可以这样：
touch.on(306, 300):step_len(2):step_delay(0):move(350, 800):msleep(1000):off()
--
-- 上面那个例子也能写成这样：
touch.on(306, 300)  -- 模拟手指在 306,300 这个坐标点接触屏幕
	:step_len(2)   -- 设置移动步长为 2
	:step_delay(0) -- 设置移动每步延迟为 0
	:move(350, 800) -- 以上面两个参数所设置移动到 350,800 这个坐标
	:msleep(1000)   -- 等 1000 毫秒 (也就是 1 秒) 
:off()             -- 手指离开屏幕
--
-- 或是这样：
local te = touch.on(306,300)
te:step_len(2)
te:step_delay(0)
te:move(350, 800)
te:msleep(1000)
te:off()
--
-- 通常情况下，滑动代码可以写成这样
touch.on(306, 300)
	:move(350, 800)
	:msleep(1000)
:off()
--
-- 等效于
touch.on(306, 300):move(350, 800):msleep(1000):off()
--
-- 也可以这样用于模拟轻触屏幕一次
touch.on(306, 300):msleep(30):off()
--
```


#### 快速精确滑动技巧
```lua
-- 快速精确滑动可能需要一些技巧，看下面的例子以及注释
touch.on(125, 2000) -- 在起始坐标按下
	:step_len(10)   -- 步长设长以便加速滑动
	:move(125, 555) -- 快速移动到接近目标位置
	:step_len(1)    -- 步长设短缓冲防止惯性
	:move(125, 505) -- 慢速移动目标位置
	:delay(100)     -- 抬起前等待一段时间
:off()              -- 抬起手指
```

