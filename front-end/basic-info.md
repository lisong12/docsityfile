# 下拉组件 #

### 功能介绍 ### 

下拉组件可以从下拉列表的多个项目中选择其中一项。在正常状态下，只显示一个当前选定的列表项，当点击下拉列表时，会下拉出所有的列表项目以供选择。
  

### 使用方法 ###

     <sf-select
          :is-lock="false"
          :value="name"
          :is-multiple="true"
          url="https://k-basic-api.szhibu.com/api/knitIndex/yarn?status=1"
          attribute="name"
          item-value-frist="abbreviation"
          @set-select-val="selectVal"
        ></sf-select>


### 使用示例 ###
    使用示例后续添加。。。。





### props参数说明 ###

       props: {
    //绑定的字段
    value: {
      type: [Number, String, Array],
      default: "",
      required: true
    },
    // 是否禁用
    isLock: {
      type: Boolean,
      default: false,
      required: true
    },
    // 请求地址
    url: {
      type: String,
      default: ""
    },
    // 下拉数据
    dataOrigin: {
      type: Array,
      default: function() {
        return [];
      }
    },
    // 是否多选
    isMultiple: {
      type: Boolean,
      default: false
    },
    // 多选时，选择的值  ？？？？？？？？？
    changeVal: {
      type: [Number, String],
      default: "name"
    },
    // 对应绑定的字段名
    attribute: {
      type: String,
      default: "",
      required: true
    },
    // 搜索对应的字段 默认按pinyin搜索
    serverValue: {
      type: String,
      default: "pinyin"
    },
    // 循环渲染中的key
    itemKey: {
      type: String,
      default: "id"
    },
    // 循环渲染中 需要首先渲染的值 默认渲染 abbreviation字段
    itemValueFrist: {
      type: String,
      default: "abbreviation"
    },
    //循环渲染中 需要最后显示的值 （在itemValueFrist为空情况下）
    itemValueEnd: {
      type: String,
      default: "name"
    },
    //分录中，对应的index
    firstIndex: {
      type: [Number, String],
      default: "0"
    },
    //分录中，第firstIndex行 对应 secondIndex行 的index
    secondIndex: {
      type: [Number, String],
      default: "0"
    }
  },