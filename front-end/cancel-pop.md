# 取消订单弹窗组件 #


### 功能介绍 ### 

取消订单组件是销售订单根据客户订单要求录入产品信息以及生产中所需工艺流程、注意事项等信息后，根据需要对订单进行取消操作的一个流程。
   
  

### 使用方法 ###

     <sf-cancel
          url="http://sfabric.sm/api/sales-fill-cloth-order/8755/cancel"
          discancel-url="http://sfabric.sm/api/sales-fill-cloth-order/8755/discancel"
          :cancel-status="cancelStatus"
          :complex-info="complexInfo"
          @set-cancel-info="setCancelInfo"
          @handel-open-cancel="handelOpenCancel"
        >
        </sf-cancel>


### 使用示例 ###
    使用示例后续添加。。。。





### props参数说明 ###

      props: {
      // 取消订单的接口
      url:{
        type: String,
        required: true,
        default: ""
      },
      // 恢复订单的接口
      discancelUrl:{
        type: String,
        required: true,
        default: ""
      },
      // 取消状态
      cancelStatus:{
        type: Boolean,
        required: true,
        default: false
      },
      // 下拉选框的信息
      complexInfo:{
        type: Array,
        default: function(){
          return []
        }
      },
    }