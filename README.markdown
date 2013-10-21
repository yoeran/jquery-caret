# jQuery Caret

This is a very simple lightweight plugin to allow you to move the
caret (or cursor) position in an &lt;input /&gt; or &lt;textarea&gt;
element and/or modify text according to position and selection.

## $.fn.caret()

Use this method with no parameters to get the current position of the
caret within the first element matched.

```javascript
var position = $('input').caret();
```

## $.fn.caret( index , [ offset ] )

This methods first parameter is the index of where you want to move
the caret to. In order to move to an index, index must be an integer.

Alternatively you can pass a string as an index and it will be used
via .indexOf() the element's value to get an index to move to.

The second parameter is to be used to move the caret to an offset of
the index. When set to true, it will move the cursor after the string
if a string was passed.

```javascript
$('input').caret(10);
```

## $.fn.caretToEnd()

This method moves the caret to the end of the content within your
element, also for your convenience.

```javascript
$('input').caretToEnd();
```

## $.fn.insertAtCaret()

This method inserts text at the current caret position.

```javascript
$('textarea').insertAtCaret('text');
```

## $.fn.replaceAtCaret()

This method replaces the selected text and will be maintained if you add two % signs in your string.
You could use this to surround a selected text with <strong>-tags (or MarkDown codes).

```javascript
$('textarea').replaceAtCaret('<strong>%%</strong>');
```

## Author(s)

* Luke Morton ([original](https://github.com/DrPheltRight/jquery-caret))
* Pat Benatar ([insertAtCaret fn](https://github.com/patbenatar/jquery-caret))
* Yoeran Luteijn ([replaceAtCaret fn](https://github.com/yoeran/jquery-caret))

## License

MIT
