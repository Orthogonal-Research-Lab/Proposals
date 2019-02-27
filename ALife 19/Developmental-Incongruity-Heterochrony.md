# Explaining Developmental Incongruity Through Dynamical Heterochrony

## Abstract  
The original theory of heterochrony [1,2] provides us with a generalized quantitative perspective on the dynamics of developmental trajectories. While useful, these developmental trajectories merely characterize changes in the speed and extent of growth in developmental time. More recent work on sequence heterochrony [3] reconsiders heterochrony as a series of developmental events such as tissue development or morphogenetic transformations positioned according to their relative occurrence. One open problem in the literature involves how to characterize developmental trajectories for rare and incongruous modes of development such as proposed by [4]. By applying suitable representations of development along with the appropriate mathematical constructs, we hope to reveal interesting features of changes in growth given the plasticity and complexity of developmental timing.  

We will present a range of potential dynamical approaches to characterizing heterochrony [5] in a way that goes beyond existing models. Our approach is unique in that we reconsider the developmental trajectory as a series of autonomous developmental programs called triangular state machines (TSMs). With a focus on developmental timing, we will use formal techniques to characterize delays and bifurcations in the developmental trajectory. We also consider the role of multiple developmental programs operating either in parallel or serially that are able to characterize some of the immense diversity observed in animal development. Along the way, we will employ concepts such as delay dynamical equations and bifurcation theory that can enrich our understanding of heterochrony and complex developmental processes more generally.  

## Introduction  
The theory of heterochrony provides a framework for characterizing the nature of growth relative to adaptive changes in phenotype expressed in development and indicative of evolutionary history. Taking a dynamical systems view of heterochrony allows us to characterize less common modes of growth and transformation during development called _developmental incongruities_. Two examples of developmental incongruities are metamorphosis and the presence of nervous system with both ancestral and derived components. In both of these cases, features such as delays and switches between stable developmental trajectories can explain such phenomena. The dynamical view of heterochrony defines these phenomena in two ways: multiphasic heterochrony and compound heterochrony. These type of heterochrony in the developing phenotype are underlain by overlapping gene expression networks, which form something we call a triangular state machine (TSM). In short, TSMs produce one or more developmental trajectories, changes in which can be described using a dynamical systems approach. The solution to these systems can be mapped to a phenotypic model, and may explain complexity in the developmental process.

### Acquisition of Developmental Sequences  
In Williamson [4], several examples are given (Echinoderms, Decapods, Trochophorates, and Bryozoans) with respect to incongruous larvae, or larvae stages that resemble those of distantly-related taxa. Two phylogenetic mechanisms [4, 6] have been proposed for developmental incongruity: hybridization and horizontal gene transfer. In the case of these mechanisms, there are two problems with purely empirical investigations. The first involves distinguishing between different larval stages originating in various species, particularly in terms of genetic control. Secondarily, there is a question of acquisition. While several candidate mechanisms are proposed, there is no theoretical model that explains such developmental incongruities.  

Related to these problems is whether multiple developmental stages accumulate through singular events that contributing to genetic variation within a species, or are acquired through mass acquisition. In the case of hybrids, combinations of genetic material from two independent species occur either in convergence zones [7, 8] or as multiple independent interbreeding events resulting in reticulate evolution [9, 10]. Furthermore, hybridization events can lead to both large-scale genomic rearrangements and changes in gene expression [11, 12]. Horizontal gene transfer provides a more explicit mechanism [13-15], but specific instances of such are no easier to empirically identify.  

### Expression of Developmental Sequences  
Heterochrony can be defined as changes in the rate of change in development for a specific trait, the resulting acceleration or deceleration being a result of tweaks made to the expression of genes in any given genetic regulatory network (GRN). In many cases including the hybridization cases Williamson describes, heterochrony is quite fluid relative to a linear developmental sequence and life-history. This is even true to the extent that adult sequences from distant taxa can be present in a given species' life-history [4, 6] observes two types of overlapping body symmetry in modern Holothurian life-history. This overlap is due to heterochronic changes in the expression of each type of symmetry relative to their ancestral expression: radial symmetry is accelerated and expressed in late larvae, while the disappearance of bilateral symmetry is decelerated so that it persists throughout adulthood. Williamson [6] also observes what he calls "start again" developmental sequences. An example of this is found in Trochophores, which express a Bryozoan-typical juvenile period in its life-history.  

