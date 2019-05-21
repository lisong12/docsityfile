# 删除确认弹窗 #


### 功能介绍 ### 


 删除弹窗组件根据传入的delID判断是否删除弹窗，是，则根据delID与传入的接口信息进行相应信息的删除。
  

### 使用方法 ###

    <sf-delpop :popupdata="popupData" url="https://k-basic-api.szhibu.com/api"></sf-delpop>


### 使用示例 ###
    使用示例后续添加。。。。





### props参数说明 ###

    props: {
      //弹窗信息
      popupdata: {
        type: Object,
        default: function() {
          return {};
        },
        required: true
      },
      // 请求地址
      url: {
        type: String,
        default: '',
        required: true
      },
    }