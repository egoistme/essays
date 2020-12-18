## getSeletion的定义
`window.getSelection`用于获取用户选区的文本范围以及相关的参数。

## 使用
可以监听mouseup事件以获取selection对象，所有参数都从selection中获取
```js
document.addEventLitsener('mouseup',this.handleMouseup)
handleMouseup(e){
  const selection = window.getSelection()
}
```
### 常用的参数
1. `selection.toString()` 该函数会返回一个选区的纯文本

```js
const text = selection.toString()
console.log(text)
```

![image-20201218211910508](getSelection%E7%9A%84%E4%BD%BF%E7%94%A8.assets/image-20201218211910508.png)

2. `anchor`、`focus` 他们分别指向选区开始的位置和选区结束的位置，现在先将selection对象打印出来

![image-20201218212822449](getSelection%E7%9A%84%E4%BD%BF%E7%94%A8.assets/image-20201218212822449.png)

​		