# Ti.SlideCards
It's a Titanium widget which displays list of cards along with collapsible parent and child view.

![image](docs/slide.gif?raw=true)

## Installation

Add in your *config.json*, under `dependencies`:

```
"dependencies": {
    "SlideCards": "1.0"
}
```

## Usage
```javascript
var slideCards = Alloy.createWidget("SlideCards", {
	cards : [ {
		parentView : Ti.UI.createView({
			height : "450dp",
			width : "300dp",
			backgroundColor : "#C69E40",
		}),
		childView : Ti.UI.createView({
			height : "450dp",
			width : "400dp",
			backgroundColor : "#616B42"
		})
	}],
	style : { 
		height : "500dp", // heignt of container
		width : "800dp", // width of container
		child : {
			height : "200dp", // child cards height || default - container size
			width : "300dp" // child cards width || default - "300dp"
		},
		spacing : [ "10dp", "10dp" ] //padding between cards top/bottom, left/right || default ["10dp", "10dp"]
	}
});
```
