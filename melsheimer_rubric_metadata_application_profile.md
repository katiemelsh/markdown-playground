# Rubric: Metadata Application Profile
## Checklist of items
### Description of context, content, and users
- Fully describes context, content, and users
    - Good. More context might be the popularity of subscriptions and special signed copies in the 21st century.
- Lists specific functional requirements
    - Good
- Clear connection between metadata elements (fields) and functional requirements
    - Good
  
### Documentation of elements
- Includes all required CollectionBuilder elements
    - missing objectid and format (the format where the value is mime-type. Your format field could be called type, but I also don't think you really need it since all the items are books. It's redundant.)
- Includes at least two CollectionBuilder visualization elements
    - Assuming that genre is equivalent to subject for visualization. Note that in your metadata CSV, genre will have to be called "subject" to make the visualization work (or you can change what fields feed into the subject visualization), but you can have it display as "Genre" on each item page.
- Includes any applicable optional Collection Builder elements
    - You probably want to include a rightsstatement/rights. Description is also probably helpful. 
- Includes at least one new custom element
    - Yes
- For each element, the following are specified:
  - cardinality
  - obligation
  - content guidelines
  - (if relevant) applicable controlled vocabularies or syntax encoding schemes (must have link)
  - mapping to Dublin Core
  - example(s)
  - notes (if relevant)

## Overall factors
- **Includes all assignment components**: Each component of the assignment is present and complete. (40 points)
    - Missing some metadata elements. Missing cardinality for all and DC mapping for some.
- **Coherent design**: There is a clear connection between context, content, users, functional requirements, and the metadata elements chosen. The chosen elements and choices for cardinality, obligation, controlled vocabularies, syntax encoding schemes, and/or content guidelines facilitate the stated functional requirements. (40 points)
    - Overall good. I think there are some additional fields that I mention above that would enrich the metadata overall. 
- **Documentation**: Complete, informative, and logical documentation for individual metadata elements. Each element is fully documented with information about obligation, cardinality, and relevant vocabulary, syntax, and content standards and guidelines. Examples relevant to your collection are included for each element. (40 points)
    - Good documentation, but you are missing cardinality and DC mapping.
- **Structure and organization**: Application profile has a strong and clear organization; appropriate use of headings; typography is used to aid readability; appropriate use of tables and lists; links to various standards are included and working. (40 points)
    - organization is good, and structure is readable.
- **Mechanics**: Very few or no sentence-level errors in expression, grammar, spelling, citations (40 points)

**200 points total**
