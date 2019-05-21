# 自动添加货币符号 #

### 功能介绍 ### 

	过滤器，自动在数字前面加上货币符号
	

### 引入 ###
 
	在sfabric-component组件中统一引入


### 使用方法 ###

直接在管道符后面添加 thousand 方法：

    
```html
    <p>{{number | currency('$')}}</p>
```

```html
	<p>{{number | thousand | currency('$')}}</p>
```