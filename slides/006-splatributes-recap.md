---
notes: |
  Let's recap a little bit here first, how many people know what splattributes are in general?
---

#### Forwarding Element Modifiers with "Splattributes" (#435)

Splatributes recap:

```html
<!-- /app/templates/components/foo-bar.hbs -->
<div ...attributes>foo bar!</div>
```
<!-- .element: class="fragment" -->

```html
<!-- Usage -->
<FooBar class="foo-bar" />
```
<!-- .element: class="fragment" -->


```html
<!-- Output: -->
<div class="foo-bar">foo bar!</div>
```
<!-- .element: class="fragment" -->
