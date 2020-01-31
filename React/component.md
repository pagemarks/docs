# 组件

## 函数式组件(stateless)
接收唯一带有数据的 “props”（代表属性）对象与并返回一个 React 元素

```jsx
function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}
```

## class组件(statefull)

```jsx
class Welcome extends React.Component {
  render() {
    return <h1>Hello, {this.props.name}</h1>;
  }
}
```

## 组合组件
组件可以在其输出中引用其他组件。这就可以让我们用同一组件来抽象出任意层次的细节

```jsx
function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}

function App() {
  return (
    <div>
      <Welcome name="Sara" />
      <Welcome name="Cahal" />
      <Welcome name="Edite" />
    </div>
  );
}

ReactDOM.render(
  <App />,
  document.getElementById('root')
);
```
### 组合VS继承
https://zh-hans.reactjs.org/docs/composition-vs-inheritance.html

- 所有 React 组件都必须像纯函数一样保护它们的 props 不被更改


https://zh-hans.reactjs.org/docs/components-and-props.html
