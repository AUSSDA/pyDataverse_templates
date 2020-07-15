
# AUSSDA pyDataverse templates

AUSSDA specific templates for [pyDataverse](https://github.com/AUSSDA/pyDataverse).


**Copyright**

* Open Source ([MIT](https://opensource.org/licenses/MIT))

## DESCRIPTION

This template files offer a first starting-point to collect data for later imports via the Dataverse API. They contain some pre-defined attributes in the first row, which are the used ones from the Dataverse API and by AUSSDA internally. The attributes are described in the 2nd and 3rd row. Additional attributes can be added as needed.

Format:
* Seperator: `,`
* Encoding: `utf-8`
* Quotation: `"`

Rows:
* Column names (1st row): Here stands the attribute name for each column. Mostly, it's Dataverse metadata or organization specific data. But you can add or remove columns as you want, as you can read below.
* Description (2nd row): Describes the type of data [`serial`, `string`, `numeric`]. Strings can also be valid JSON strings to use more complex relations. This row is for support, and must be deleted before useage.
* Attribute type (3rd row): Describes the type of the attribute. This is just a supportive/descriptive row the template users. This row is for support, and must be deleted before useage.
* `org`: organization specific data
* `dv`: Dataverse metadata, with specific metadatablock attribute-name added after point denominator.
* `alma`: ALMA specific metadata

## USAGE

1. Save the file: The easiest and most intuitive way to work with the templates, is to first open the template and save it somewhere under a new, descriptive filename (`e.g. datasets_20200117.csv`).
2. Update columns: The pre-defined columns are only a first offer. You can remove columns, which you don't need, or add new ones as you want.
3. Add rows: Then you should start to enter new data entries after the third row - each row one entry. If you use JSON, pay attention to escape the quotation character `"` --> `\"`. You can keep the 2nd and 3rd row for this as long as you need the information inside to create proper data entries and as long as you don't use the file for further steps, where they could be handled inadequately by humans or machines. Once you know how to enter rows, simply delete the 2nd and 3rd row, so you only have a header row and data entries.
4. Remove supportive rows: Once you feel used to the workflow with the data-structure, you can delete the supportive rows 2 to 4. This must be done at least before you use the template for pyDataverse.

## DATA SOURCES

* Dataverses Example: Data taken from [dataverse_full.json](https://github.com/AUSSDA/pyDataverse/blob/master/tests/data/dataverse_full.json)
* Datasets Example: Data taken from [dataset_full.json](https://github.com/AUSSDA/pyDataverse/blob/master/tests/data/dataset_full.json)
* Datafiles Example: Data taken from [Native API documentation](http://guides.dataverse.org/en/latest/api/native-api.html#add-a-file-to-a-dataset)
