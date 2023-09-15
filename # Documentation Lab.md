# Documentation Lab
## Instructions
In this lab, we'll practice reading documentation and looking for answers to our questions in the following documentation sources:
1. [CollectionBuilder documentation](https://collectionbuilder.github.io/cb-docs/)
2. [SUCHO documentation](https://wiki.sucho.org/en/tutorials/internet-archive/spreadsheet-metadata-template)
3. [Alex's TEI guidelines for archival transcription](https://alexandraewingate.com/projects/encoding-guidelines-for-initial-archival-tei-transcription/)

Answer the following questions using the documentation above. Turn in your completed Markdown file to the assignment on Canvas.
## Collection Builder
***For all answers in this section, give the answer and the URL of the page where you found it.***

1. **Which fields are required for *all items* in CollectionBuilder-GH metadata?**  
objectid, filename, title, and format (https://collectionbuilder.github.io/cb-docs/docs/metadata/gh_metadata/)
2. **What file do you need to edit to add a new page to your navigation bar?**  
You should edit the "config-nav.csv” file to add a new page to your navigation bar. (https://collectionbuilder.github.io/cb-docs/docs/pages/add_page/) 
3. **What metadata fields are required to support the map visualization in CollectionBuilder-GH metadata?**  
The latitude and longitude are required for map visualization (https://collectionbuilder.github.io/cb-docs/docs/metadata/gh_metadata/)
4. **What four columns are included in the config-metadata.csv file?**  
Field, display_name, browse_link, and external_link (https://collectionbuilder.github.io/cb-docs/docs/customization/config-metadata/#metadata--item-page-configuration-config-metadatacsv)
5. **If you wanted a metadata field called "archive" in your metadata field to display as "Holding Institution" in the metadata section of each item's page, what file would you edit? (Bonus point: what columns of that file would you edit and what text would you input in each column?)**  
“_data/config-metadata.csv” if you want to update the metadata field (https://collectionbuilder.github.io/cb-docs/docs/customization/config-metadata/#metadata--item-page-configuration-config-metadatacsv). In the row that is for the field called "archive" you should update the display name field to say "holding institution".
6. **How should the date September 8, 2023 be formatted so that the timeline visualization works?**  
Dates should be written in the yyyy-mm-dd format to work with timeline visualization (https://collectionbuilder.github.io/cb-docs/docs/metadata/gh_metadata/#fields-required-for-visualizations)
7. **What column in what file allows you determine whether a field can be used for sorting on the Browse page of your website?**  
The sort_name column in the _data/config-browse.csv file is what can be updated to set whether or not a field is able to be used to sort on the Browse page (https://collectionbuilder.github.io/cb-docs/docs/customization/config-browse/#browse-page-configuration-config-browsecsv)
8. **How do you change which metadata fields contribute values to the "Subjects" visualization page?**  
(https://collectionbuilder.github.io/cb-docs/docs/theme/subjects/)
9. **What three items (keys) are in the YAML front matter of any of the markdown page files?**  
Title, layout, permalink (https://collectionbuilder.github.io/cb-docs/docs/pages/basics/)
10. **When filling in "metadata: " with the name of your metadata sheet on your "\_config.yml" file, should you include the file extension?**  
No. (https://collectionbuilder.github.io/cb-docs/docs/config/collection/)
11. **Which file controls the display options for most of your website?**  
The "_data/theme.yml” file controls the display options. (https://collectionbuilder.github.io/cb-docs/docs/theme/)
12. **How can you separate multiple values in a single field in your metadata file?**  
You can use a semicolon to separate multiple values in a single field. (https://collectionbuilder.github.io/cb-docs/docs/metadata/formatting/)
13. **Find the example code for including a PDF from your collection (with a caption) on one of your interpretive pages (hint: start with the "Feature Includes" page)**  
{% include feature/pdf.html objectid="demo_002" width="50" caption="a pdf from the collection" %} (https://collectionbuilder.github.io/collectionbuilder-gh/feature_options.html)
## SUCHO Metadata
1. **Which metadata fields are always required for a SUCHO item?**  
Progress, Claimed by, Title, Identifier, Subject Headings, Original Subject Headings (if present), Creator (if present), Date (if present), Language (if applicable), Source URL, Host Institution, Host Location, Original Description (if present) and Description are all required. 
2. **What character separates multiple values in Column E and Column F?**  
Semi-colons separate multiple values.
3. **Format the name "Yevhen Federovych Stankovych" according to the content guidelines for Creator**  
Stankovych, Yevhen Federovych
4. **What is the cardinality of the field "date?""**  
Year should be displayed first, followed by month, and then day (e.g. YYYY-MM-DD). The "date" field should be entered as the date the item was originally created/published (if a poster was printed in 1890 that date would be listed as 1890 and not 2023 when the record was created).
5. **What would be the correctly formatted value for the field "Host Location" for an item held by an institution in Lviv, the capital of Ukraine's Lviv Oblast?**
 Lviv (Q36036)
6. **If you wanted to indicate that you were working on a row in our metadata spreadsheet, how would you do that?**
You would type your name into Column B, the Claimed by field.  

## Alex's TEI guidelines
1. **What tag should be used to indicate deleted text?**  
You should use the `<del>` tag to indicated deleted text. Text should be surrounded by the tag.
2. **When should `<damage>` be used instead of `<gap>`?**  
`<damage>` should be used when the text is still readable but there has been physical damange to the item. `<gap>` should be used when there is a section of the text isn't readable for a variety of reasons (including damage). 
3. **How would you indicate that a word is repeated in the following code block?**
```xml
<p>
The quick brown fox jumped over the the lazy dog.
</p>
```  
You should add <sic @rend="repeated word"> before the repeated word and then <sic> after the repeated word.  
 
4. **Which tag is used to enclose an entire list of non-book items and which tag is used to enclose a list of books? Which tag should be used to enclose an individual non-book item, and which tag should enclose an individual book item?**  
You should use `<list>` and `<item>` to enclose a list of non-book items and you should use `<listBibl>` and then each item inside a `<bibl>` for a list of book items. I'm a little confused about this because it looks like you use the same tag for individual non-book items as you use for a list of non-book items and the same tag for individual book items that you use for a list of book items, but I could be misreading the documentation?
