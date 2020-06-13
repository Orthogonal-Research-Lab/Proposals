<p align="center">
  <H2>Developmental Embodied Agents as Meta-brain Models</H2>
</p>
<p align="center">
  <H3>Abstract</H3>
</p>
We present a framework for meta-brain models, or hybrid models that capture multiple aspects of developmental neurobiology and behavior. A developmentally-inspired embodied learning agent architecture is combined with a contextually-explicit representational layer to form a complex artificial nervous system. The architectural description is summarized in terms of morphological differentiation, context-handling, and generalized architectural features. In conclusion, we propose potential functional milestones that help further explicate the usefulness of our approach. 
<p align="center">
  <H3>Introduction</H3>
</p>
Building life-like architectures introduces a modeling challenge. On the one hand, it is parsimonious to create a minimal model [1]. This produces a desired behavior according to extremely simplified mechanisms and metaphors [2]. An opposing view is that maximal representation [3] is the only way we can truly capture realistic phenomena. This approach requires the synthesis of data and mechanisms from many different parts of an organism's biology [4]. We will propose a third path toward simulating intelligent behavior, a generalized hybrid architecture called _meta-brain models_. Meta-brain models are abstractions that capture essential structural and functional features of biological nervous systems. Additionally, meta-brain models should be computationally and conceptually diverse, encompassing multiple attributes of the simulated biology in a biologically-inspired manner. These include a variety of features that include but are not limited to: explicit developmental processes, layering of hybrid model components, the introduction of innate mechanisms, and a distinction between degrees of representation.
<p align="center">
  <H3>Embodied Developmental Hybrid Agents</H3>
</p>
We propose that embodied developmental agents that can integrate context are the way forward. In [5], developmental Braitenberg Vehicles (dBVs) are used to build a nervous system and interact with its environment. Braitenberg Vehicles [6] are embodied agents that utilize a neuronal network (consisting of a dBVs intermediate nodes) to transfer information between sensor and effector. The vehicle interacts explicitly with the environment, as well as exhibiting both internal regulation and spatial awareness. The developmental component is implemented through changes in neuronal network connectivity with respect to time. Yet the developmental aspects of dBVs are not limited to mere connectivity. More generally, connectionist models [7] have been found suitable for representing developmental phenomena such as the nonlinear generation of sequential growth and critical periods of learning.

Despite their developmental aspect, dBVs are largely representation-free in that they do not make any assumptions about the external world. There are in fact innate aspects to this architecture that serve well as a basal component of the meta-brain architecture. In their non-developmental models, BVs tend to exhibit habits that reflect excitatory and inhibitory connections between sensors, intermediate nodes, and effectors [8]. BVs can exhibit rudimentary behaviors identified as "happiness", "love", or "aggression", which are associated with static body plans. The behaviors are rudimentary because they are essentially the outcome of hard-wired configurations. Suppose we make these connections plastic, and thus change their configuration over time. Will this result in significant fluctuations in the observed emotional state? To minimize this, a second layer is required to control behavioral degeneration due to the developmental process, particularly one that enables a contextual representation of emotional states.

### Morphological Differentiation as Growth
Before we discuss the second layer of context, we must first address how to implement the growth of a representation. Growth can be characterized as a form of morphological differentiation in which structure and/or function can become increasingly diverse. In this case, growth reflects increasing the size of a network. Yet as mentioned earlier, the growth of a dBV neuronal network can diversify (or in some cases obscure) the expression of habits and other behaviors. 

The meta-brain architecture presented here involves implementing a technique for neuronal network growth in dBVs (Figure 1). Network growth proceeds through _connectivity-activation encoding_, in which matrix _W(i,j)_ of potential connections between intermediate nodes expands (potential connections removed) and/or is pruned (potential connections removed) over developmental time. Updating _W(i,j)_ is generally a discrete process. We have approached connectivity-activation encoding using two different techniques: Hebbian Learning and Genetic Algorithms [9]. Hebbian Learning has been used to introduce a basic form of multisensory integration to the dBV, while genetic algorithms have been used to enforce developmental recombination of existing nodes.

