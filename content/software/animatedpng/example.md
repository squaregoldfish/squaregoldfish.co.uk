---
title: 'Animated PNG Example'
date: 2020-04-25:14:07+02:00
weight: 2
---

This page shows an example of the AnimatedPNG javascript library in action.
The example uses images named `fish0001.png` through `fish0023.png`.

The animation is initialised with the following code:
```javascript
fishAnim = new AnimatedPNG('fish', 'fish0001.png', 23, 100);
fishAnim.draw(false);
```
<!--more-->
<div id="fishAnimDiv" style="position: fixed; top: 100px; right: 20px; width: 200px">
  <script type="text/javascript" src="/animatedpng/animatedpng.js"></script><br />
  <script type="text/javascript">
    fishAnim = new AnimatedPNG('fish', '/animatedpng/fish0001.png', 23, 100);
    fishAnim.draw(false);
    var background = "FFFFFF";
    function changeBackground() {
      if (background == "FFFFFF") {
        background = "376797";
      } else {
        background = "FFFFFF";
      }
      document.getElementById('fishAnimDiv').style.backgroundColor = '#' + background;
    }
  </script>
</div>

Click the various links below to alter the behaviour of the animation.

#### <a href="{{< relref "example.md#change-background-colour" >}}" onclick="changeBackground()">Change background colour</a>
(just to prove it's a PNG with transparency)
```javascript
document.getElementById('fishAnimDiv').style.backgroundColor = '#<color>';
```
#### <a href="{{< relref "example.md#stop-animation" >}}" onclick="fishAnim.stopAnimation()">Stop animation</a>
```javascript
fishAnim.stopAnimation();
```
#### <a href="{{< relref "example.md#start-animation" >}}" onclick="fishAnim.startAnimation()">Start animation</a>
```javascript
fishAnim.startAnimation();
```
#### <a href="{{< relref "example.md#disable-repeat" >}}" onclick="fishAnim.setRepeat(false)">Disable repeat</a>
```javascript
fishAnim.setRepeat(false);
```
#### <a href="{{< relref "example.md#enable-repeat" >}}" onclick="fishAnim.setRepeat(true)">Enable repeat</a>
```javascript
fishAnim.setRepeat(true);
```
#### <a href="{{< relref "example.md#add-frame-delays" >}}" onclick="fishAnim.setFrameDelay(3, 500);fishAnim.setFrameDelay(15, 500);">Add frame delays</a>
```javascript
fishAnim.setFrameDelay(3, 500);
fishAnim.setFrameDelay(15, 500);
```
#### <a href="{{< relref "example.md#clear-frame-delays" >}}" onclick="fishAnim.clearFrameDelays()">Clear frame delays</a>
```javascript
fishAnim.clearFrameDelays();
```

