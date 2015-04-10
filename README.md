Convert and replace src attrs within your data.

## Example

##### gulpfile.js

```js
var gulp = require('gulp');
var inlineImagePath = require('gulp-inline-image-path');

gulp.task('default', function () {
	gulp.src('index.html')
		...
		.pipe(inlineImagePath({path:"build/images"}))
		...
});
```


##### index.html // Before...

```js
<html>
	<head>
	</head>
	<body>
		<img src="images/sample.png" />
...
```


##### path/index.html // ...after:

```html
<html>
	<head>
	</head>
	<body>
		<img src="build/images/sample.png">

...
```


### License

MIT © catindev
