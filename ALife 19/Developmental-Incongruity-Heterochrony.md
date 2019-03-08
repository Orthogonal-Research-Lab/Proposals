# Understanding Developmental Incongruity Through Dynamical Heterochrony

## Abstract  
The theory of heterochrony provides us with a generalized quantitative perspective on the dynamics of developmental trajectories. While useful, these linear developmental trajectories merely characterize changes in the speed and extent of growth in developmental time. One open problem in the literature involves how to characterize developmental trajectories for rare and incongruous modes of development. By combining nonlinear mathematical representations of development with models of gene expression networks (GRNs), the dynamics of growth given the plasticity and complexity of developmental timing are revealed. The approach presented here also characterizes heterochrony as a dynamical system as well as introduces putative developmental features called triangular state machines (TSMs). With a focus on developmental timing, formal techniques are developed to characterize delays and bifurcations in the developmental trajectory. These techniques take into consideration the existance of multiple developmental genotypes operating in parallel, which ultimately characterize the exquisite phenotypic diversity observed in animal development.  

## Introduction  
Heterochrony [1,2] provides a framework for characterizing the nature of growth relative to adaptive changes in phenotype expressed in development and indicative of evolutionary history. More recent work on sequence heterochrony [3] reconsiders heterochrony as a series of developmental events such as tissue development or morphogenetic transformations positioned according to their relative occurrence. Taking a dynamical systems view of heterochrony [4] allows for the characterization of less common modes of growth and transformation during development called developmental incongruities [5]. Two examples of developmental incongruities are metamorphosis and the presence of nervous system with both ancestral and derived components. In both of these cases, features such as delays and phase switching between stable developmental trajectories can explain such phenomena. The dynamical view of heterochrony defines these phenomena generally in terms of dynamical multiphasic heterochrony and in particular as compound heterochrony. Underlying compound heterochrony are genetic regulatory networks (GRNs), which when overlapping form a triangular state machine (TSM). TSMs produce one or more developmental trajectories, changes in which can be described using a dynamical systems approach. The solution to these systems can be mapped to a phenotypic model, and may explain complexity in the developmental process.

### Acquisition of Developmental Sequences  
According to Williamson [4], incongruous larval stages that resemble those of distantly-related taxa can be observed in several orders of marine invertebrate. Two phylogenetic mechanisms [4, 6] have been proposed for these developmental incongruities: hybridization and horizontal gene transfer. Purely empirical investigations of developmental incongruity are difficult for two reasons. The first involves distinguishing between different larval stages originating in various species, particularly in terms of genetic control. Secondarily, there is a question of acquisition. While several candidate mechanisms are proposed, there is no theoretical model that explains such developmental incongruities. A theoretical and computational model is provided here which provides a clearer basis for how these incongruities might arise and be expressed in the course of development.

The model presented here may also help address a related question: whether multiple developmental stages accumulate through singular events that contributing to genetic variation within a species, or are acquired through mass acquisition. In the case of hybrids, combinations of genetic material from two independent species occur either in convergence zones [7, 8] or as multiple independent interbreeding events resulting in reticulate evolution [9, 10]. Furthermore, hybridization events can lead to both large-scale genomic rearrangements and changes in gene expression [11, 12]. Horizontal gene transfer provides a more explicit mechanism [13-15], but specific instances of such are no easier to empirically identify.  

### Expression of Developmental Sequences  
Heterochrony can be defined as changes in the rate of change in development for a specific trait, the resulting acceleration or deceleration being a result of tweaks made to the expression of genes in any given genetic regulatory network (GRN). In many cases including the hybridization cases Williamson describes, heterochrony is quite fluid relative to a linear developmental sequence and life-history. This is even true to the extent that adult sequences from distant taxa can be present in a given species' life-history  observes two types of overlapping body symmetry in the development of sea cucumbers [4-6]. This overlap is due to heterochronic changes in the expression of each type of symmetry relative to their ancestral expression: radial symmetry is accelerated and expressed in late larvae, while the disappearance of bilateral symmetry is decelerated so that it persists throughout adulthood. Williamson [6] also observes what he calls "start again" developmental sequences. An example of this is found in Trochophores, which unexpectedly expresses a Bryozoan-typical juvenile period in its life-history.  

