---
notes: |
  The reason I wanted to show you that more complicated example is because it's a bit truer to life when you're thinking about forwarding on modifiers. Let's take a look at a more real-world example. And also keeping with the theme of Global Accessiblity Awareness Day, the example is about using labels for Inputs
---

#### Forwarding Element Modifiers with "Splattributes" (#435)

Splatributes for modifiers:

```html
<!-- /app/templates/components/labeled-checkbox.hbs -->
<label for={{@name}}>Subscribe to newsletter</label>
<input
  type="checkbox" name={{@name}}
  id={{@name}} ...attributes
>
```
<!-- .element: class="fragment" -->

```html
<!-- Usage -->
<LabeledCheckbox
  @name="subscribe" {{on 'click' this.subscribe}}/>
```
<!-- .element: class="fragment" -->


```html
<!-- Output: -->
<label for="subscribe">Subscribe to newsletter</label>
<input type="checkbox" name="subscribe"
  id="subscribe" onclick="whateverFunction(🙈)">
```
