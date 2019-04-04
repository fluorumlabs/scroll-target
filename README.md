# &lt;scroll-target&gt;

[Live Demo ↗]()

&lt;scroll-target&gt; is a really simple web component for making scrolling easier. 
ll you need to do is to wrap the content you want to scroll to and call `ensureVisibility()`:

```html
<button onclick="document.getElementById('target').ensureVisibility()">Click me!</button>

...

<scroll-target id="target">
    <h2>I'm the content you want to see</h2>
    <p>...</p>
</scroll-target>
```

## Properties

```html
<scroll-target top-offset="<offset_in_pixels>">
```

`top-offset` defines a space that should be reserved for fixed top menu when scrolling. `0` by default. Can be changed in runtime by calling `scrollTargetElement.setTopOffset(...)`.

## Methods

```javascript
scrollTargetElement.setTopOffset(<offset_in_pixels>);
```

`setTopOffset` defines a space that should be reserved for fixed top menu when scrolling. Can be set via `top-offset` attribute.

```javascript
scrollTargetElement.ensureVisibility(<delay_in_milliseconds>);
```

`ensureVisibility` scrolls to make the wrapped content visible. If optional `<delay_in_milliseconds>` is specified, scrolling will be delayed by specified amount of time.

# Getting started

```bash
bower install --save fluorumlabs/scroll-target"#^1.0.0"
```
