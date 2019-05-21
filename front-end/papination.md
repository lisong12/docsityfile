# 分页组件 #

### 功能介绍 ### 


   分页组件在数据展示中发挥着特别重要的作用，在组件中涉及到的总页数的多少取决于数据的总条数以及当前显示条数的影响。
  

### 使用方法 ###

        <sf-pagination url="https://k-basic-api.szhibu.com/api/employees" @get-list="getPaginationList"></sf-pagination>

     


### 使用示例 ###
    使用示例后续添加。。。。





### props参数说明 ###

      props: {
    // 请求地址
    url: {
      type: String,
      default: "",
      required: true
    },
    // 请求参数
    query: {
      type: Object,
      default: function() {
        return {};
      }
    },
    // 是否需要添加到路由
    isAppendRouter: {
      type: Boolean,
      default: true
    },
    // 是否自定义点击方法
    isSelf: {
      type: Boolean,
      default: false
    }
  }
