---
notes: |
  Now to make sure you know how they work in a more complicated example:
---

#### Forwarding Element Modifiers with "Splattributes" (#435)

Splatributes pro mode:

```html
<!-- /app/templates/components/foo-bar.hbs -->
<div class="wrapper" ...attributes>
  <h2>Foo title</h2>
  <p ...attributes>foo bar!</p>
</div>
```
<!-- .element: class="fragment" -->

```html
<!-- Usage -->
<FooBar class="foo-bar" data-thing="wow"/>
```
<!-- .element: class="fragment" -->


```html
<!-- Output: -->
<div class="wrapper foo-bar" data-thing="wow">
  <h2>Foo title</h2>
  <p class="foo-bar" data-thing="wow">foo bar!</p>
</div>
```
<!-- .element: class="fragment" -->
