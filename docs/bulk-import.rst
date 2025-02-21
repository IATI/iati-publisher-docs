###################
Bulk data import
###################

IATI Publisher allows you to import and export activity data in three file formats (XML, CSV and XLS). This functionality can be useful if you want to import multiple activities, transactions, budgets or results in one go.

For importing via CSV or XLS, it is normally easiest to export your activity data first, make edits to the activity file, then re-import the data.

.. caution::

   IATI Publisher will overwrite your data in the interface if you upload data for an existing activity. Activity identifiers are checked on import to assess whether the activity is new or existing, and you will have the option to review this on a summary screen prior to import. Be careful to avoid data loss caused by this overwriting.

Import via XML
---------------
XML is the file format used by the IATI Standard. IATI Publisher creates and stores IATI XML files for you when you publish your activity and organisation data from the interface. The XML import functionality may be useful if you are transferring IATI data from a different publishing tool to IATI Publisher.


Import via CSV
--------------
You can download the IATI Publisher CSV template from the `CSV/XML data import page <https://publisher.iatistandard.org/import>`_. This template contains a wide range of IATI Standard fields and it is not necessary to populate everything. Refer to IATI Standard guidance on how to interpret the fields. 

Note: it is not possible to upload activity results, indicators or periods via the CSV import.


Import via XLS
--------------
You can find templates and further guidance for XLS file imports on the `XLS import page <https://publisher.iatistandard.org/import/xls>`_.


Pre-import checks
---------------
Once you have uploaded your data, IATI Publisher will list the activities ready for import with information on any data validation errors. These errors are from the `IATI Validator <https://validator.iatistandard.org/>`_.

Critical errors prevent the activity from being imported, whereas other errors will not prevent import. It is usually easier to fix errors in your data file before importing, rather than after in the interface.


