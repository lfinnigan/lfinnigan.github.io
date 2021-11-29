# PA Digital Metadata Guidelines	Version 2.1 (MONTH 2021) <img src="images/logo.jpg" alt="alt_text" title="image_tooltip" width="128" height="128">

## Requirements, Recommendations, and Best Practices for Preparing Metadata for PA Digital’s DPLA Aggregator


# History and Acknowledgements

The PA Digital Metadata Team develops and maintains these guidelines, which were initially drafted in 2015 and first published in 2016. They are reviewed and updated annually. Group members have included:

* Rachel Appel, Formerly Temple University
* Linda Ballinger, Penn State
* Doreva Belfiore, Formerly HSLC
* Anastasia Chiu, Formerly Temple University
* Will Echevarria, Free Library of Philadelphia
* Bill Fee, State Library of Pennsylvania
* Leanne Finnigan, Temple University
* Gabe Galson, Temple University
* Eileen Kocher, State Library of Pennsylvania
* Alison Oskam, State Library of Pennsylvania
* Stefanie Ramsay, Formerly Temple University
* Katy Rawdon, Temple University
* Matthew Strauss, Detre Library and Archives, Heinz History Center
* Holly Tomren, Temple University
* Elise Warshavsky, Formerly Temple University
* Kristen Yarmey, Formerly University of Scranton

Between 2015 and 2021, this project was funded in part by a grant from the Institute of Museum and Library Services as administered by the Pennsylvania Department of Education through the Office of Commonwealth Libraries, and the Commonwealth of Pennsylvania, Tom Wolf, Governor.

Questions or comments on these guidelines are welcome and may be sent to [info@padigital.org](mailto:info@padigital.org).


<table>
  <tr>
   <td><p style="text-align: right">

<img src="images/email.png" alt="alt_text" title="image_tooltip">
<strong><a href="mailto:info@padigital.org">info@padigital.org</a></strong></p>

   </td>
   <td>

<img src="images/web.png" alt="alt_text" title="image_tooltip">
<strong><a href="http://www.padigital.org/">www.padigital.org</a></strong>
   </td>
   <td>

<img src="images/twitter.png" alt="alt_text" title="image_tooltip">
<strong><a href="https://twitter.com/PADigitalNews">@PADigitalNews</a></strong>
   </td>
  </tr>
</table>



# Table of Contents


[TOC]



# Introduction

These guidelines are meant to assist contributing institutions as they plan metadata creation for digital projects. They also serve as an assessment tool for legacy collections and remediation planning. We recognize that contributing shareable metadata takes time and resources. To support our partners, the PA Digital Metadata Team provides consultation services on description, remediation, and rights assessment during the onboarding process and beyond. To inquire about these services, please contact [info@padigital.org](mailto:info@padigital.org).

