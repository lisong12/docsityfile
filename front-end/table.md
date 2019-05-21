# 列表组件 #


### 功能介绍 ### 
    
    列表框组件作为良好的数据展示平台，使用数组作为初始化列表框参数，将要展示的数据通过以列表的形式展示出来。
   
  

### 使用方法 ###

    <sf-table :table-data="$assistKey.tableData" :table-tools="$assistKey.tableTools"></sf-table>



### 使用示例 ###
    使用示例后续添加。。。。





### props参数说明 ###

         props: {
            // 列表操作及头部
            tableTools: {
              type: Object,
              default: function() {
                return {};
              },
              required: true
            },
            // 列表数据源
            tableData: {
              type: Array,
              default: function() {
                return [];
              },
              required: true
            },
            // 排序参数及顺序
            defaultSort: {
              type: Object,
              default: function() {
                return {};
              }
            }
          },