### Assumptions  
One way to interpret the interactions of developmental sequences is by treating then as a dynamical system. Based on _Drosophila_ embryogenesis, a number of studies [16-20] suggest that development can be characterized as a dynamical system rather than a series of discrete programs executed serially. This view seems to conflict with convential views of heterochrony, so a series of assumptions need to be made in order to bridge the gap between the language of heterochrony and developmental dynamics.

In this paper, we will use Cayley trees [21] to model the expression of phenotypic change. This model demonstrates the contingent nature of single factors and their effect on collective behavior. The Cayley tree structures can be overlapped to simulate cross-talk between developmental regulatory networks. These overlapping structures not only allow us to simulate switching behaviors and nonlinear behaviors [22], but form computational mechanisms in their own right.  

This paper also introduces a number of new concepts related to heterochrony, including basic functions for multiphasic (Figure 1) and compound (Figure 2) heterochrony. Each of these types of heterochrony produce a function of degree of differentiation over the life-history (time) of the developmental process. The mathematical development of these newly-identified forms of heterochrony are defined in Supplementary Materials (https://orthogonal-research-lab.github.io/Compound-Heterochrony.html), which provides details and mathematical formalisms, conceptual results, and theoretical scenarios for nonlinear switches during developmental growth (Figure 3).  

## Results

### Compound and Multiphasic Heterochrony  
We can go beyond the empirical work of Williamson and further define the two alternate models for characterizing heterochrony in life-history: multiphasic and compound. Multiphasic heterochrony involves plastic responses to growth stimuli over developmental time. Compound heterochrony involves developmental trajectories inherited from multiple species. These types of heterochrony are demonstrated in Figures 1 and 2, respectively. Both of these types can also be characterized using a dynamical formulation of previous descriptions of heterochrony.  

<p align="center">
  <img width="1008" height="500" src="https://user-images.githubusercontent.com/38323286/53188873-db932e80-35cb-11e9-84f8-8bb181b4a1b6.png">
</p>

__Figure 1__ A step-by-step description of multiphasic heterochrony, in which the larval form (caterpillar) dedifferentiates into an intermediate pupae. The developmental trajectories of two different programs expressed as two different parts of life history. A) the caterpillar developmental program is active early in life-history, B) an intermediate stage occurs where all existing structure is obliterated, C) the butterfly developmental program is active later in life history. Click to enlarge.

<p align="center">
  <img width="1008" height="500" src="https://user-images.githubusercontent.com/38323286/53188958-0bdacd00-35cc-11e9-9f82-e1f4a1b722aa.png">
</p>

__Figure 2__ A step-by-step description of compound heterochrony, in which developmental trajectories from two different species overlap, resulting in a switch from one program to the other during the course of life history. A) the program from Species A is active early in life-history, B) a switch between developmental programs is activated, C) the program from species B is active later in life-history.  Click to enlarge.

<p align="center">
  <img width="884" height="497" src="https://user-images.githubusercontent.com/38323286/53510304-47214400-3a83-11e9-8efc-45189e7ad854.png">
</p>

__Figure 3__ . An example of a nonlinear switching event during developmental growth. In this example of compound heterochrony, two developmental programs are separated by a dedifferentiation and decellularization process (gray dashed line between $\beta_1$ and $\alpha_2$).Click to enlarge.

### Computational Genetic Regulatory Network Model  
We use the computational model of Artyomov, Meissner, and Chakraborty [21] to approximate a suitable GRN. In this case, we represent the hierarchical GRN with a binary tree structure. Each node represents a hypothetical gene in its order of expression. Each level consist of hypothetical genes with equivalent order of expression. As a result, daughter genes at a single level of the binary tree are considered to be a single functional unit (cis) of DNA. By contrast, when a gene at one level turns on or off a gene at the next level, it is said to act in trans. This is because a binary division creates a new operon consisting of two genes: the mother gene activates the gene in trans and the daughter genes activate each other in cis. Lateral activations (within the same level of the tree) occurring between daughter pairs also activate each other in trans.  

