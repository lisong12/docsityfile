# 千位符格式化 #

### 功能介绍 ### 

	过滤器，自动给数字添加千位符
	

### 引入 ###
 
	在sfabric-component组件中统一引入


### 使用方法 ###

直接在管道符后面添加 thousand 方法：

    
```html
    <input type="text" :value="numbers | thousand">
```
