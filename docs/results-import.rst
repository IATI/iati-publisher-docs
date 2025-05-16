###################
How do I import results data?
###################

Activity results data can be imported to IATI Publisher via XLSX files. There is a separate XLSX template to use for each of results, indicators and periods.

Instead of populating the blank XLSX templates, it is typically easiest to add at least one result, indicator and period via IATI Publisher's interface first. This way, you can `export your existing activity data <https://docs.publisher.iatistandard.org/en/latest/bulk-import/#exporting-your-existing-data>`_ and see how it appears in each of IATI Publisher's XLSX templates. You can then add to or edit the data as required, before re-importing. 

What information do I need in the import templates?
-----------------

1) Result template
""""""""""""""""""
The *Result_Mapper* sheet contains the following three columns:

- **Activity Identifier** - this is used to associate your result with the right activity in IATI Publisher. The activity identifier is the second part of the 'iati-identifier' string, which uniquely identifies each of your activities within your organisation's data.
- **Result Number** - a number or text string that uniquely identifies each result within a particular activity. You can choose what this string is if creating a new result via the import template. Results created within the IATI Publisher interface will have their result number automatically created by the system.
- **Result Identifier** - this is autopopulated in the Result import template, based on the Activity Identifier and Result Number entered in the previous columns.

2) Indicator template
""""""""""""""""""
The *Indicator_Mapper* sheet contains the following three columns:

- **Result Identifier** - this is used to associate your indicator with the right result in IATI Publisher.
- **Indicator Number** - a number or text string that uniquely identifies each indicator within a particular result (similar to Result Number).
- **Indicator Identifier** - this is autopopulated in the Indicator import template, based on the Result Identifier and Indicator Number entered in the previous columns.

3) Period template
""""""""""""""""""
The *Period_Mapper* sheet contains the following three columns:

- **Indicator Identifier** - this is used to associate your period with the right indicator in IATI Publisher.
- **Period Number** - a number or text string that uniquely identifies each period within a particular indicator (similar to Indicator Number).
- **Period Identifier** - this is autopopulated in the Period import template, based on the Indicator Identifier and Period Number entered in the previous columns.


