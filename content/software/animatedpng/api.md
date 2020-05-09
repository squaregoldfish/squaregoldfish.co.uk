---
title: 'Animated PNG API'
date: 2020-04-25:14:07+02:00
weight: 2
---

## Constructor
`new AnimatedPNG(name, firstImage, imageCount, delay);`

### Parameters

| Parameter    | Purpose                                                                 |
| ------------ | ------------------------------------------------------------------------|
| `name`       | The name of the animation object.                                       |
| `firstImage` | The filename of the first image of the animation.                       |
| `imageCount` | The number of frames in the animation.                                  |
| `delay`      | The number of milliseconds to wait between each frame of the animation. |

This is used to create and initialise the animation with the basic settings.
The animation is created as a Javascript object called `name`, on which the
other functions are invoked to alter its behaviour.
The `firstImage` parameter specifies the filename of the first frame of the animation.
This should be in the same directory as the current page, and should be of the form
`<letters><numbers>.png`. The library will automatically calculate the filenames
of the subsequent frames by deconstructing the filename. If you wish to zero-pad
the numbers in the filename, that will also be detected automatically.
Some suitable filename formats are as follows:

* `fish1.png`
* `fish01.png`
* `fish-1.png`
* `fish-01.png`


The `delay` parameter will set the delay between all the frames in the animation.
If you wish to set different delays for some frames, you can use the
<a href="{{< relref "api.md#setframedelay" >}}">`setFrameDelay`</a> function.

**Note**: This constructor will not actually draw the animation in the page.
You must call the <a href="{{< relref "api.md#draw" >}}">`draw`</a> function to display the animation.



## draw
`draw(delayStart);`

| Parameter    | Purpose                                                          |
| ------------ | -----------------------------------------------------------------|
| `delayStart` | Indicates whether the animation should start immediately or not. |

Draws the animation in the page. This can be called directly after the constructor,
or after other function calls if you wish to alter the animation’s settings before it is drawn.

If `delayStart` is set to false (the default), the animation will be started immediately.
If true, the animation will not be started until <a href="{{< relref "api.md#startanimation" >}}">`startAnimation()`</a>
is called. You can add <a href="{{< relref "api.md#startanimation" >}}">`startAnimation()`</a>
to the onload attribute to delay the animation until the whole page has loaded.

## setRepeat
`setRepeat(repeatFlag);`

| Parameter    | Purpose                                                        |
| ------------ | ---------------------------------------------------------------|
| `repeatFlag` | Indicates whether the animation will repeat when it completes. |

Specifies whether or not the animation will repeat when it completes.
If `repeatFlag` is set to `true` when the animation is not running, it will be restarted.

## setFrameDelay
`setFrameDelay(frame, delay);`

| Parameter | Purpose                                           |
| ----------| --------------------------------------------------|
| `frame`   | The frame number for which the delay will be set. |
| `delay`   | The frame delay in milliseconds.                  |

Sets the delay for an individual frame of the animation.
This will override the delay specified in the <a href="{{< relref "api.md#constructor" >}}">constructor</a>.

## clearFrameDelays
`clearFrameDelays();`

Clears any custom frame delays set using <a href="{{< relref "api.md#setframedelay" >}}">`setFrameDelay`</a>.
All frame delays are set to the delay specified in the <a href="{{< relref "api.md#constructor" >}}">constructor</a>.

## startAnimation
`startAnimation();`

Restarts the animation if it has been stopped.

## stopAnimation
`stopAnimation();`

Stops the animation on the current frame.
