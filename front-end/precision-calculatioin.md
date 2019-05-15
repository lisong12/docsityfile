
# 精确计算 #

[github数字精确](ttps://github.com/zhangshu360/number-precision)
 
 
    使用javascript精确地执行加法、减法、乘法和除法运算  
      

### 引入 ###

    npm install number-precision --save


### 使用方法 ###

    NP.strip(num)                    // 把数字剥到最接近的右边
    NP.plus(num1, num2, num3, ...)   // 加法，至少需要两个数字
    NP.minus(num1, num2, num3, ...)  // 减法, num1 - num2 - num3
    NP.times(num1, num2, num3, ...)  // 乘法, num1 * num2 * num3
    NP.divide(num1, num2, num3, ...) // 除法, num1 / num2 / num3
    NP.round(num, ratio)             // 根据比例ratio四舍五入


### 实例 ###
    import NP from 'number-precision'
    NP.strip(0.09999999999999998); // = 0.1
    NP.plus(0.1, 0.2);             // = 0.3,  不是  0.30000000000000004
    NP.plus(2.3, 2.4);             // = 4.7,  不是  4.699999999999999
    NP.minus(1.0, 0.9);            // = 0.1,  不是  0.09999999999999998
    NP.times(3, 0.3);              // = 0.9,  不是  0.8999999999999999
    NP.times(0.362, 100);          // = 36.2, 不是  36.199999999999996
    NP.divide(1.21, 1.1);          // = 1.1,  不是  1.0999999999999999
    NP.round(0.105, 2);            // = 0.11, 不是  0.1

   PS : 如果你想在转换为整数的时候去掉xxx是越界的，结果可能不准确，在你的app开始使用这个来关闭边界检查。 

    NP.enableBoundaryChecking(false); // 默认参数为true
  