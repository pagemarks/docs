# state 和 生命周期
## state
- 不要直接修改 State
- State 的更新可能是异步的(出于性能考虑，React 可能会把多个 setState() 调用合并成一个调用)
- 要解决这个问题，可以让 setState() 接收一个函数而不是一个对象。这个函数用上一个 state 作为第一个参数，将此次更新被应用时的 props 做为第二个参数
- State 的更新会被合并

数据是向下流动的

### 状态提升
https://zh-hans.reactjs.org/docs/lifting-state-up.html

## lifecycle api

### componentDidMount()
在组件已经被渲染到 DOM 中后运行

### componentWillUnmount()


https://zh-hans.reactjs.org/docs/state-and-lifecycle.html
