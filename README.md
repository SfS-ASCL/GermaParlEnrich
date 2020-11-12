# GermaParlEnrich

## General Description

This repository contains the code to create the enriched metadata for the corpus "GermaParl", a subcorpus of the German and Czech Parliamentary Proceedings (GCPP) (which is part of the "Mellon Project").
The 'GermaParl' corpus consists of several 'speech events', each speech event is associated with a speaker. 
For this project the corpus files of 'GermaParl' were pre-processed and the raw text of the single speech events was automatically tokenized (SomaJo) and tagged with named entities (sticker1). 
The data was tagged with 4 different entity types (PERS = persons, LOC = locations, GPE = geographical entities, ORG = organizations). For each entity the 'viaf extraction / geocoder' was executed, using the name of the entity to query the authority records (VIAF or GeoNames), resulting in one or several candidate identifiers per entity (or no ID, if the query was not sucessful). These candidate authority IDs were integrated into a new metadata file, each metadata file (CMDI) corresponding to one parliamentary protocol.

## Report
The source code of the latex file and all pngs are available under /MellonReport
