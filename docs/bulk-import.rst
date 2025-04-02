###################
Bulk data import
###################

IATI Publisher allows you to import and export activity data in three file formats (XML, CSV and XLS). This functionality can be useful if you want to import multiple activities, transactions, budgets or results in one go.

For importing via CSV or XLS, it is normally easiest to export your activity data first, make edits to the activity file, then re-import the data.

**Example:** `How do I upload transactions in bulk? <https://docs.publisher.iatistandard.org/en/latest/import-transactions/>`_

.. caution::

   IATI Publisher will overwrite your data in the interface if you upload data for an existing activity. Activity identifiers are checked during import to assess whether you are importing a new or updating an existing activity. You will have the option to review this on a summary screen prior to import. Be careful to avoid data loss when your existing activities are overwritten.

Importing your data file
================

You can access the data import pages from 'Add or Import Activity' in IATI Publisher's header. Select the file format from the dropdown menu that you wish to use:

.. figure:: images/dropdown-import-options.png
    :width: 100 %
    :align: center
    :alt: A screenshot of the dropdown header menu, which allows the user to select whether they want to add activity data manually, via XML/CSV, or via XLSX file.

All three file formats require complete activities to be uploaded (i.e. activities that include all mandatory elements according to the IATI Standard). 

New activities will be added to your list of activities in IATI Publisher. Existing activities (based on the activity identifier) will be overwritten.

Import via XML
""""""""""""""""""
XML is the file format used by the IATI Standard. IATI Publisher creates and stores IATI XML files for you when you publish your activity and organisation data from the interface. The XML import functionality may be useful if you are transferring IATI activity data from a different publishing tool to IATI Publisher.


Import via CSV
""""""""""""""""""
You can download the IATI Publisher CSV template from the `CSV/XML data import page <https://publisher.iatistandard.org/import>`_. This template contains a wide range of IATI Standard fields and it is not necessary to populate everything. Refer to IATI Standard guidance on how to interpret the fields. 

.. note:: 
   It is not possible to upload results, indicators or periods for your activities via the CSV import. Use the XLSX import functionality instead.


Import via XLSX
""""""""""""""""""
You can find templates and further guidance for XLSX file imports on the `XLSX import page <https://publisher.iatistandard.org/import/xls>`_.

There are four templates available:
1. Basic Activity Data
2. Results
3. Indicators
4. Periods

If you are not publishing results data, you will only need to use the 'Basic Activity Data' template.


Pre-import checks
================
Once you have uploaded your data, IATI Publisher will list the activities ready for import with information on any data validation errors. These errors are from the `IATI Validator <https://validator.iatistandard.org/>`_.

Critical errors prevent the activity from being imported, whereas other errors will not prevent import. It is usually easier to fix errors in your data file before importing, rather than after in the interface.

You will have the chance to confirm the activities that you want to add or overwrite on the 'Import Activity' page:

.. figure:: images/upload-existing-activity.png
    :width: 100 %
    :align: center
    :alt: The 'Import Activity' screen allows you to confirm which activities you want to add or update.

.. toctree::
    :hidden:
    :titlesonly:
    :maxdepth: 3

    import-transactions
