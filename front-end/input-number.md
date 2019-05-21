 # input数字输入组件 #

### 功能介绍 ### 

input数字输入组件默认输入框只能输入两位小数，并且规定只能输入0-9的数字，假若输入字符或其他类型值，输入框将弹出对应规范提示框信息。
 # input数组输入组件 #

### 功能介绍 ### 


   
  

### 使用方法 ###

    <sf-input v-model="value" type="number" class="content-input"></sf-input>

     


### 使用示例 ###
    使用示例后续添加。。。。





### props参数说明 ###

      props: {
    //文本框里的值，默认为零
    value: {
      type: Number | String,
      default: 0,
      required: true
    },
    //类型为text
    type: {
      type: String,
      default: 'text'
    },
    //是否选择只输入两位小数，默认否
    isFixed: {
      type: Boolean,
      default: false
    },
    //默认为可以编辑的状态
    disabled: {
      type: Boolean,
      default: false
    },
    //默认输入字段为可编辑状态，一旦状态改变为只读
    readonly: {
      type: Boolean,
      default: false
    }
  }
     
