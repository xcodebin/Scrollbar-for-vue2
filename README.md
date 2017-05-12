
## Usage

npm install vue-cli -g

npm install

npm run dev 

npm run dist

```
main.js

import Scrollbar from './components/scrollbar';
Vue.use(Scrollbar);

```
```
App.vue

 @import './assets/scrollbar.css';
 
```
 

``` 
**.vue

<template>
  <Scrollbar class="my-scrollbar" classes="" styles="" v-bind:speed=100>
         <div class="scroll-me">
         </div>
  </Scrollbar>
</template>

<script>


 
</script>

```


## Props
##### clasess (String)
Just the ordinary class name for styling the wrapper. So, It's TOTALLY **CUSTOMIZABLE!**
```css
/*The Wrapper*/
.my-scrollbar{
  width: 35%;
  min-width: 300px;
  max-height: 450px;
}

/*The Content*/
.scroll-me{
  min-width: 750px;
}
```


##### styles (Object)
If you prefer to use inline style to styling the scrollbar, you can pass the styling object to this props.

```javascript
this.styling = {

  /* Scrollbar */
  scrollbar: {
    width: "35%",
    minWidth: "300px",
    maxHeight: "450px"
  },

}
```

```html
<Scrollbar :styles="styling.scrollbar"></Scrollbar>
```

##### speed (Number)
The wheel step in pixel. The default is 53 pixel per wheel.



## Methods
You can do some methods by accessing the component via javascript.
```javascript
this.$refs.scrollbar.someMethod()
```

##### scrollToY(y)
To scroll the scrollbar to the Y
```javascript
// Examples
someMethod() {
  this.$refs.Scrollbar.scrollToY(100)
}
```

##### scrollToX(x)
To scroll the scrollbar to the X
```javascript
// Examples
someMethod() {
  this.$refs.Scrollbar.scrollToX(100)
}
````

## Thank You for Making this useful~
Just Contact Me At:
- Email: [xcodebin@outlook.com](mailto:xcodebin@outlook.com)
- Web: [https://github.com/xcodebin](https://github.com/xcodebin)
- Web: [https://git.oschina.net/xubinxcode](https://git.oschina.net/xubinxcode)

##Tips:
```
 draw on the experience of vue2-scrollbar
```
