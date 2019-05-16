# 审核组件 #


### 功能介绍 ### 

审核组件主要是在审核订单和生产要素过程中进行，调用审核组件，根据需要更改审核状态。
   
  

### 使用方法 ###

    <sf-check 
            :is-lock="false"
            :order-id="20201"
            @check-status="checkStatus" 
            :button-name="buttonName" 
            url="https://k-basic-api.szhibu.com/api/yarn-stock-in"
            :status="status"></sf-check>


### 使用示例 ###
    使用示例后续添加。。。。





### props参数说明 ###

    props:{
            isLock: {
                //是否编辑状态；false 编辑状态，true 不可编辑
                type: Boolean,
                default: false,
                required: true
            },
            orderId:{
                //订单ID
                type: Number,
                default: -1,
                required: true
            },
            url:{
                //请求地址
                type:String,
                default:'',
                required: true
            },
            newFlow:{
                //是否使用新状态改变 
                type: Boolean,
                default: false
            },
            buttonName:{
                //按钮名称 如newFlow为true则必传
                type:String,
                default:''
            },
            statusName:{
                //状态名称 如newFlow为true则必传
                type:String,
                default:'已确认'
            },
            status:{
                //当前状态 如newFlow为true则必传
                type:Number,
                default:-1
            },
            newStatus:{
                //新状态 如newFlow为true则必传
                type:Number,
                default:-1           
            },
            newType:{
                //状态名称 如newFlow为true则必传
                type:String,
                default:''    
            }

        }