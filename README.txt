The code in this repository supports the 
journal paper (insert title) published in ...

The code pertains to the implementation of a blend
of the geometric configuration of a Hasse diagram
and the image schema of SCALE. We use this blend
as a model of how humans reason with Hasse diagrams.

This code is written in CASL and can be used with the toolset
HETS online ( http://rest.hets.eu/ ) to compute the blends
as described in the paper, using the button:
commands --> compute colimit.

Namely, files blend1 and blend2
contain specifications and views (mappings) needed to compute
two different blends of the SCALE schema with the Hasse
geometric configuration:
1 maps the SCALE schema elements to very few shapes 
of the geometry, and removes many of the shapes of the geometry
2 maps the SCALE schema elements to all the shapes of the geometry
effectively identifying everything into one element,
and not removing any elements
The remaining files include specifications necessary
to compute the governing principles, i.e., measures of cognitive
utility, of these two blends.