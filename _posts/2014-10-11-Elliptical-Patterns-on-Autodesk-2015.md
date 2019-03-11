---
title: Elliptical Patterns on Autodesk Inventor 2015
tags: CAD
type: article
license: false
show_subscribe: false
---


I got stuck in this issue while working on an Autodesk Inventor 2015 project with a colleague of mine. At one point we find ourselves in need of replicate a pattern (some kind of hole feature) on an elliptical line. According to my colleague opinion, the only way would have been design each center point by hand. But that’s just a ~~cake~~ lie.

<!--more-->

The hack itself is really basics, but you might just pass by never noticing. Try yourself with these steps:

{% include image.html url="/images/20141011_rectangular-pattern.png" caption="The dialogue window of the “rectangular pattern” tool" alt="How to apply pattern to any path" align="right" captionStyle="" %}

1. create feature to be patterned, say a hole with all the parameters you need;

2. create a centered, constrained elliptical shape;

3. using the rectangular pattern tool, select the feature, then select the ellipse (step 2) in the sketch as the “direction 1”, expand dialogue window (bottom right corner button), select “direction 1” radio button under orientation, set the parameters and don’t forget to set a direction 1 start point.

Once you hit OK the magic should be done. I leave here a figure to help you guys with different language packs of Inventor.

Please notice that the tricky Circular Pattern tool won’t let you do the trick, I think that’s just a shortcut tool for straight circular patterns only (ellipsis are not tolerated).

Also, this procedure can be applied to any shape or line, not being constrained to the elliptical trajectory itself. For more details, I suggest reading this Tutorial: [How to pattern along a geometry line in Autodesk Inventor](http://grabcad.com/questions/tutorial-how-to-pattern-along-a-geometry-line-in-autodesk-inventor).