### Assumptions and Methods
One way to interpret the interactions of developmental sequences is by treating then as a dynamical system. Based on _Drosophila_ embryogenesis, a number of studies [16-20] suggest that development can be characterized as a dynamical system rather than a series of discrete programs executed serially. This view seems to conflict with convential views of heterochrony, so a series of assumptions need to be made in order to bridge the gap between the language of heterochrony and developmental dynamics.

This first new concept is to extend the theory of heterochrony, including defining a mathematical formalism for dynamical multiphasic heterocrony and in particular the compound case. As an extension of the mathematical model of heterochrony proposed in [1], synamical multiphasic heterochrony explains distinct phases of phenotypic complexity across developmental time, as well as the transition from one phase to the other. Compound heterochrony relies on three parameters: $\alpha$, $\beta$, and $\tau$. Consistent with the formalism in [1], $\alpha$ and $\beta$ represent the initiation and termination of growth, respectively. The $\tau$ parameter is consistent with the notation of delay differential equations (DDEs), and represents the length of delay between two growth phases, each being a function defined by an $\alpha$, $\beta$ pair. The nature of these compound dynamics depends on the value $\tau$, operationalized as the length of time between $\beta_t$ and $\alpha_t+1$. When $\tau$ is positive, there are two distinct phases of growth in the organism. When $\tau$ is negative, the transition between phases is smoother. The specific trajectories of compound heterochrony also rely upon the parameter _k_, or the overall growth rate. 

**Heterochrony.** The growth law of [1] can be stated as

$$ \frac{dy}{da} = 
\begin{cases}
0, & \text{a < $\alpha$}\\
ky,& \text{$\alpha$ < a < $\beta$}\\
0, & \text{a > $\beta$}\\
\end{cases}
\tag{1}
$$

where *y* grows according to 

$$y(a) = y_0e^ka \tag{2}$$ 

between onset age $\alpha$ and offset age $\beta$. 

To bring together the simple model of heterochrony with a compound model, we can use Delay Differential Equations (DDEs). DDEs are characterized by time-delay systems in [21]. In their general form, a time-delay system is  

$$ \frac{d}{dt} x(t) = f(t, x(t), x_t) \tag {4}$$

where $x_t = [x(\tau): \tau$ &#x2264; $t]$ represents the trajectory of a solution in the past. Reformulated as a delay differential equation (DDE) with a single delay, the equation can be structured as

$$ \frac{d}{dt} x(t) = f[x(t), x(t-\tau)]   \tag{3}$$

We can also characterize time delays more specifically with respect to heterochrony and developmental growth trajectories.  In equation (1), $\alpha$ and $\beta$ both exhibit systematic time delays ($\tau$): $\alpha(\tau)$, $\beta(\tau)$. 

Delay in the growth trajectory is characterized over the interval ($\alpha$, $\beta$), and is equivalent to &#x2206;$k$. The total length of the delayed process is $(\beta + \tau) - (\alpha + \tau)$. Using this formulation, the rate of a delay process is $k_0$, the delay rate is $\frac{k_1}{k_0}$, and the length of a delay process is $\beta_x - \alpha_x$   

Additional mathematical and graphical details of these newly-identified forms of heterochrony are defined in a [Supplementary Notebook](https://orthogonal-research-lab.github.io/Compound-Heterochrony.html), which provides details and mathematical formalisms, conceptual results, connections to the developmental constraints such as the critical period, and theoretical scenarios for nonlinear switches during developmental growth.  

A variant of the Cayley tree model described by Artyomov, Meissner, and Chakraborty [22] is used to approximate a suitable GRN. In this case, we represent the hierarchical GRN with a binary tree structure. Each node represents a hypothetical gene in its order of expression. Each level consist of hypothetical genes with equivalent order of expression which will be further presented in the results. As a result, daughter genes at a single level of the binary tree are considered to be a single functional unit (_cis_) of DNA. By contrast, when a gene at one level turns on or off a gene at the next level, it is said to act in _trans_. This is because a binary division creates a new operon consisting of two genes: the mother gene activates the gene in _trans_ and the daughter genes activate each other in _cis_. Lateral activations (within the same level of the tree) occurring between daughter pairs also activate each other in trans. These overlapping structures, which result in a Triangular State Machine (TSM), not only allow us to simulate switching behaviors and nonlinear behaviors [23], but also result in emergent computational mechanisms. More details about the hypothetical function of overlapping trees can be found in a [Supplementary Repository]https://github.com/Orthogonal-Research-Lab/Developmental-Incongruities-and-Heterochrony).

## Results

### Compound and Multiphasic Heterochrony  
We can bolster the anecdotal observations of Williamson and further define the two alternate models for characterizing heterochrony in life-history: multiphasic and compound. Multiphasic heterochrony involves plastic responses to growth stimuli over developmental time. Compound heterochrony involves developmental trajectories inherited from multiple species. These types of heterochrony are demonstrated in Figures 1 and 2, respectively. Both of these types can also be characterized using a dynamical formulation of previous descriptions of heterochrony.  

<p align="center">
  <img width="450" height="750" src="https://user-images.githubusercontent.com/38323286/53979023-3fd8e680-40d2-11e9-8028-3358700b453b.png">
</p>

__Figure 1__. A step-by-step description of multiphasic heterochrony, in which the larval form (caterpillar) dedifferentiates into an intermediate pupae. The developmental trajectories of two different programs expressed as two different parts of life history. A) the caterpillar developmental program is active early in life-history, B) an intermediate stage occurs where all existing structure is obliterated, C) the butterfly developmental program is active later in life history. Click to enlarge.  

