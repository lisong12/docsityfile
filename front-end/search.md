# 搜索组件 #


### 功能介绍 ### 

     搜索组件搜索允许通过查询操作员、操作时间和其他待选特定搜索条件。
   
  

### 使用方法 ###

            <sf-search :search-source="searchSource" @search-result="onSearchResult"></sf-search>



### 使用示例 ###
    使用示例后续添加。。。。





### props参数说明 ###

    props: {
      //搜索的所有条件；必传
    searchSource: {
      type: Array,
      required: true
    },
    //是否需要将搜索条件添加到路由
    isAppendRouter: {
      type: Boolean,
      default: true
    }
  },