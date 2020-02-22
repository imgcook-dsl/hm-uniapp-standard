# imgcook使用说明

> 作者：胡小根

> 邮箱：hxg@haomo-studio.com

## 说明

在imgcook的web编辑器/IDE编辑器中，需要注意以下事项：

* 为了降低生成的组件，在xmind2code中进一步生成代码时产生过多冗余，组件除'dataId'之外的属性，全部放到options对象中。见下面的示例。
* image/text的className将会设置为 props.options.className。例如：

```javascript
props: {
  dataId: {
    type: String,
    default: 'hm-uni-app-demo-component'
  },
  options: {
    type: Object,
    default: function() {
      return {  // 所有的属性将放置在options中，并且生成默认的结果
        image:
          'https://ai-sample.oss-cn-hangzhou.aliyuncs.com/test/47f5f060557b11eabde03dd163252f26.png',
        title: 'Quick Brown Fox Jumps Over',
        author: 'TRAVELLING',
        date: '16 MAY 2016',
        summary:
          'Synth polaroid bitters chillwave pickled. Vegandisrupt tousled, Portland keffiyeh aesthetic food',
        comments: '14 COMMENTS',
        likes: '254 LIKES'
      };
    }
  }
},
```