Figure 3 demonstrates a compound heterochronic process with a positive value for $\tau$. This example confirms that compound trajectories also rely on different values for _k_, in addition to the importance of $\delta$, or the difference in individual $\alpha$ and $\beta$ points along each part of the greater developmental trajectory. In this case, $\delta\beta$ is much greater than $\delta\alpha$, which suggests exponential growth in the later phases of development. As an $\alpha, \beta$ pair represent a single Cayley tree model of the genotype, $\tau$ is also related to the degree of overlap in adjoining Cayley trees and the size of a TSM.  

<p align="center">
  <img width="450" height="750" src="https://user-images.githubusercontent.com/38323286/53978979-246ddb80-40d2-11e9-870b-b813570ff247.png">
</p>

__Figure 2__. A step-by-step description of compound heterochrony, in which developmental trajectories from two different species overlap, resulting in a switch from one program to the other during the course of life history. A) the program from Species A is active early in life-history, B) a switch between developmental programs is activated, C) the program from species B is active later in life-history.  Click to enlarge.

<p align="center">
  <img width="442" height="249" src="https://user-images.githubusercontent.com/38323286/53510304-47214400-3a83-11e9-8efc-45189e7ad854.png">
</p>

__Figure 3__. An example of a nonlinear switching event during developmental growth between two growth trajectories. Parameter $\alpha$ represents the start of the growth trajectory, and parameter $\beta$ represents the end of this growth process. In this example of compound heterochrony, two developmental programs are separated by a dedifferentiation and decellularization process (gray dashed line between $\beta_1$ and $\alpha_2$). Click to enlarge.  

### Computational Regulatory Model  
Cayley trees model the expression of phenotypic change by the genotype. Each node in the tree represents a gene or regulatory element, and the tree structure itself is structured according to their relative causal effect on each other. This model demonstrates the contingent nature of single factors and their effect on collective behavior. The Cayley tree structures can be overlapped to simulate cross-talk between developmental regulatory networks. Let us walk through a Suppose a binary tree $T$ rooted at node $t_0$. This node can be defined as a master control gene, which turns on daughter nodes 0 and 1 at $t_1$. Each of these daughter nodes respresent a gene under contingent upon the master gene. Subsequent layers of the tree represent genes that are dependent upon genes $0$ and $1$, in addition to promoters, enhancers, and post-transcriptional/translational modifications that contribute to the phenotype.  

