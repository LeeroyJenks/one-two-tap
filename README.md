# one-two-tap
A bare-bones jQuery plugin to allow for callback on double tap and single tap, with threshold selection

##Demo
[plugins.getdans.info/one-two-tap](http://plugins.getdans.info/one-two-tap)

##Installation
Download from GitHub

###Requirements
jQuery

###Use
```html
<script>
    $(document).ready(function(){
        $('.click-container').onetwotap({
            callback: function(){ /* Do Something */ }
        });
    });
</script>
```
###Description

one-two-tap is meant to be used with a callback. It's nothing without your input. You can set a threshold where, when the window width is above it, a single click/tap will fire the callback and, when the window width is below or equal to it, a double click/tap will fire it. You can also set a single click/tap callback for when the window width is below the threshold.

###Options

Options          | Definition
---------------- | -------------------------------------------------------------------------------------------------------------------- 
`threshold`      | Below, callback will fire on double tap/click.<br>Above, callback will fire on single.<br>`default: 500`
`callback`       | `function(){}`
`oneTapCallback` | `function(){}`<br>Will only fire on single tap/click<br>when window width is less than<br>or equal to the threshold.