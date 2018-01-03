# jQuery-Colorwheel
A jQuery Widget for selecting a color from a predefined palette.

## Usage
### Basic
![jQuery Colorwheel](https://raw.githubusercontent.com/bamberjp/jQuery-Colorwheel/master/images/colorwheel_simple.png "jQuery Colorwheel")

Include the plugin and it's stylesheet after jQuery.
```html
<script src="../dist/jquery.colorwheel.js"></script>
<link rel="stylesheet" type="text/css" href="../dist/jquery.colorwheel.css">
```
In the body of the document create a container.
```html
<div id="widget"></div>
```
Define the containers dimensions.
```css
<style>
#widget {
	display: block;
	width: 200px;
	height: 200px;	
 }
</style>
```
Initialize the widget
```javascript
jQuery(document).ready(function($) {
  $("#widget").colorwheel();
});
```
### Custom Palette
```javascript
jQuery(document).ready(function($) {
  $("#widget").colorwheel('init',
    ['000000', 
		 '111111', 
		 '222222', 
		 '333333', 
		 '444444', 
		 '555555', 
		 '666666', 
		 '777777', 
		 '888888', 
		 '999999', 
		 'aaaaaa', 
		 'bbbbbb', 
		 'cccccc', 
		 'dddddd', 
		 'eeeeee', 
		 'ffffff']
  );
});
```
![jQuery Colorwheel](https://raw.githubusercontent.com/bamberjp/jQuery-Colorwheel/master/images/colorwheel.gif "jQuery Colorwheel")
### Get the value
```javascript
jQuery(document).ready(function($) {
  var value = $("#widget").colorwheel('value');
});
```
## License
Software is licensed under [MIT License](https://github.com/bamberjp/jQuery-Colorwheel/blob/master/LICENSE).
## Support
Have a thought on how to improve this software? Contact me directly via email for support at [bamberjp@gmail.com](mailto:bamberjp@gmail.com). Feel free to share how you are using this code in your own projects.
