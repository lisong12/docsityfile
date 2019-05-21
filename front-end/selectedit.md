# 可编辑下拉组件 #

### 功能介绍 ### 

可编辑下拉框在点击下拉框之后，可以根据需要进行编辑或搜索，选择在下拉框中需要的数据。
   
  

### 使用方法 ###

     <sf-selectedit
          :select-data="$assistKey.selectData"
          value-first="name"
          value-last="address"
          :disabled="false"
          :filterable="true"
          @select-edit-val="selectEditVal"
        ></sf-selectedit>


### 使用示例 ###
    使用示例后续添加。。。。





### props参数说明 ###

       props: {
    selectData: {
      type: Array,
      default: function () { 
        return []
       }
    },
    valueFirst: {
      type: String,
      required: true
    },
    index: {
      type: [Number,String],
      default: "-1"
    },
    valueLast: {
      type: String,
      default: ""
    },
    disabled: {
      type: Boolean,
      default: false
    },
    filterable: {
      type: Boolean,
      default: true
    },
    size: {
      type:String,
      default: "small"
    },
  }
