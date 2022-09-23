The code in this repository supports the paper
Characterising Cognitively Useful Blends: Formalising the
Governing Principles of Conceptual Blending
published in journal ...

The code pertains to the implementation of a blend
of the geometric configuration of a Hasse diagram
and the image schema of SCALE. We use this blend
as a model of how humans reason with Hasse diagrams.

This code is written in CASL and can be ran with the toolset
HETS online ( http://rest.hets.eu/ ), In our code we show
the blends already (colimits) but with HETS they can be 
computed again through the button:
commands --> compute colimit.

Namely, files blend1 and blend2
contain the specifications and views (mappings) needed to compute
two different blends of the SCALE schema with the Hasse
geometric configuration.
The input spaces are I and J, refering to the Hasse geometric configuration, and the SCALE schema respectively.
The SCALE schema (J) is not generalized, but the Hasse geometry (I) is.
1 maps the SCALE schema elements to very few shapes 
of the geometry, and generalises lots of info from the geometry
2 maps the SCALE schema elements to all the shapes of the geometry
effectively identifying everything into one element,
and not generalising almost anything

The remaining files specify the spans needed to compute the value of governing principles, i.e., measures of cognitive utility, of each blend

Accordingly, we specify a span V: I <- G -> J,
a generalization of that span, V0: I_0 <- G_0 -> J
and then the ideal spans, whose pushouts are the blends
that maximize each of the 4 governing principles we
address in our paper, are the following: 
Ve: I_e <-  G  -> J_e (max Integration)
Vm:  I  <- G_m ->  J  (max Topology)
Vc:  I  <- G_c ->  J  (max Compression)
Vu:  I  <-  0  ->  J  (max Unpacking)

G_m is the generic space that leads to monomormphisms 
from the input spaces to the colimit.
G_c is the product I x J
0 is the empty generic space, with the empty morphism to I and J
I_0 is the generalization of I that we use in
the amalgam. I_e and J_e are generalizations of I and J
needed to obtain a max Integration blend.




Note:

Some blends that compress much of the two input spaces together,
have to be computed in two steps
because in the first step we compress all sorts with each other
and only then can we also compress all predicates with each other.



