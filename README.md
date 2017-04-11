## Extension "FrCranMetr" for RDFBones-O
This is an RDFBones extension for craniometrics. The landmark-based cranial and mandibular measurements of FrCranMetr are according to Burns 2007. However, the extension was named "FrCranMetr" for two reasons. First, the abbreviation should be consistent with all the other extensions developed for RDFBones. Second, table 3.3 of Burns 2007 was used at the department of Biological Anthropology Freiburg to record a subset of craniometric measurements taken from skulls from the Alexander Ecker Collection in order to deal with repatriation claims. For further information on the Alexander Ecker Collection cf. Kästner et al. 2011.

Since the set of measurements contained in FrCranMetr is congruent with [FORDISC](https://fac.utk.edu/fordisc-3-1-personal-computer-forensic-discriminant-functions/), the data sets generated in FrCranMetr investigations can be further used for ancestry or sex estimation with [FORDISC](https://fac.utk.edu/fordisc-3-1-personal-computer-forensic-discriminant-functions/).

Furthermore, FrCranMetr is enriched with detailed information on the landmarks used. In the [OBO-version of the FMA](http://www.obofoundry.org/ontology/fma.html), cranial and mandibular landmarks are subclasses of 'Anatomical points of skull'. These classes were integrated in FrCranMetr and the landmark definitions from Burns 2007 were added as descriptions to the relevant classes. Thus, FrCranMetr is more than just a spreadsheet for data entry: FrCranMetr documents the whole investigation process and thereby contributes to transparency and repeatability of anthropological investigations. 

## Wiki index
A thorough documentation of this ontology can be found here: https://github.com/RDFBones/CranioMetrics/wiki The structure of the FrCranMetr ontology is based on the concept of RDFBones extensions first elaborated in the extension FrSexEst. Thus, this wiki is shorter than the [FrSexEst wiki](https://github.com/RDFBones/FrSexEst/wiki) and focuses more on the anthropological workflow. Readers interested in developing their own extension should rather have a look at the [FrSexEst wiki](https://github.com/RDFBones/FrSexEst/wiki) which discusses some technical as well as philosophical/ontological issues related to extension writing. This wiki covers the following topics:
* Anthropological background
* General structure of FrCranMetr
* Investigation planning
     - Study design
* Study design execution
     - Specimen collection
     - Data collection
* Conclusion

The network graphs shown in this wiki follow the [key to symbols in network graphs](https://github.com/RDFBones/RDFBones-O/wiki/Network-graph-legend) defined in the RDFBones-O wiki.

## References
Burns, K. R. (2007). Forensic anthropology training manual. Pearson Education.

FORDISC help file: http://math.mercyhurst.edu/~sousley/Fordisc/Help/Fordisc3_Help.pdf, accessed on the 28th of February 2017

Kästner, M., Ortolf, S., Rüdell, A., Möller, D., & Wittwer-Backofen, U. (2011). The Alexander Ecker Collection in Freiburg. Documenta Archaeobiologiae, 8, 275-284.

## For future development
* xsd:float is not the best data type for skull measurements; it would be better to have a variety of data types to choose, for example integers or specifically non-negative integers
* The input of the specimen collection process is complicated since all bones which constitute the lambda, for instance, are required; a secondary inventory which consists of craniometric points instead of whole bones is required
* The Conclusion.FrCranMentr is superfluous and should be omitted
* Cardinality restrictions could be used more often if the RDFBones software would evaluate them correctly