These rules create something we call a Triangular State Machine (TSM). The TSM maps the three types of behavior embedded in network arcs to numeric states: a state of “0” equals “off”, a state of “1” equals “on in trans”, and a state of “2” equals “on in cis”. Table 1 shows all possible ordinal paths and their corresponding states for an order 3 binary tree.  

__Table 1__ All pairwise ordinal paths (network arcs) in an order 3 binary tree. Ordinal path leads from source to destination.

Source        |Destination   | State        
:---:         |:---:         |:---:
N/A           |0             |1             
N/A           |0             |1             
0             |00            |1             
0             |01            |1             
1             |10            |1             
1             |11            |1             
01            |10            |1             
0             |1             |2             
00            |01            |2             
10            |11            |2             

Triangular state machines can also be organized to show reciprocal connections between nodes. In such cases, the rules of the original tree hold, with the only difference being a potential regulatory mechanism between the mother and daughter gene(s).  

<p align="center">
  <img width="1008" height="500" src="https://user-images.githubusercontent.com/38323286/53188983-1b5a1600-35cc-11e9-9dc7-8245b402391b.PNG">
</p>

__Figure 3__ An order-3 GRN with nodes acting in both cis and trans. INSET: an example of a TSM as network motif. Click to enlarge.  

Each tree has an identity (0,1) that comes before the node identity (0,1). The leftmost node at order 3 in tree 0 is (000). An order 3 tree is classified as if it has four layers, but this order is discontinuous within a single tree depending on the amount of overlap between each tree. For an overlapping set of order 2 trees, nodes 00 and 01 belong to tree A and nodes 10 and 11 belong to tree B, but their order from left to right is 00, 10, 01, 11. This order is referred to as an introgressed order.   

<p align="center">
  <img width="1008" height="500" src="https://user-images.githubusercontent.com/38323286/53189065-45abd380-35cc-11e9-81fb-34be4d99cc1a.PNG">
</p>

__Figure 4__ Two overlapping GRNs with introgressed nodes and ordered arcs forming a hierarchical compound model. Click to enlarge.

### Discussion  
In the developmental program responsible for Drosophila eye morphogenesis, switch-like behavior results from positive feedback between genes in the regulatory network [23]. Nonlinear positive feedback in the form of interacting positive feedbacks loops, sets the stage for dynamic bistability [24], or the conditions that enable switching mechanism responsible for both multiphasic and compound heterochrony. Dynamic bistability can be demonstrated in small and complex GRNs alike [25, 26]. More generally, epigenetic landscapes [27] can be used to demonstrate switching as a function of differentiation and historical contingency.  

## References:
[1] Alberch, P., Gould, S.J., Oster, G.F., and Wake, D. (1979). Size and shape in ontogeny and phylogeny. _Paleobiology_, 5(3), 296.  

[2] McKinney, M.L. and McNamara, J.K. (2013). Heterochrony and the evolution of ontogeny. Springer.  

[3] Smith, K.K. (2001). Heterochrony revisited: the evolution of developmental sequences. _Biological Journal of the Linnean Society_, 73, 169-186. doi:10.1006/bij1.2001.0535.  

[4] Williamson, D.I. (1992). Larvae and Evolution: towards a new zoology. Chapman and Hall, New York.  

[5] Antonelli, P.L., Bradbury, R., Krivan, V., Shimada, H. (1993). A dynamical theory of heterochrony: Time-sequencing changes in ecology, development, and evolution. _Journal of Biological Systems_, 1(4), 451-487. doi:10.1142/S0218339093000264.  

[6] Williamson, D.I. (2003). The Origins of Larvae. Kluwer Academic Publishers, London.  

[7] Costedoat, C., Pech, N., Chappaz, R., and Gilles, A. (2007). Novelties in Hybrid Zones: crossroads between population genomic and ecological approaches. _PLoS One_, 2(4), e357.  

[8] Begun, D.J. et al. (2007). Population genomics: whole-genome analysis of polymorphism and divergence in Drosophila simulans. _PLoS Biology_, 5(11), e310.  

