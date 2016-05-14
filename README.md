#base64-to-image

To install  
`npm install base64-to-image --save`  

To run test  
`npm test`  

### Usage  

Require the library in your .js file  
`var base64ToImage = require('base64-to-image');`  

#### Change base64 string to image and save it to disk  
```
var base64Str = "Add valid base64 str";
var path ='put a valid path where you want to save the image';
var optionalObj = {'fileName': 'imageFileName', 'type':'png'};

	base64ToImage(base64Str,path,optionalObj); 
```

##### Parameters  
 - `base64Str` (string) - base64 string.
 - `path` (string) - a valid path where you want to save the image.
 - `optionalObj` (object) - have two properties fileName and type
 	- fileName holds image file name. If this value is not passed the image will be saved as 'img-' + Date.now().
 	- type holds image type e.g. ('png' or 'jpg'  and so on). If this value is not passed it will extract the image type from the base64 if present ..if not the default is 'png'


### License  
  

### Issues  
Report a bug in the issues.   