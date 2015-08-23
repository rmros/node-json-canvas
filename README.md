# node-json-canvas
Describe a node canvas image with JSON.

Built so that I can make all figures for my dissertation declarative.

Makes images like this

![](https://github.com/danprince/node-json-canvas/raw/master/example/example_a.png?raw=true)

From files like this

```json
{
  "config": {
    "width": 500,
    "height": 500,
    "background": "#fff"
  },
  "objects": [
    {
      "name": "path",
      "points": [[50, 50], [100, 100]],
      "stroke": true,
      "context": {
        "strokeStyle": "red",
        "lineWidth": 3
      }
    },
    {
      "name": "rect",
      "x1": 50,
      "y1": 50,
      "x2": 400,
      "y2": 400,
      "stroke": true,
      "context": {
        "strokeStyle": "blue",
        "lineWidth": 2
      }
    },
    {
      "name": "text",
      "text": "Hello world",
      "fill": true,
      "x": 100,
      "y": 100,
      "context": {
        "font": "20px serif",
        "fillStyle": "#000"
      }
    }
  ]
}
```

