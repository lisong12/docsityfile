 # 注意事项组件 #


### 功能介绍 ### 

通过点击添加注意事项按钮，发送注意事项弹窗，在弹窗内操作新建事项、编辑事项、删除事项对注意事项进行管理。已编辑事项将展示在组件文本框中，点击文本框将内容全部展开，点击文本框之外的地方收起。
  

### 使用方法 ###

    <sf-attention
          url="http://sfabric.sm/api/remarks?type=3"
          update-atte-url="http://sfabric.sm/api/remarks/1"
          :attention="attention"
          :editable="true"
          @get-attention-info="getAttentionInfo"
        ></sf-attention>


### 使用示例 ###
    使用示例后续添加。。。。 





### props参数说明 ###

       props:{
     // 获取注意事项的接口
      url:{
        type: String,
        default: ""
      },
      // 是否能编辑
      editable:{
        type: Boolean,
        required: true,
        default: false
      },
      // 绑定（展示）的值
      attention:{
        type: String,
        required: true,
        default: ""
      },
      //更新注意事项数据的接口
      updateAtteUrl:{
        type: String,
        default: ""
      },
    }