
# Class: population to population association


An association between a two populations

URI: [biolink:PopulationToPopulationAssociation](https://w3id.org/biolink/vocab/PopulationToPopulationAssociation)

![img](http://yuml.me/diagram/nofunky;dir:TB/class/\[Provider]<provided%20by(i)%200..1-%20\[PopulationToPopulationAssociation|relation:iri_type;id(i):identifier_type;negated(i):boolean%20%3F],%20\[Publication]<publications(i)%200..*-%20\[PopulationToPopulationAssociation],%20\[OntologyClass]<qualifiers(i)%200..*-%20\[PopulationToPopulationAssociation],%20\[OntologyClass]<association%20type(i)%200..1-%20\[PopulationToPopulationAssociation],%20\[PopulationOfIndividualOrganisms]<object%201..1-%20\[PopulationToPopulationAssociation],%20\[PopulationOfIndividualOrganisms]<subject%201..1-%20\[PopulationToPopulationAssociation],%20\[Association]^-\[PopulationToPopulationAssociation])

## Parents

 *  is_a: [Association](Association.md) - A typed association between two entities, supported by evidence

## Referenced by class


## Attributes


### Own

 * [object](population_to_population_association_object.md)  <sub>REQ</sub>
    * range: [PopulationOfIndividualOrganisms](PopulationOfIndividualOrganisms.md)
 * [relation](population_to_population_association_relation.md)  <sub>REQ</sub>
    * range: [IriType](IriType.md)
 * [subject](population_to_population_association_subject.md)  <sub>REQ</sub>
    * range: [PopulationOfIndividualOrganisms](PopulationOfIndividualOrganisms.md)

### Inherited from association:

 * [id](association_id.md)  <sub>REQ</sub>
    * Description: A unique identifier for an association
    * range: [IdentifierType](IdentifierType.md)
    * inherited from: [Association](Association.md)
    * in subsets: (translator_minimal)
 * [subject](subject.md)  <sub>REQ</sub>
    * Description: connects an association to the subject of the association. For example, in a gene-to-phenotype association, the gene is subject and phenotype is object.
    * range: [IriType](IriType.md)
    * inherited from: [Association](Association.md)
 * [relation](relation.md)  <sub>REQ</sub>
    * Description: the relationship type by which a subject is connected to an object in an association
    * range: [IriType](IriType.md)
    * inherited from: [Association](Association.md)
 * [object](object.md)  <sub>REQ</sub>
    * Description: connects an association to the object of the association. For example, in a gene-to-phenotype association, the gene is subject and phenotype is object.
    * range: [IriType](IriType.md)
    * inherited from: [Association](Association.md)
 * [negated](negated.md)  <sub>OPT</sub>
    * Description: if set to true, then the association is negated i.e. is not true
    * range: [Boolean](Boolean.md)
    * inherited from: [Association](Association.md)
 * [association type](association_type.md)  <sub>OPT</sub>
    * Description: connects an association to the type of association (e.g. gene to phenotype)
    * range: [OntologyClass](OntologyClass.md)
    * inherited from: [Association](Association.md)
 * [qualifiers](qualifiers.md)  <sub>0..*</sub>
    * Description: connects an association to qualifiers that modify or qualify the meaning of that association
    * range: [OntologyClass](OntologyClass.md)
    * inherited from: [Association](Association.md)
 * [publications](publications.md)  <sub>0..*</sub>
    * Description: connects an association to publications supporting the association
    * range: [Publication](Publication.md)
    * inherited from: [Association](Association.md)
 * [provided by](provided_by.md)  <sub>OPT</sub>
    * Description: connects an association to the agent (person, organization or group) that provided it
    * range: [Provider](Provider.md)
    * inherited from: [Association](Association.md)

### Domain for slot:

 * [object](population_to_population_association_object.md)  <sub>REQ</sub>
    * range: [PopulationOfIndividualOrganisms](PopulationOfIndividualOrganisms.md)
 * [relation](population_to_population_association_relation.md)  <sub>REQ</sub>
    * range: [IriType](IriType.md)
 * [subject](population_to_population_association_subject.md)  <sub>REQ</sub>
    * range: [PopulationOfIndividualOrganisms](PopulationOfIndividualOrganisms.md)
