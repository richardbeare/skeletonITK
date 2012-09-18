skeletonITK
===========

Consolidation of skeleton/medial curve tools and medial surface tools for ITK

In ITK we currently have the itkBinaryThinningImageFilter as the only class
for thinning or skeletonizing binary objects. This filter uses the algorithm
from the Gonzales and Woods textbook, with extension to 3D.

There are a couple of contributions at the Insight Journal:

http://hdl.handle.net/1926/560
http://hdl.handle.net/1926/304

However these haven't been ported and the code quality needs some work.

Both of these contributions reference the work of Malandain and Bertrand,
which provided ways for characterizing points based on the number of 
foreground or background connected components in a neighborhood, thus
forming a dimension-independent basis for skeletonization and medial
surface extraction.