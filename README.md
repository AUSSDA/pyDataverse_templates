
# AUSSDA pyDataverse templates

AUSSDA specific templates for [pyDataverse](https://github.com/AUSSDA/pyDataverse).


**Copyright**

* Open Source ([MIT](https://opensource.org/licenses/MIT))

## CSV

This template files offer a first starting-point to collect data for later imports via the Dataverse API. They contain some pre-defined attributes in the first row, which are the used ones from the Dataverse API and by AUSSDA internally. The attributes are described in the 2nd and 3rd row. Additional attributes can be added as needed.

Format:
* Seperator: `;`
* Encoding: `utf-8`
* Seperator: `"`

Rows:
* Header / First row: Here stands the attribute name for each column. Mostly, it's Dataverse API metadata or AUSSDA specific attribute names. But you can add or remove as you want, as you can read below.
* Second row: Describes the type of data [serial, string, numeric]. For strings, also valid JSON strings can be used to be able to use more complex data-types, as you can see in the examples offered. This is just a supportive/descriptive row the template users.
* Third row: Describes the category of data [aussda, dataverse, dataverse.METADATA_TYPE]. This is just a supportive/descriptive row the template users.

Columns:
* The templates include columns for each Dataverse API metadata attribute.

Application:
1. Save the file: The easiest and most intuitive way to work with the templates, is to first open the template and save it somewhere under a descriptive filename.
2. Adapt columns: The pre-defined columns are only a first offer, which consist of all Dataverse API attributes and AUSSDA specific metadata. You can remove columns, which you don't need, or add new ones as you want.
3. Adapt rows: Then you should start to enter new data entries after the third row - each row one entry. You can keep the 2nd and 3rd row for this as long as you need the information inside to create proper data entries and as long as you don't use the file for further steps, where they could be handled inadequately by humans or machines. Once you know how to enter rows, simply delete the 2nd and 3rd row, so you only have a header row and data entries.

**Dataverses Template**

**Datasets Template**

**Datafiles Template**

### Examples

**Dataverses Example**

Data taken from [dataverse_full.json](https://github.com/AUSSDA/pyDataverse/blob/master/tests/data/dataverse_full.json).

**Datasets Example**

Data taken from [dataset_full.json](https://github.com/AUSSDA/pyDataverse/blob/master/tests/data/dataset_full.json).

**Datafiles Example**

Data taken from [Native API documentation](http://guides.dataverse.org/en/latest/api/native-api.html).
