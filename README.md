# jQuery.shiftLetters

This is the jQuery plugin which adds shift-letter animation to element.

## Demo

![demo](https://raw.githubusercontent.com/aziev/jQuery.shiftLetters/master/demo.gif)

## Usage

Asset jQuery to your page:
```
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.0/jquery.min.js"></script>
```
and the plugin:
```
<script src="jquery.shiftLetters.js"></script>
```
Now you can call the animation for any element:
```
$(document).ready(function(){
    $('#heading').shiftLetters();
});
```

## Customization

To customize the animation you can pass object as first parameter of the plugin.

Plugin parameters:

**duration**: sets the animation duration in milliseconds (default: 800).
```
$('#heading').shiftLetters({
    duration: 1000
});
```

**easing**: sets the animation easing function (default: 'swing').
```
$('#heading').shiftLetters({
    easing: 'linear'
});
```

**minOffset**, **maxOffset**: sets the minimum and maximum offset of letters start position (default: from 2 to 5).
```
$('#heading').shiftLetters({
    minOffset: 3
});
```

Of course you can use preferred parameters together:
```
$('#heading').shiftLetters({
    duration: 1000,
    easing: 'linear',
    minOffset: 3,
    maxOffset: 6,
});
```
