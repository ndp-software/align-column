align-column
============

jQuery table formatting plugin for decimal alignment and other prettifying of table columns.

## Features

Transform hard-to-compare right-aligned numeric tables:

<img src="https://raw.github.com/ndp/align-column/master/examples/decimals-right.png">

to easier to read:

<img src="https://raw.github.com/ndp/align-column/master/examples/decimals-after.png">

Center based on characters besides a decimal separator:

<img src="https://raw.github.com/ndp/align-column/master/examples/other-characters-after.png">
<!--img src="https://raw.github.com/ndp/align-column/master/examples/other-characters-before.png"-->

<a href="http://ndpsoftware.com/align-column/examples/chemical_elements.html">Scientific tables</a> can be much improved:

<img src="https://raw.github.com/ndp/align-column/master/examples/chemicals.png">

## Usage

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
* <a href="http://ndpsoftware.com/align-column/examples/typographic_style.html">Table 4.4.4, p. 72</a> from
  <iframe src="http://rcm.amazon.com/e/cm?lt1=_blank&bc1=FFFFFF&IS2=1&npa=1&bg1=FFFFFF&fc1=000000&lc1=BB2401&t=ndso-20&o=1&p=8&l=as1&m=amazon&f=ifr&ref=qf_sp_asin_til&asins=0881792063" style="width:120px;height:240px;" scrolling="no" marginwidth="0" marginheight="0" frameborder="0"></iframe>


## Related Projects

* TextAlign: http://www.bramstein.com/projects/text-align/  This project has very much
the same goal, and looks like an excellent choice. The main difference is the technique--
it uses spans to align the text, whereas `alignColumn` uses the table cells themselves.
