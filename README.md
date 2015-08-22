# linmap

Linear map function for node and browser (browserify or similar)

## Usage
	
	var map = require('linmap')

	// map(min1, max1, min2, max2, input)
	var result = map(0, 100, 0, 10, 50)
	// => 5
	
## Example

Maps the mouseX position from 0 to 10

	window.addEventListener('mousemove', function (e) {
		var result = map(0, window.innerWidth, 0, 10, e.pageX)
		console.log(result)
	})