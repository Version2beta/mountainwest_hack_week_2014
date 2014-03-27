# Sixty Frames or Bust

Jeremy Kahn, Jellyvision, @jeremyckahn

Animation is a communication tool

## Methodology

Predefined and algorithmic animations

Algorithmic are based on external events and change as a result. Rendered real time. Example, video game

Predefined is prerendered.

Easing: see easing.net

Robert Penner developed many of these

## APIs

CSS

* Transitions

* Animations

Javascript

* setTimeout - works everywhere, fixed frame period

* requestAnimationFrame - newer browsers, takes care of timing for you

CSS / Javascript hybrid solutions

* Easiest - trigger CSS changes with Javascript

* Another way to separate presentation from content (?)

http://jeremyckahn.github.io/blog/2013/07/28/60-fps-or-bust-dynamically-prerendering-css-animations/

## Performance

60 FPS is the goal - perceived as "perfect motion" by human eye

"Jank kills the precious illusion of life." Rachel Nabors

Leverage the GPU:

* New. Start taking advantage.

* Better for writing to the screen than the CPU is.

* translateZ(0) ftw? not quite. Implementation detail of some browsers.

* limit GPU texture uploads - CPU -> GPU pipeline is slow

    * IMPORTANT! Only animate opacity and transform for best frame rate

## Tooling

Greensock.com?

Code is an ineffective animation tool. "Using code to make an animation is like using poetry to draw a painting."

Animatron - free

Adobe Edge

Adobe Flash - can export to HTML5 canvas (in case you already use it, don't have to give up tooling)

Stylie - Jeremy wrote this. Keyframe generator in GUI.


