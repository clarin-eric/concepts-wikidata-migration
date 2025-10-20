# Mappings from CLARIN concepts to Wikidata entities

This repository is used to maintain mappings from concepts that have been registered
in the [CLARIN Concept Registry](https://concepts.clarin.eu/ccr/) (CCR) to 
[Wikidata](https://www.wikidata.org) entities (items and properties).

The mapping is intended to be applied to the CLARIN metadata infrastructure,
specifically the [Component Registry](https://catalog.clarin.eu/ds/ComponentRegistry/),
[Virtual Language Observatory](https://vlo.clarin.eu) (VLO), and as annotations to
the Concept Registry itself.

## Background

The CCR has been populated with terms created by or adopted from individual researchers or projects. Over the years we have identified internal issues such as inconsitency and duplication, and governance has proven to be difficult. In order to solve these problem, the CLARIN Technical Centres committee and the CMDI task force started in 2024 a project to map the CCR concepts to Wikidata entities.

For this purpose, we used semi-automatic mappings based on string matching to wikidata items or properties. The semi-automatic matching resulted in a series of candidate mappings. These went through several rounds of manual validations, not only by the team members, but also involvind different collaborators within CLARIN. In the final stage before releasing v1.1, a round of manual evaluation to a sample of items was included, after which the final selection of mappings was made and integrated in the VLO.


## Version history

### v1.1 (September 2025)

* 693 verified mappings
* Applied to the Component Registry and VLO on 26 September 2025

This is an overview of the results offered in v1.1 (see below) include:

- We started with 3079 CCR concepts.
- From those 3079, 933 concepts are actually used (by individuals or projects).
- Mappings to wikidata were found for 693 concepts, out of which 404 are used concepts.

Some observations about the non-matched concepts:

- There are 529 used concepts for which there was no mapping, they are in [this file](https://github.com/clarin-eric/concepts-wikidata-migration/blob/main/CCR_Wikdata_no_mappings_v1.1.csv):
  - Observation: most of them seem to be concepts referring to properties, probably assigned as concept links to elements or components during the creation of a profile in the component registry (not to the value vocabularies) 
    - from clarin: 84 
    - from nalida: 78 
    - from tei: 30 
    - from clarin-d: 20
- There are 1857 non used concepts for which there was no mapping found (but these were not included in all the mapping rounds, thus, it is possible but they have a mapping, but we decided not to look for it since they are not used in the Virtual Language Observatory)

Files:
- The file "CCR-concepts-to-wikidata-v1-1_complete_metadata_with_provenance.csv" includes more detailed metadata and provenance information (i.e., indicating if the mapping originates from manual validation, manual inputation, or an automatic matching via an ISOCAT Id).
- The file "[CCR-Wikdata_complete_v1.1.csv](https://github.com/clarin-eric/concepts-wikidata-migration/blob/main/CCR-Wikdata_complete_v1.1.csv)" contains all the aggregated metadata for the 3.079 CCR concepts, plus the mappings (for the 933 concepts), the provenance of these mappings, and the toDos for the next version.


  
### v1.0 (September 2025)

Unpublished, not applied

## Contributors

- Alexander König (CLARIN ERIC)
- Dieter Van Uytvanck (CLARIN ERIC)
- Liliana Melgar (KNAW HuC)
- Menzo Windhouwer (KNAW HuC)
- Twan Goosen (CLARIN ERIC)

## Contact

E-mail: [cmdi@clarin.eu](cmdi@clarin.eu)
