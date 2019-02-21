# Explaining Developmental Incongruity Through Heterochrony

## Abstract  
The original theory of heterochrony [1,2] provides us with a generalized quantitative perspective on the dynamics of developmental trajectories. While useful, these developmental trajectories merely characterize changes in the speed and extent of growth in developmental time. More recent work on sequence heterochrony [3] reconsiders heterochrony as a series of developmental events such as tissue development or morphogenetic transformations positioned according to their relative occurrence. One open problem in the literature involves how to characterize developmental trajectories, particularly for rare modes of development such as proposed by [4]. By applying better representations of development along with the appropriate mathematical constructs, we hope to reveal interesting features of changes in growth given the plasticity and complexity of developmental timing.  

We will present a range of potential dynamical approaches to characterizing heterochrony [5] in a way that goes beyond existing models. Our approach is unique in that we reconsider the developmental trajectory as a series of autonomous developmental programs called triangular state machines (TSMs). With a focus on developmental timing, we will use formal techniques to characterize delays and bifurcations in the developmental trajectory. We also consider the role of multiple developmental programs operating either in parallel or serially that are able to characterize some of the immense diversity observed in animal development. Along the way, we will employ concepts such as delay dynamical equations and bifurcation theory that can enrich our understanding of heterochrony and complex developmental processes more generally.  

## Introduction  
The theory of heterochrony provides a framework for characterizing the nature of growth relative to adaptive changes in phenotype expressed in development and indicative of evolutionary history. Taking a dynamical systems view of heterochrony allows us to characterize less common modes of growth and transformation during development called _developmental incongruities_. Two examples of developmental incongruities are metamorphosis and the presence of nervous system with both ancestral and derived components. In both of these cases, features such as delays and switches between stable developmental trajectories can explain such phenomena. These type of features are underlain by overlapping gene expression networks, which form something we call a triangular state machine (TSM). In short, TSMs produce one or more developmental trajectories, changes in which can be described using a dynamical systems approach. The solution to these systems can be mapped to a phenotypic model, and may explain complexity in the developmental process.

### Acquisition of Developmental Sequences  
In Williamson [4], several examples are given (Echinoderms, Decapods, Trochophorates, and Bryozoans) with respect to incongruous larvae, or larvae stages that resemble those of distantly-related taxa. Two phylogenetic mechanisms [4, 6] have been proposed for developmental incongruity: hybridization and horizontal gene transfer. In the case of these mechanisms, there are two problems with purely empirical investigations. The first involves distinguishing between different larval stages originating in various species, particularly in terms of genetic control. Secondarily, there is a question of acquisition. While several candidate mechanisms are proposed, there is no theoretical model that explains such developmental incongruities.  

Related to these problems is whether multiple developmental stages accumulate through singular events that contributing to genetic variation within a species, or are acquired through mass acquisition. In the case of hybrids, combinations of genetic material from two independent species occur either in convergence zones [7, 8] or as multiple independent interbreeding events resulting in reticulate evolution [9, 10]. Furthermore, hybridization events can lead to both large-scale genomic rearrangements and changes in gene expression [11, 12]. Horizontal gene transfer provides a more explicit mechanism [13-15], but specific instances of such are no easier to empirically identify.  

### Expression of Developmental Sequences  
Heterochrony can be defined as changes in the rate of change in development for a specific trait, the resulting acceleration or deceleration being a result of tweaks made to the expression of genes in any given genetic regulatory network (GRN). In many cases including the hybridization cases Williamson describes, heterochrony is quite fluid relative to a linear developmental sequence and life-history. This is even true to the extent that adult sequences from distant taxa can be present in a given species' life-history [4, 6] observes two types of overlapping body symmetry in modern Holothurian life-history. This overlap is due to heterochronic changes in the expression of each type of symmetry relative to their ancestral expression: radial symmetry is accelerated and expressed in late larvae, while the disappearance of bilateral symmetry is decelerated so that it persists throughout adulthood. Williamson [6] also observes what he calls "start again" developmental sequences. An example of this is found in Trochophores, which express a Bryozoan-typical juvenile period in its life-history.  

### Predictions  

**H1:** a reconstituted tree can be used to represent compound heterochrony (swap tree branch sets at a node between trees).  

**H2:** a recombined tree can be used to represent compound heterochrony (file branch sets at a node within trees).  

**H3:** a differentially-stretched tree can be used to represent compound heterochrony (provides access to different parts of development).  

## Results

### Compound and Multiphasic Heterochrony  
We can go beyond the empirical work of Williamson and define two alternate models for characterizing heterochrony in life-history: multiphasic and compound. Each type relies upon the presence of two different developmental programs in the same organism.  



**Figure 1.** A step-by-step description of multiphasic heterochrony, in which the larval form (caterpillar) dedifferentiates into an intermediate pupae. The developmental trajectories of two different programs expressed as two different parts of life history. A) the caterpillar developmental program is active early in life-history, B) an intermediate stage occurs where all existing structure is obliterated, C) the butterfly developmental program is active later in life history.  


**Figure 2.** A step-by-step description of compound heterochrony, in which developmental trajectories from two different species overlap, resulting in a switch from one program to the other during the course of life history. A) the program from Species A is active early in life-history, B) a switch between developmental programs is activated, C) the program from species B is active later in life-history.  

### Computational Genetic Regulatory Network Model  
We use the computational model of Artyomov, Meissner, and Chakraborty [16] to approximate a suitable GRN. In this case, we represent the hierarchical GRN with a binary tree structure. Each node represents a hypothetical gene in its order of expression. Each level consist of hypothetical genes with equivalent order of expression. As a result, daughter genes at a single level of the binary tree are considered to be a single functional unit (cis) of DNA. By contrast, when a gene at one level turns on or off a gene at the next level, it is said to act in trans. This is because a binary division creates a new operon consisting of two genes: the mother gene activates the gene in trans and the daughter genes activate each other in cis. Lateral activations (within the same level of the tree) occurring between daughter pairs also activate each other in trans.  

These rules create something we call a Triangular State Machine (TSM). The TSM maps the three types of behavior embedded in network arcs to numeric states: a state of “0” equals “off”, a state of “1” equals “on in trans”, and a state of “2” equals “on in cis”. Table 1 shows all possible ordinal paths and their corresponding states for an order 3 binary tree.  

**Table 1.** All pairwise ordinal paths (network arcs) in an order 3 binary tree.  

| Ordinal Path      | State          |
|--------:|:-------:|:--------------:|
|-        |0        |1               |
|-        |0        |1               |
|0        |00       |1               |
|0        |01       |1               |
|1        |10       |1               |
|1        |11       |1               |
|01       |10       |1               |
|0        |1        |2               |
|00       |01       |2               |
|10       |11       |2               |



