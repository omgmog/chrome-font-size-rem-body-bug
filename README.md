# What is this trickery?

I presume that delaying the CSSOM by having a failed or mis-delivered Stylesheet causes Chrome to calculate what 1rem is incorrectly. 

This seems to only effect the body element, and can be gotten around by using 1em on body. But that just hides the issue.

Annoyingly this can be intermittent, so you'll need to have the devtools open while you refresh a couple of times.

## Some facts

- The font-size on html is 14px.
- The font-size on body is 1rem.
- Chrome is rendering the font-size of body as 16px.

## See it in action:

[Demo](https://blog.omgmog.net/chrome-font-size-rem-body-bug/demo.html)

## Screenshots
![](http://i.imgur.com/iXtVRUM.png)
![](http://i.imgur.com/QOWPIts.png)
