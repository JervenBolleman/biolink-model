
# Class: macromolecular machine to molecular activity association


A functional association between a macromolecular machine (gene, gene product or complex) and a molecular activity (as represented in the GO molecular function branch), where the entity carries out the activity, or contributes to its execution

URI: [biolink:MacromolecularMachineToMolecularActivityAssociation](https://w3id.org/biolink/vocab/MacromolecularMachineToMolecularActivityAssociation)

![img](http://yuml.me/diagram/nofunky;dir:TB/class/\[Provider]<provided%20by(i)%200..1-%20\[MacromolecularMachineToMolecularActivityAssociation|id(i):identifier_type;relation(i):iri_type;negated(i):boolean%20%3F],%20\[Publication]<publications(i)%200..*-%20\[MacromolecularMachineToMolecularActivityAssociation],%20\[OntologyClass]<qualifiers(i)%200..*-%20\[MacromolecularMachineToMolecularActivityAssociation],%20\[OntologyClass]<association%20type(i)%200..1-%20\[MacromolecularMachineToMolecularActivityAssociation],%20\[MacromolecularMachine]<subject(i)%201..1-%20\[MacromolecularMachineToMolecularActivityAssociation],%20\[MolecularActivity]<object%201..1-%20\[MacromolecularMachineToMolecularActivityAssociation],%20\[FunctionalAssociation]^-\[MacromolecularMachineToMolecularActivityAssociation])

## Parents

 *  is_a: [FunctionalAssociation](FunctionalAssociation.md) - An association between a macromolecular machine (gene, gene product or complex of gene products) and either a molecular activity, a biological process or a cellular location in which a function is executed

## Referenced by class


## Attributes


### Own

 * [object](macromolecular_machine_to_molecular_activity_association_object.md)  <sub>REQ</sub>
    * range: [MolecularActivity](MolecularActivity.md)

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

### Inherited from functional association:

 * [subject](functional_association_subject.md)  <sub>REQ</sub>
    * range: [MacromolecularMachine](MacromolecularMachine.md)
    * inherited from: [FunctionalAssociation](FunctionalAssociation.md)
 * [object](functional_association_object.md)  <sub>REQ</sub>
    * range: [GeneOntologyClass](GeneOntologyClass.md)
    * inherited from: [FunctionalAssociation](FunctionalAssociation.md)

### Domain for slot:

 * [object](macromolecular_machine_to_molecular_activity_association_object.md)  <sub>REQ</sub>
    * range: [MolecularActivity](MolecularActivity.md)
