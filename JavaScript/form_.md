elements

submit() 不触发form的submit事件
reset() 触发form的reset事件
*form下不能有name或id为reset的表单元素,否则覆盖reset()方法


# 交互优化设计

- form btn submit 原生跳转带参数

- form submit 自动监听回车事件 

## codes
- 表单序列化
- 表单验证
    * 统一文案和UI
    * 异步验证(用户名)
    * 多重类型验证
    * 自定义验证器
    