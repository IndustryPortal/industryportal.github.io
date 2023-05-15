# Effective guide to maintain the metadata of your ontology #
IndustryPortal aims to ensure that curated ontologies are FAIR by attaching detailed metadata for finding, accessing, integrating and reusing every ontology with ease. The team at IndustryPortal continuously make effort in improving the quality of metadata of every ontology but the it is also a responsibility of every submitter of ontology to provide accurate information for various metadata for each version of the ontology submitted by them. It is therefore highly recommended for every stakeholder of IndustryPortal to review the following guide before submitting an ontology. 

## Key Properties ##

### URI ###
The default IRI of the ontology. 

The value of this metadata is same as the base namespace in the corresponding RDF/XML or OWL/XML encoding, e.g., `xml:base="http://www.w3.org/2002/07/owl"`. OWL 2.0 specification saves this value in vocabulary `ontologyIRI`.   

***Note**: Default IRI of an ontology may not be resolvable in some cases.*

> URI of [ROMAIN](http://industryportal.enit.fr/ontologies/ROMAIN) is `http://www.semanticweb.org/hedi/ontologies/2018/11/ROMAIN`, 
> URI of [SSN](http://industryportal.enit.fr/ontologies/SSN/?p=summary) is `http://www.w3.org/ns/ssn/`

### Status ###
Information about the ontology status (alpha, beta, production, retired).

***Note**: The interpretation of the status labels are up to the ontology developers. However, they should loosely corresponds to the standard understanding of software development community, e.g., the status of an ontology is alpha if the ontology has been encoded completety but is not yet tested or under testing, beta if the ontology has been completely tested for all primary features but may still contain several errors or pending issues to be resolved, production if the ontology is released, and retired if the ontology has been deprecated.*

*Industrial Ontology Foundry (IOF) prescribe vocabulary for maturity levels, which can be mapped to the ontology status as: if maturity level is iof-av:Released then the status is production and if iof-av:Provisional then the status is beta*

### Deprecated ###
To specify if the ontology IRI is deprecated.

### Version ###
The version of the released ontology.

***Note**: Only the version number of the ontology with respect to the versioning scheme of the ontology should be mentioned. If the version numbering scheme contains an “alpha” or ”beta” string, they should be separated from the version number and mentioned in the Status metadata. the release date can be mentioned in this field if an explicit version number is not provided, e.g., no version IRI and no annotation for version.*

e.g : “v.3.2.0” 
### Is Of Type ###
The nature of the content of the ontology.	
Properties are taken from DCMI KOS type vocabularies. 

***Note**: IndustryPortal mostly contains “Ontology”.*

### Natural Language ### 
The language of the content of the ontology.
Consider using a Lexvo URI with ISO639-3 code.

e.g.: `http://lexvo.org/id/iso639-3/eng`
## Description ##

### Description ###
Description of the ontology is a short (single sentence) summary of the ontology. 

***Note**: The best practice is to provide a single sentence for this metadata. For a longer summary, use Abstract.*
### Homepage ###
Dedicated webpage for the ontology.

***Note**: If no such page is available, keep it empty.*

### Documentation ### 
URL of the documentation page for the ontology.

the documentation page for [SAREF-Core](https://saref.etsi.org/core/v3.1.1/) is `https://saref.etsi.org/core/v3.1.1/`

***Note**: This metadata should be empty If no dedicated documentation is not found. A journal article, white paper, blog, or news article cannot be provided as the documentation of the ontology.*

### Publication ### 
All publications (jounal articles, white paper, preprint, archive) related to ontology. 

***Note**: blog or news articles should not be mentioned for this metadata. Instead, use Associated media for such information. Multiple entries should be separated by a comma. It is advisable that the DOI link (not just the DOI number but the entire HTTP link) of the article is used if available.*

### Used ontology engineering tool ###

Information about the tool used to create the ontology
## More description details ##

### Abstract ###
Longer summary of the ontology (multiple sentences).

***Note**: The abstract may be copied from a dedicated jounrmal article if found.*


### Notes ###
This metadata is free for interpretation.

### Keywords ###
List of keywords related to the ontology.

***Note**: Multiple entries should be separated by comma.*

e.g: "gene function, biology" 

### Alternative name ###
Any alternative name for the ontology is known in the community.

### Identifier ###
An unambiguous reference to the ontology. Use the ontology URI if not provided in the ontology metadata. 

***Note**: This metadata should contain a persistent and resolvable URL. For example, purl, w3id, doi, etc.*

Example : `http://purl.XXXX.org/ontologyX`

Ideally, the URI version of an external identifier
e.g.,  `https://doi.org/10.15454/1.4690062322351956E12` 

## Define Usage ## 

### Known Usage ###
The applications where the ontology is being used.

Used to annotate phenotypes and patterns of gene expression

### Designed for ontology task ###
The purpose for which the ontology was originally designed.

### Has domain ###
Typically, the domain can refer to established topic hierarchies such as the general purpose topic hierarchy DMOZ or the domain-specific topic hierarchy ACM for the computer science domain

### Coverage ###
The spatial or temporal topic of the ontology, the spatial applicability of the ontology, or the jurisdiction under which the ontology is relevant.

***Note**: The applicability of the ontology, is it specific to a certain region? Does the (industrial) knowledge refer to a specific country (France, Tunisia, ...) or is it general? Does the ontology cover only a certain subarea or aspect of the domain mentioned in Has domain metadata (Has domain: IoT, but the ontology covers only IoT-Energy)?                                 In case the ontology is not restricted, put No. Otherwise, some information (free text size and format) about the context should be provided.*

### Example of use ###
A reference to a resource that provides an example of how this ontology can be used.

***Note**: This can be also a free text describing such use.*
## Methodology Information ##
Emna

## More Links ##
Emna

## Ontology Images ##
Emna

## More Community Information ##
Emna

## More People Information ##
Nasro

## Ontology Relation ##
Nasro

## More Relations ##
Nasro










