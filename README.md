# Mappings from CLARIN concepts to Wikidata entities

This repository is used to maintain mappings from concepts that have been registered
in the [CLARIN Concept Registry](https://concepts.clarin.eu/ccr/) (CCR) to 
[Wikidata](https://www.wikidata.org) entities (items and properties).

The mapping is intended to be applied to the CLARIN metadata infrastructure,
specifically the [Component Registry](https://catalog.clarin.eu/ds/ComponentRegistry/),
[Virtual Language Observatory](https://vlo.clarin.eu) (VLO), and as annotations to
the Concept Registry itself. For this purpsose, there are two projects that automate the conversion
from a tabular mapping to 
* an updated VLO configuration ([vlo-wikidata-migration](https://github.com/clarin-eric/vlo-wikidata-migration))
* or update statements for the Component Registry database ([compreg-wikidata-migration](https://github.com/clarin-eric/compreg-wikidata-migration))

## Background
The CCR has been populated with terms created by or adopted from individual researchers or projects. Over the years we have identified internal issues such as inconsitency and duplication, and governance has proven to be difficult. In order to solve these problem, the CLARIN Technical Centres committee and the CMDI task force started in 2024 a project to map the CCR concepts to Wikidata entities.
For this purpose, we used semi-automatic mappings based on string matching to wikidata items or properties. The semi-automatic matching resulted in a series of candidate mappings. These went through several rounds of manual validations, not only by the team members, but also involving different collaborators within CLARIN. In the final stage before releasing v1.1, a round of manual evaluation to a sample of items was included, after which the final selection of mappings was made and integrated in the VLO.

## Version history
### v1.3 (February 2, 2026)
- In this version the team did a last round of mappings checking the concepts that had non-confirmed mapping candidates.
- As a result, we mapped manually 47 more concepts to wikidata URis.
#### Files v1.3
- "[CCR_Wikidata-result-new-mappings-20260202.csv](https://github.com/clarin-eric/concepts-wikidata-migration/blob/main/v1.3/CCR_Wikidata-result-new-mappings-20260202.csv)" contains the resulting mappings done in this round (aggregated from the team members contributions via the internally shared Google spreadsheet: "CCR_Wikidata-complete-toDo-v1.2-20251211")
- "[CCR-Wikidata-complete-done-v1.3.csv]()" contains all the metadata, provenance and mappings from all the versions up to 1.3.
  - columns: "status_20260202-latest-round" and "toDo_20260202" -> include the final status until this point. Since no more mapping rounds are planned, these two columns show the final status of the mappings (see the updated statistics below).

### v1.2 (November/December 2025)
#### Files v1.2
- "[CCR_Wikidata-complete-toDo-v1.2.csv](https://github.com/clarin-eric/concepts-wikidata-migration/blob/main/v1.2/CCR_Wikidata-complete-toDo-v1.2.csv)" contains all the aggregated metadata for the 3.079 CCR concepts, plus the mappings (for the 933 concepts), the provenance of these mappings, some suggested mapping candidates to evaluate, and the toDos for the next version.
  - This file contains all the metadata, provenance and mappings from version 1.1 plus columns with ToDos for the next round:
    - column: toDo_20251124 -> describes what needs to be done
    - column: toDo_WHO -> assigns it to a person, there are two types: mandatory and optional
    - column: status_202511-latest-round -> to be filled in during the toDos

### v1.1 (September 2025)
#### Files v1.1
- "[CCR-Wikdata_complete_v1.1.csv](https://github.com/clarin-eric/concepts-wikidata-migration/blob/main/v1.1/CCR-Wikidata_complete_v1.1.csv)" contains all the aggregated metadata for the 3.079 CCR concepts, plus the mappings (for the 933 concepts), the provenance of these mappings, and the toDos for the next version.
- "[CCR-Wikdata_mappings_v1.1.csv](https://github.com/clarin-eric/concepts-wikidata-migration/blob/main/v1.1/CCR-Wikidata_mappings_v1.1.csv)" a two-column file that contains only the 693 used concepts that have a mapping, and the wikidata URI.
- "[CCR-concepts-to-wikidata-v1-1_complete_metadata_with_provenance.csv](https://github.com/clarin-eric/concepts-wikidata-migration/blob/main/v1.1/CCR-Wikidata_mappings_v1.1_complete_metadata_and_provenance.csv)" includes the 933 concepts with mappings, with more detailed metadata and provenance information (i.e., indicating if the mapping originates from manual validation, manual inputation, or an automatic matching via an ISOCAT Id).
- "[CCR-Wikidata_no_mappings_v1.1.csv](https://github.com/clarin-eric/concepts-wikidata-migration/blob/main/v1.1/CCR-Wikidata_no_mappings_v1.1.csv)" contains the 529 concepts for which a mapping was not found (all metadata is included).
- "[CCR-Wikidata_not_mapped_concepts_list_v1.1.txt](https://github.com/clarin-eric/concepts-wikidata-migration/blob/main/v1.1/CCR-Wikidata_not_mapped_concepts_list_v1.1.txt)" plain list with the non-mapped 529 concepts, labels only (no extra metadata)
- "[Working-notes.txt](https://github.com/clarin-eric/concepts-wikidata-migration/blob/main/v1.1/working-notes.txt)" document with some observations and notes.

### v1.0 (September 2025)
Unpublished, not applied

## Statistics v1.1
This is an overview of the results offered in v1.1 (see below) include:
- We started with 3079 CCR concepts.
- From those 3079, 933 concepts are actually used (by individuals or projects).
- Mappings to wikidata were found for 693 concepts, out of which 404 are used concepts.
Thus:
* 693 verified mappings
* Applied to the Component Registry and VLO on 26 September 2025

## Statistics v1.3 (final)
- We started with 3079 CCR concepts.
- From those 3079, 933 concepts are actually used (by individual or projects). These are the so-called "used concepts"
- Mappings to wikidata were found for 740 concepts, out of which 451 are used concepts.
Thus:
- 740 verified mappings
- Applied to the Component Registry and VLO on ....

## More information
- Forum post: https://forum.clarin.eu/t/wikidata-replaces-the-clarin-concept-registry-in-the-component-registry/1205
- Updated documentation: https://www.clarin.eu/content/component-registry-documentation#ConceptLinks 

## Contributors
- Alexander König (CLARIN ERIC)
- Dieter Van Uytvanck (CLARIN ERIC)
- Liliana Melgar (KNAW HuC)
- Menzo Windhouwer (KNAW HuC)
- Twan Goosen (CLARIN ERIC)

## Contact
E-mail: [cmdi@clarin.eu](cmdi@clarin.eu)