In the case of our Hebbian Learning approach, development is instantiated by building associations between olfactory and gustatory stimuli. The developmental process changes the connection weights in matrix _W(i,j)_ such that it can acquire spatially-explicit multimodal associations. Unfortunately, the Hebbian Learning approach is brittle and reveals a limited capacity for learning dynamically-changing spatial distributions of stimuli.

Our genetic algorithm generates a variety of topological orderings of matrix _W(i,j)_ through mutation and recombination. The distance between stimuli and the vehicle, as well as the force generated by vehicles in response to a given stimulus are used as a fitness function to evaluate the dBV neuronal network. Even though evolutionary variety randomizes matrix elements over time, selection nevertheless favors the emergence of specific behaviors such as spatial navigation. For larger dBV neuronal networks, we could use a Genetic Algorithm that encodes coordinated projection identity, which is similar to how axonogenesis proceeds in the _Drosophila_ nervous system [10].

<p align="center">
   <IMG SRC="https://github.com/Orthogonal-Research-Lab/Proposals/blob/master/Developmental%20Neural%20Networks/Figure%201.png">
</p>
Figure 1. An example of wiring expansion in a hybrid dBV/CGS agent.

### Morphological Differentiation as Layering
The developmental process also includes a form of morphological differentiation called layering (Figure 2). Implementing a second layer as an extension of the first allows us to both benefit from the diversity of multiple models and better utilize the processing potential of structures like the thalamocortical system in mammalian brains. We utilize an representational approach called Contextual Geometric Structures (CGS), which allows us to capture multiple features of the environment as a surface bounded by overlapping dimensions [9]. A soft classification scheme is used to build representations with meaning and significance that resemble cultural referents. We can use phototaxis, or attraction/repulsion behaviors in response to light, as an example. While an unlayered dBV will simply exhibit a reactive behavior to light, a layered dBV coupled to a CGS will be able to evaluate the light source in the context of all physical gradations ranging from absolute light to absolute dark. 

<p align="center">
   <IMG SRC="https://github.com/Orthogonal-Research-Lab/Proposals/blob/master/Developmental%20Neural%20Networks/Figure%202.png">
</p>
Figure 2. An example of generic layering in a sample agent.

CGS kernels create a binary opposition between two extreme labels, then use empirical data to build a model of the world. These empirical observations are made by the dBV, with connections between the intermediate nodes of the dBV and the CGS kernel. A CGS does not observe the world directly in this case, but operates on information processed by the dBV. When coupled with dBVs, CGS allow for stimuli for be mapped to a representational space that adds relational context to the original signal (Figure 2). This context then allows for greater control of outputs to the effector, as well as modulation of temporal changes in the dBV's neuronal network. 
<p align="center">
  <H3>How to Develop Context</H3>
</p>
Contextual behaviors emerge from interactions between the dBV architecture and the CGS classification kernel. Contextual behaviors are informed by long-term observations of the environment, and the representation of such behaviors result from combining taxis and proportional membership in related binary categories (see Figure 3). We can take phototaxis as an example: dBVs will exhibit phototaxis, which are simple attraction/repulsion behaviors to a light stimulus. We can then use a one-dimensional CGS kernel to classify the relative presence or absence of light in the environment. The membership function over time will reflect the agent's experience with light (whether it is present or absent). In this way, we can incorporate not only probabilistic information, but higher-level interpretation of what the presence or absence of light means. 

Suppose we expand our representation to a two-dimensional kernel, with light-dark and safety-danger as the axes. Now we can establish lineages between observations of the presence of light and the result of being exposed to light (whether it is harmful or not). In this way, we combine the associative learning introduced by a developing neuronal network in the dBV with conditional learning introduced by the CGS kernel. By combining the action of both types of models, this can be done without large amounts of data or a formal statistical distribution. While this does not prevent the agent from making category errors, it does provide a means to build nuance from observations of the world using a common conceptual framework.
<p align="center">
  <H3>Architectural Features</H3>
