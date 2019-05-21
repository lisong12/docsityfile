
# 精确计算 #

 
 ### 功能介绍 ### 
 

    使用javascript精确地执行加法、减法、乘法和除法等算术运算


### 引入 ###

    在sfabric-component组件中统一引入
    可以通过this.$math调用


### 使用方法 ###

```js
    this.$math.plus(num1, num2, num3, ...)   // 加法，至少需要两个数字
    this.$math.minus(num1, num2, num3, ...)  // 减法, num1 - num2 - num3
    this.$math.times(num1, num2, num3, ...)  // 乘法, num1 * num2 * num3
    this.$math.divide(num1, num2, num3, ...) // 除法, num1 / num2 / num3
    this.$math.round(num, ratio)             // 根据比例ratio四舍五入,ratio是需要保留的小数位数

```

### 使用实例 ###

```js
    this.$math.plus(0.1, 0.2);             // = 0.3,  不是  0.30000000000000004
    this.$math.plus(2.3, 2.4);             // = 4.7,  不是  4.699999999999999
    this.$math.minus(1.0, 0.9);            // = 0.1,  不是  0.09999999999999998
    this.$math.times(3, 0.3);              // = 0.9,  不是  0.8999999999999999
    this.$math.times(0.362, 100);          // = 36.2, 不是  36.199999999999996
    this.$math.divide(1.21, 1.1);          // = 1.1,  不是  1.0999999999999999
    this.$math.round(0.105, 2);            // = 0.11, 不是  0.1

```