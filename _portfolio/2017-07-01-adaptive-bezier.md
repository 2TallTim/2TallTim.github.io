---
layout: page
permalink: /portfolio/bezier
title: Adaptive Bezier Subdivision
image:
    thumbnail: /assets/images/teaser/bezier.jpg
excerpt: Interactive demonstration of bezier curve subdivision and deCasteljau's algorithm
---

{% raw %}
<iframe src="/assets/frames/bezier.html" frameborder="0" sandbox="allow-scripts" style="width:100%;min-width: 1100px;height: 100%;min-height: 650px"></iframe>
{% endraw %}

Bezier splines are a foundation of modern computer graphics. They're used in font rendering, graphics design software, and a myriad of other places. The spline is shaped by its control points, passing through the first and last points.  The curve is defined in terms of these points, weighted by a number of polynomial basis functions. In this demo, drag the red points around to  manipulate the  control points, and see how it influences the curve.

Evaluating high-degree polynomial functions accurately poses computational problems. Instead, the deCasteljau algorithm is used, which is a recursive algorithm that subdivides the control polygon, and splits the curve into two new control polygons. This algorithm is far more stable than directly evaluating the polynomials. This demo draws curves as a series of line segments generated from recursively subdividing the initial polygon. A number of adaptive criteria are available to tell the algorithm when to stop subdividing the curve. Each method has advantages and disadvantages in terms of performance and accuracy. Adjusting the Epsilon for each criterion will change when the algorithm stops. You can see the results of these in challenging situations in some of the presets. 

You can also directly visualize the process of deCasteljau's algorithm using the controls under the "deCasteljau Visualizer" tab. Each line represents one iteration of the algorithm, and each color is a different recursive level. The lines are subdivided at a given ratio until only one is left, which represents the point on the curve. 

This demo allows you to visualize curves with a degree between 3 and 9. In practice however, curves with a degree higher than three are rarely used. Often, many degree 3 splines are chained together. One property of Bezier splines is that if two control polygons have their last edges tangent, the resulting curves will also be tangent to each other. 

Bezier splines also belong to a larger family of curves known as basis splines, which includes B-Splines and NURBS. Future iterations of this demonstration may include those splines. 
