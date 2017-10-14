# jsZoom.js
网页放大插件,主要针对的是容器,不单单是图片
# js-zoom.js
网页放大插件,主要针对的是容器,不单单是图片
# zoom.js

Enables a minimal JS API for zooming in on specific points or DOM elements.

*Note that this is only a proof of concept so don't use it for anything important. Does not work in IE, yet.*

[Try out the demo](http://lab.hakim.se/zoom-js/).

# Usage

#### Zoom in on an element:

```javascript
  zoom.to({
    element: document.querySelector( 'img' )
  });
```

Additional options:

```
  zoom.to({
    element: document.querySelector( 'img' ),

    // Amount of empty space around zoomed element
    padding: 20,

    // Function to call once zooming completes
    callback: function() { /* ... */ }
  });
```

#### Zoom in on a point:

```javascript
  zoom.to({
    x: 100,
    y: 200,
    width: 300,
    height: 300
  });
```

```javascript
  zoom.to({
    x: 100,
    y: 200,
    scale: 3
  });
```

#### Reset
```javascript
  zoom.out();
```
