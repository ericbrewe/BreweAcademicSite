---
date: "2019-05-05T00:00:00+01:00"
draft: true
linktitle: Prog 1
menu:
  PHYS_115:
    parent: Physics 115
    weight: 3
title: PHYS 115 Page 1
toc: true
type: docs
weight: 3
---

**Drawing magnetic field lines**

The Biot-Savart law for constant currents is:

$$\mathbf B = I\frac{\mu_{0}}{4\pi} \int \frac{\vec{dl} \times \hat{r}} {r^2} $$

In general this is an integral for every point in space around the loop of current. There are however, a few geometrical configurations that permit considerable simplification. In the case of a wire that passes perpendicular to the plane, the lines of constant magnetic field will curl around the wire according to the right hand rule (i.e. they will have no component out of the plane). You will be modeling such a system in this assignment.  Please set $\frac{\mu_{0}}{4\pi} = 1$  for this problem.

First, create a grid of points over the interval [-1,-1]:[1,1]. That is, create an array of x and y coordinates and call them X, and Y. For each point on that grid you will need to calculate the magnetic field. Save the components of the magnetic field in the arrays $B_x$ and $B_y$. You can plot these vector field lines with the following code:
```python
from pylab import *
quiver (X, Y, Bx, By, scale = 150)
show()
```

What does $\vec{dl}$ look like in the plane? If the wire is coming out of the x-y plane then $\vec{dl} = <0,0,1>$. You do not need to consider other sections of the wire because they do not contribute to the magnetic field (Why not?). Plot the magnetic field for the following configurations of wire.

* A single wire coming out of the page at the origin.
* Two wires separated by a distance of 1, running in parallel.
* Two wires separated by a distance of 1, running antiparallel.

You **must** answer these questions by leaving a comment in the code to get credit on the assignment. Look at the magnetic field lines from far away;

* what do the magnetic field lines look like when the wires run in parallel? 
* What do the magnetic field lines look like when the wires run antiparallel?



