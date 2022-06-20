# SVG Animation (Lottie)

**SVG Animation (Lottie)** is a *presentational component* that renders Lottie animations exported from Adobe After Effect using the Bodymovin plugin.

Uses v5.7.6 of Lottie.

## Settings Overview

The attributes listed below are used in *components.json* to configure **Adapt SVG**, and are properly formatted as JSON in [*example.json*](https://github.com/deltanet/adapt-svg-animation-lottie/blob/master/example.json).

### Attributes


**\_isReducedMotionSupportEnabled** (Boolean): Respect operating system prefers-reduced-motion setting by disabling the animations. Defaults to `false`.

**\_animation** (object): It contains values for **\_src**, **\alt**, **\description**, **\attribution**, **\_loops**, **\_autoPlay**, **\_onScreenPercentInviewVertical**, **\_offScreenPause**, **\_offScreenRewind**, **\_showPauseControl**, **\_onPauseRewind**, **\_renderer**

>**\_src** (String): Set the path to the Bodymovin export file or folder. A folder should contain the animation *data.json* file plus any associated static images in an *images* folder (if applicable). A file should contain just the animation *data.json*.

>**alt** (String): The short alternative text for the animation.

>**description** (String): A longer description of the animation to be used when the animation content is not described in adjacent text.

>**attribution** (String): Text to be displayed as an attribution of animation.

>**\_loops** (Number): Controls how many times the animation should loop. To set an infinite loop, use a value of `-1`. Defaults to `0` (don't loop).

>**\_autoPlay** (Boolean): Should the animation play when on screen. Note: Percentage onscreen determines when autoplay occurs. Defaults to `true`.

>**\_onScreenPercentInviewVertical** (Number): What percentage of the SVG container should be on-screen before the animation is triggered. Defaults to `1`.

>**\_offScreenPause** (Boolean): Pause when off screen. Defaults to `true`.

>**\_offScreenRewind** (Boolean): Rewind when off screen. Defaults to `true`.

>**\_showPauseControl** (Boolean): Show the play / pause button. Defaults to `false`.

>**\_onPauseRewind** (Boolean): Rewind when the pause button is clicked. Defaults to `false`.

>**\_renderer** (String): Sets which renderer to use. Acceptable values are `svg` `canvas` and `html` - default should be `svg` when using vector based animation and `canvas` if animation is comprised of just images. Defaults to `"svg"`.

**\_fallback** (object): It contains values for **\_src**, **\alt**, **\description**, **\attribution**

>**\_src** (String): Set the path for a fallback graphic.  

>**alt** (String): The short alternative text for the fallback graphic.

>**description** (String): A longer description of the fallback graphic to be used when the graphic content is not described in adjacent text.

>**attribution** (String): Text to be displayed as an attribution of fallback graphic.
