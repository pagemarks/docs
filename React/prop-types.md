# prop-types

## install
```shell
npm install prop-types
```

## use
```js
ComponentName.propTypes = {
  key: PropTypes.string.isRequired,
  key2: PropTypes.number,
}
```

## types
string | array | bool | func | number | object | node | element

### PropTypes.instanceOf(ComponentName)

### PropTypes.oneOf(array: set)

### PropTypes.oneOfType(array: types)

### PropTypes.arrayOf(type)

### PropTypes.objectOf(type)

### PropTypes.shape(object keysTypeMap)
至少含相关定义属性及其类型

## custom validator

```js
function customValidator(props, propName, componentName) {
  // here, propName === "myCustomProp"
  if (props[propName].length !== 3) {
    return new Error(
      'Invalid prop `' + propName + '` supplied to' +
      ' `' + componentName + '`. Length is not 3.'
    );
  }
}

const CustomTest = ({ myCustomProp }) => (
  <span>{myCustomProp}</span>
);
CustomTest.propTypes = {
  myCustomProp: customValidator
}
```
