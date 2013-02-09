align-column
============

jQuery table formatting plugin for decimal alignment and other prettifying of table columns.

Change sloppily right aligned numeric tables from:

https://raw.github.com/ndp/align-column/master/examples/decimals-right.png

to:

https://raw.github.com/ndp/align-column/master/examples/decimals-after-bordered.png


Center based on characters besides a decimal separator:

https://raw.github.com/ndp/align-column/master/examples/other-characters-before.png

into:

https://raw.github.com/ndp/align-column/master/examples/other-characters-after-bordered.png


Scientific tables:

<img src="https://raw.github.com/ndp/align-column/master/examples/chemicals.png">

### Usage

To align numeric columns of an HTML table, use:
```
  $('table').alignColumn(3); // column index
```

Multiple columns can be aligned at once:
```
  $('table').alignColumn([4,5]);
```

By default, columns are aligned by the decimal point (or a best guess as to where it is). To
center by some other character or characters:
```
  $('table').alignColumn(2, {center: ':'});
```



### Related Projects

* TextAlign: http://www.bramstein.com/projects/text-align/  This project has very much
the same goal, and looks like an excellent choice. The main difference is the technique--
it uses spans to align the text, whereas `alignColumn` uses the table cells themselves.
