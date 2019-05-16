# 上机工艺弹窗组件 #


### 功能介绍 ### 


  上机工艺是订单在生产流程织模块的织布方式。通过在页面上绑定上机工艺数据，添加一个点击事件@click="showCraftWrap"用来控制上机工艺弹窗的显示；该弹窗通过创建新的上机工艺模板、勾选需要的上机工艺，来确定该订单的织布方式。
  

### 使用方法###

    <sf-craft-wrap
        :craft-visible="craftVisible"
        :craft-text="craftText"
        url="http://sfabric.sm/api/fabric-craft"
        @set-fabric-craft="setFabricCraft"
        @reset-craft-visible="resetCraftVisible"
    ></sf-craft-wrap>


### 使用示例 ###
    使用示例后续添加。。。。





### props参数说明 ###

     props:{
      //获取上机工艺的接口
      url:{
        type: String,
        required: true,
        default: ""
      },
      //控制上机工艺弹窗显示与关闭
      craftVisible:{
        type: Boolean,
        required: true,
        default: false
      },
      //父组件传进来的上机工艺
      craftText:{
        type: String,
        required: false,
        default: ""
      },
    },