# Effective guide to maintain the metadata of your ontology #
IndustryPortal aims to ensure that curated ontologies are FAIR by attaching detailed metadata for finding, accessing, integrating and reusing every ontology with ease. The team at IndustryPortal continuously make effort in improving the quality of metadata of every ontology but the it is also a responsibility of every submitter of ontology to provide accurate information for various metadata for each version of the ontology submitted by them. It is therefore highly recommended for every stakeholder of IndustryPortal to review the following guide before submitting an ontology. 

## URI ##
The default IRI of the ontology. 

The value of this metadata is same as the base namespace in the corresponding RDF/XML or OWL/XML encoding, e.g., `xml:base="http://www.w3.org/2002/07/owl"`. OWL 2.0 specification saves this value in vocabulary `ontologyIRI`.   

***Note**: Default IRI of an ontology may not be resolvable in some cases.*

> URI of [ROMAIN](http://industryportal.enit.fr/ontologies/ROMAIN) is `http://www.semanticweb.org/hedi/ontologies/2018/11/ROMAIN`, 
> URI of [SSN](http://industryportal.enit.fr/ontologies/SSN/?p=summary) is `http://www.w3.org/ns/ssn/`

## Status ##
Information about the ontology status (alpha, beta, production, retired).

***Note**: The interpretation of the status labels are up to the ontology developers. However, they should loosely corresponds to the standard understanding of software development community, e.g., the status of an ontology is alpha if the ontology has been encoded completety but is not yet tested or under testing, beta if the ontology has been completely tested for all primary features but may still contain several errors or pending issues to be resolved, production if the ontology is released, and retired if the ontology has been deprecated.*

*Industrial Ontology Foundry (IOF) prescribe vocabulary for maturity levels, which can be mapped to the ontology status as: if maturity level is iof-av:Released then the status is production and if iof-av:Provisional then the status is beta*









