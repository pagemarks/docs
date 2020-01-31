# jsx
js语法扩展,模板+逻辑

## {}
- 属性中嵌入表达式时,不要用引号.属性值要么用引号要么表达式
- 注释须放在{}里,支持js // /* */ 

### ()
包裹元素,return

## 条件渲染
- if () else
- condition && template
- condition ? template: template
- 返回null,不渲染

## list
### map

### key
key 帮助 React 识别哪些元素改变了，比如被添加或删除.

一个元素的 key 最好是这个元素在列表中拥有的一个独一无二的字符串。通常，我们使用数据中的 id 来作为元素的 key

数组元素中使用的 key 在其兄弟节点之间应该是独一无二的

## form
### input,select,textarea
通常自己维护 state，并根据用户输入进行更新。而在 React 中，可变状态（mutable state）通常保存在组件的 state 属性中，并且只能通过使用 setState()来更新

- input file 只读,不能用state
- checkbox checked=true/flase

```jsx
class NameForm extends React.Component {
  constructor(props) {
    super(props);
    this.state = {value: ''};

    this.handleChange = this.handleChange.bind(this);
    this.handleSubmit = this.handleSubmit.bind(this);
  }

  handleChange(event) {
    this.setState({value: event.target.value});
  }

  handleSubmit(event) {
    alert('提交的名字: ' + this.state.value);
    event.preventDefault();
  }

  render() {
    return (
      <form onSubmit={this.handleSubmit}>
        <label>
          名字:
          <input type="text" value={this.state.value} onChange={this.handleChange} />
           // <textarea value={this.state.value} onChange={this.handleChange} />
        </label>
        
        <input type="submit" value="提交" />
      </form>
    );
  }
}
```

## camelCase attribute name
jsx语法更贴近JavaScript,而不是html.所以相关多单词属性名须用camelCase命名.className,tabIndex

## 自闭合</>

### 自定义组件首字母大写

## 防注入攻击
直接插入数据,会进行转义,有效防止XSS攻击

- https://zh-hans.reactjs.org/docs/introducing-jsx.html
- https://zh-hans.reactjs.org/docs/conditional-rendering.html
- https://zh-hans.reactjs.org/docs/lists-and-keys.html
- https://zh-hans.reactjs.org/docs/forms.html
