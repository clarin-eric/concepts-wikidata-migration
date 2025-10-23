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

#### Files
- "[CCR-Wikdata_complete_v1.1.csv](https://github.com/clarin-eric/concepts-wikidata-migration/blob/main/CCR-Wikdata_complete_v1.1.csv)" contains all the aggregated metadata for the 3.079 CCR concepts, plus the mappings (for the 933 concepts), the provenance of these mappings, and the toDos for the next version.
- "[CCR-Wikdata_mappings_v1.1.csv](https://github.com/clarin-eric/concepts-wikidata-migration/blob/main/CCR-Wikdata_mappings_v1.1.csv)" a two-column file that contains only the 693 used concepts that have a mapping, and the wikidata URI.
- "[CCR-concepts-to-wikidata-v1-1_complete_metadata_with_provenance.csv](https://github.com/clarin-eric/concepts-wikidata-migration/blob/main/CCR-Wikdata_mappings_v1.1_complete_metadata_and_provenance.csv)" includes the 933 concepts with mappings, with more detailed metadata and provenance information (i.e., indicating if the mapping originates from manual validation, manual inputation, or an automatic matching via an ISOCAT Id).
- "[CCR_Wikdata_no_mappings_v1.1.csv](https://github.com/clarin-eric/concepts-wikidata-migration/blob/main/CCR_Wikdata_no_mappings_v1.1.csv)" contains the 529 concepts for which a mapping was not found (all metadata is included).
- "[Working-notes.txt](https://github.com/clarin-eric/concepts-wikidata-migration/blob/main/working-notes.txt)" document with some observations and notes.


#### Statistics
This is an overview of the results offered in v1.1 (see below) include:

- We started with 3079 CCR concepts.
- From those 3079, 933 concepts are actually used (by individuals or projects).
- Mappings to wikidata were found for 693 concepts, out of which 404 are used concepts.

Thus:
* 693 verified mappings
* Applied to the Component Registry and VLO on 26 September 2025

  
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
