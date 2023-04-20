# HINQ302_assessment_02
Raw tidied data from migrant dataset
An initial visual inspection identified the lack of clarity and units of measurement in headers, formatting errors, data that was not discrete and no unique record identifier.

The following steps were used to clean the data using faceting, cell transforms and GREL expressions:

1.  headers were renamed (edit column -- rename this column) to reduce ambiguity and include a unit of measurement, where applicable.

2.  a unique identifier column was added (edit column -- add column based on this column) for identification of individual records.[

3.  each variable was examined using the 'text facet' to identify standardisation issues. The 'date' variable was standardised into a single format; the mix of words and numerals in the 'age' variable were changed to numerals; and misspellings in the 'gender' and 'race' variables were corrected. 'None' was retained as an occupation category under the assumption that it referred to no occupation.

4.  ambiguity was removed from the 'age' variable for standardisation based on logical assumption with an explanation provided in a new 'comment_data_and_sources' column.

5.  inconsistencies in case were corrected in the 'occupation', 'gender' and 'name' variables using transforms (edit cells -- common transforms - to lower case). All words were put in lower case to standardise for case sensitive analyses.

6.  the 'name' and 'date' variables containing data that was not discrete were transformed into separate columns for machine readability (edit column - split into several columns).

7.  the variables 'age' and deck' containing numerical data were converted from text data using the 'numeric facet' feature.
