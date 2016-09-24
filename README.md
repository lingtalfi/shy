Shy
=================
2016-09-24




Shy is a css convention for implementing fast css selectors.




Documentation
-----------------

shy is a system for naming your dom target elements based on fast selectors.

shy only uses/is applied to css classes.

The shy system is as follow:
 
- the default case is camelCase, for instance: closeBtn
- hierarchy is induced by one underscore between the parent and its child, for instance: container_child_subChild
- namespace is induced by two underscores between the "module" name and the "target" name, for instance: myModule__logo
- states are induced by two dashes between the "module" name and the "state" name, for instance navDrawer--open 


I recommend that you never use the hierarchy notation, but use namespace notation instead.






Random thoughts
-----------------------
You shouldn't use hierarchy, but rather namespaces.

That's because hierarchy tends to be more verbose, and so in the end it makes more bytes to download.

For instance, using the hierarchy system, you can end up with this type of class:

```html
<div class="container_header_topDiv_logo"></div>
```

If you were using the namespace system, you could just use something like that:

```html
<div class="myModule__logo"></div>
```






Why shy?
-------------

I don't know, I just like the should of it,
and that's the first idea that came in.
