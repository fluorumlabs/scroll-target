[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/fluorumlabs/scroll-target)
[![Published on Vaadin  Directory](https://img.shields.io/badge/Vaadin%20Directory-published-00b4f0.svg)](https://vaadin.com/directory/component/fluorumlabsscroll-target)
[![Latest version on vaadin.com/directory](https://img.shields.io/vaadin-directory/v/fluorumlabsscroll-target.svg)](https://vaadin.com/directory/component/fluorumlabsscroll-target)
[![Rating on vaadin.com/directory](https://img.shields.io/vaadin-directory/rating/fluorumlabsscroll-target.svg)](https://vaadin.com/directory/component/fluorumlabsscroll-target)
[![](https://data.jsdelivr.com/v1/package/gh/fluorumlabs/scroll-target/badge)](https://www.jsdelivr.com/package/gh/fluorumlabs/scroll-target)

# &lt;scroll-target&gt;

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

![ScrollTarget demo recording](https://raw.githubusercontent.com/fluorumlabs/scroll-target-for-flow/master/demo-recording.gif)

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

```html
<link rel="import" href="//cdn.jsdelivr.net/gh/fluorumlabs/scroll-target@1.0.0/scroll-target.html">
```

Or, if you prefer having it locally,

```bash
bower install --save fluorumlabs/scroll-target"#^1.0.0"
```

```html
<link rel="import" href="bower_components/scroll-target/scroll-target.html">
```

