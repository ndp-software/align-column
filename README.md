align-column
============

jQuery table formatting plugin for decimal alignment and other prettifying of table columns.

## Features

Transform hard-to-compare right-aligned numeric tables:

<img src="https://raw.github.com/ndp/align-column/master/examples/decimals-right.png">

to easier to read:

<img src="https://raw.github.com/ndp/align-column/master/examples/decimals-after.png">

Center based on characters besides a decimal separator:

<img src="https://raw.github.com/ndp/align-column/master/examples/other-characters-after-bordered.png">
<!--img src="https://raw.github.com/ndp/align-column/master/examples/other-characters-before.png"-->

<a href="http://ndpsoftware.com/align-column/examples/chemical_elements.html">Scientific tables</a> can be much improved:

<img src="https://raw.github.com/ndp/align-column/master/examples/chemicals.png">

## Usage

```
  <script type="text/javascript" src=".../jquery...min.js"></script>
  <script type="text/javascript" src=".../jquery.align-column.js"></script>
```

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

## Examples

* <a href="http://ndpsoftware.com/align-column/examples/chemical_elements.html">Wikipedia table of chemical elements</a>
* <a href="http://ndpsoftware.com/align-column/examples/typographic_style.html">Table 4.4.4, p. 72</a> from <a href="http://www.amazon.com/gp/product/0881792063/ref=as_li_qf_sp_asin_tl?p ie=UTF8&camp=1789&creative=9325&creativeASIN=0881792063&linkCode=as2&tag=ndso-20">The Elements of Typographic Style</a><img src="http://www.assoc-amazon.com/e/ir?t=ndso-20&l=as2&o=1&a=0881792063" width="1" height="1" border="0" alt="" style="border:none !important; margin:0px !important;" /> 

## Related Projects

* TextAlign: http://www.bramstein.com/projects/text-align/  This project has very much
the same goal, and looks like an excellent choice. The main difference is the technique--
it uses spans to align the text, whereas `alignColumn` uses the table cells themselves.
