# Proofs of DOLCE version in OWL2

## DOLCEbasic<sub>OWL</sub>

**DOLCEbasic<sub>OWL</sub>** [ontology](https://w3id.org/DOLCE/OWL/DOLCEbasic) (accessible in [this repo](https://github.com/appliedontolab/DOLCE/tree/main/OWL/)) formalizes the core theory of DOLCE in OWL2 language.
DOLCEbasic<sub>OWL</sub> was developed by Laure Vieu and Daniele Porello with contributions by
W. Terkaj, S. Borgo, C. Masolo, E. M. Sanfilippo, F. Compagno.

PROVER9 was used to prove that the first-order logic version of DOLCE (named DOLCEsimple<sub>FOL</sub>) entails DOLCEbasic<sub>OWL</sub>. Relevant files supporting the proof are provided in the following folders.

1. The folder [DOLCEsimpleConsistency](DOLCEsimpleConsistency/) contains:
    * the first-order logic version of DOLCE ([DOLCEsimpleConsistency.in](./DOLCEsimpleConsistency/DOLCEsimpleConsistency.in)) in the syntax of [PROVER9/MACE4](https://www.cs.unm.edu/~mccune/prover9/).
    * the proof of its consistency by including a model generated by MACE4 ([DOLCEsimpleConsistency.cooked](./DOLCEsimpleConsistency/DOLCEsimpleConsistency.cooked)).

2. The folder [DOLCEsimpleFOL_to_DOLCEbasicOWL](./DOLCEsimpleFOL_to_DOLCEbasicOWL/) contains:
    * the translation of the axioms of the OWL2 ontology DOLCEbasic<sub>OWL</sub> into first-order logic in the syntax of PROVER9 ([report_DOLCEbasicOWL_axioms.txt](./DOLCEsimpleFOL_to_DOLCEbasicOWL/report_DOLCEbasicOWL_axioms.txt)). A dictionary to read the names of the classes in DOLCEsimple<sub>FOL</sub> and DOLCEbasic<sub>OWL</sub> is presented at the beginning of the file. The list of axioms of DOLCEbasic<sub>OWL</sub> is commented to indicate the definitions of DOLCEsimple<sub>FOL</sub> required to prove each axiom.
    * The Ontology DOLCEsimple to perform the proof by means of PROVER9 ([DOLCEsimpleFOL_to_DOLCEbasicOWL.in](./DOLCEsimpleFOL_to_DOLCEbasicOWL/DOLCEsimpleFOL_to_DOLCEbasicOWL.in)). The axioms of DOLCEbasic<sub>OWL</sub> are translated into first-order logic using an [extension of Gavel](https://github.com/gavel-tool/python-gavel-owl).
