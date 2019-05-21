# 修改密码组件 #


### 功能介绍 ### 

修改密码组件在用户忘记密码或需要进行更改密码时进行修改密码的一个流程。用户输入原始密码、新密码、确认密码，在验证密码新密码格式正确及新密码跟确认密码一致时，请求修改密码接口并返回信息，后验证旧密码是否正确，正确则修改成功并关闭弹窗。
   
  

### 使用方法 ###

    <sf-reset-password
          url="https://k-basic-api.szhibu.com/api/user/change-passwd"
          @reset-password="resetPassword()"
        ></sf-reset-password>


### 使用示例 ###
    使用示例后续添加。。。。





### props参数说明 ###

      props:{
    // 修改密码的接口
      url:{
        type: String,
        required: true,
        default: ""
      },
  }