In this non-overlapping example, one daughter gene ($g_0$) is a gene of lesser effect, while the other daughter gene ($g_1$) is a gene of greater effect. The expression of both genes are mediated by promotors. The gene of lesser effect ($g_0$) has two promotors _p_: $p_{00}$ and $p_{01}$, while the gene of greater effect ($g_1$) also has two promoters: $p_{10}$ and $p_{11}$. Each pair of promoters (genes expressed at $t_2$) are expressed according to probabilities $p$ and $1-p$, respectively. The relative probability of switching is context-dependent. Enhancers, present at $t_3$ in this example, mediate the expression of genes $0$ and $1$ as the daughter nodes of a promoter node. In this example, each promoter would have two enhancer nodes, for a total of eight (8) enhancer nodes. Unlike promoters, enhancers act as analogue tuners, while each enhancer produces a modified output of its mother promoter.  

In an overlapping example, the TSM maps the three types of behavior embedded in network arcs to numeric states: a state of “0” equals “off”, a state of “1” equals “on in trans”, and a state of “2” equals “on in cis”. Table 1 shows all possible ordinal paths and their corresponding states for an order 3 binary tree.  

__Table 1__. All pairwise ordinal paths (network arcs) in an order 3 binary tree. Ordinal path leads from source to destination.

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

TSMs can also be organized to show reciprocal connections between nodes. In such cases, the rules of the original tree hold, with the only difference being a potential regulatory mechanism between the mother and daughter gene(s). Figures 4 and 5 demonstrate these relationships, with Figure 4 deonstrating reciprocal connections and a TSM and Figure 5 providing an example of an introgressed tree.

<p align="center">
  <img width="504" height="250" src="https://user-images.githubusercontent.com/38323286/53188983-1b5a1600-35cc-11e9-9dc7-8245b402391b.PNG">
</p>

__Figure 4__. An order-3 GRN with nodes acting in both cis and trans. INSET: an example of a TSM as network motif. Click to enlarge.  

Each tree has an identity (0,1) that comes before the node identity (0,1). The leftmost node at order 3 in tree 0 is (000). An order 3 tree is classified as if it has four layers, but this order is discontinuous within a single tree depending on the amount of overlap between each tree. For an overlapping set of order 2 trees, nodes 00 and 01 belong to tree A and nodes 10 and 11 belong to tree B, but their order from left to right is 00, 10, 01, 11. This order is referred to as an introgressed order, and results in reversals, asymmetries, and spatially-restricted increases in complexity.

<p align="center">
  <img width="504" height="250" src="https://user-images.githubusercontent.com/38323286/53189065-45abd380-35cc-11e9-81fb-34be4d99cc1a.PNG">
</p>

__Figure 5__. Two overlapping GRNs with introgressed nodes and ordered arcs forming a hierarchical compound model. Click to enlarge.

Due to the origin of TSMs in overlapping genetic regulatory networks, we expect to see complex phenotypes resulting from these interactions. One such phenotypic pattern we expect to see are interference patterns similar to Moire patterns form applied mathematics. This interference mechanisms might reveal itself in the form of overlapping coloration patterns along the body, or the juxtaposition of differing connectivity patterns in a nervous system. The $\tau$ parameter can also play a role in determining what these interference patterns look like, whether they look more like a overlapping sets of concentric circles (negative values for $\tau$) or the orderly meeting of two orientations of a city street grid ($\tau$ of 0).

### Discussion  
In this paper, the theory of heterochrony has been advanced and a mechanism for the genomic expression of systematic growth has 
been proposed. In terms of heterochrony, the basic mathematical structure of heterochrony theory has been extended to include multiple
phases of growth. The genomic expression models introduced here utilize Cayley trees and their overlapping components to form functional 
units and produce outputs that result in a growth trend. There are also several themes revealed in this paper. The first is the role of 
delays and differential time in the expression of phenotypes. Based on anectodal observations made by Williamson [5,6], changes in phase 
across the developmental process are hypothesized to be due to multiple growth processes (expressed in the genotype) and changes in the 
rate and linkage of these growth processes. Representing the genotype, the Cayley tree representations also reveal how these dynamics might be regulated. Cayley trees rely on both regulation and gene-gene interactions [24] to produce a dynamical output. In cases where two Cayley trees overlap, it is hypothesized that a TSM exists that provides a mechanism for local feedback. This may result in nonlinear outputs and other examples of complex regulation.