</p>
We can potentially use a wide range of model types to introduce layering. Here, we use dBVs to process data from the environment along with CGS as a means to introduce representation of context. Using these two models in tandem creates both advantages and drawbacks. Any implementation of layering must allow for the following architectural features: innate components, dynamic components, and bio-inspired components.

### Innate Components
In the implementation of contemporary neural networks, innateness is a forgotten but potentially crucial component in aiding the artificial learning process [11]. According to [12], combining symbolic and connectionist architectures can draw upon the strengths of each type of formalism. Connectionist architectures are considered a form of sub-symbolic cognition, which can only approximate symbolic processes, and even then only under certain circumstances [13]. Yet the dBV architecture is not the only innate aspect of our featured model. CGS kernels use basic concepts as innate components, often encoded as limits of a metric space.

In a traditional BV [6], simple behaviors are not so much learned as they are the product of excitation and inhibition of connections that link the sensors and effectors. The sensors take in information about the stimulus and transfer information towards the effector. This connection exists in either an excitatory or inhibitory state. This in turn controls movement of the vehicle's trajectory, which determines the behavioral state. We define vehicle trajectories in two ways: as a dot product (angle between two vectors) and as differential bilateral motion (continuous difference between left and right wheel rotation speeds) [6]. 

<p align="center">
   <IMG SRC="https://github.com/Orthogonal-Research-Lab/Proposals/blob/master/Developmental%20Neural%20Networks/Figure%203.png">
</p>
Figure 3. Membership functions for _R,G,B,Polygon_. A and B represent the _R,G,B_ color space as CGS membership functions. C represents a gradient of shapes transformations (+ is increasing membership).

### Dynamic Components
There are a number of ways to implement a dynamic set of processes that unfold over developmental time. These range from increasing numbers of neuronal cells to the cumulative effects of stimulus encounters and even the gradual interfacing between layers. The dBV-CGS layered can be referred to as a tightly-coupled hybrid architecture [11]. In such an architecture, it is critical to have an embodied lower layer. In general, embodiment is a critical component of animal development, as it enables learning and behavioral coordination via the sensorimotor loop [14].

One dynamic component is the relationship between the connectivity-activation encoding of a traditional BV and the more dynamic (and potentially unstable) connectivity-activation encoding of a dBV. We can revisit this not as something that needs to be dynamically regulated, but as something that can be used as a difference to be understood. This differential output is captured in terms of trajectory (as mentioned in the last section), and is fed to the CGS representational layer to enable contextual classification. 

### Bio-inspired Components
We can also exploit the biological features of development to govern both the growth of neuronal networks within dBVs and the layering of dBVs and CGS components. For example, morphogenesis of the _C. elegans_ connectome is defined by three properties: most neuronal cells are born within a 135 minute window, conservation of cell spatial position from development to adulthood, and temporal separation of neuronal differentiation and electrical connectivity [15, 16]. We can also build upon heterochronic mechanisms [17, 18] to control the growth of our systems in a manner that also invokes innate mechanisms. Of particular interest is the ability to simulate how different modules of the hybrid system develop at distinct rates.
<p align="center">
  <H3>Discussion</H3>
</p>
Now that we have demonstrated how a hybrid representation using different formalisms can work together to simulate development and behavior [19], we must consider how a expansive and layered system might improve performance on a number of functional milestones. While we have not formally benchmarked our architecture on these tasks, they might serve as future goals for implementation.

One example of how a representation-rich architecture might improve the performance of a dBV is the ability to learn chromotaxis. Chromotaxis are built from phototaxis exhibited by the dBV, but use a CGS representation of _R,G,B_ components of a light source to enable distinctions between different properties in the same source. While this requires color information and the appropriate CGS representation, it also allows for more nuanced behaviors to be exhibited by the dBV.

Multisensory integration is known for its nonlinear effects, particularly the sub- and super-additive effects of spatial coincidence [20]. When multiple sensory components of a stimulus are presented in the same location, the nervous system response is superadditive. We have shown that this can be a mechanism of connectivity-activation encoding in dBVs. In future work, we will seek to understand multisensory integration as a function of the representational layer (CGS).

