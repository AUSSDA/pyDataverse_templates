
# AUSSDA pyDataverse templates

AUSSDA specific templates for [pyDataverse](https://github.com/AUSSDA/pyDataverse).


**Copyright**

* Open Source ([MIT](https://opensource.org/licenses/MIT))

## CSV

This template files offer a first starting-point to collect data for later imports via the Dataverse API. They contain some pre-defined attributes in the first row, which are the used ones from the Dataverse API and by AUSSDA internally. The attributes are described in the 2nd and 3rd row. Additional attributes can be added as needed.

Format
* Seperator: `;`

Rows:
* First row: Attribute name for the column. Often the same one as the one needed for
* Second row: Type of data [serial, string, numeric]. For strings, also valid JSON strings can be used to be able to use more complex data-types, as you can see in the examples offered.
* Third row: Category of data. [aussda, dataverse, dataverse.METADATA_TYPE]
* Fourth row and higher: The data entries itself.

Columns:
* The templates include columns for each Dataverse API metadata attribute.

**Dataverses**

**Datasets**

**Datafiles**
