
# Class: pairwise interaction association


An interaction at the molecular level between two physical entities

URI: [biolink:PairwiseInteractionAssociation](https://w3id.org/biolink/vocab/PairwiseInteractionAssociation)

![img](http://yuml.me/diagram/nofunky;dir:TB/class/\[Provider]<provided%20by(i)%200..1-%20\[PairwiseInteractionAssociation|id:identifier_type;relation:iri_type;negated(i):boolean%20%3F],%20\[Publication]<publications(i)%200..*-%20\[PairwiseInteractionAssociation],%20\[OntologyClass]<qualifiers(i)%200..*-%20\[PairwiseInteractionAssociation],%20\[OntologyClass]<association%20type(i)%200..1-%20\[PairwiseInteractionAssociation],%20\[MolecularEntity]<object%201..1-%20\[PairwiseInteractionAssociation],%20\[MolecularEntity]<subject%201..1-%20\[PairwiseInteractionAssociation],%20\[PairwiseGeneToGeneInteraction]uses%20-.->\[PairwiseInteractionAssociation],%20\[Association]^-\[PairwiseInteractionAssociation])

## Parents

 *  is_a: [Association](Association.md) - A typed association between two entities, supported by evidence

## Mixin for

 * [PairwiseGeneToGeneInteraction](PairwiseGeneToGeneInteraction.md) (mixin)  - An interaction between two genes or two gene products. May be physical (e.g. protein binding) or genetic (between genes). May be symmetric (e.g. protein interaction) or directed (e.g. phosphorylation)

## Referenced by class


## Attributes


### Own

 * [id](pairwise_interaction_association_id.md)  <sub>REQ</sub>
    * range: [IdentifierType](IdentifierType.md)
 * [object](pairwise_interaction_association_object.md)  <sub>REQ</sub>
    * range: [MolecularEntity](MolecularEntity.md)
 * [relation](pairwise_interaction_association_relation.md)  <sub>REQ</sub>
    * range: [IriType](IriType.md)
 * [subject](pairwise_interaction_association_subject.md)  <sub>REQ</sub>
    * range: [MolecularEntity](MolecularEntity.md)

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

 * [interacting molecules category](interacting_molecules_category.md)  <sub>OPT</sub>
    * range: [OntologyClass](OntologyClass.md)
 * [id](pairwise_interaction_association_id.md)  <sub>REQ</sub>
    * range: [IdentifierType](IdentifierType.md)
 * [object](pairwise_interaction_association_object.md)  <sub>REQ</sub>
    * range: [MolecularEntity](MolecularEntity.md)
 * [relation](pairwise_interaction_association_relation.md)  <sub>REQ</sub>
    * range: [IriType](IriType.md)
 * [subject](pairwise_interaction_association_subject.md)  <sub>REQ</sub>
    * range: [MolecularEntity](MolecularEntity.md)
