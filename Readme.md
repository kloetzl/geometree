# GeoMeTree

GeoMeTree is a tool to compute distances between weighted, unrooted phylogenies. Among the supported distances are the Robinson-Foulds (symmetric distance), branch-score, cone distance and geodesic distance.

This particular version (1.41) is a fork from Kupczok et al (see below). It has a redesigned command-line interface but keeps the core algorithms.


## Usage

GeoMeTree takes as input a file containing two trees in Newick format. It then outputs one number based on the selected distance.

    $ ./geometree --file examples/two.trees --branch
    1.174734012447073

To see the available options use `--help`.


## References

The cone distance was first described in *Nina Amenta, Matthew Godwin, Nicolay Postarnakevich, and Katherine St. John.* Approximating geodesic tree distance. Inf. Process. Lett., 103(2):61–65, 2007.

The algorithm for finding the geodesic distance comes from *Anne Kupczok, Arndt Von Haeseler, and Steffen Klaere.* An exact algorithm for the geodesic distance between phylogenetic trees. J Comput Biol, 15(6):577–591, 2008. doi: 10.1089/cmb.2008.0068. The code is at http://www.cibiv.at/software/geometree/.


## License

Copyright (C) 2009  Anne Kupczok, Arndt von Haeseler and Steffen Klaere  
Copyright (C) 2018  Fabian Klötzl <kloetzl@evolbio.mpg.de>

This is a heavily modified version of the original GeoMeTree by the authors given above. The same license (GPL-2+) applies.

This program is free software; you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; either version 2 of the License, or (at your option) any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

