RDTool exampleReaction-Diffusion Explorer Tool by Karl Sims

RD Tool is an interactive web application for generating dynamic shapes and
patterns by simulating two virtual chemicals that react and diffuse on a 2D
grid, using the Gray-Scott model. Chemical A is added throughout the grid at a
given "feed" rate. Chemical B replicates by consuming A, but dies off at a given
"kill" rate. Different types of patterns emerge when using different values for
the feed and kill rates. The varying concentrations of B are colorized and shown
during the simulation.

Browser compatibility

This application should work on current versions of Chrome, Firefox, or Safari,
but Chrome seems to be better at handling higher resolutions. It requires WebGL
2 support including the EXT_color_buffer_float extension. It also requires Web
Assembly support.

Hardware

RD Tool will run faster if your computer has a decent GPU that accelerates
graphics and gaming applications. On iPhone, some simulations may look different
due to unsupported 32bit texture filtering.

Getting started

To begin, click on the black and white "pattern map" on the upper-right of the
RD Tool window to move the blue cursor around and select different types of
patterns. The feed rate (f) varies along the vertical axis, and the kill rate
(k) approximately varies along the horizontal axis. Lower feed rates at the
bottom of the map usually generate faster motion, because for B to survive, it
needs to consume A in new areas where it has had time to build up. Lower kill
rates on the left side of the map tend to produce more solid shapes because B
lasts longer before dying out. A new pattern grows from the previous pattern, so
moving the cursor from one position to another can give many unique results.

Press the Regrow button to clear the screen and start a new pattern from a
single seed at the center.

Press the Reset button to set all parameters back to their default values.

Press the Example button to load some preset parameter combinations and receive
a demo of various possible results.

Press the Full Screen button to display the simulation at full resolution.

Draw

You can interact with the simulation by drawing on the canvas. Press the Clear
button to clear the entire canvas and then draw to seed a new pattern. Hold down
the ctrl key to erase instead of draw.

Scale

The Scale sliders adjusts the relative size of the pattern. The scales can vary
across the simulation grid using the Scale Radial, Scale Random, or Scale Ring
sliders, and these effects can be combined. Larger scales usually require less
computation, so that can help the simulation run faster if your hardware is
limited.

Speed

This slider allows speeding up or slowing down the simulation. However, you
might not see any effect when increasing the speed if the fps shown in the
application is already below your screen's refresh rate. A typical refresh rate
is 60 frames per second (fps). To stop the simulation altogether press the Pause
button.

Vary pattern

These options cause the type of pattern to vary across the simulation grid. When
you enable one of these, a yellow cursor appears on the pattern map that
determines a second type of pattern with its own feed and kill rates. For
example, if you select the first "radial" vary-pattern button, the yellow cursor
determines the pattern at the center of the simulation grid, and the blue cursor
determines the pattern for the outer areas. You can press the active
vary-pattern button again to deselect it.

Flow

These sliders add a velocity field to the the simulation, with options to flow
in various ways across the grid. The different types of flow can be combined,
and each can be in a positive or negative direction. The center positions of the
sliders represent zero, and they should snap there slightly when you slide past
that position. To avoid the snap at zero, hold down the ctrl key while sliding.

Orientation

These sliders give an orientation map to the results by causing the diffusion to
occur faster in one direction than another. The positive and negative directions
will usually appear the same, but can make a difference if you combine multiple
orientation types. The Orientation Linear slider gives vertical orientation when
positive, or horizontal when negative.

Adjust colors

Experiment with different color map and color settings. Hopefully these are self
explanatory.

Aspect ratio

The aspect ratio of the simulation canvas should default to the aspect ratio of
your monitor, so it will fit your screen when in fullscreen mode. You can adjust
the aspect ratio manually by dragging the lower left corner of the canvas up or
down. If the canvas reaches the bottom of the browser window, try making your
whole window narrower first.

Saving settings

As you adjust the sliders and options, the URL in your browser is automatically
updated with a random looking string of characters that encodes all the current
parameter values. You can save, forward, or bookmark that URL to preserve
specific combinations of settings.

To save a still image, use the screen grab option of your operating system. You
can first pause the simulation at a good place and enter fullscreen mode.

Hotkey summary

Space: Pause or Unpause C or Delete: Clear ctrl-Z: Undo parameter change
ctrl-shift-Z or ctrl-Y: Redo parameter change R: Regrow N or E: Next example P:
Previous example

Explore further

This tutorial explains more detailed technical information about the
reaction-diffusion simulation.

The Reaction-Diffusion Media Wall was a related exhibit at the Museum of Science
in Boston.
