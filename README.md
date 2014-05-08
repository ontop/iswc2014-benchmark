iswc2014-benchmark
==================
### Ontop Benchmark ###
To test the Ontop system use **OntopLUBM.jar** in Ontop folder and add the project parameters as follows:

 `java -jar OntopLUBM.jar ontology.owl mapping.obda [optional parameter]`
 
 The ontology and mappings are provided in the folder Ontop.

For examples:
* To run LUBM(1,0) with the standard 14 LUBM queries type:
 `java -jar OntopLUBM.jar univ-benchQL.owl univ-benchQL.obda`

* To run LUBM(9,0) with the 4 added queries type:
 `java -jar OntopLUBM.jar univ-benchQL.owl univ-bench9QL.obda special`

* To run LUBM(20,0) with the SPARQLDL queries type:
 `java -jar OntopLUBM.jar univ-benchQL.owl univ-bench20QL.obda DL`

### OWL-BGP Benchmark ###
To test OWL-BGP system use OWLBGPHermit.jar or OWLBGPPellet.jar and project parameters.

These jar files modify the  [OWL-BGP code] (https://code.google.com/p/owl-bgp/).

To run OWL-BGP code with OWL 2 QL modeling of LUBM use the jar OWLBGPPelletQL or OWLBGPHermitQL and project parameters.

The ontologies are given in [evaluation.7z] (https://github.com/ontop/iswc2014-benchmark/raw/master/OWL-BGP/evaluation.7z) . 

It is necessary to unzip the file and keep the folders ''/evaluation/ontologies'' to execute the jar.

To execute the jar only one parameter is necessary as follows:

 `java -jar OWLBGPHermit.jar  -parameter to use OWL-BGP with Hermit Reasoner`
 
 `java -jar OWLBGPPellet.jar  -parameter to use OWL-BGP with Pellet Reasoner`

For examples:
* To run LUBM(1,0) with the standard 14 LUBM queries and Pellet reasoner type: 
 `java -jar OWLBGPPellet.jar -LUBM1`

* To run LUBM(9,0) with the 4 added queries and Hermit reasoner type:
 `java -jar OWLBGPHermit.jar -special9`

* To run LUBM(20,0) with the SPARQLDL queries and Hermit reasoner type:
 `java -jar OWLBGPHermit.jar -DL20`

### Pellet Benchmark ###
To test Pellet system use Pellet.jar and project parameters.
The ontologies are given in [evaluation.7z] (https://github.com/ontop/iswc2014-benchmark/raw/master/Pellet/ontologies.7z).

To execute the jar add parameters as follows:

 `java -jar Pellet.jar ontology.owl -parameter`
 
 For examples:
* To run LUBM(1,0) with the standard 14 LUBM queries type: 
 `java -jar Pellet.jar Uni1.owl LUBM`

* To run LUBM(9,0) with the 4 added queries type:
 `java -jar Pellet.jar Uni9.owl special`

* To run LUBM(20,0) with the SPARQLDL queries type:
 `java -jar Pellet.jar Uni20.owl DL`
