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

### Conforms to knowledge representation paradigm ###
A representation formalism that is followed to describe knowledge in an ontology. An established standard to which the described resource conforms. Examples include description logic, first-order logic, etc. 

### Used ontology engineering methodology ###
Information about the method model used to create the ontology.

### Accrual method ###
The method by which items are added to the ontology.   
Here, the author(s) should describe in a few sentences the process by which an item is added. How are new terms identified? What are the validation steps for including new terms ? How are the deprecated terms handled ? Who participates (individual/group of persons) in the process ? etc.

> Recommended values ⇒ "We are adding terms to the ontology after verifying …."

### Competency question ###
A set of questions made to build an ontology at the design time.  

***Note**: Each CQ should be written in a sentence that starts with a capital letter and ends with a question mark—one CQ by line.*

> Recommended values ⇒ "What are the vernacular names of a plant cultivated on the French territory?"

## More Links ##

### Version IRI ###
List of keywords related to the ontology.

***Note**: This metadata should contain the version IRI of the ontology if present. Otherwise, default IRI may be mentioned.*

> Recommended values ⇒ https://w3id.org/myonto/2.0 

### Source ###
A related resource from which the described resource is derived.

***Note**: It is expected to provide a URL (referring to any type of significant online resource, it could be a Web page, a database, a technical document, etc.).*

### Is format of ###
URL to the original document that describe this ontology in a not ontological format (i.e.: the OBO original file).

### Has format ###
URL to a document that describes this ontology in a not ontological format (i.e.: the OBO original file) generated from this ontology.   

### included in data catalogue ###
A data catalog which contains this ontology (i.e.: OBOfoundry, aber-owl, EBI, VEST registry...).

## Ontology Images ##

### Depiction ###
A diagram describing the ontology.

***Note**: This should be a resolvable URL.*

### Logo ###
A logo of the ontology if present.

***Note**: This should be a resolvable URL.*

### Associated media ###
A media object that encodes this ontology. This property is a synonym for encoding.  

***Note**: This should be any blog, whitepaper, news or webpage mentioning or describing the ontology. this should a resolvable URL.*

### Valid until ###
Date (often a range) of validity of the ontology.

***Note**: For most of the ontologies, the latest submission is valid indefinitely. So this field should be empty.*

> Recommended values ⇒ 2022-09-06T10:09:04+02:00 

### Curated on ###
The date the ontology was curated. 

***Note**: This will be populated by the curator of the metadata. By default, this is the same as the submission date of the ontology.*

> Recommended values ⇒ 2022-09-06T10:09:04+02:00 

## More Community Information ##

### Audience ###
Description of the target user base of the ontology.

***Note**: Free text, no formalism. It is expected to provide: a list of words describing the audience.*

> Recommended values ⇒ "Any stakeholders in the life sciences."


### To do list ###
Describes future tasks planned by a resource curator.

***Note**: Free text, no formalism. It is expected to provide: a list of to-do list.*

> Recommended values ⇒ "To curate and add new concepts to the thesaurus. Translating the vocabulary to as many languages as requested."

### User guidelines ###
A related resource which defines how the ontology should be used.

### Repository ###
Link to the source code repository.

***Note**: This contains the URL of the source code repository (e.g., GitHub repository).*

> Recommended values ⇒ https://github.com/Planteome/plant-trait-ontology

### Bug Database ###
Link to the bug tracker of the ontology (i.e.: GitHub issues).  

***Note**: This is an URL of the issue tracker (e.g., github issue tracker).*

> Recommended values ⇒ https://github.com/EnvironmentOntology/envo/issues  

### Mailing list ###
Mailing list home page or email address.

### Award ###
An award won by this ontology.

***Note**: Free text or URL.*

## More People Information ##

### Was generated by ###
People who generated the ontology.

***Note**: The person(s)/organisation(s) who developed the ontology. This metadata may also be populated with the domain exports.*

### Was invalidated by ###
People who invalidated the ontology.