Lastly, the CGS representation allows for membership functions of objects to be derived for multiple categories. For example, suppose we assume all objects are a combination of aggression-provoking, cowardness-provoking, and love-provoking. A particular stimulus is classified as 55 percent aggression-provoking, 30 percent cowardness-provoking, and 10 percent love-provoking. This allows us to refine the classification of objects in the environment, and contributes to ambiguous or novel intermediate behaviors.

<p align="center">
  <H3>References</H3>
</p>

[1] Lyon, P. (2019).  Of what is ”minimal cognition” the half-baked version? _Adaptive Behavior_, 1–18.  

[2] Levins, R. (2006). Strategies of abstraction. _Biology and Philosophy_, (21), 741–755.

[3] Feig, M. and Sugita, Y. (2013). Reaching New Levels of Realism in Modeling Biological Macromolecules in Cellular Environments. _Journal of Molecular Graphics and Modeling_, 45, 144–156.

[4] Fan, X. and Markram, H. (2019). A Brief History of Simulation Neuroscience. _Frontiers in Neuroinformatics_, 13(10), 32.

[5] Dvoretskii, S., Gong, Z., Gupta, A., Parent, J., and Alicea, B. (2020). Braitenberg Vehicles as Developmental Neurosimulation. _arXiv_, 2003.07689.

[6] Braitenberg, V. (1984). Vehicles: Experiments in synthetic psychology. MIT Press, Cambrdige, MA.

[7] Munakata, Y. and McClelland, J. (2003). Connectionist models of development. _Developmental Science_, 6(4), 413–429.

[8] Egbert, M. and Barandiaran, X. (2014). Modeling habits as self-sustaining patterns of sensorimotor behavior. _Frontiers in Human Neuroscience_, 8, 590.

[9] Alicea, B. (2012).  Contextual Geometric Structures: modeling the fundamental components of cultural behavior. _Proceedings of Artificial Life_, 13, 147–154.

[10] Zhang, M., Ergin, V., Lin, L., Stork, C., Chen, L., and Zheng, S.(2019). Axonogenesis Is Coordinated by Neuron-Specific Alternative Splicing Programming and Splicing Regulator PTBP2. _Neuron_, 101, 690–706.

[11] Zador, A. (2019). A critique of pure learning and what artificial neural networks can learn from animal brains. _Nature Communications_, 10(3770).

[12] Wermter, S. and Sun, R. (1998).  An overview of hybrid neural systems. _International Workshop on Hybrid Neural Systems_, 1–13.

[13] Smolensky, P. (1988). On the proper treatment of connectionism. _Behavioral and Brain Sciences_, 11, 1–74.

[14] Smith, L. (2005). Cognition as a dynamic system: Principles from embodiment. _Developmental Review_, 25(3-4), 278–298.

[15] Alicea, B. (2018). The Emergent Connectome in _Caenorhabditis elegans_ Embryogenesis. _BioSystems_, 173, 247–255.

[16] Pathak, A., Chatterjee, N., and Sinha, S. (2020). Developmental trajectory of _Caenorhabditis elegans_ nervous system governs its structural organization. _PLoS Computational Biology_, 16(1), e1007602.

[17] Antonelli, P., Bradbury, R., Krivan, V., and Shimada, H. (1993). A dynamical theory of heterochrony: time-sequencing changes in ecology, development, and evolution. _Journal of Biological Systems_, 1(4), 451–487.

[18] Richardson, M. (1999). Vertebrate evolution: the developmental origins of adult variation. _BioEssays_, 21, 604–613.

[19] Bardini, R., Politano, G., Benso, A., and Di Carlo, S. (2017). Multi-level and hybrid modelling approaches for systems biology. _Computational and Structural Biotechnology Journal_, 15, 396–402.

[20] Jiang, W., Jiang, H., and Stein, B. (2002). Two Corticotectal Areas Facilitate Multisensory Orientation Behavior. _Journal of Cognitive Neuroscience_, 14(8), 1240–1255.
