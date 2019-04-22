# SASS / LESS

* [SASS Style Guide](http://css-tricks.com/sass-style-guide/)

## Mixin, Extend, Placeholders
http://krasimirtsonev.com/blog/article/SASS-mixins-extends-and-placeholders-differences-use-cases

Mixin vs Extend
- Mixin: composition (different kind of things composite together), similar to "has-a" in OO.
  - _ex_: a `.dance-on-hover-btn` and a `.dance-on-hover-link` could both **mixin** the same `.dance-on-hover` behavior
- Extend is about inheritance (same kind of things in the inheritance chain), similar to "is-a" in OO.
  - _ex_: a `.round-secondary-btn` **extends** from a `.-secondary-btn`

 Real world example:
 ```css
 .table-header {
  text-transform: uppercase;
  color: gray;
}

// order-history-header is a kind of table-header, thus using 'extend'
.order-history:extend(.table-header) {
}
 ```
