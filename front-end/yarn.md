# 纱属性弹窗组件 #


### 功能介绍 ### 

 
纱属性弹窗组件分为短纤和长纤两个弹窗组件，在短纤中选择配棉和可染属性，其他的可录入在输入框中。配选完成后，点击保存，将显示出所选短纤属性。在长纤中亦是如此录入信息。

   
  

### 使用方法 ###

     <sf-yarn
            :yarn-type="1"
            :brightness="{
              id: 42,
              name: '透明'
            }"
            other=""
            url="https://cloth-api.szhibu.com/api/yarn-type/attribute?type=1"
            @yarn-result="onYarnResult"
           ></sf-yarn>


### 使用示例 ###
    使用示例后续添加。。。。


### props参数说明 ###

     props: {
      //纱属性类型  2 短纤  1 长纤 必填
    yarnType: {
      type: Number, 
      required: true
    },
    //请求地址 必填
    url: {  
      type: String,
      required: true
    },
    //配棉 可填 
    contton: {
      type: Object,
      default: function () {
        return {
          name: '',
          id: null
        }
      }
    },
    //可染属性 可填
    properties: {
      type: Object,
      default: function () {
        return {
          name: '',
          id: null
        }
      }
    },
    //亮度 可填  
    brightness: {
      type: Object,
      default: function () {
        return {
          name: '',
          id: null
        }
      }
    },
    //其它 必填 
      other: {
      type: String,
      required: true
    },
    //下标值 可填
    firstIndex: {
      type: Number,
      default: function () {
        return -1
      }
    },
    //下标值 可填
    secondIndex: {
      type: Number,
      default: function () {
        return -1
      }
    }
  }