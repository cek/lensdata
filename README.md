# Camera lens data

These files contain lens design data used in:

Craig Kolb, Don Mitchell, and Pat Hanrahan. *A Realistic Camera Model
for Computer Graphics*.  SIGGRAPH '95 Proceedings, ACM SIGGRAPH,
pages 317-324, August 1995

The tables are adapted from:

Warren J. Smith and Genesee Optics Software, Inc.
*Modern Lens Design: A Resource Manual*.  McGraw Hill, 1992
ISBN 0-07-059178-4

which in turn references corresponding patents.

## Data format ##

Each table consists of a row for each lens surface.  The final
row indicates the distance from the last element to the image plane
when focused at infinity.  Comment lines start with the '#' character.

Each row consists of a number of columns.  Each lens, except where noted,
is given as a 100mm EFL design; the linear proportions of the design
can be scaled by F/100 to arrive at a lens with a focal length of F mm.

Linear measurements are given in mm.  Surfaces are listed from "front"
(nearest object space) to "back" (nearest image space).

The first column indicates the type of surface:

* s: spherical
* d: diaphragm

The second column gives the radius of curvature of the surface.  This
column is blank for diaphragm entries.

The third column gives the axial position of the surface relative to
the previous surface.  Note that this differs from from
traditional tables, where "thickness" is used.

The fourth column gives the index of refraction at the d line
(.5876 microns) of the material on the "far" side of the interface.
This column is blank for diaphragm entries.  I have not included the
Abbe number or the like in these tables, as we do not model chromatic aberration
in our system.

The fifth column gives the diameter of the clear aperture of the interface.

Craig Kolb
<br>
June, 1996
