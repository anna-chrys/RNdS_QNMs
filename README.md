This notebook is a companion to the article [arxiv number]. It contains interactive plots that demonstrate the evolution of the quasinormal frequencies (QNFs), calculated using the semi-classical method presented by Gonzalez, Papantonopoulos, Saavedra. and Vasquez [https://link.springer.com/article/10.1007/JHEP06(2022)150], for the allowed values of $(M,Q)$ corresponding to the phase space (the  "sharkfin" diagram)  drawn for $L^2_{dS} = 3 / \Lambda = 1.$ This parametrisation is used throughout the notebook. 

DO NOT CHANGE the ```$\Lambda=3$`` input $-$ it will render most of this notebook useless !

Section 1 contains the preamble needed to draw the sharkfin diagram, the explicit definitions of the horizons $r=r_i$ for $i=[-,+,c]$ and the surface gravities $\kappa_i$ thereof, as well as the minutiae for the aesthetics of the plot diagrams.

Section 2 imports the necessary notebooks for subsequent calculations: the QNF computations and the WKB notebook against which we can compare our output. A small comment on the notation:

``QNFminus`` in this notebook $=$ "black hole (event horizon) family" $=$ $\omega_+$ in the manuscript;

``QNMplus`` in this notebook $=$ "cosmological (horizon) family" $=$ $\omega_c$ in the manuscript.

 To use this notebook, you must first evaluate sections 1 and 2 !

Section 3 plots the interactive sharkfin plot: it allows the user to observe the behaviour of the QNM potential on the physically-relevant domain between event and cosmological horizon (i.e. on $r_+ \leq r \leq r_c$), the "locations" of the horizons, and the corresponding QNF values for the "black hole" and "cosmological" QNFs. 

Section 4 compares the QNFs calculated here with those calculated using Konoplya's WKB package [https://arxiv.org/abs/gr-qc/0303052].

Section 5 shows how the imaginary component of the QNF scales with the mass of the scalar field. We demonstrate how we determine the "critical mass" $\mu_{crit}$ visually and directly.

Section 6 highlights the parameter space in which the semi-classical method predicts instability ($\mathbb{I}m [ \omega ] < 0$) and superradiance  ($qQ/r_c < \mathbb{R} e [ \omega ] < qQ/ r_+$).

Section 7 highlights the parameter space in which there is evidence for the violation of strong cosmic censorship (SCC) ($-\mathbb{I}m [ \omega ]/\kappa_- > 1/2$) .
