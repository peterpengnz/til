## Child selectors

A `child selector` matches when an element is the child of some element.
A child selector is made up of two or more selectors separated by `>`.

The following rule sets the style of all `P` elements that are children of `BODY`:

```
body > P { line-height: 1.3 }
```

The following example combines descendant selectors and child selectors:

```
div ol>li p
```

It matches a `P` element that is a descendant of an `LI`; 
the `LI` element must be the child of an `OL` element; 
the `OL` element must be a descendant of a `DIV`. 

Notice that the optional white space around the `>` combinator has been left out.

[Reference](http://www.w3.org/TR/css3-selectors/#selectors)
