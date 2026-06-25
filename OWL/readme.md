Folder to contain files of versions of DOLCE serialized in the OWL2 language.

The main references for the ontologies here contained are:

- Porello, D., Vieu, L., Terkaj, W., Borgo, S., Compagno, F., & Sanfilippo, E. M. (2024, July). DOLCE in OWL: The core theory. In 8th Workshop on Foundational Ontology (FOUST VIII)-Joint Ontology Workshops (JOWO)-Episode X: The Tukker Zomer of Ontology, and satellite events. CEUR Workshop Proceedings.
  [https://doi.org/10.1177/15705838251401](https://doi.org/10.1177/15705838251401)
  
- Masolo, C., Porello, D. Borgo, S., Ferrario, R., Mosca, A., Sanfilippo, E.M., Stufano, R., Terkaj, W. (2026). Adding an Epistemic Layer to DOLCE. Proceedings of the 16th International Conference on Formal Ontology in Information Systems (to appear), IOS Press

### Contents

- [DOLCEbasic.owl](https://github.com/appliedontolab/DOLCE/blob/main/OWL/DOLCEbasic.owl): the DOLCEbasic module of DOLCE in OWL;
- [DOLCEnaryRel.owl](https://github.com/appliedontolab/DOLCE/blob/main/OWL/DOLCEnaryRel.owl): the DOLCenaryRel module of DOLCE in OWL;
- [DOLCEepistemic.owl](https://github.com/appliedontolab/DOLCE/blob/main/OWL/DOLCEepistemic.owl): the DOLCEepistemic module of DOLCE in OWL;
- [DOLCEtweaks.owl](https://github.com/appliedontolab/DOLCE/blob/main/OWL/DOLCEtweaks.owl): the DOLCEtweaks module of DOLCE in OWL (an experimental module containing an object property that is not directly derivable from DOLCE, but it is still aligned with its philosophical approach.

### Versioning instructions

Upload a file called DUMMY.owl to upload the most recent version of DUMMY ontology. Then requests to the address https://www.w3id.org/DOLCE/OWL/DUMMY and similar (e.g. https://www.w3id.org/DOLCE/OWL/DUMMY/, https://www.w3id.org/DOLCE/OWL/DUMMY.owl) will be answered with the file <NAME>.owl

Upload a file called DUMMY-n.m (but also DUMMY-n.m.p, or DUMMY-nm, ecc.) to upload a specific version of DUMMY ontology. Then requests to the address https://www.w3id.org/DOLCE/OWL/DUMMY/n.m will be answered with the file DUMMY-n.m.owl

For instance, the last version of DOLCEbasic should always be accessible at https://www.w3id.org/DOLCE/OWL/DOLCEbasic.owl

### Current rules for versioning
Semantic versioning is employed, with the following conventions:
- The version number can either be in the form *n.m* or *n.m.r*. The form *n.m* is a shortcut for *n.m.0*
- Only versions like *n.m* are published as version IRIs, while forms like *n.m.r* are used internally to track minor changes
- Every ontology file must have an owl:versionInfo annotation with the version number in a shape of either *n.m* or *n.m.r*
- Every version number change corresponds to a GitHub commit. GitHub commits may not correspond to version changes, this happens when they correspond to e.g. correcting errors related to GitHub workflow and such. 
- The first digit changes only when significant ontological aspects are changed
- The second digit changes only when incompatibilities may arise with previous versions (e.g. anytime that an IRI is modified)
- The third digit changes only when minor changes happen (e.g. change of the text of an annotation)
