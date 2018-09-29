# im2model_dissertation

This dissertation has 7 chapters, each with their summary presented bellow. The first 3
chapters go through the fundamental ideas that apply to both scientific software and high
performance software, whether running on a single machine or distributed across a cluster
of machines.

 Introduction: Presenting the motivation for this dissertation, and illustrating the desired
sample input and output of Im2Model.

 Atomic Models for TEM Image Simulation and Matching: Presenting the state-ofthe-
art regarding the crystallographic indexing of nano-structured materials, methodologies
for TEM image simulation, and image correlation algorithms, presenting us
to the internals of scientific simulation.

 Computational Efficiency: Presenting the state-of-the-art art in terms of hardware
and software performance metrics and modelling.
It examines what we actually mean by words like efficiency and scalability, and how
we can try to achieve these goals.
Later, the following 4 chapters will turn to the particular issues of the simulation of the
described physical process in distributed systems.

 The Product: Describing in detail the current solution legacy systems dependencies,
and dividing different models and their components by their specific Ubiquitous Language
and forming multiple Bounded Contexts.

 Efficient implementations of Im2model workflow:
The previously described architecture, had functionality built on the same machine.
These functional groups are tightly coupled, symbiotic systems. They depend on local,
shared resources like disk, network interface, or inter-process communications.
This chapter focus on modelling and implementing the system to achieve the level of
reliability, agility, and scale expected, built out of many different components running
in different processes and communicating over distinct means spread across multiple
machines, with elastic on-demand resource allocation. We will also be focusing
attention on the resources that are exchanged between Bounded Contexts.
Considering we are modelling software to runs on several machines, connected by
several distinct networks, faults and failures will be also taken in account in the design
and implementation stages. We are no longer operating in an ideal system model, but
in nondeterministic one with the possibility of partial failures. Therefore, we will
discuss a wide range of problems that can occur in the modelled distributed system.

 The test boundary:
This chapter dives into the different types of tests we have run to effectively and
efficiently test the system functionalities when they spanned into a distributed system,
while also breaking down the problems associated with testing finer-grained systems.
It presents an overview of the results obtained by the preliminary experimental work
developed.

 Conclusion: Presenting an overview of Im2Model major challenges until the current
developing stage and future steps.
