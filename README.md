# Formal Methods Workbench

The Formal Methods Workbench is composed of various analysis and
synthesis tools targeting model-based development of cyber-resilient
systems.  Presently, several tools are in development.  Presently,
this Eclipse P2 composite repository contains the following tools.

## Assume-Guarantee REasoning Environment

The [Assume Guarantee REasoning
Environment](https://github.com/loonwerks/AGREE.git) (AGREE) is a
compositional, assume-guarantee-style model checker for
[AADL](https://aadl.info) models. It is compositional in that it
attempts to prove properties about one layer of the architecture using
properties allocated to subcomponents. The composition is performed in
terms of assumptions and guarantees that are provided for each
component. Assumptions describe the expectations the component has on
the environment, while guarantees describe bounds on the behavior of
the component. AGREE is integrated into the [OSATE](https://osate.org)
AADL model development environment and uses k-induction as the
underlying algorithm for the model checking.

## Resolute Assurance Case Analysis

[Resolute](https://github.com/loonwerks/Resolute.git) allows users to
define a set of claim functions and associate them with an AADL
model. You can use these claim functions to represent the requirements
to be satisfied, the verification actions used to verify them, and
assumptions made by a verification action in order to produce a valid
result. With the Resolute tool, users define claim functions and
computational functions in Resolute annex libraries, i.e., Resolute
annex clauses placed directly in an AADL package. The verification
results are then displayed in a view labeled Assurance Case.

## Safety Analysis

The Safety Annex for the Architecture Analysis and Design Language (AADL)
provides the ability to reason about faults and faulty component behaviors in
AADL models. In the Safety Annex approach, we use formal assume-guarantee
contracts to define the nominal behavior of system components. The nominal
model is then verified using the Assume Guarantee Reasoning Environment
(AGREE). The Safety Annex provides a way to weave faults into the nominal
system model and analyze the behavior of the system in the presence of faults.
We also providea library of common faultnode definitions that is customizable
to the needs of system and safety engineers.  The Safety Annex supports model
checking and quantitative reasoning by attaching behavioral faults to
components and then using the normal behavioral propagation and proof
mechanisms built into the AGREE AADL annex. This allows users to reason about
the evolution of faults over time, and produce counterexamples demonstrating
how component faults lead to system failures. It can serve as the shared model
to capture system design and safety-relevant information, and produce both
qualitative and quantitative description of the causal relationship between
faults/failures and system safety requirements.

## BriefCASE

BriefCASE is a collection formal system modeling and transformation
tools supporting and developed by the DARPA CASE program.

## JKind Model Checker Plug-in

Packages the [JKind](https://github.com/agacek/jkind) model checker
into [jkind-plugin](https://github.com/loonwerks/jkind-plugin), an
Eclipse Plugin for convenient use in Eclipse-based analysis tools.

## Z3-Prover Plug-in

Packages the Microsoft [Z3-Prover](https://github.com/Z3Prover/z3) SMT
solver into [z3-plugin](https://github.com/loonwerks/z3-plugin), an
Eclipse Plugin for convenient use in Eclipse-based analysis tools.
