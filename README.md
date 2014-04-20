ace编辑器常用操作（中文版） | ace_common_operations_zh
========================
常用操作

- 设置内容/获取内容:

```js
  editor.setValue("新的内容"); // 或 session.setValue
  editor.getValue(); // 或 session.getValue
```
- 获取被选定文本:

```js
editor.session.getTextRange(editor.getSelectionRange());
```

-在光标处添加内容:

```js
editor.insert("新的内容");
```

获取光标所在行的内容:

```js
editor.selection.getCursor();
```
- 跳转到指定行:

```js
editor.gotoLine(行数);
```

- 获取文本总行数:

```js
editor.session.getLength();
```

- 设置缩进长度:

```js
editor.getSession().setTabSize(4);
```

- 设置自动缩进:

```js
editor.getSession().setUseSoftTabs(true);
```

- 设置字体大小:

```js
document.getElementById('editor').style.fontSize='12px';
```

- 设置代码折叠:

```js
editor.getSession().setUseWrapMode(true);
```

- 设置光标所在行高亮:

```js
editor.setHighlightActiveLine(false);
```

- 设置内容只读:

```js
editor.setReadOnly(true);  // false to make it editable
```
