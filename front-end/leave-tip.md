# 离开页面提示组件 #

### 功能介绍 ### 

  离开页面提示组件，是在页面编辑状态下，弹出的确认提示窗口。其中必须对页面内容进行检测，若编辑内容没有保存，需弹出确认提示信息窗口。
页面在编辑状态时，点击浏览器后退按钮，或者点击菜单按钮跳转其他路由时给出消息提示。
   
  

### 使用方法 ###

     <sf-leave :route-obj="routeObj" :flagstatus="flag" @reset-flag="resetFlag"></sf-leave>
 


### 使用示例 ###
    使用示例后续添加。。。。





### props参数说明 ###

     props:{
      routeObj:{
        type:Object,
        default:null
      },
      flagstatus: {
        type: Boolean,
        default: false
      }
    },