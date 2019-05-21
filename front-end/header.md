# 头部组件 #


### 功能介绍 ### 

登录组件库网址，进入首页。该头部组件就是首页的头部，包含公司的logo、搜索框、邮件、管理员以及菜单列表功能。
  
  

### 使用方法 ###

        <sf-header
		      :no-read="noRead"
		      :get-all-company-url="'/user/user_all_company'"
		      :update-company-url="'/user/update_company/'"
		      @returnHome="returnHome"
		      @updateCompany="updateCompany()"
	      >
	      </sf-header>


### 使用示例 ###
    使用示例后续添加。。。。





### props参数说明 ###

       props:{
          //非必传；未读消息条数;
      noRead:{
        type: String,
        default: '',
      },
          //   必传；超管登录时获取所有公司的接口路径;
      getAllCompanyUrl :{
        type: String,
        default: '',
        required: true,
      },
          //必传；超管切换公司的接口路径;
		  updateCompanyUrl:{
        type: String,
        default: '',
        required: true,
		  }
	  },