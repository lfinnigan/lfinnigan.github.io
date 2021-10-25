# PA Digital Metadata Guidelines    
### Version 2.1 (MONTH 2021)
Requirements, Recommendations, and Best Practices for Preparing Metadata for PA Digital’s DPLA Aggregator

### History and Acknowledgements

The PA Digital Metadata Team develops and maintains these guidelines, which were initially drafted in 2015 and first published in 2016. They are reviewed and updated annually. Group members have included:

- Rachel Appel, Formerly Temple University
- Linda Ballinger, Penn State
- Doreva Belfiore, Formerly HSLC
- Anastasia Chiu, Formerly Temple University
- Will Echevarria, Free Library of Philadelphia
- Bill Fee, State Library of Pennsylvania
- Leanne Finnigan, Temple University
- Gabe Galson, Temple University
- Eileen Kocher, State Library of Pennsylvania
- Alison Oskam, State Library of Pennsylvania
- Stefanie Ramsay, Formerly Temple University
- Katy Rawdon, Temple University
- Matthew Strauss, Detre Library and Archives, Heinz History Center
- Holly Tomren, Temple University
- Elise Warshavsky, Formerly Temple University
- Kristen Yarmey, Formerly University of Scranton

Between 2015 and 2021, this project was funded in part by a grant from the Institute of Museum and Library Services as administered by the Pennsylvania Department of Education through the Office of Commonwealth Libraries, and the Commonwealth of Pennsylvania, Tom Wolf, Governor.

Questions or comments on these guidelines are welcome and may be sent to [info@padigital.org](mailto:info@padigital.org).

### Introduction

These guidelines are meant to assist contributing institutions as they plan metadata creation for digital projects. They also serve as an assessment tool for legacy collections and remediation planning. We recognize that contributing shareable metadata takes time and resources. To support our partners, the PA Digital Metadata Team provides consultation services on description, remediation, and rights assessment during the onboarding process and beyond. To inquire about these services, please contact [info@padigital.org](mailto:info@padigital.org).

Potential contributors should review PA Digital’s [Readiness Checklist](https://padigital.org/pa-digital-readiness/) in addition to these guidelines. Adhering to these guidelines makes the onboarding process much easier, but PA Digital is able to accommodate institutions whose metadata do not conform to the mapping recommendations outlined here as long as use is consistent.

Our aggregation software uses the [Open Archives Initiative’s Protocol for Metadata Harvesting](https://www.openarchives.org/OAI/openarchivesprotocol.html) (OAI-PMH). The following best practices apply to metadata contributed to PA Digital generally:

We recommend the use of qualified Dublin Core elements whenever possible. If your repository does not support the use of qualified Dublin Core, use the matching simple Dublin Core element recommended in these guidelines.
Unless otherwise specified, metadata should describe the original resource, not its digital representation.
Common delimiting characters such as pipes (“ | “) and semicolons (“ ; ”) should be avoided; unless otherwise specified, PA Digital uses semicolons to delimit fields with multiple values.
URIs that communicate rights held over the digitized resource, such as those from [rightsstatements.org](rightsstatements.org) and [creativecommons.org](creativecommons.org), are preferred; textual rights statements are acceptable.

We also accept metadata in MODS or MARC in XML, as well as in consistently structured, delimited text files (CSVs, TSVs, etc.).

Incoming metadata are normalized and mapped using Extensible Stylesheet Language Transformations (XSLT) scripts, which are maintained and located here: https://github.com/tulibraries/aggregator_mdx
