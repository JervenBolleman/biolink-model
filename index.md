---
layout: default
---

[![Build Status](https://travis-ci.org/biolink/biolink-model.svg?branch=master)](https://travis-ci.org/biolink/biolink-model)

# Biolink Model

A high level datamodel of biological entities ([genes](docs/Gene), [diseases](docs/Disease),
[phenotypes](docs/Phenotype), [pathways](docs/Pathway), [individuals](docs/IndividualOrganism), [substances](docs/ChemicalSubstance), etc) and their
[associations](docs/Association).

One of the main uses of the model is as a way of standardizing types
and relational structures in knowledge graphs (KGs), where the KG may
be either a property graph or RDF.

The schema is expressed as a [yaml file](https://github.com/biolink/biolink-model/blob/master/biolink-model.yaml), which is translated into:

 * Individual pages for each class in the model, e.g [https://w3id.org/biolink/vocab/Gene](https://w3id.org/biolink/vocab/Gene)
 * An [OWL ontology](biolink-model.owl), also available on [bioportal](https://bioportal.bioontology.org/ontologies/BLM)
 * [ShEx](biolink-model.shex) (RDF shape constraints)
 * (Experimental) [graphql](biolink-model.graphql), [protobuf](biolink-model.proto), [json-schema](json-schema/biolink-model.json)

## Datamodel

The schema assumes a property graph, where nodes represent individual entities, and edges represent associations between nodes. The biolink model provides a schema for both nodes and edges.

### Nodes

 * [named thing](docs/NamedThing.html) - all nodes are a sub class of 'named thing'

### Edges

 * [association](docs/Association.html) - all edges are a sub class of 'association'

### Slots

 * [Slots](docs#slots) - slots are used to collectively refer to, both, node and edge properties.
    * [node property](docs/node_property.html) - all node properties are a sub class of 'node property'
    * [association slot](docs/association_slot.html) - all edge properties are a sub class of 'association slot'
 

See the [Datamodel index](docs/) for a list nodes, edges, and slots.


# Identifiers

See [biolink json-ld context](context.jsonld) to see CURIE prefix mappings.


# BioLink model representation

## Neo4J representation

See [mapping to neo4j](about/mapping-neo4j.html)

## RDF representation

See [mapping to RDF](about/mapping-rdf.html)