Potential contributors should review PA Digital’s [Readiness Checklist](https://padigital.org/pa-digital-readiness/) in addition to these guidelines. Adhering to these guidelines makes the onboarding process much easier, TPlease note that although the onboarding process is made easier by the adherence to these guidelines, but PA Digital is able to accommodate institutions whose metadata do not conform to the mapping recommendations outlined here as long as use is consistent. we are able to accommodate institutions whose metadata do not conform to the mapping recommendations outlined herebelow.

Our aggregation software usesis based on the [Open Archives Initiative’s Protocol for Metadata Harvesting](https://www.openarchives.org/OAI/openarchivesprotocol.html) (OAI-PMH) and on the [Dublin Core metadata terms](http://dublincore.org/documents/dcmi-terms/). The following best practices apply to metadata contributed to PA Digital generally:

* We recommend the use of qualified Dublin Core elements whenever possible. If your repository does not support the use of qualified Dublin Core, use the matching simple Dublin Core element recommended in these guidelines.
* Unless otherwise specified, metadata should describe the **_original resource_**, not its digital representation.
* Common delimiting characters such as pipes (“ | “) and semicolons (“ ; ”) should be avoided; unless otherwise specified, PA Digital uses semicolons to delimit fields with multiple values.
* URIs that communicate rights held over the digitized resource, such as those from rightsstatements.org and creativecommons.org, are preferred; textual rights statements are acceptable.When using URIs, they should be added in addition to string values, not in place of them.

We also accept metadata in MODS or MARC in XML, as well as in consistently structured, delimited text files (CSVs, TSVs, etc.).

Incoming metadata are normalized and mapped using Extensible Stylesheet Language Transformations (XSLT) scripts, which are maintained and located here: https://github.com/tulibraries/aggregator_mdx


# Shareable Metadata

Contributors to PA Digital should strive to provide shareable, quality metadata. In _[Best Practices for OAI Data Provider Implementations and Shareable Metadata](http://webservices.itcs.umich.edu/mediawiki/oaibp/index.php/ShareableMetadataPublic)_ (2007), the authors provide recommendations to assure that aggregated records retain meaning within a shared portal. The characteristics they describe are useful for contributors to PA Digital and DPLA.

* **Context.** Records within DPLA are removed from the context provided by local systems and users. Descriptions that make sense locally may not be ideal in a large, shared system such as DPLA. Quality, shareable metadata remain meaningful even in an aggregated environment removed from the originating repository.

* **Completeness.** Records in a shared system are most discoverable and meaningful when they are complete and robust. They should make sense standing on their own and they should be rich enough to enable discovery in a system with roughly 30 million records. Avoid the use of abbreviations or ambiguous references.

* **Consistency.** Syntax, elements, and vocabularies should be used consistently. This allows PA Digital and DPLA to more easily assess, prepare, and aggregate your metadata and provide discovery platforms that increase access to your valuable, contributed resources.

* **Controlled vocabularies.** The use of widely-adopted vocabularies helps to better integrate records from other contributing institutions.

In the spirit of shareable metadata, note that PA Digital and DPLA require that metadata (_but not digital content_) be licensed as [CC0](https://creativecommons.org/about/cc0) (“No rights reserved”). The following excerpt from _[The ­Digital Public Library of America Policy Statement on Metadata](https://pro.dp.la/hubs/metadata-application-profile)_ speaks to the importance of this policy in fulfilling DPLA’s mission and values: 

_“The DPLA aims to make the cultural and scientific record available, free of charge, to all through databases of metadata. The DPLA, for this purpose, has undertaken the task of ingesting, indexing, enriching, and making available descriptive metadata and wishes to make such metadata widely available for reuse._

_The DPLA wishes to promote innovation in the development of applications and tools that use and rely on this metadata. In order to foster such innovation, the DPLA is committed to ensuring such metadata is unencumbered by legal restrictions. This policy and statement on metadata contained in the DPLA’s databases reflects that commitment. To that same end, the DPLA believes this policy is in accord with the letter and spirit of United States copyright law and would be fully respected in a court of law._

_The DPLA hopes that the content and resources in the library will be put to creative uses that educate, inform, and empower current and future generations.”_


# Wikimedia Commons

[LF to add]


# Quick Reference: Mapping Recommendations for Dublin Core


<table>
  <tr>
   <td><strong>PA Digital Label</strong>
   </td>
   <td><strong>PA Digital Status</strong>
   </td>
   <td><strong>Qualified DC Element</strong>
   </td>
   <td><strong>Simple DC Element</strong>
   </td>
  </tr>
  <tr>
   <td>Alternative Title
   </td>
   <td>Optional
   </td>
   <td>dcterms:alternative
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Contributor
   </td>
   <td>Optional
   </td>
   <td>dcterms:contributor
   </td>
   <td>dc:contributor
   </td>
  </tr>
  <tr>
   <td>Collection Name
   </td>
   <td>Required or Derived**
   </td>
   <td>dcterms:isPartOf
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Contributing Institution
   </td>
   <td>Derived
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Creator
   </td>
   <td>Recommended
   </td>
   <td>dcterms:creator
   </td>
   <td>dc:creator
   </td>
  </tr>
  <tr>
   <td>Date
   </td>
   <td>Recommended
   </td>
   <td>dcterms:created
   </td>
   <td>dc:date
   </td>
  </tr>
  <tr>
   <td>Description
   </td>
   <td>Recommended
   </td>
   <td>dcterms:description
   </td>
   <td>dc:description
   </td>
  </tr>
  <tr>
   <td>Extent
   </td>
   <td>Optional
   </td>
   <td>dcterms:extent
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>File Format
   </td>
   <td>Optional
   </td>
   <td>dcterms:format
   </td>
   <td>dc:format
   </td>
  </tr>
  <tr>
   <td>Format
   </td>
   <td>Recommended
   </td>
   <td>dcterms:type
   </td>
   <td>dc:type
   </td>
  </tr>
  <tr>
   <td>Identifier
   </td>
   <td>Optional
   </td>
   <td>dcterms:identifier
   </td>
   <td>dc:identifier
   </td>
  </tr>
  <tr>
   <td>IIIF Base URL
   </td>
   <td>Optional or Derived**
   </td>
   <td>dcterms:identifier
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>IIIF Manifest
   </td>
   <td>Optional or Derived**
   </td>
   <td>dcterms:isReferencedBy
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Intermediate Provider
   </td>
   <td>Derived
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>URL
   </td>
   <td>Required or Derived**
   </td>
   <td>dcterms:identifier
   </td>
   <td>dc:identifier
   </td>
  </tr>
  <tr>
   <td>Language
   </td>
   <td>Recommended for textual and spoken material
   </td>
   <td>dcterms:language
   </td>
   <td>dc:language
   </td>
  </tr>
  <tr>
   <td>Media Master
   </td>
   <td>Optional or Derived**
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Place
   </td>
   <td>Recommended
   </td>
   <td>dcterms:spatial
   </td>
   <td>dc:coverage
   </td>
  </tr>
  <tr>
   <td>Preview
   </td>
   <td>Strongly recommended or Derived**
   </td>
   <td>dcterms:identifier
   </td>
   <td>dc:identifier
   </td>
  </tr>
  <tr>
   <td>Publisher
   </td>
   <td>Optional
   </td>
   <td>dcterms:publisher
   </td>
   <td>dc:publisher
   </td>
  </tr>
  <tr>
   <td>Relation
   </td>
   <td>Optional
   </td>
   <td>dcterms:relation
   </td>
   <td>dc:relation
   </td>
  </tr>
  <tr>
   <td>Replaced By
   </td>
   <td>Optional
   </td>
   <td>dcterms:isReplacedBy
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Replaces
   </td>
   <td>Optional
   </td>
   <td>dcterms:replaces
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Rights
   </td>
   <td>Required (or Rights URI)
   </td>
   <td>dcterms:rights
   </td>
   <td>dc:rights
   </td>
  </tr>
  <tr>
   <td>Rights Holder
   </td>
   <td>Optional
   </td>
   <td>dcterms:rightsholder
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Source
   </td>
   <td>Optional
   </td>
   <td>dcterms:source
   </td>
   <td>dc:source
   </td>
  </tr>
  <tr>
   <td>Rights URI
   </td>
   <td>Required (or Rights)
   </td>
   <td>dcterms:rights
   </td>
   <td>dc:rights
   </td>
  </tr>
  <tr>
   <td>Subject
   </td>
   <td>Recommended
   </td>
   <td>dcterms:subject
   </td>
   <td>dc:subject
   </td>
  </tr>
  <tr>
   <td>Temporal Coverage
   </td>
   <td>Optional
   </td>
   <td>dcterms:temporal
   </td>
   <td>dc:subject
   </td>
  </tr>
  <tr>
   <td>Title
   </td>
   <td>Required
   </td>
   <td>dcterms:title
   </td>
   <td>dc:title
   </td>
  </tr>
  <tr>
   <td>Type
   </td>
   <td>Recommended
   </td>
   <td>dcterms:type
   </td>
   <td>dc:type
   </td>
  </tr>
</table>


*_To see mapping changes from PA Digital Guidelines v1.2 (August 2018), see [UPDATE THIS LINK](#heading=h.l01zhzdf43zj)_

*_Values for some fields may be derived from metadata elsewhere in the record. For example, an object or thumbnail URL may be derived from a consistently formatted identifier present in the record, or a collection name may be derived from the setSpec value in the OAI-PMH output._

# Guidelines Key

Fields are arranged alphabetically by PA Digital label. Descriptors with no content are omitted. 


<table>
  <tr>
   <td><strong>PA Digital Label</strong>
   </td>
   <td>Field label used by PA Digital
   </td>
  </tr>
  <tr>
   <td><strong>Status</strong>
   </td>
   <td>Identifies whether a field is required, strongly recommended, recommended, optional, or derived
   </td>
  </tr>
  <tr>
   <td><strong>Description</strong>
   </td>
   <td>A description of the field
   </td>
  </tr>
  <tr>
   <td><strong>Qualified DC Element</strong>
   </td>
   <td>The qualified Dublin Core term to which a field should map
   </td>
  </tr>
  <tr>
   <td><strong>Simple DC Element </strong>
   </td>
   <td>The simple Dublin Core element to which a field should map if qualified term is unavailable
   </td>
  </tr>
  <tr>
   <td><strong>CONTENTdm Mapping</strong>
   </td>
   <td>The DC Map value in Field properties
   </td>
  </tr>
  <tr>
    <td><strong>CSV Header</strong>
   </td>
   <td>Recommended header value for delimited text files
   </td>
  </tr>
  <tr>
   <td><strong>Repeatable</strong>
   </td>
   <td>Whether a field may be repeated
   </td>
  </tr>
  <tr>
   <td><strong>CV/Syntax</strong>
   </td>
   <td>Recommended controlled vocabularies or syntax
   </td>
  </tr>
  <tr>
   <td><strong>Notes and Best Practices</strong>
   </td>
   <td>Includes recommendations for a field’s content, application, and punctuation
   </td>
  </tr>
  <tr>
   <td><strong>Examples</strong>
   </td>
   <td>Examples that illustrate best practices
   </td>
  </tr>
</table>



# 


# Fields


<table>
  <tr>
   <td><strong>PA Digital Label</strong>
   </td>
   <td>
<strong>Alternative Title</strong>


   </td>
  </tr>
  <tr>
   <td><strong>Status</strong>
   </td>
   <td>Optional
   </td>
  </tr>
  <tr>
   <td><strong>Description</strong>
   </td>
   <td>Any alternative title of the described resource including abbreviations and translations
   </td>
  </tr>
  <tr>
   <td><strong>Qualified DC Element</strong>
   </td>
   <td>dcterms:alternative
   </td>
  </tr>
  <tr>
   <td><strong>CONTENTdm Mapping</strong>
   </td>
   <td>Title-Alternative
   </td>
  </tr>
  <tr>
   <td>CSV Header
   </td>
   <td>Alternative_Title
   </td>
  </tr>
  <tr>
   <td><strong>Repeatable</strong>
   </td>
   <td>Yes
   </td>
  </tr>
  <tr>
   <td><strong>CV/Syntax</strong>
   </td>
   <td>
<ul>

<li>Natural language
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Notes and Best Practices</strong>
   </td>
   <td>
<ul>

<li>Comparable to MARC variations of titles (such as alternative spellings)

<li>May also be used for translations of titles in foreign languages

<li>Avoid use of explanatory or qualifying symbols (e.g., brackets)

<li>Where there are multiple Title fields, any instance after the first will map to Alternative Title
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Examples</strong>
   </td>
   <td>
<ul>

<li>Undergraduate course catalog, 1961-62
</li>
</ul>
   </td>
  </tr>
</table>




<p id="gdcalert6" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "[Back to Field Table]"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert7">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[[Back to Field Table]](#heading=h.3sf8crbrgxc)


<table>
  <tr>
   <td><strong>PA Digital Label</strong>
   </td>
   <td>
<h3>Collection Name</h3>


   </td>
  </tr>
  <tr>
   <td><strong>Status</strong>
   </td>
   <td>Recommended or Derived (or Required, see below)
   </td>
  </tr>
  <tr>
   <td><strong>Description</strong>
   </td>
   <td>Collection or aggregation of which described resource is a part
   </td>
  </tr>
  <tr>
   <td><strong>Qualified DC Element</strong>
   </td>
   <td>dcterms:isPartOf
   </td>
  </tr>
  <tr>
   <td><strong>CONTENTdm Mapping</strong>
   </td>
   <td>Relation-Is Part Of
   </td>
  </tr>
  <tr>
   <td>CSV Header
   </td>
   <td>Collection_Name
   </td>
  </tr>
  <tr>
   <td><strong>Repeatable</strong>
   </td>
   <td>Yes
   </td>
  </tr>
  <tr>
   <td><strong>Notes and Best Practices</strong>
   </td>
   <td>
<ul>

<li>Whenever possible, PA Digital will use the setSpec, or collection identifier, value in the OAI-PMH output to generate a human-readable, normalized Collection Name

<li>SetSpec values must be valid; see the pattern requirements under setSpecType in the OAI-PMH specifications

<li>Institutions that wish to map collectionmapFor institutions that do not supply collection names fromin their metadata rather than the setSpec should inform PA Digital during the onboarding processor that want to apply dcterms:isPartOf differently than what is recommended here, Collection Name(s) may be derived from metadata elsewhere in the record. For example, a collection name may be derived from the setSpec value in the OAI-PMH output
</li>
</ul>
   </td>
  </tr>
</table>




<p id="gdcalert7" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "[Back to Field Table]"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert8">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[[Back to Field Table]](#heading=h.3sf8crbrgxc)


<table>
  <tr>
   <td><strong>PA Digital Label</strong>
   </td>
   <td>
<h3>
    Contributing Institution</h3>


   </td>
  </tr>
  <tr>
   <td><strong>Status</strong>
   </td>
   <td>Derived or PA Digital supplied
   </td>
  </tr>
  <tr>
   <td><strong>Description</strong>
   </td>
   <td>The organization that supplies metadata to PA Digital
   </td>
  </tr>
  <tr>
   <td>CSV Header
   </td>
   <td>Data_Provider
   </td>
  </tr>
  <tr>
   <td><strong>Repeatable</strong>
   </td>
   <td>Yes
   </td>
  </tr>
  <tr>
   <td><strong>Notes and Best Practices</strong>
   </td>
   <td>
<ul>

<li>Values for this field may be mapped from consistently formatted metadata elsewhere in a record; examples include identifiers and object URLs

<li>Values may also be supplied by PA Digital during the ingestion process. Institutions should specify during onboarding the desired value(s) for this field

<li>Under certain circumstances, Contributing Institution values may be mapped from metadata; names should be normalized, consistent, and identifiable
</li>
</ul>
   </td>
  </tr>
</table>




<p id="gdcalert8" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "[Back to Field Table]"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert9">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[[Back to Field Table]](#heading=h.3sf8crbrgxc)


<table>
  <tr>
   <td><strong>PA Digital Label</strong>
   </td>
   <td>
<h3>Contributor</h3>


   </td>
  </tr>
  <tr>
   <td><strong>Status</strong>
   </td>
   <td>Optional
   </td>
  </tr>
  <tr>
   <td><strong>Description</strong>
   </td>
   <td>An entity responsible for making secondary contributions to the described resource. Examples of a Contributor include a person, an organization, or a service
   </td>
  </tr>
  <tr>
   <td><strong>Qualified DC Element</strong>
   </td>
   <td>dcterms:contributor
   </td>
  </tr>
  <tr>
   <td><strong>Simple DC Element </strong>
   </td>
   <td>dc:contributor
   </td>
  </tr>
  <tr>
   <td><strong>CONTENTdm Mapping</strong>
   </td>
   <td>Contributor
   </td>
  </tr>
  <tr>
   <td>CSV Header
   </td>
   <td>Contributor
   </td>
  </tr>
  <tr>
   <td><strong>Repeatable</strong>
   </td>
   <td>Yes
   </td>
  </tr>
  <tr>
   <td><strong>CV/Syntax</strong>
   </td>
   <td>
<ul>

<li>Use standard vocabularies such as <a href="http://id.loc.gov/">LCNAF</a>, <a href="https://viaf.org/">VIAF</a>, or <a href="http://www.getty.edu/research/tools/vocabularies/ulan/">ULAN</a> whenever possible; consistently applied local vocabularies are acceptable

<li>If an authorized form is unavailable, use similar syntax (Lastname, Firstname, YYYY-YYYY)
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Notes and Best Practices</strong>
   </td>
   <td>
<ul>

<li>Use a semicolon to separate multiple values

<li>Avoid use of placeholder values (e.g., “Unknown”)

<li>For oral histories, Contributor is the interviewer

<li>Use name only without indication of role except in cases where a person’s role is included in an authorized form. For example, prefer “Smith, John, 1880-1960” not “Smith, John, 1880-1960, publisher”
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Examples</strong>
   </td>
   <td>
<ul>

<li>Beck, James M. (James Montgomery), 1861-1936

<li>United States. Army Map Service
</li>
</ul>
   </td>
  </tr>
</table>




<p id="gdcalert9" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "[Back to Field Table]"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert10">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[[Back to Field Table]](#heading=h.3sf8crbrgxc)


<table>
  <tr>
   <td><strong>PA Digital Label</strong>
   </td>
   <td>
<h3>Creator</h3>


   </td>
  </tr>
  <tr>
   <td><strong>Status</strong>
   </td>
   <td>Recommended
   </td>
  </tr>
  <tr>
   <td><strong>Description</strong>
   </td>
   <td>An entity primarily responsible for making the described resource. Examples of a Creator include a person, an organization, or a service
   </td>
  </tr>
  <tr>
   <td><strong>Qualified DC Element</strong>
   </td>
   <td>dcterms:creator
   </td>
  </tr>
  <tr>
   <td><strong>Simple DC Element </strong>
   </td>
   <td>dc:creator
   </td>
  </tr>
  <tr>
   <td><strong>CONTENTdm Mapping</strong>
   </td>
   <td>Creator
   </td>
  </tr>
  <tr>
   <td>CSV Header
   </td>
   <td>Creator
   </td>
  </tr>
  <tr>
   <td><strong>Repeatable</strong>
   </td>
   <td>Yes
   </td>
  </tr>
  <tr>
   <td><strong>CV/Syntax</strong>
   </td>
   <td>
<ul>

<li>Use standard vocabularies such as <a href="http://id.loc.gov/">LCNAF</a>, <a href="https://viaf.org/">VIAF</a>, or <a href="http://www.getty.edu/research/tools/vocabularies/ulan/">ULAN</a> whenever possible; consistently applied local vocabularies are acceptable

<li>If an authorized form is unavailable, use similar syntax (Lastname, Firstname, YYYY-YYYY)
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Notes and Best Practices</strong>
   </td>
   <td>
<ul>

<li>Use a semicolon to separate multiple values

<li>Avoid use of placeholder values (e.g., “Unknown”)

<li>For oral histories, Creator is the interviewee

<li>Use name only without indication of role except in cases where a person’s role is included in an authorized form. For example, prefer “Smith, John, 1880-1960” not “Smith, John, 1880-1960, publisher”
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Examples</strong>
   </td>
   <td>
<ul>

<li>Littell, Franklin H. (Franklin Hamlin), 1917-2009

<li>Catholic Church. Archdiocese of Philadelphia (Pa.)
</li>
</ul>
   </td>
  </tr>
</table>




<p id="gdcalert10" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "[Back to Field Table]"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert11">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[[Back to Field Table]](#heading=h.3sf8crbrgxc)


<table>
  <tr>
   <td><strong>PA Digital Label</strong>
   </td>
   <td>
<h3>Date</h3>


   </td>
  </tr>
  <tr>
   <td><strong>Status</strong>
   </td>
   <td>Recommended
   </td>
  </tr>
  <tr>
   <td><strong>Description</strong>
   </td>
   <td>Date of creation of the described resource
   </td>
  </tr>
  <tr>
   <td><strong>Qualified DC Element</strong>
   </td>
   <td>dcterms:date
   </td>
  </tr>
  <tr>
   <td><strong>Simple DC Element </strong>
   </td>
   <td>dc:date
   </td>
  </tr>
  <tr>
   <td><strong>CONTENTdm Mapping</strong>
   </td>
   <td>Date
   </td>
  </tr>
  <tr>
   <td>CSV Header
   </td>
   <td>Date
   </td>
  </tr>
  <tr>
   <td><strong>Repeatable</strong>
   </td>
   <td>Yes
   </td>
  </tr>
  <tr>
   <td><strong>CV/Syntax</strong>
   </td>
   <td>
<ul>

<li>Prefer use of <a href="https://www.loc.gov/standards/datetime/">EDTF</a> for both known and uncertain dates

<li>DPLA can parse many types and formats of dates. Please refer to their <a href="https://docs.google.com/document/d/1lfiJ8yoZf1fAoR5vmJoHpWQO63eKeL8HDGVupCocfoM/edit?usp=sharing">Geographic and Temporal Guidelines</a> for examples
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Notes and Best Practices</strong>
   </td>
   <td>
<ul>

<li>Avoid use of placeholder values (e.g., “Unknown”, “n.d.”). If a date is unknown, we encourage including an estimated date range or value compatible with EDTF. If an estimate cannot be made, leave the field blank

<li>For guidance on dates or date ranges that reflect “aboutness” (for example, a memoir <em>about</em> the 1870s) please see 

<p id="gdcalert11" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "Temporal Coverage"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert12">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

<a href="#heading=h.tso54ioou99r">Temporal Coverage</a>

<li>Except where appropriate for born-digital objects, do not map dates of digitization or digital publication (as opposed to the creation of the original) to dcterms:date or dc:date. Institutions with QDC support may use alternate mappings such as dcterms:issued or dcterms:available. Institutions without QDC support should map only the date the item was created to dc:date
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Examples</strong>
   </td>
   <td>Known date
<ul>

<li>1999

<li>1999-05

<li>1999-05-01

<p>
Uncertain date
<ul>

<li>1999?

<li>199u

<li>1999-05?

<li>1999-05-01?

<p>
Approximate date
<ul>

<li>1999~

<li>1999-05~

<li>1999-05-01~

<p>
Date range
<ul>

<li>1992/1995

<li>1990-02-08/2017-03-09

<li>1984/2004-06~

<p>
Acceptable non-EDTF values
<ul>

<li>circa 1999

<li>ca. 1999

<li>approximately 1999

<li>1992-1995
</li>
</ul>
</li>
</ul>
</li>
</ul>
</li>
</ul>
</li>
</ul>
   </td>
  </tr>
</table>




<p id="gdcalert12" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "[Back to Field Table]"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert13">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[[Back to Field Table]](#heading=h.3sf8crbrgxc)


<table>
  <tr>
   <td><strong>PA Digital Label</strong>
   </td>
   <td>
<h3>Description</h3>


   </td>
  </tr>
  <tr>
   <td><strong>Status</strong>
   </td>
   <td>Recommended
   </td>
  </tr>
  <tr>
   <td><strong>Description</strong>
   </td>
   <td>A free text account of the described resource that succinctly captures its “aboutness”
   </td>
  </tr>
  <tr>
   <td><strong>Qualified DC Element</strong>
   </td>
   <td>dcterms:description
   </td>
  </tr>
  <tr>
   <td><strong>Simple DC Element</strong>
   </td>
   <td>dc:description
   </td>
  </tr>
  <tr>
   <td><strong>CONTENTdm Mapping</strong>
   </td>
   <td>Description
   </td>
  </tr>
  <tr>
   <td>CSV Header
   </td>
   <td>Description
   </td>
  </tr>
  <tr>
   <td><strong>Repeatable</strong>
   </td>
   <td>Yes
   </td>
  </tr>
  <tr>
   <td><strong>CV/Syntax</strong>
   </td>
   <td>
<ul>

<li>Natural language; semicolons may be used as punctuation
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Notes and Best Practices</strong>
   </td>
   <td>
<ul>

<li>Description at the object-level is highly preferred

<li>Contributing institutions should consider the utility of the Description field in the DPLA portal as a rich source of keywords for discovery

<li>Do not map fields with OCR or full-text transcription into the Description field

<li>Revise potentially harmful content descriptions with more respectful terminology
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Examples</strong>
   </td>
   <td>
<ul>

<li>Program dated February 14, 1943 for a lecture titled "This Year of Our Lord," given by Fordham University President Robert I. Gannon, S.J. at the Hotel Casey in Scranton, Pennsylvania. Gannon's lecture was part of the University of Scranton Lecture series. The program also advertises the next lecture in the series, a talk on "Christendom and the Coming Peace" by Fordham University professor Gerald Groveland Walsh, S.J. scheduled for March 14, 1943. 4 pages.

<li>Mummer's Parade on New Year's Day. South Broad Street, South Philadelphia, PA.

<li>Oral history recorded December 23, 1981 and May 20, 1982 in Newark, N.J. and Rochester, N.Y.
</li>
</ul>
   </td>
  </tr>
</table>




<p id="gdcalert13" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "[Back to Field Table]"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert14">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[[Back to Field Table]](#heading=h.3sf8crbrgxc)


<table>
  <tr>
   <td><strong>PA Digital Label</strong>
   </td>
   <td>
<h3>Extent</h3>


   </td>
  </tr>
  <tr>
   <td><strong>Status</strong>
   </td>
   <td>Optional
   </td>
  </tr>
  <tr>
   <td><strong>Description</strong>
   </td>
   <td>The size or duration of the described resource. Examples for print materials include number of pages, a specification of length, width, and breadth, or for audio-visual materials, a time period of duration in hours, minutes, and seconds
   </td>
  </tr>
  <tr>
   <td><strong>Qualified DC Element</strong>
   </td>
   <td>dcterms:extent
   </td>
  </tr>
  <tr>
   <td><strong>CONTENTdm Mapping</strong>
   </td>
   <td>Format-Extent
   </td>
  </tr>
  <tr>
   <td>CSV Header
   </td>
   <td>Extent
   </td>
  </tr>
  <tr>
   <td><strong>Repeatable</strong>
   </td>
   <td>Yes
   </td>
  </tr>
  <tr>
   <td><strong>CV/Syntax</strong>
   </td>
   <td>
<ul>

<li>Natural language; semicolons may be used as punctuation
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Notes and Best Practices</strong>
   </td>
   <td>
<ul>

<li>Recommend use of a content standard such as <a href="https://www.loc.gov/aba/rda/">RDA</a>, <a href="http://vraweb.org/resources/cataloging-cultural-objects/">CCO</a>, or <a href="http://rbms.info/dcrm/dcrms/">DCRMS</a> when applicable

<li>Use a semicolon to separate multiple values

<li>For dimensions, include units. Spell out abbreviations for maximum clarity

<li>For video or sound recording run times, use HH:MM:SS format with leading zeros when necessary
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Examples</strong>
   </td>
   <td>
<ul>

<li>4 7/8 x 8 3/16 inches

<li>1 map on 13 sheets

<li>00:14:21
</li>
</ul>
   </td>
  </tr>
</table>




<p id="gdcalert14" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "[Back to Field Table]"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert15">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[[Back to Field Table]](#heading=h.3sf8crbrgxc)


<table>
  <tr>
   <td><strong>PA Digital Label</strong>
   </td>
   <td>
<h3>File Format</h3>


   </td>
  </tr>
  <tr>
   <td><strong>Status</strong>
   </td>
   <td>Optional 
   </td>
  </tr>
  <tr>
   <td><strong>Description</strong>
   </td>
   <td>The file format of the digital object
   </td>
  </tr>
  <tr>
   <td><strong>Qualified DC Element </strong>
   </td>
   <td>dcterms:format
   </td>
  </tr>
  <tr>
   <td><strong>Simple DC Element </strong>
   </td>
   <td>dc:format
   </td>
  </tr>
  <tr>
   <td><strong>CONTENTdm Mapping</strong>
   </td>
   <td>Format
   </td>
  </tr>
  <tr>
   <td>CSV Header
   </td>
   <td>Format
   </td>
  </tr>
  <tr>
   <td><strong>Repeatable</strong>
   </td>
   <td>Yes
   </td>
  </tr>
  <tr>
   <td><strong>CV/Syntax</strong>
   </td>
   <td>
<ul>

<li>Recommend use of <a href="https://www.iana.org/assignments/media-types/media-types.xhtml">IANA Media Types</a>
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Notes and Best Practices</strong>
   </td>
   <td>
<ul>

<li>Entries include a media type and subtype, separated with a slash

<li>Use a semicolon to separate multiple values
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Examples</strong>
   </td>
   <td>
<ul>

<li>application/pdf

<li>audio/mpeg

<li>image/jpeg

<li>image/jp2

<li>image/tiff

<li>video/mpeg

<li>video/mp4
</li>
</ul>
   </td>
  </tr>
</table>




<p id="gdcalert15" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "[Back to Field Table]"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert16">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[[Back to Field Table]](#heading=h.3sf8crbrgxc)


<table>
  <tr>
   <td><strong>PA Digital Label</strong>
   </td>
   <td>
<h3>Format</h3>


   </td>
  </tr>
  <tr>
   <td><strong>Status</strong>
   </td>
   <td>Recommended
   </td>
  </tr>
  <tr>
   <td><strong>Description</strong>
   </td>
   <td>Physical medium of the described resource
   </td>
  </tr>
  <tr>
   <td><strong>Qualified DC Element</strong>
   </td>
   <td>dcterms:type
   </td>
  </tr>
  <tr>
   <td><strong>Simple DC Element </strong>
   </td>
   <td>dc:type
   </td>
  </tr>
  <tr>
   <td><strong>CONTENTdm Mapping</strong>
   </td>
   <td>Type
   </td>
  </tr>
  <tr>
   <td>CSV Header
   </td>
   <td>Type
   </td>
  </tr>
  <tr>
   <td><strong>Repeatable</strong>
   </td>
   <td>Yes
   </td>
  </tr>
  <tr>
   <td><strong>CV/Syntax</strong>
   </td>
   <td>
<ul>

<li>Use standard vocabularies such as <a href="http://www.getty.edu/research/tools/vocabularies/aat">AAT</a> or <a href="http://id.loc.gov/vocabulary/graphicMaterials">TGM</a>; consistently applied local vocabularies are acceptable
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Notes and Best Practices</strong>
   </td>
   <td>
<ul>

<li>Format is a more granular description of an object’s type than what is possible with the DCMI vocabulary used in the 

<p id="gdcalert16" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "Type"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert17">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

<a href="#heading=h.l92nrwdn8o6p">Type</a> field

<li>Values in an incoming Type field not found in the DCMI Type vocabulary will map to Format in PA Digital and DPLA. Please see 

<p id="gdcalert17" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "Type"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert18">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

<a href="#heading=h.l92nrwdn8o6p">Type</a> for additional mappings from our Type field

<li>Use a semicolon to separate multiple values
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Examples</strong>
   </td>
   <td>
<ul>

<li>Fire insurance maps

<li>Zines
</li>
</ul>
   </td>
  </tr>
</table>




<p id="gdcalert18" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "[Back to Field Table]"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert19">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[[Back to Field Table]](#heading=h.3sf8crbrgxc)


<table>
  <tr>
   <td><strong>PA Digital Label</strong>
   </td>
   <td>
<h3>Identifier</h3>


   </td>
  </tr>
  <tr>
   <td><strong>Status</strong>
   </td>
   <td>Required or Derived. PA Digital does not map local record identifiers, but generates its own based on metadata elsewhere in the record. Best practices indicated here are offered as a resource
   </td>
  </tr>
  <tr>
   <td><strong>Description</strong>
   </td>
   <td>An unambiguous reference to the described resource within a given context
   </td>
  </tr>
  <tr>
   <td><strong>Qualified DC Element</strong>
   </td>
   <td>dcterms:identifier
   </td>
  </tr>
  <tr>
   <td><strong>Simple DC Element </strong>
   </td>
   <td>dc:identifier
   </td>
  </tr>
  <tr>
   <td><strong>CONTENTdm Mapping</strong>
   </td>
   <td>Identifier
   </td>
  </tr>
  <tr>
   <td>CSV Header
   </td>
   <td>Identifier
   </td>
  </tr>
  <tr>
   <td><strong>Repeatable</strong>
   </td>
   <td>No
   </td>
  </tr>
  <tr>
   <td><strong>CV/Syntax</strong>
   </td>
   <td>
<ul>

<li>Recommend alphanumeric strings only with no spaces or special characters such as “ @ “, “ # “, “ $ “, “ % “, “ &“,
    “ * “, “ ’ “, “ . “
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Notes and Best Practices</strong>
   </td>
   <td>
<ul>

<li>Recommended best practice is to uniquely identify the resource within an institution’s collections by means of a string conforming to a formal identification system

<li>Values from this field may be used to generate metadata for other fields such as URL and Preview

<li>For institutions that do not supply identifiers, they may be derived from metadata elsewhere in the record
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Examples</strong>
   </td>
   <td>
<ul>

<li>P441110B

<li>HPHWPZ201404000165

<li>1999-002_006
</li>
</ul>
   </td>
  </tr>
</table>




<p id="gdcalert19" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "[Back to Field Table]"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert20">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[[Back to Field Table]](#heading=h.3sf8crbrgxc)


<table>
  <tr>
   <td><strong>PA Digital Label</strong>
   </td>
   <td>
<h3>IIIF Base URL</h3>


   </td>
  </tr>
  <tr>
   <td><strong>Status</strong>
   </td>
   <td>Optional or Derived
   </td>
  </tr>
  <tr>
   <td><strong>Description</strong>
   </td>
   <td>The base URL required to access a IIIF service for the digital resource
   </td>
  </tr>
  <tr>
   <td><strong>Qualified DC Element</strong>
   </td>
   <td>dcterms:identifier
   </td>
  </tr>
  <tr>
   <td>CSV Header
   </td>
   <td>IIIF_Base
   </td>
  </tr>
  <tr>
   <td><strong>Repeatable</strong>
   </td>
   <td>No
   </td>
  </tr>
  <tr>
   <td><strong>Notes and Best Practices</strong>
   </td>
   <td>
<ul>

<li>Must resolve to a IIIF service

<li>For institutions that do not supply IIIF information with their metadata, it may be derived from metadata elsewhere in the record. For example, a IIIF Base URL may be derived from the URL for the digital object
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Examples</strong>
   </td>
   <td>
<ul>

<li>https://digital.library.temple.edu/digital/iiif/p245801coll0/4024/

<li>https://media.philamuseum.org/image/JGJ_B008_F009_001_001/
</li>
</ul>
   </td>
  </tr>
</table>




<p id="gdcalert20" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "[Back to Field Table]"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert21">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[[Back to Field Table]](#heading=h.3sf8crbrgxc)


<table>
  <tr>
   <td><strong>PA Digital Label</strong>
   </td>
   <td>
<h3>IIIF Manifest</h3>


   </td>
  </tr>
  <tr>
   <td><strong>Status</strong>
   </td>
   <td>Optional or Derived
   </td>
  </tr>
  <tr>
   <td><strong>Description</strong>
   </td>
   <td>A URI for the manifest of a IIIF resource; may be used to support inclusion of object in Wikimedia Commons
   </td>
  </tr>
  <tr>
   <td><strong>Qualified DC Element</strong>
   </td>
   <td>dcterms:isReferencedBy
   </td>
  </tr>
  <tr>
   <td>CSV Header
   </td>
   <td>IIIF_Man
   </td>
  </tr>
  <tr>
   <td><strong>Repeatable</strong>
   </td>
   <td>No
   </td>
  </tr>
  <tr>
   <td><strong>Notes and Best Practices</strong>
   </td>
   <td>
<ul>

<li>Must resolve to a IIIF manifest

<li>For institutions that do not supply IIIF information with their metadata, it may be derived from metadata elsewhere in the record. For example, a IIIF Manifest URI may be derived from the URL for the digital object
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Examples</strong>
   </td>
   <td>
<ul>

<li>https://digital.library.temple.edu/iiif/info/p245801coll0/4024/manifest.json

<li>https://digital.library.villanova.edu/Item/vudl:92879/Manifest
</li>
</ul>
   </td>
  </tr>
</table>




<p id="gdcalert21" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "[Back to Field Table]"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert22">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[[Back to Field Table]](#heading=h.3sf8crbrgxc)


<table>
  <tr>
   <td><strong>PA Digital Label</strong>
   </td>
   <td>
<h3>Intermediate Provider</h3>


   </td>
  </tr>
  <tr>
   <td><strong>Status</strong>
   </td>
   <td>Derived or PA Digital supplied
   </td>
  </tr>
  <tr>
   <td><strong>Description</strong>
   </td>
   <td>An intermediate organization that selects, collates, curates, or provides a repository for data from a contributing institution or institutions that is then aggregated from a single point by PA Digital
   </td>
  </tr>
  <tr>
   <td>CSV Header
   </td>
   <td>Intermediate_Provider
   </td>
  </tr>
  <tr>
   <td><strong>Repeatable</strong>
   </td>
   <td>No
   </td>
  </tr>
  <tr>
   <td><strong>Notes and Best Practices</strong>
   </td>
   <td>
<ul>

<li>Values for this field may be mapped from consistently formatted metadata elsewhere in the record; examples include identifiers and object URLs

<li>Values may also be supplied by PA Digital during the ingestion process. Intermediate organizations should specify during onboarding the desired value for this field
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Examples</strong>
   </td>
   <td>
<ul>

<li>POWER Library PA Photos and Documents

<li>Historic Pittsburgh
</li>
</ul>
   </td>
  </tr>
</table>




<p id="gdcalert22" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "[Back to Field Table]"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert23">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[[Back to Field Table]](#heading=h.3sf8crbrgxc)


<table>
  <tr>
   <td><strong>PA Digital Label</strong>
   </td>
   <td>
<h3>Language</h3>


   </td>
  </tr>
  <tr>
   <td><strong>Status</strong>
   </td>
   <td>Recommended for textual and spoken material
   </td>
  </tr>
  <tr>
   <td><strong>Description</strong>
   </td>
   <td>Language expressed in a resource that contains text or speech
   </td>
  </tr>
  <tr>
   <td><strong>Qualified DC Element </strong>
   </td>
   <td>dcterms:language
   </td>
  </tr>
  <tr>
   <td><strong>Simple DC Element </strong>
   </td>
   <td>dc:language
   </td>
  </tr>
  <tr>
   <td><strong>CONTENTdm Mapping</strong>
   </td>
   <td>Language
   </td>
  </tr>
  <tr>
   <td>CSV Header
   </td>
   <td>Language
   </td>
  </tr>
  <tr>
   <td><strong>Repeatable</strong>
   </td>
   <td>Yes
   </td>
  </tr>
  <tr>
   <td><strong>CV/Syntax</strong>
   </td>
   <td>
<ul>

<li>Use standard or consistently applied local vocabularies; <a href="https://iso639-3.sil.org/code_tables/639/data ">ISO 639-3</a> is preferred
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Notes and Best Practices</strong>
   </td>
   <td>
<ul>

<li>Use a semicolon to separate multiple values

<li>Do not use for non-linguistic content such as images containing no text
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Examples</strong>
   </td>
   <td>
<ul>

<li>eng

<li>fre

<li>afr ; afu ; eng
</li>
</ul>
   </td>
  </tr>
</table>




<p id="gdcalert23" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "[Back to Field Table]"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert24">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[[Back to Field Table]](#heading=h.3sf8crbrgxc)


<table>
  <tr>
   <td><strong>PA Digital Label</strong>
   </td>
   <td>
<h3>Media Master</h3>


   </td>
  </tr>
  <tr>
   <td><strong>Status</strong>
   </td>
   <td>Optional
   </td>
  </tr>
  <tr>
   <td><strong>Description</strong>
   </td>
   <td>URL that points to a downloadable version of the digital object; used to support inclusion of non-IIIF media objects in Wikimedia Commons
   </td>
  </tr>
  <tr>
   <td><strong>Qualified DC Element </strong>
   </td>
   <td><em>See notes below</em>
   </td>
  </tr>
  <tr>
   <td><em>CSV Header</em>
   </td>
   <td><em>Media_Master</em>
   </td>
  </tr>
  <tr>
   <td><strong>Repeatable</strong>
   </td>
   <td>Yes
   </td>
  </tr>
  <tr>
   <td><strong>CV/Syntax</strong>
   </td>
   <td>
<ul>

<li>
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Notes and Best Practices</strong>
   </td>
   <td>
<ul>

<li>Please contact PA Digital metadata specialists before implementing this field

<li>Must resolve to a downloadable version of the digital object; thumbnails that represent the digital object for the purposes of providing a preview are not acceptable

<li>Records for compound, multipage objects such as books should include a URL to each file associated with the object. Where these are not available via the ingestion process, a CSV supplement may be supplied
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Examples</strong>
   </td>
   <td>
<ul>

<li>https://archives.philamuseum.org/jgj/JCC_B043_F001_001/cat-0003
</li>
</ul>
   </td>
  </tr>
</table>




<p id="gdcalert24" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "[Back to Field Table]"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert25">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[[Back to Field Table]](#heading=h.3sf8crbrgxc)


<table>
  <tr>
   <td><strong>PA Digital Label</strong>
   </td>
   <td>
<h3>Place</h3>


   </td>
  </tr>
  <tr>
   <td><strong>Status</strong>
   </td>
   <td>Recommended
   </td>
  </tr>
  <tr>
   <td><strong>Description</strong>
   </td>
   <td>Geographic location referenced or depicted by the described resource; captures its “aboutness”
   </td>
  </tr>
  <tr>
   <td><strong>Qualified DC Element</strong>
   </td>
   <td>dcterms:spatial
   </td>
  </tr>
  <tr>
   <td><strong>Simple DC Element </strong>
   </td>
   <td>dc:coverage 
   </td>
  </tr>
  <tr>
   <td><strong>CONTENTdm Mapping</strong>
   </td>
   <td>Coverage-Spatial
   </td>
  </tr>
  <tr>
   <td>CSV Header
   </td>
   <td>Place
   </td>
  </tr>
  <tr>
   <td><strong>Repeatable</strong>
   </td>
   <td>Yes
   </td>
  </tr>
  <tr>
   <td><strong>CV/Syntax</strong>
   </td>
   <td>
<ul>

<li>Use standard vocabularies such as <a href="http://id.loc.gov/authorities/names.html">LCNAF</a>, <a href="http://www.getty.edu/vow/TGNSearchPage.jsp">TGN</a>, <a href="http://www.geonames.org/">GeoNames</a>, or <a href="http://fast.oclc.org/searchfast/ ">FAST</a> whenever possible; consistently applied local vocabularies are acceptable
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Notes and Best Practices</strong>
   </td>
   <td>
<ul>

<li>Use a semicolon to separate multiple values

<li>This field does not represent the physical location or address of the physical or digital repository where the original item or digital facsimile is held

<li>Consistency when using hierarchical values is recommended (e.g., “Pittsburgh, Pennsylvania, United States of America”)

<li>Addresses, latitude/longitude, or other forms of location markers may also be mapped to this field for the purposes of geolocation and/or digital mapping

<li>For latitude/longitude, DPLA prefers latitude first, with the two coordinates separated by a comma, limited to whole numbers and decimals as opposed to degree-minutes-seconds (e.g., “6.703, 46.627”). If used, compass directions should appear after the number

<li>See DPLA’s <a href="https://docs.google.com/document/d/1lfiJ8yoZf1fAoR5vmJoHpWQO63eKeL8HDGVupCocfoM/edit?usp=sharing">Geographic and Temporal Guidelines</a> for more information 
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Examples</strong>
   </td>
   <td>
<ul>

<li>Pittsburgh (Pa.)

<li>Allegheny County (Pa.)

<li>Harrison (Allegheny County, Pa. : Township)

<li>40.85N, 77.84W

<li>40.85, -77.84
</li>
</ul>
   </td>
  </tr>
</table>




<p id="gdcalert25" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "[Back to Field Table]"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert26">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[[Back to Field Table]](#heading=h.3sf8crbrgxc)


<table>
  <tr>
   <td><strong>PA Digital Label</strong>
   </td>
   <td>
<h3>Preview</h3>


   </td>
  </tr>
  <tr>
   <td><strong>Status</strong>
   </td>
   <td>Strongly recommended or Derived
   </td>
  </tr>
  <tr>
   <td><strong>Description</strong>
   </td>
   <td>The URL of a thumbnail, extract, or other type of resource representing the digital object for the purposes of providing a preview
   </td>
  </tr>
  <tr>
   <td><strong>Qualified DC Element</strong>
   </td>
   <td>dcterms:identifier
   </td>
  </tr>
  <tr>
   <td><strong>Simple DC Element </strong>
   </td>
   <td>dc:identifier
   </td>
  </tr>
  <tr>
   <td>CSV Header
   </td>
   <td>Preview
   </td>
  </tr>
  <tr>
   <td><strong>Repeatable</strong>
   </td>
   <td>No
   </td>
  </tr>
  <tr>
   <td><strong>Notes and Best Practices</strong>
   </td>
   <td>
<ul>

<li>The URL must resolve to a preview of the digital object

<li>Values for this field may be mapped from consistently formatted metadata elsewhere in the record
</li>
</ul>
   </td>
  </tr>
</table>




<p id="gdcalert26" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "[Back to Field Table]"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert27">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[[Back to Field Table]](#heading=h.3sf8crbrgxc)


<table>
  <tr>
   <td><strong>PA Digital Label</strong>
   </td>
   <td>
<h3>Publisher</h3>


   </td>
  </tr>
  <tr>
   <td><strong>Status</strong>
   </td>
   <td>Optional
   </td>
  </tr>
  <tr>
   <td><strong>Description</strong>
   </td>
   <td>An entity responsible for making the described, original resource available. Typically, this is a publishing house, a corporate body, a government agency, a university, or other organization
   </td>
  </tr>
  <tr>
   <td><strong>Qualified DC Element</strong>
   </td>
   <td>dcterms:publisher
   </td>
  </tr>
  <tr>
   <td><strong>Simple DC Element </strong>
   </td>
   <td>dc:publisher
   </td>
  </tr>
  <tr>
   <td><strong>CONTENTdm Mapping</strong>
   </td>
   <td>Publisher
   </td>
  </tr>
  <tr>
   <td>CSV Header
   </td>
   <td>Publisher
   </td>
  </tr>
  <tr>
   <td><strong>Repeatable</strong>
   </td>
   <td>Yes
   </td>
  </tr>
  <tr>
   <td><strong>CV/Syntax</strong>
   </td>
   <td>
<ul>

<li>Use standard vocabularies such as <a href="http://id.loc.gov/">LCNAF</a> or <a href="https://viaf.org/">VIAF</a> whenever possible; consistently applied local vocabularies are acceptable

<li>If an authorized form is unavailable, use similar syntax; semicolons may be used as punctuation
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Notes and Best Practices</strong>
   </td>
   <td>
<ul>

<li>Use this field for published materials such as books, magazines, and journals

<li>Use a semicolon to separate multiple values

<li>Avoid use of placeholder values (e.g., “Unknown”, “s.n.”); leave the field blank if a publisher cannot be accurately determined or if there is no publisher

<li>Avoid use of qualifying terms except in cases where a role is included in the authorized form. For example, prefer “Rand McNally and Company” not “Rand McNally and Company, publisher”

<li>Not to be used for the entity responsible for digitizing or making the digital representation available
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Examples</strong>
   </td>
   <td>
<ul>

<li>Rand McNally and Company

<li>Philadelphia Evening Bulletin
</li>
</ul>
   </td>
  </tr>
</table>




<p id="gdcalert27" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "[Back to Field Table]"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert28">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[[Back to Field Table]](#heading=h.3sf8crbrgxc)


<table>
  <tr>
   <td><strong>PA Digital Label</strong>
   </td>
   <td>
<h3>Relation</h3>


   </td>
  </tr>
  <tr>
   <td><strong>Status</strong>
   </td>
   <td>Optional
   </td>
  </tr>
  <tr>
   <td><strong>Description</strong>
   </td>
   <td>A related resource, such as the name of a collection, series, or group of thematic works. May be suitable for items that are part of an archival collection
   </td>
  </tr>
  <tr>
   <td><strong>Qualified DC Element</strong>
   </td>
   <td>dcterms:relation
   </td>
  </tr>
  <tr>
   <td><strong>Simple DC Element </strong>
   </td>
   <td>dc:relation
   </td>
  </tr>
  <tr>
   <td><strong>CONTENTdm Mapping</strong>
   </td>
   <td>Relation
   </td>
  </tr>
  <tr>
   <td>CSV Header
   </td>
   <td>Relation
   </td>
  </tr>
  <tr>
   <td><strong>Repeatable</strong>
   </td>
   <td>Yes
   </td>
  </tr>
  <tr>
   <td><strong>CV/Syntax</strong>
   </td>
   <td>
<ul>

<li>Natural language; semicolons may be used as punctuation
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Notes and Best Practices</strong>
   </td>
   <td>
<ul>

<li>Use a semicolon to separate multiple values
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Examples</strong>
   </td>
   <td>
<ul>

<li>George D. McDowell Philadelphia Evening Bulletin Collection

<li>The Zaner-Bloser, Inc. / Sonya Bloser Monroe Collection
</li>
</ul>
   </td>
  </tr>
</table>




<p id="gdcalert28" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "[Back to Field Table]"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert29">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[[Back to Field Table]](#heading=h.3sf8crbrgxc)


<table>
  <tr>
   <td><strong>PA Digital Label</strong>
   </td>
   <td>
<h3>Replaced By</h3>


   </td>
  </tr>
  <tr>
   <td><strong>Status</strong>
   </td>
   <td>Optional
   </td>
  </tr>
  <tr>
   <td><strong>Description</strong>
   </td>
   <td>A related resource that supplants, displaces, or supersedes the described resource
   </td>
  </tr>
  <tr>
   <td><strong>Qualified DC Element</strong>
   </td>
   <td>
    dcterms:isReplacedBy
   </td>
  </tr>
  <tr>
   <td><strong>CONTENTdm Mapping</strong>
   </td>
   <td>Relation-Is Replaced By
   </td>
  </tr>
  <tr>
   <td>CSV Header
   </td>
   <td>Replaced_By
   </td>
  </tr>
  <tr>
   <td><strong>Repeatable</strong>
   </td>
   <td>Yes
   </td>
  </tr>
  <tr>
   <td><strong>CV/Syntax</strong>
   </td>
   <td>
<ul>

<li>Natural language
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Notes and Best Practices</strong>
   </td>
   <td>
<ul>

<li>This field is intended for series and title changes, for example government documents or serial publications and periodicals
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Examples</strong>
   </td>
   <td>
<ul>

<li>Federal Highway Administration Office of Motor Carrier and Highway Safety Register

<li>Grants for Foreign and International Programs
</li>
</ul>
   </td>
  </tr>
</table>




<p id="gdcalert29" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "[Back to Field Table]"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert30">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[[Back to Field Table]](#heading=h.3sf8crbrgxc)


<table>
  <tr>
   <td><strong>PA Digital Label</strong>
   </td>
   <td>
<h3>Replaces</h3>


   </td>
  </tr>
  <tr>
   <td><strong>Status</strong>
   </td>
   <td>Optional
   </td>
  </tr>
  <tr>
   <td><strong>Description</strong>
   </td>
   <td>A related resource that is supplanted, displaced, or superseded by the described resource
   </td>
  </tr>
  <tr>
   <td><strong>Qualified DC Element</strong>
   </td>
   <td>dcterms:replaces
   </td>
  </tr>
  <tr>
   <td><strong>CONTENTdm Mapping</strong>
   </td>
   <td>Relation-Replaces
   </td>
  </tr>
  <tr>
   <td>CSV Header
   </td>
   <td>Replaces
   </td>
  </tr>
  <tr>
   <td><strong>Repeatable</strong>
   </td>
   <td>Yes
   </td>
  </tr>
  <tr>
   <td><strong>CV/Syntax</strong>
   </td>
   <td>
<ul>

<li>Natural language
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Notes and Best Practices</strong>
   </td>
   <td>
<ul>

<li>This field is intended for series and title changes, for example government documents or serial publications and periodicals
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Examples</strong>
   </td>
   <td>
<ul>

<li>Federal Highway Administration Office of Motor Carriers Register

<li>Grants for International and Foreign Programs
</li>
</ul>
   </td>
  </tr>
</table>




<p id="gdcalert30" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "[Back to Field Table]"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert31">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[[Back to Field Table]](#heading=h.3sf8crbrgxc)


<table>
  <tr>
   <td><strong>PA Digital Label</strong>
   </td>
   <td>
<h3>Rights</h3>


   </td>
  </tr>
  <tr>
   <td><strong>Status</strong>
   </td>
   <td>A rights statement, whether natural language or a URI in 

<p id="gdcalert31" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "Rights URI"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert32">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

<a href="#heading=h.gtqxhqb41kn">Rights URI</a>, is required
   </td>
  </tr>
  <tr>
   <td><strong>Description</strong>
   </td>
   <td>Information about rights held in and over the digitized resource. Typically, rights information includes a statement about various property rights associated with the resource, including intellectual property rights
   </td>
  </tr>
  <tr>
   <td><strong>Qualified DC Element</strong>
   </td>
   <td>dcterms:rights
   </td>
  </tr>
  <tr>
   <td><strong>Simple DC Element </strong>
   </td>
   <td>dc:rights
   </td>
  </tr>
  <tr>
   <td><strong>CONTENTdm Mapping</strong>
   </td>
   <td>Rights
   </td>
  </tr>
  <tr>
   <td>CSV Header
   </td>
   <td>Rights
   </td>
  </tr>
  <tr>
   <td><strong>Repeatable</strong>
   </td>
   <td>Yes
   </td>
  </tr>
  <tr>
   <td><strong>CV/Syntax</strong>
   </td>
   <td>
<ul>

<li>Natural language; semicolons may be used as punctuation
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Notes and Best Practices</strong>
   </td>
   <td>
<ul>

<li>Values that are not URIs will map to PA Digital’s Rights field; URIs will map to 

<p id="gdcalert32" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "Rights URI"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert33">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

<a href="#heading=h.gtqxhqb41kn">Rights URI</a>

<li>Use of a URI is preferred over natural language or textual statements

<li>If supplying both a URI and a natural language statement, use separate fields. Both may be mapped to dcterms:rights or dc:rights

<li>If using natural language, use clear, standardized statements; statements that provide only contact or reproduction information are insufficient

<li>Natural language statements should not contradict, or merely reiterate, the rights statement from <a href="http://rightsstatements.org/en/">RightsStatements.org</a> or <a href="https://creativecommons.org/">Creative Commons</a>; URIs will resolve to a textual statement in the DPLA portal

<li>See 

<p id="gdcalert33" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "Rights URI"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert34">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

<a href="#heading=h.gtqxhqb41kn">Rights URI</a> for guidance on using and mapping rights statement URIs
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Examples</strong>
   </td>
   <td>
<ul>

<li>Copyright status of the resource is unknown.

<li>In the public domain and may be used without copyright restriction.
</li>
</ul>
   </td>
  </tr>
</table>




<p id="gdcalert34" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "[Back to Field Table]"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert35">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[[Back to Field Table]](#heading=h.3sf8crbrgxc)


<table>
  <tr>
   <td><strong>PA Digital Label</strong>
   </td>
   <td>
<h3>Rights Holder</h3>


   </td>
  </tr>
  <tr>
   <td><strong>Status</strong>
   </td>
   <td>Optional
   </td>
  </tr>
  <tr>
   <td><strong>Description</strong>
   </td>
   <td>A person or organization owning or managing rights over the described resource
   </td>
  </tr>
  <tr>
   <td><strong>Qualified DC Element</strong>
   </td>
   <td>dcterms:rightsholder
   </td>
  </tr>
  <tr>
   <td><strong>CONTENTdm Mapping</strong>
   </td>
   <td>Rights-RightsHolder
   </td>
  </tr>
  <tr>
   <td>CSV Header
   </td>
   <td>Rights_Holder
   </td>
  </tr>
  <tr>
   <td><strong>Repeatable</strong>
   </td>
   <td>No
   </td>
  </tr>
  <tr>
   <td><strong>CV/Syntax</strong>
   </td>
   <td>
<ul>

<li>Use standard vocabularies such as <a href="http://id.loc.gov/">LCNAF</a> or <a href="https://viaf.org/">VIAF</a> whenever possible; consistently applied local vocabularies are acceptable

<li>If an authorized form is unavailable, use similar syntax (Lastname, Firstname, YYYY-YYYY)
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Notes and Best Practices</strong>
   </td>
   <td>
<ul>

<li>If using simple Dublin Core, do not map this information to dc:rights
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Examples</strong>
   </td>
   <td>
<ul>

<li>University of Scranton
</li>
</ul>
   </td>
  </tr>
</table>




<p id="gdcalert35" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "[Back to Field Table]"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert36">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[[Back to Field Table]](#heading=h.3sf8crbrgxc)


<table>
  <tr>
   <td><strong>PA Digital Label</strong>
   </td>
   <td>
<h3>Rights URI</h3>


   </td>
  </tr>
  <tr>
   <td><strong>Status</strong>
   </td>
   <td>A rights statement, whether a uniform resource identifier (URI) in this field or a natural language statement in 

<p id="gdcalert36" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "Rights"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert37">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

<a href="#heading=h.r7eiqqmk3qbk">Rights</a>, is required.  This can be a uniform resource identifier (URI) from RightsStatements.org/Creative Commons or a natural language statement. 
   </td>
  </tr>
  <tr>
   <td><strong>Description</strong>
   </td>
   <td>A standardized rights statement URI from RightsStatements.org or Creative Commons that conveys information about rights held in and over the digitized resource
   </td>
  </tr>
  <tr>
   <td><strong>Qualified DC Element</strong>
   </td>
   <td>dcterms:rights
   </td>
  </tr>
  <tr>
   <td><strong>Simple DC Element </strong>
   </td>
   <td>dc:rights
   </td>
  </tr>
  <tr>
   <td><strong>CONTENTdm Mapping</strong>
   </td>
   <td>Rights
   </td>
  </tr>
  <tr>
   <td>CSV Header
   </td>
   <td>Rights_URI
   </td>
  </tr>
  <tr>
   <td><strong>Repeatable</strong>
   </td>
   <td>No
   </td>
  </tr>
  <tr>
   <td><strong>CV/Syntax</strong>
   </td>
   <td>
<ul>

<li>Must use URIs from <a href="http://rightsstatements.org/en/">RightsStatements.org</a> or <a href="https://creativecommons.org/">Creative Commons</a>
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Notes and Best Practices</strong>
   </td>
   <td>
<ul>

<li>Use this field for persistent URIs from <a href="http://rightsstatements.org/en/">RightsStatements.org</a> or <a href="https://creativecommons.org/">Creative Commons</a>. These URIs will enable machine-readable and machine-actionable rights statements. URIs will point to web pages that provide more information on each rights statement and will resolve to a textual statement in the DPLA portal

<li>The value must be the URI and not the URL for the web page describing the statement 
<ul>
 
<li>Correct: <a href="http://rightsstatements.org/vocab/NoC-US/1.0/">http://rightsstatements.org/vocab/NoC-US/1.0/</a>
 
<li>Incorrect: <a href="https://rightsstatements.org/page/NoC-US/1.0/?language=en">https://rightsstatements.org/page/NoC-US/1.0/?language=en</a>
</li> 
</ul>

<li>Fields with URIs should contain no other text

<li>If supplying both a URI and a natural language statement, use separate fields. Both may be mapped to dcterms:rights or dc:rights

<li>See 

<p id="gdcalert37" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "Rights"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert38">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

<a href="#heading=h.r7eiqqmk3qbk">Rights</a> for guidance on using and mapping natural language rights statements
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Examples</strong>
   </td>
   <td>
<ul>

<li><a href="http://rightsstatements.org/vocab/InC-RUU/1.0/">http://rightsstatements.org/vocab/InC-RUU/1.0/</a>

<li><a href="http://rightsstatements.org/vocab/NoC-US/1.0/">http://rightsstatements.org/vocab/NoC-US/1.0/</a>

<li><a href="https://creativecommons.org/publicdomain/zero/1.0/">https://creativecommons.org/publicdomain/zero/1.0/	</a>
</li>
</ul>
   </td>
  </tr>
</table>




<p id="gdcalert38" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "[Back to Field Table]"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert39">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[[Back to Field Table]](#heading=h.3sf8crbrgxc)


<table>
  <tr>
   <td><strong>PA Digital Label</strong>
   </td>
   <td>
<h3>Source</h3>


   </td>
  </tr>
  <tr>
   <td><strong>Status</strong>
   </td>
   <td>Optional
   </td>
  </tr>
  <tr>
   <td><strong>Description</strong>
   </td>
   <td>A resource from which the described resource is derived. May include information the user would need to locate the original item in a physical archives
   </td>
  </tr>
  <tr>
   <td><strong>Qualified DC Element</strong>
   </td>
   <td>dcterms:source
   </td>
  </tr>
  <tr>
   <td><strong>Simple DC Element </strong>
   </td>
   <td>dc:source
   </td>
  </tr>
  <tr>
   <td><strong>CONTENTdm Mapping</strong>
   </td>
   <td>Source
   </td>
  </tr>
  <tr>
   <td>CSV Header
   </td>
   <td>Source
   </td>
  </tr>
  <tr>
   <td><strong>Repeatable</strong>
   </td>
   <td>Yes
   </td>
  </tr>
  <tr>
   <td><strong>CV/Syntax</strong>
   </td>
   <td>
<ul>

<li>Use a consistently applied, standardized syntax
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Notes and Best Practices</strong>
   </td>
   <td>
<ul>

<li>Use a semicolon to separate multiple values
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Examples</strong>
   </td>
   <td>
<ul>

<li>Collection, Box 1, Folder 1

<li>File A93-25 Folder 1
</li>
</ul>
   </td>
  </tr>
</table>




<p id="gdcalert39" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "[Back to Field Table]"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert40">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[[Back to Field Table]](#heading=h.3sf8crbrgxc)


<table>
  <tr>
   <td><strong>PA Digital Label</strong>
   </td>
   <td>
<h3>Subject</h3>


   </td>
  </tr>
  <tr>
   <td><strong>Status</strong>
   </td>
   <td>Recommended
   </td>
  </tr>
  <tr>
   <td><strong>Description</strong>
   </td>
   <td>The topic of the described resource
   </td>
  </tr>
  <tr>
   <td><strong>Qualified DC Element</strong>
   </td>
   <td>dcterms:subject
   </td>
  </tr>
  <tr>
   <td><strong>Simple DC Element </strong>
   </td>
   <td>dc:subject
   </td>
  </tr>
  <tr>
   <td><strong>CONTENTdm Mapping</strong>
   </td>
   <td>Subject
   </td>
  </tr>
  <tr>
   <td>CSV Header
   </td>
   <td>Subject
   </td>
  </tr>
  <tr>
   <td><strong>Repeatable</strong>
   </td>
   <td>Yes
   </td>
  </tr>
  <tr>
   <td><strong>CV/Syntax</strong>
   </td>
   <td>
<ul>

<li>Use standard vocabularies such as <a href="http://id.loc.gov/authorities/subjects.html">LCSH</a>, <a href="https://meshb.nlm.nih.gov/search">MeSH</a>, <a href="http://fast.oclc.org/searchfast/ ">FAST</a>, or <a href="http://id.loc.gov/authorities/names.html">LCNAF</a> whenever possible; consistently applied local vocabularies are acceptable
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Notes and Best Practices</strong>
   </td>
   <td>
<ul>

<li>Use a semicolon to separate multiple values

<li>Use uncoordinated subject headings when possible and enter geographic and format information in separate fields. See 

<p id="gdcalert40" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "Place"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert41">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

<a href="#heading=h.gxlh1sslrfqx">Place</a> and 

<p id="gdcalert41" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "Format"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert42">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

<a href="#heading=h.or6g2dfj8ekl">Format</a>

<li>When subdividing a subject term, prefer one space between LCSH subjects and dashes (Term -- Term)

<li>If using a geographic or form subdivision, provide a corresponding value in 

<p id="gdcalert42" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "Place"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert43">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

<a href="#heading=h.gxlh1sslrfqx">Place</a> or 

<p id="gdcalert43" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "Format"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert44">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

<a href="#heading=h.or6g2dfj8ekl">Format</a> respectively
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Examples</strong>
   </td>
   <td>
<ul>

<li>Coal miners -- Social conditions

<li><code>&lt;dc:subject>Civil rights movements&lt;/dc:subject> AND</code>
    <code>&lt;dc:coverage>Philadelphia (Pa.)&lt;/dc:coverage></code>
<p>

    Instead of:
<p>

    <code>&lt;dc:subject>Civil rights movements -- Pennsylvania -- Philadelphia&lt;/dc:subject></code>
<ul>

<li><code>&lt;dc:subject>Harlem Renaissance&lt;/dc:subject> AND</code>
<p>

    <code>&lt;dc:type>Maps&lt;/dc:type></code>
<p>

    Instead of:
<p>

    <code>&lt;dc:subject>Harlem Renaissance -- Maps&lt;/dc:subject></code>
</li>
</ul>
</li>
</ul>
   </td>
  </tr>
</table>




<p id="gdcalert44" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "[Back to Field Table]"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert45">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[[Back to Field Table]](#heading=h.3sf8crbrgxc)


<table>
  <tr>
   <td><strong>PA Digital Label</strong>
   </td>
   <td>
<h3>Temporal Coverage</h3>


   </td>
  </tr>
  <tr>
   <td><strong>Status</strong>
   </td>
   <td>Optional
   </td>
  </tr>
  <tr>
   <td><strong>Description</strong>
   </td>
   <td>Temporal characteristics of the described resource
   </td>
  </tr>
  <tr>
   <td><strong>Qualified DC Element</strong>
   </td>
   <td>dcterms:temporal
   </td>
  </tr>
  <tr>
   <td><strong>Simple DC Element </strong>
   </td>
   <td>dc:subject
   </td>
  </tr>
  <tr>
   <td><strong>CONTENTdm Mapping</strong>
   </td>
   <td>Coverage-Temporal
   </td>
  </tr>
  <tr>
   <td>CSV Header
   </td>
   <td>Temporal
   </td>
  </tr>
  <tr>
   <td><strong>Repeatable</strong>
   </td>
   <td>Yes
   </td>
  </tr>
  <tr>
   <td><strong>CV/Syntax</strong>
   </td>
   <td>
<ul>

<li>If using a named period, use standard vocabularies such as <a href="http://id.loc.gov/authorities/subjects.html">LCSH</a> or <a href="http://fast.oclc.org/searchfast/ ">FAST</a> whenever possible; consistently applied local vocabularies are acceptable

<li>For dates or date ranges, prefer use of <a href="https://www.loc.gov/standards/datetime/">EDTF</a>
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Notes and Best Practices</strong>
   </td>
   <td>
<ul>

<li>If qualified Dublin Core is not supported, map to dc:subject (see 

<p id="gdcalert45" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "Subject"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert46">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

<a href="#heading=h.e8fofo9ojz2m">Subject</a>); use dc:coverage only for geographic information

<li>The field should describe the time period covered or represented by the resource’s content, not the date when the resource was created or published. See 

<p id="gdcalert46" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "Date"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert47">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

<a href="#heading=h.s47v3ptpnnic">Date</a> for guidance on describing the date or date range of a resource

<li>Temporal topics may be a named period, date, or date range

<li>Use a semicolon to separate multiple values
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Examples</strong>
   </td>
   <td>
<ul>

<li>Dust Bowl Era, 1931-1939

<li>1958-07/1959-06
</li>
</ul>
   </td>
  </tr>
</table>




<p id="gdcalert47" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "[Back to Field Table]"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert48">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[[Back to Field Table]](#heading=h.3sf8crbrgxc)


<table>
  <tr>
   <td><strong>PA Digital Label</strong>
   </td>
   <td>
<h3>Title</h3>


   </td>
  </tr>
  <tr>
   <td><strong>Status</strong>
   </td>
   <td>Required
   </td>
  </tr>
  <tr>
   <td><strong>Description</strong>
   </td>
   <td>A name given to the described resource. Typically, a title will be a name by which the described resource is formally known
   </td>
  </tr>
  <tr>
   <td><strong>Qualified DC Element</strong>
   </td>
   <td>dcterms:title
   </td>
  </tr>
  <tr>
   <td><strong>Simple DC Element </strong>
   </td>
   <td>dc:title
   </td>
  </tr>
  <tr>
   <td><strong>CONTENTdm Mapping</strong>
   </td>
   <td>Title
   </td>
  </tr>
  <tr>
   <td>CSV Header
   </td>
   <td>Title
   </td>
  </tr>
  <tr>
   <td><strong>Repeatable</strong>
   </td>
   <td>No
   </td>
  </tr>
  <tr>
   <td><strong>CV/Syntax</strong>
   </td>
   <td>
<ul>

<li>Natural language; semicolons may be used as punctuation
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Notes and Best Practices</strong>
   </td>
   <td>
<ul>

<li>Keep the title descriptive yet brief. The 

<p id="gdcalert48" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "Description"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert49">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

<a href="#heading=h.6iko3zl5weqn">Description</a> field may be used to provide more detail

<li>Avoid use of explanatory or qualifying symbols (e.g., brackets)

<li>Descriptive and informative titles are preferred whenever possible (as opposed to things like "unknown" or an id number). Not all materials can or should be titled uniquely

<li>If a formal title does not exist, create a contrived title that succinctly describes the item. Refer to content standards such as <a href="https://github.com/saa-ts-dacs/dacs">DACS</a> and <a href="https://www.rdatoolkit.org/">RDA</a> for guidance
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Examples</strong>
   </td>
   <td>
<ul>

<li>1025 South Fairhill Street

<li>Swimsuit parade at Stanley Green's

<li>Senator J. William Fulbright awarded honorary degree, 1983
</li>
</ul>
   </td>
  </tr>
</table>




<p id="gdcalert49" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "[Back to Field Table]"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert50">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[[Back to Field Table]](#heading=h.3sf8crbrgxc)


<table>
  <tr>
   <td><strong>PA Digital Label</strong>
   </td>
   <td>
<h3>Type</h3>


   </td>
  </tr>
  <tr>
   <td><strong>Status</strong>
   </td>
   <td>Recommended
   </td>
  </tr>
  <tr>
   <td><strong>Description</strong>
   </td>
   <td>The nature or genre of the described resource
   </td>
  </tr>
  <tr>
   <td><strong>Qualified DC Element</strong>
   </td>
   <td>dcterms:type
   </td>
  </tr>
  <tr>
   <td><strong>Simple DC Element </strong>
   </td>
   <td>dc:type
   </td>
  </tr>
  <tr>
   <td><strong>CONTENTdm Mapping</strong>
   </td>
   <td>Type
   </td>
  </tr>
  <tr>
   <td>CSV Header
   </td>
   <td>Type
   </td>
  </tr>
  <tr>
   <td><strong>Repeatable</strong>
   </td>
   <td>Yes
   </td>
  </tr>
  <tr>
   <td><strong>CV/Syntax</strong>
   </td>
   <td>
<ul>

<li>Values from the <a href="https://www.dublincore.org/specifications/dublin-core/dcmi-type-vocabulary/">DCMI Type Vocabulary</a> map to PA Digital’s Type field
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Notes and Best Practices</strong>
   </td>
   <td>
<ul>

<li>Assign the type Text to images of textual materials

<li>Please see 

<p id="gdcalert50" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "Format"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert51">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

<a href="#heading=h.or6g2dfj8ekl">Format</a> for additional mappings from our Type field

<li>Use a semicolon to separate multiple values
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td><strong>Examples</strong>
   </td>
   <td>
<ul>

<li>Text

<li>Image

<li>Physical Object

<li>Sound

<li>Moving Image
</li>
</ul>
   </td>
  </tr>
</table>




<p id="gdcalert51" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "[Back to Field Table]"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert52">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[[Back to Field Table]](#heading=h.3sf8crbrgxc)


<table>
  <tr>
   <td><strong>PA Digital Label</strong>
   </td>
   <td>
<h3>URL</h3>


   </td>
  </tr>
  <tr>
   <td><strong>Status</strong>
   </td>
   <td>Required or Derived
   </td>
  </tr>
  <tr>
   <td><strong>Description</strong>
   </td>
   <td>Unambiguous URL reference to the digital object in its local repository
   </td>
  </tr>
  <tr>
   <td><strong>Qualified DC Element</strong>
   </td>
   <td>dcterms:identifier
   </td>
  </tr>
  <tr>
   <td><strong>Simple DC Element </strong>
   </td>
   <td>dc:identifier
   </td>
  </tr>
  <tr>
   <td>CSV Header
   </td>
   <td>URL
   </td>
  </tr>
  <tr>
   <td><strong>Repeatable</strong>
   </td>
   <td>No
   </td>
  </tr>
  <tr>
   <td><strong>Notes and Best Practices</strong>
   </td>
   <td>
<ul>

<li>The URL must resolve to a digital object and its associated metadata record

<li>Values for this field may be mapped from consistently formatted metadata elsewhere in the record
</li>
</ul>
   </td>
  </tr>
</table>



# 


# Appendix A - Changes From Version 1.2



* Updated field mappings and recommendations throughout to conform with PA Digital MAP 2.0
* Standardized and updated language and punctuation throughout
* The following sections were updated:
    * History and Acknowledgements
        * Updated names
    * Introduction
    * Appendix B - Other Resources and Guidelines
    * Appendix D - PA Digital to DPLA Crosswalk


# 


# Appendix B - Other Resources and Guidelines

The Guidelines were greatly informed and influenced by the following documents, prepared by DPLA and their hubs, service providers, and other information professionals:



* DPLA [Metadata Resources](https://pro.dp.la/hubs/documentation), particularly
    * [DPLA Metadata Application Profile](https://drive.google.com/file/d/1fJEWhnYy5Ch7_ef_-V48-FAViA72OieG/view) (v5.0, December 2017)
    * [DPLA Geographic and Temporal Guidelines](https://docs.google.com/document/d/1lfiJ8yoZf1fAoR5vmJoHpWQO63eKeL8HDGVupCocfoM/edit?pref=2&pli=1) (December 2015)
    * [DPLA Metadata Quality Guidelines](https://docs.google.com/document/d/1dITqEYEWsMX1a2pLPmkL78k1LN2b4im03spn8_QFscY/edit) (December 2016)
    * [DPLA Standardized Rights Statements Implementation Guidelines](https://docs.google.com/document/d/1aInokOIIsgf-B4iMTXU33qYN5B2jA3s91KgWoh7DZ7Q/edit) (December 2017)
* [DCMI Metadata Terms](https://www.dublincore.org/specifications/dublin-core/dcmi-terms)
* [Dublin Core Metadata Element Set](http://dublincore.org/documents/dces/) (v1.1, 2012)
* [South Carolina Digital Library Metadata Schema and Guidelines](http://scmemory.org/wp-content/uploads/2016/08/SCDLMetadataSchema_2016.pdf) (July 2016)
* [South Carolina Digital Library Dublin Core Mapping for CONTENTdm Administrators](http://scmemory.org/wp-content/uploads/2014/08/SCDL-DC-Mapping-Guidelines.pdf) (June 2013)
* [Metadata Requirements for DPLA Participation through the North Carolina Service Hub](http://www.digitalnc.org/wp-content/uploads/2014/04/DPLAmetadatarequirements.pdf) (April 2014)
* [Mountain West Digital Library Dublin Core Application Profile](http://mwdl.org/docs/MWDL_DC_Profile_Version_2.0.pdf) (v2.0, July 2011)
* [Empire State Digital Network Metadata Requirements](http://empirestate.digital/contributors/metadata-requirements/)
* [Best Practices for CONTENTdm and other OAI-PMH Compliant Repositories: Creating Sharable Metadata](http://www.oclc.org/content/dam/support/wcdigitalcollectiongateway/MetadataBestPractices.pdf) (v3.1, June 2013)
* [Digital Library Federation (DLF) Best Practices for Shareable Metadata](http://webservices.itcs.umich.edu/mediawiki/oaibp/index.php/ShareableMetadataPublic)
* [Recommendations for Standardized International Rights Statements](http://rightsstatements.org/files/160208recommendations_for_standardized_international_rights_statements_v1.1.pdf) (January 2016)
* [PA Digital Rights Resources](https://padigital.org/rights-resources/), particularly
    * [PA Digital Rights Statement Selection Tool](http://bit.ly/RightsTool)
* [Library of Congress MARC to Qualified Dublin Core crosswalk](https://www.loc.gov/marc/marc2dc.html#qualifiedlist)
* [MARC 21 to MODS 3.6 Mapping](https://www.loc.gov/standards/mods/mods-mapping.html)


## 


# Appendix C - Standards and Controlled Vocabularies Referenced


<table>
  <tr>
   <td><strong>Abbreviation</strong>
   </td>
   <td><strong>Full name</strong>
   </td>
   <td><strong>URL</strong>
   </td>
  </tr>
  <tr>
   <td>AAT
   </td>
   <td>Getty Art & Architecture Thesaurus
   </td>
   <td><a href="http://www.getty.edu/research/tools/vocabularies/aat">http://www.getty.edu/research/tools/vocabularies/aat</a> 
   </td>
  </tr>
  <tr>
   <td>CCO
   </td>
   <td>Cataloging Cultural Objects
   </td>
   <td><a href="http://vraweb.org/resources/cataloging-cultural-objects/">http://vraweb.org/resources/cataloging-cultural-objects/</a>
   </td>
  </tr>
  <tr>
   <td>DCMI
   </td>
   <td>DCMI Type Vocabulary
   </td>
   <td><a href="https://www.dublincore.org/specifications/dublin-core/dcmi-type-vocabulary/">https://www.dublincore.org/specifications/dublin-core/dcmi-type-vocabulary/</a>
   </td>
  </tr>
  <tr>
   <td>DCRM(S)
   </td>
   <td>Descriptive Cataloging of Rare Materials (Serials)
   </td>
   <td><a href="http://rbms.info/dcrm/dcrms/">http://rbms.info/dcrm/dcrms/</a> 
   </td>
  </tr>
  <tr>
   <td>EDTF
   </td>
   <td>Extended Date/Time Format
   </td>
   <td><a href="https://www.loc.gov/standards/datetime/">https://www.loc.gov/standards/datetime/</a>
   </td>
  </tr>
  <tr>
   <td>FAST
   </td>
   <td>Faceted Application of Subject Terminology
   </td>
   <td><a href="http://fast.oclc.org/searchfast/">http://fast.oclc.org/searchfast/</a> 
   </td>
  </tr>
  <tr>
   <td>GeoNames
   </td>
   <td>GeoNames
   </td>
   <td><a href="http://www.geonames.org/">http://www.geonames.org/</a> 
   </td>
  </tr>
  <tr>
   <td>IANA
   </td>
   <td>IANA Media Types
   </td>
   <td><a href="https://www.iana.org/assignments/media-types/media-types.xhtml">https://www.iana.org/assignments/media-types/media-types.xhtml</a> 
   </td>
  </tr>
  <tr>
   <td>ISO 639-3
   </td>
   <td>Codes for the Representation of Names of Languages
   </td>
   <td><a href="https://iso639-3.sil.org/code_tables/639/data">https://iso639-3.sil.org/code_tables/639/data</a> 
   </td>
  </tr>
  <tr>
   <td>LCNAF
   </td>
   <td>Library of Congress Name Authority File
   </td>
   <td><a href="http://id.loc.gov/authorities/names">http://id.loc.gov/authorities/names</a> 
   </td>
  </tr>
  <tr>
   <td>LCSH
   </td>
   <td>Library of Congress Subject Headings
   </td>
   <td><a href="http://id.loc.gov/authorities/subjects.html">http://id.loc.gov/authorities/subjects.html</a> 
   </td>
  </tr>
  <tr>
   <td>RDA
   </td>
   <td>Resource Description & Access
   </td>
   <td><a href="https://www.rdatoolkit.org/">https://www.rdatoolkit.org/</a>
   </td>
  </tr>
  <tr>
   <td>RightsStatements
   </td>
   <td>RightsStatements.org
   </td>
   <td><a href="http://rightsstatements.org/">http://rightsstatements.org/</a>
   </td>
  </tr>
  <tr>
   <td>TGM
   </td>
   <td>Library of Congress Thesaurus for Graphic Materials
   </td>
   <td><a href="http://id.loc.gov/vocabulary/graphicMaterials">http://id.loc.gov/vocabulary/graphicMaterials</a> 
   </td>
  </tr>
  <tr>
   <td>TGN
   </td>
   <td>Getty Thesaurus of Geographic Names
   </td>
   <td><a href="http://www.getty.edu/vow/TGNSearchPage.jsp">http://www.getty.edu/vow/TGNSearchPage.jsp</a> 
   </td>
  </tr>
  <tr>
   <td>ULAN
   </td>
   <td>Getty Union List of Artist Names
   </td>
   <td><a href="http://www.getty.edu/research/tools/vocabularies/ulan/index.html">http://www.getty.edu/research/tools/vocabularies/ulan/index.html</a> 
   </td>
  </tr>
  <tr>
   <td>VIAF
   </td>
   <td>Virtual International Authority File
   </td>
   <td><a href="https://viaf.org/">https://viaf.org/</a>
   </td>
  </tr>
</table>



# Appendix D - PA Digital to DPLA Crosswalk


<table>
  <tr>
   <td><strong>PA Digital Label (Guidelines v1.2)</strong>
   </td>
   <td><strong>PA Digital inbound property (Guidelines v1.2)</strong>
   </td>
   <td><strong>PA Digital Label</strong>
   </td>
   <td><strong>PA Digital inbound property</strong>
   </td>
   <td><strong>PA Digital outbound property</strong>
   </td>
   <td><strong>DPLA label</strong>
   </td>
   <td><strong>DPLA DC class</strong>
   </td>
   <td><strong>DPLA DC property</strong>
   </td>
  </tr>
  <tr>
   <td colspan="2" >NA
   </td>
   <td>Alternative Title
   </td>
   <td>dcterms:alternative
   </td>
   <td>dcterms:alternative
   </td>
   <td>Alternative Title
   </td>
   <td>dpla:SourceResource
   </td>
   <td>dcterms:alternative
   </td>
  </tr>
  <tr>
   <td>Collection Name
   </td>
   <td>supplied
   </td>
   <td>Collection Name
   </td>
   <td>dcterms:isPartOf
   </td>
   <td>dcterms:isPartOf
   </td>
   <td>Collection
   </td>
   <td>dpla:SourceResource
   </td>
   <td>dcterms:isPartOf
   </td>
  </tr>
  <tr>
   <td>Contributing Institution
   </td>
   <td>supplied
   </td>
   <td>Contributing Institution
   </td>
   <td>supplied
   </td>
   <td>edm:dataProvider
   </td>
   <td>Data Provider
   </td>
   <td>ore:Aggregation
   </td>
   <td>edm:dataProvider
   </td>
  </tr>
  <tr>
   <td>Contributor
   </td>
   <td>dcterms:contributor
   </td>
   <td>Contributor
   </td>
   <td>dcterms:contributor
   </td>
   <td>dcterms:contributor
   </td>
   <td>Contributor
   </td>
   <td>dpla:SourceResource
   </td>
   <td>dc:contributor
   </td>
  </tr>
  <tr>
   <td>Coverage
   </td>
   <td>dc:coverage
   </td>
   <td>Place
   </td>
   <td>dcterms:coverage
   </td>
   <td>dcterms:spatial
   </td>
   <td>Place
   </td>
   <td>dpla:SourceResource
   </td>
   <td>dcterms:spatial
   </td>
  </tr>
  <tr>
   <td>Coverage
   </td>
   <td>dcterms:spatial
   </td>
   <td>Place
   </td>
   <td>dcterms:spatial
   </td>
   <td>dcterms:spatial
   </td>
   <td>Place
   </td>
   <td>dpla:SourceResource
   </td>
   <td>dcterms:spatial
   </td>
  </tr>
  <tr>
   <td>Creator
   </td>
   <td>dc:creator
   </td>
   <td>Creator
   </td>
   <td>dcterms:creator
   </td>
   <td>dcterms:creator
   </td>
   <td>Creator
   </td>
   <td>dpla:SourceResource
   </td>
   <td>dcterms:creator
   </td>
  </tr>
  <tr>
   <td>Date
   </td>
   <td>dc:date
   </td>
   <td>Date
   </td>
   <td>dcterms:date
   </td>
   <td>dcterms:date
   </td>
   <td>Date
   </td>
   <td>dpla:SourceResource
   </td>
   <td>dc:date
   </td>
  </tr>
  <tr>
   <td><del>Date</del>
   </td>
   <td><del>dcterms:created</del>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td><del>Date</del>
   </td>
   <td><del>dpla:SourceResource</del>
   </td>
   <td><del>dc:date</del>
   </td>
  </tr>
  <tr>
   <td><del>Date</del>
   </td>
   <td><del>dcterms:issued</del>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td><del>Date</del>
   </td>
   <td><del>dpla:SourceResource</del>
   </td>
   <td><del>dc:date</del>
   </td>
  </tr>
  <tr>
   <td>Description
   </td>
   <td>dc:description
   </td>
   <td>Description
   </td>
   <td>dcterms:description
   </td>
   <td>dcterms:description
   </td>
   <td>Description
   </td>
   <td>dpla:SourceResource
   </td>
   <td>dc:description
   </td>
  </tr>
  <tr>
   <td colspan="2" >NA
   </td>
   <td>Extent
   </td>
   <td>dcterms:extent
   </td>
   <td>dcterms:extent
   </td>
   <td>Extent
   </td>
   <td>dpla:SourceResource
   </td>
   <td>dcterms:extent
   </td>
  </tr>
  <tr>
   <td>Format
   </td>
   <td>dc:format
   </td>
   <td>File Format
   </td>
   <td>dcterms:format
   </td>
   <td>schema:fileFormat
   </td>
   <td>File Format
   </td>
   <td>edm:WebResource
   </td>
   <td>dc:format
   </td>
  </tr>
  <tr>
   <td colspan="2" >NA
   </td>
   <td>IIIF Base URL
   </td>
   <td>dcterms:identifier
   </td>
   <td>svcs:hasService
   </td>
   <td>IIIF Base URL
   </td>
   <td>edm:WebResource
   </td>
   <td>svcs:hasService
   </td>
  </tr>
  <tr>
   <td colspan="2" >NA
   </td>
   <td>IIIF Manifest
   </td>
   <td>dcterms:isReferencedBy
   </td>
   <td>dcterms:isReferencedBy
   </td>
   <td>IIIF Manifest
   </td>
   <td>edm:WebResource
   </td>
   <td>dcterms:isReferencedBy
   </td>
  </tr>
  <tr>
   <td>Identifier
   </td>
   <td>dc:identifier
   </td>
   <td>URL
   </td>
   <td>dcterms:identifier
   </td>
   <td>edm:isShownAt
   </td>
   <td>Is Shown At
   </td>
   <td>ore:Aggregation
   </td>
   <td>edm:isShownAt
   </td>
  </tr>
  <tr>
   <td>Identifier
   </td>
   <td>dc:identifier
   </td>
   <td>Preview
   </td>
   <td>dcterms:identifier
   </td>
   <td>edm:preview
   </td>
   <td>Preview
   </td>
   <td>ore:Aggregation
   </td>
   <td>edm:preview
   </td>
  </tr>
  <tr>
   <td>Intermediate Provider
   </td>
   <td>supplied
   </td>
   <td>Intermediate Provider
   </td>
   <td>supplied
   </td>
   <td>dpla:intermediateProvider
   </td>
   <td>Intermediate Provider
   </td>
   <td>ore:Aggregation
   </td>
   <td>dpla:intermediateProvider
   </td>
  </tr>
  <tr>
   <td>Language
   </td>
   <td>dc:language
   </td>
   <td>Language
   </td>
   <td>dcterms:language
   </td>
   <td>dcterms:language
   </td>
   <td>Language
   </td>
   <td>dpla:SourceResource
   </td>
   <td>dc:language
   </td>
  </tr>
  <tr>
   <td>Publisher
   </td>
   <td>dc:publisher
   </td>
   <td>Publisher
   </td>
   <td>dcterms:publisher
   </td>
   <td>dcterms:publisher
   </td>
   <td>Publisher
   </td>
   <td>dpla:SourceResource
   </td>
   <td>dc:publisher
   </td>
  </tr>
  <tr>
   <td>Relation
   </td>
   <td>dc:relation
   </td>
   <td>Relation
   </td>
   <td>dcterms:relation
   </td>
   <td>dcterms:relation
   </td>
   <td>Relation
   </td>
   <td>dpla:SourceResource
   </td>
   <td>dc:relation
   </td>
  </tr>
  <tr>
   <td colspan="2" >NA
   </td>
   <td>Replaced By
   </td>
   <td>dcterms:isReplacedBy
   </td>
   <td>dcterms:isReplacedBy
   </td>
   <td>Replaced By
   </td>
   <td>dpla:SourceResource
   </td>
   <td>dpla:isReplacedBy
   </td>
  </tr>
  <tr>
   <td colspan="2" >NA
   </td>
   <td>Replaces
   </td>
   <td>dcterms:replaces
   </td>
   <td>dcterms:replaces
   </td>
   <td>Replaces
   </td>
   <td>dpla:SourceResource
   </td>
   <td>dpla:replaces
   </td>
  </tr>
  <tr>
   <td>Rights
   </td>
   <td>dc:rights
   </td>
   <td>Rights
   </td>
   <td>dcterms:rights
   </td>
   <td>dcterms:relation
   </td>
   <td>Rights
   </td>
   <td>dpla:SourceResource
   </td>
   <td>dc:rights
   </td>
  </tr>
  <tr>
   <td>Rights
   </td>
   <td>dc:rights
   </td>
   <td>Rights URI
   </td>
   <td>dcterms:rights
   </td>
   <td>edm:rights
   </td>
   <td>Rights Statement
   </td>
   <td>edm:WebResource
   </td>
   <td>edm:rights
   </td>
  </tr>
  <tr>
   <td colspan="2" >NA
   </td>
   <td>Rights Holder
   </td>
   <td>dcterms:rightsholder
   </td>
   <td>dcterms:rightsholder
   </td>
   <td>Rights Holder
   </td>
   <td>dpla:SourceResource
   </td>
   <td>dcterms:rightsholder
   </td>
  </tr>
  <tr>
   <td><del>Source</del>
   </td>
   <td><del>supplied</del>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td><del>Contributing Institution</del>
   </td>
   <td><del>ore:Aggregation</del>
   </td>
   <td><del>dpla:intermediateProvider</del>
   </td>
  </tr>
  <tr>
   <td colspan="2" >NA
   </td>
   <td>Source
   </td>
   <td>dcterms:source
   </td>
   <td>dcterms:source
   </td>
   <td colspan="3" >Not mapped
   </td>
  </tr>
  <tr>
   <td>Subject
   </td>
   <td>dc:subject
   </td>
   <td>Subject
   </td>
   <td>dcterms:subject
   </td>
   <td>dcterms:subject
   </td>
   <td>Subject
   </td>
   <td>dpla:SourceResource
   </td>
   <td>dc:subject
   </td>
  </tr>
  <tr>
   <td>Subject
   </td>
   <td>dc:subject
   </td>
   <td>Temporal Coverage
   </td>
   <td>dcterms:temporal
   </td>
   <td>dcterms:temporal
   </td>
   <td>Temporal Coverage
   </td>
   <td>dpla:SourceResource
   </td>
   <td>dcterms:temporal
   </td>
  </tr>
  <tr>
   <td>Title
   </td>
   <td>dc:title
   </td>
   <td>Title
   </td>
   <td>dcterms:title
   </td>
   <td>dcterms:title
   </td>
   <td>Title
   </td>
   <td>dpla:SourceResource
   </td>
   <td>dc:title
   </td>
  </tr>
  <tr>
   <td>Type
   </td>
   <td>dc:type
   </td>
   <td>Type
   </td>
   <td>dcterms:type
   </td>
   <td>dcterms:type
   </td>
   <td>Type
   </td>
   <td>dpla:SourceResource
   </td>
   <td>dc:type (where value = DCMI Type)
   </td>
  </tr>
  <tr>
   <td>Type
   </td>
   <td>dc:type
   </td>
   <td>Format
   </td>
   <td>dcterms:type
   </td>
   <td>dcterms:format
   </td>
   <td>Format
   </td>
   <td>dpla:SourceResource
   </td>
   <td>dc:format
   </td>
  </tr>
</table>


_*Cells highlighted in yellow reflect updates to PA Digital MAP that may affect current mapping configurations_
