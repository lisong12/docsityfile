# 文件上传和显示组件 #

### 功能介绍 ### 

文件上传和显示组件为文件上传功能，支持多个文件上传，默认最大允许上传文件个数为5个，接受多种上传文件类型并并允许更改附件名称。

   
  

### 使用方法 ###

     <sf-upload url="https://k-basic-api.szhibu.com/api/upload"
          :file-list="order.files"
          :data="order.upload_params"
          :is-lock="false"
          :limit="5"
          :is-erp-created="order.is_erp_created"
          @changeData="getPaginationList"
        ></sf-upload>


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
        uploadName:{
            //附件名称 需要更改附件显示名称时上传
            type:String,
            default:'附件'
        },
        showFileList: {
            //是否显示已上传文件列表
            type: Boolean,
            default: true
        },
        fileList: {
            //列表展示上传的文件
            type: Array,
            default: function() {
                return [];
            },
            required: true
        }