[9] Liu, J., Yu, L., Arnold, M.L., Wu, C-H., Wu, S-F., Lu, X., and Zhang, Y-P. (2011). Reticulate evolution: frequent introgressive hybridization among Chinese hares (genus Lepus) revealed by analyses of multiple mitochondrial and nuclear DNA loci. _BMC Evolutionary Biology_, 11, 223.  

[10] Figueiro, H.V. et.al (2017). Genome-wide signatures of complex introgression and adaptive evolution in the big cats. _Science Advances_, 3(7), e1700299.  

[11] Baack, E.J. and Rieseberg, L.H. (2007). A genomic view of introgression and hybrid speciation. _Current Opinion in Genetics and Development_, 17(6): 513–518.  

[12] Combes, M-C., Hueber, Y., Dereeper, A., Rialle, S., Herrera, J-C., and Lashermes, P. (2015). Regulatory Divergence between Parental Alleles Determines Gene Expression Patterns in Hybrids. _Genome Biology and Evolution_, 7(4), 1110–1121.  

[13] Boto, L. (2010). Horizontal gene transfer in evolution: facts and challenges. _Proceedings of the Royal Society B_, 277, 819-827.  

[14] Huang, J. (2013). Horizontal gene transfer in eukaryotes: the weak-link model. _Bioessays_, 35(10), 868–875.  

[15] Soucy, S.M., Huang, J., and Gogarten, J.P. (2015). Horizontal gene transfer: building the web of life. _Nature Reviews Genetics_, 16, 472-482.  

[16] Krotov, D., Dubuis, J.O., Gregor, T., and Bialek, W. (2014). Morphogenesis at criticality. _PNAS_, 111(10), 3683–3688.  

[17] Mora, T. and Bialek, W. (2011). Are Biological Systems Poised at Criticality? _Journal of Statistical Physics_, 144, 268–302.

[18] Dubuis, J.O., Tkacik, G., Wieschaus, E.F., Gregor, T., Bialek, W. (2013). Positional information, in bits. _PNAS_, 110(41), 16301-16308.

[19] Verd, B., Crombach, A., and Jaeger, J. (2017). Dynamic Maternal Gradients Control Timing and Shift-Rates for Drosophila Gap Gene Expression. PLoS Computational Biology, 13(2), e1005285.  

[20] Verd, B., Clark, E., Wotton, K.R., Janssens, H., Jimenez-Guri, E., Crombach, A., and Jaeger, J. (2018). A damped oscillator imposes temporal order on posterior gap gene expression in _Drosophila_. PLoS Biology, 16(2), e2003174.  

[21] Artyomov, M.N., Meissner, A., and Chakraborty, A.K. (2010). A Model for Genetic and Epigenetic Regulatory Networks Identifies Rare Pathways for Transcription Factor Induced Pluripotency. _PLoS Computational Biology_, 6(5), e1000785.

[22] Brookings, T., Carlson, J.M., and Doyle, J. (2005). Three mechanisms for power laws on the Cayley tree. _Physical Review E_, 72(5), 056120.

[23] Graham, T.G.W., Ali Tabei, S.M., Dinner, A.R., and Rebay, I. (2010). Modeling bistable cell-fate choices in the Drosophila eye: qualitative and quantitative perspectives. _Development_, 137, 2265-2278.  

[24]Chang, D-E., Leung, S., Atkinson, M.R., Reifler, A., Forger, D., and Ninfa, A.J. (2010). Building biological memory by linking positive feedback loops. _PNAS_, 107(1), 175–180.  

[25] Huang, S., Eichler, G., Bar-Yam, Y. and Ingber, D. E. (2005). Cell fates as high-dimensional attractor states of a complex gene regulatory network. _Physical Review Letters_, 94, 128701.  

[26] Siegal-Gaskins, D., Grotewold, E. and Smith, G. D. (2009). The capacity for multistability in small gene regulatory networks. _BMC Systems Biology_, 3, 96.  

[27] Ferrell, J.E. (2012). Bistability, Bifurcations, and Waddington’s Epigenetic Landscape. _Current Biology_, 22, R458–R466.  
