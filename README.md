# cordova-plugin-pick-crop
  This is a cordova plugin for pick and crop photo.
  Just support android and ios.
  
  
# Install
    cordova plugin add https://github.com/huangliop/cordova-plugin-pick-crop.git
# Screen Shoot

  ![android-3](./screenshot-android-3.jpg)
  ![android-4](./screenshot-android-4.jpg)
  ![android-1](./screenshot-android-1.jpg)
  ![android-2](./screenshot-android-2.jpg)

# Usage

## Just pick a photo
```
 /**
     * just pick a image ,dont crop it
     * @param {[[Type]]} params   
     * @param {[[Type]]} success [[success callback function]]
     * @param {[[Type]]} error   [[error callback function]]
     */
plugins.pickCrop.pick({
   height:500, 
   quality:75
},function(result){
    //"result" is base64 string of result photo
},function(error){
    console.error(error);
})   
```
## Pick and Crop a photo
```
 /** 
     * @param {[[Type]]} params  [[set the result image's height]]
     * @param {[[Type]]} success [[success callback function]]
     * @param {[[Type]]} error   [[error callback function]]
     */
plugins.pickCrop.crop({
   height:500,
   quality:75
},function(result){
    //"result" is base64 string of result photo
},function(error){
    console.error(error);
})   
```
# License
This android is based on [android-crop](https://github.com/jdamcd/android-crop)
