This zip contains the files and programs we used to evaluate our
SPARQL OWL Entailments implementation.

To test the Ontop system use OntopLUBM.jar and project parameters.
The ontology and mappings are in the folder Ontop.

The structure is as follows:
java -jar OntopLUBM.jar ontology.owl mapping.obda [optional parameter]

For examples:
To run LUBM(1,0) with the standard 14 LUBM queries type:
java -jar OntopLUBM.jar univ-benchQL.owl univ-benchQL.obda

To run LUBM(9,0) with the 4 added queries type:
java -jar OntopLUBM.jar univ-benchQL.owl univ-bench9QL.obda special

To run LUBM(20,0) with the SPARQLDL queries type:
java -jar OntopLUBM.jar univ-benchQL.owl univ-bench20QL.obda DL

To test OWL-BGP system use HermitLUBM.jar or PelletLUBM.jar and project parameters
The ontologies are in OWL-BGP/evaluation/ontologies unzipping the file evaluation.7z

It is necessary to have the folders /evaluation/ontologies to execute the jar.

The structure is as follows:
java -jar HermitLUBM.jar  -parameter to use OWL-BGP with Hermit Reasoner
java -jar PelletLUBM.jar  -parameter to use OWL-BGP with Pellet Reasoner

For examples:
To run LUBM(1,0) with the standard 14 LUBM queries and Pellet reasoner type: 
java -jar PelletLUBM.jar -LUBM1

To run LUBM(9,0) with the 4 added queries and Hermit reasoner type:
java -jar HermitLUBM.jar -special9

To run LUBM(20,0) with the SPARQLDL queries and Hermit reasoner type:
java -jar HermitLUBM.jar -DL20