***Note**: The person(s)/organisation(s) who tested the ontology.*

### Was curated by ###
People who curated the ontology.

***Note**: The person(s)/organisation(s) who curated the ontology (ideally associate with their ORCIDs).*

### Endorsed by ###
The parties that have expressed support or approval to this ontology.

***Note**: The organisation who funded or endorsed the ontology (ideally associated with the link to the Web site).*

> Person => "Mohamed Hedi KARRAY(0000-0002-9652-5164)"
> Organisation => "[LGP-ENIT](https://www.lgp.enit.fr/fr/lgp.html)"

### Funded by ###
The organization funding the ontology development.

***Note**: The grant or project which funded the development of the ontology.*

> Person => "Arkopaul Sarkar(0000-0002-8967-7813)"
> Organisation => "[LGP-ENIT](https://www.lgp.enit.fr/fr/lgp.html)"

### Translator ###
Organization or person who adapted the ontology to different languages, regional differences and technical requirements.

***Note**: name of the person (ideally associate with its ORCID) that translated the content of the ontology or its metadata to another language.*

> Person => "Mohamed Hedi KARRAY(0000-0002-9652-5164)"
> Organisation => "[LGP-ENIT](https://www.lgp.enit.fr/fr/lgp.html)"

## Ontology Relation ##

### Use Imports ###
This metadata should be a URI

References another ontology metadata instance that describes an ontology containing definitions, whose meaning is considered to be part of the meaning of the ontology described by this ontology metadata instance

***Note**: Resolvable URL of imports. It may be derived from owl:import from the source file. However, if an IRI of owl:import is not resolvable then they should be replaced by a resolvable URL. If a resolvable URL is not available then the imported ontology needs to be present in IndustryPortal and the resolvable URL from IndustryPortal needs to be used. Multiple imports need to be  separate by a comma.*

### Has prior version ###

An URI to the prior version of the ontology. 

***Note**: Mainly the URL of the prior version in IndustryPortal.*

> http://data.industryportal.enit.fr/ontologies/IOF-CORE/submissions/1

### Is aligned to ###

Ontologies that have an alignment which covers a substantial part of the described ontology.

### Ontology related to ###

An ontology that uses or extends some class or property of the described ontology

## More Relations ##

### Is backward compatible with ###
URI of an ontology that has its prior version compatible with the described ontology

### Is incompatible with ###
URI of an ontology that is a prior version of this ontology, but not compatible

### From the same domain than ###
Ontologies that come from the same domain.

### Similar to ###
Vocabularies that are similar in scope and objectives, independently of the fact that they otherwise refer to each other.

### Specialisation of ###

If the ontology is a latter version that is semantically equivalent to another ontology.

### Generalisation of ###
Vocabulary that is generalized by some superclasses or superproperties by the described ontology

### Disparate modeling with ###
URI of an ontology that is considered to have a different model, because they represent corresponding entities in different ways.
e.g. an instance in one case and a class in the other for the same concept


### Has Part ###
A related ontology that is included either physically or logically in the described ontology.

***Note**: This is useful in uploading a network of ontologies (modular ontology).*

### Used by ###
Ontologies that use the described ontology.

### Translated from ###
A ontology that is a translation of the content of this ontology.

### Translation of ###
The ontology that this ontology has been translated from.

## More content information ##

### Key classes ###
??

***Note**: Key classes (concepts) from the ontology.*

### Endpoint ###
This metadata should be an URI

***Note**: this metadata contains the original source file in some repository (e.g., GitHub).*

### Data dump ###
This metadata should be an URI

### CSV dump ###
This metadata should be an URI

### Open search description ###
This metadata should be an URI

### URI Lookup Endpoint ###
A protocol endpoint for simple URI lookups for the ontology.

### URI Regex Pattern ###
A regular expression that matches the URIs of the ontology entities.

### Metadata vocabulary used ###
Vocabularies that are used and/or referred to create the described ontology.


### Example identifier ###
An example identifier used by one item (or record) from a dataset.

## More metrics information ##