One overarching theme of this paper is that patterns of developmental growth and and the progression of developmental dynamics are much more complex than assumed by contemporary theory. Using a combination of genotypic network representations and heterochronic scaling in the phenotype, we can begin to move towards viewing development as a highly complex and nonlinear process. Yet this approach also provides concrete mechanisms for guided generativity. In the developmental program responsible for _Drosophila_ eye morphogenesis, switch-like behavior results from positive feedback between genes in the regulatory network [25]. Nonlinear positive feedback in the form of interacting positive feedbacks loops, sets the stage for dynamic bistability [26], or the conditions that enable switching mechanism responsible for both multiphasic and compound heterochrony. Dynamic bistability can be demonstrated in small and complex GRNs alike [27, 28]. More generally, epigenetic landscapes [29] can be used to demonstrate switching as a function of differentiation and historical contingency. Future work will invilve mapping simulations of development derived from our approach to developmental structures such as lineage trees and epigenetic landscapes.  

## References:
[1] Alberch, P., Gould, S.J., Oster, G.F., and Wake, D. (1979). Size and shape in ontogeny and phylogeny. _Paleobiology_, 5(3), 296.  

[2] McKinney, M.L. and McNamara, J.K. (2013). Heterochrony and the evolution of ontogeny. Springer.  

[3] Smith, K.K. (2001). Heterochrony revisited: the evolution of developmental sequences. _Biological Journal of the Linnean Society_, 73, 169-186. doi:10.1006/bij1.2001.0535.  

[4] Antonelli, P.L., Bradbury, R., Krivan, V., Shimada, H. (1993). A dynamical theory of heterochrony: Time-sequencing changes in ecology, development, and evolution. _Journal of Biological Systems_, 1(4), 451-487. doi:10.1142/S0218339093000264.  

[5] Williamson, D.I. (1992). Larvae and Evolution: towards a new zoology. Chapman and Hall, New York.  

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

[19] Verd, B., Crombach, A., and Jaeger, J. (2017). Dynamic Maternal Gradients Control Timing and Shift-Rates for Drosophila Gap Gene Expression. _PLoS Computational Biology_, 13(2), e1005285.  

[20] Verd, B., Clark, E., Wotton, K.R., Janssens, H., Jimenez-Guri, E., Crombach, A., and Jaeger, J. (2018). A damped oscillator imposes temporal order on posterior gap gene expression in _Drosophila_. _PLoS Biology_, 16(2), e2003174.  

[21] Richard, J-P. (2003). Time-delay systems: an overview of some recent advances and open problems. _Automatica_, 39, 1667-1694.

[22] Artyomov, M.N., Meissner, A., and Chakraborty, A.K. (2010). A Model for Genetic and Epigenetic Regulatory Networks Identifies Rare Pathways for Transcription Factor Induced Pluripotency. _PLoS Computational Biology_, 6(5), e1000785.

[23] Brookings, T., Carlson, J.M., and Doyle, J. (2005). Three mechanisms for power laws on the Cayley tree. _Physical Review E_, 72(5), 056120.

[24] Mensch, J., Carreira, V., Lavagnino, N., Goenaga, J., Folguera, G., Hasson, E., and Fanara, J.J. (2010). Stage-Specific Effects of 
Candidate Heterochronic Genes on Variation in Developmental Time along an Altitudinal Cline of _Drosophila melanogaster_. _PLoS One_, 
5(6), e11229.

[25] Graham, T.G.W., Ali Tabei, S.M., Dinner, A.R., and Rebay, I. (2010). Modeling bistable cell-fate choices in the Drosophila eye: qualitative and quantitative perspectives. _Development_, 137, 2265-2278.  

[26]Chang, D-E., Leung, S., Atkinson, M.R., Reifler, A., Forger, D., and Ninfa, A.J. (2010). Building biological memory by linking positive feedback loops. _PNAS_, 107(1), 175–180.  

[27] Huang, S., Eichler, G., Bar-Yam, Y. and Ingber, D. E. (2005). Cell fates as high-dimensional attractor states of a complex gene regulatory network. _Physical Review Letters_, 94, 128701.  

[28] Siegal-Gaskins, D., Grotewold, E. and Smith, G. D. (2009). The capacity for multistability in small gene regulatory networks. _BMC Systems Biology_, 3, 96.  

[29] Ferrell, J.E. (2012). Bistability, Bifurcations, and Waddington’s Epigenetic Landscape. _Current Biology_, 22, R458–R466.  
