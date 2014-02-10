ace_common_operations_zh
========================
Common Operations

- Set and get content:

```js
  editor.setValue("the new text here"); // or session.setValue
  editor.getValue(); // or session.getValue
```
- Get selected text:

```js
editor.session.getTextRange(editor.getSelectionRange());
```

-Insert at cursor:

```js
editor.insert("Something cool");
```

Get the current cursor line and column:

```js
editor.selection.getCursor();
```
- Go to a line:

```js
editor.gotoLine(lineNumber);
```

- Get total number of lines:

```js
editor.session.getLength();
```

- Set the default tab size:

```js
editor.getSession().setTabSize(4);
```

- Use soft tabs:

```js
editor.getSession().setUseSoftTabs(true);
```

- Set the font size:

```js
document.getElementById('editor').style.fontSize='12px';
```

- Toggle word wrapping:

```js
editor.getSession().setUseWrapMode(true);
```

- Set line highlighting:

```js
editor.setHighlightActiveLine(false);
```

- Set the print margin visibility:

```js
editor.setShowPrintMargin(false);
```

- Set the editor to read-only:

```js
editor.setReadOnly(true);  // false to make it editable
```
