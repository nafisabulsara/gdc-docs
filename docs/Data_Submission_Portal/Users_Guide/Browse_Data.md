# Browse Data

## Overview

The _"Browse"_ menu provides access to all of a project's content. Most content is driven by the GDC Data Dictionary and the interface is dynamically generated to accommodate the content.

Please refer to the [GDC Data Dictionary Viewer](../../Data_Dictionary/viewer.md) for specific details about dictionary-generated fields, columns, and filters.

[![GDC Submission Cases Default View](images/GDC_Submission_Cases_Default_2.png)](images/GDC_Submission_Cases_Default_2.png "Click to see the full image.")

## Main Interface Elements

### Filters

A wide set of filters are available for the user to select the type of entity to be displayed. These filters are dynamically created based on the [GDC Data Dictionary](../../Data_Dictionary/index.md).

Current filters are:

|Filter|Description|
| --- | --- |
| __Cases__ | Display all cases associated with the project. |
| __Clinical Entities__ | Display all clinical data uploaded to the project workspace. This is divided into subgroups including demographics, diagnoses, exposures, family histories, and treatments. |
| __Biospecimen Data__ | Display all biospecimen data uploaded to the project workspace. This is divided into subgroups including samples, portions, analytes, aliquots, and read-groups. |
| __Submittable Data Files__ | Displays all data files that have been registered with the project. This includes files that have and have not been uploaded. This category is divided into groups by file type. |
| __Annotations__ | Lists all annotations associated with the project. An annotation provides an explanatory comment associated with data in the project. |


### List View

The list view is a paginated list of all entities corresponding to the selected filter.

On the top-right section of the screen, the user can download data about all entities associated with the selected filter.

* For the case filter, it will download all clinical data.
* For all other filters, it will download the corresponding metadata (e.g., for the demographic filter, it will download all demographic data).

[![GDC Submission Case Summary Download](images/GDC_Submission_Cases_Summary_Download_2.png)](images/GDC_Submission_Cases_Summary_Download_2.png "Click to see the full image.")



### Details Panel

Clicking on a case will open the details panel. Data in this panel is broken down into multiple sections depending on the entity type. The main sections are:

* Actions: actions that can be performed relating the entity. This includes downloading the metadata (JSON or TSV) or submittable data file pertaining to the entity.  
* Summary: IDs and system properties associated with the entity.
* Details: properties of the entity (not associated with cases).
* Hierarchy or Related Entities: list of associated entities.
* Annotations: annotations on the entity.
* Transactions: transactions that affect the entity.

[![GDC Submission Case Details](images/GDC_Submission_Cases_Details_2.png)](images/GDC_Submission_Cases_Details_2.png "Click to see the full image.")

Navigation between those sections can be done either by scrolling down or by clicking on the section icon on the left side of the details panel.

#### Related Entities

Table listing all entities, grouped by type, related to the selected case.
This section is available only at the case level.

[![GDC Submission Cases Related Entities](images/GDC_Submission_Cases_Summary_Related_Entities_2.png)](images/GDC_Submission_Cases_Summary_Related_Entities_2.png "Click to see the full image.")


This table contains the following columns:

* Category: category of the entity (clinical, biospecimen, submittable data file).
* Type: type of entity (based on Data Dictionary).
* Count: number of occurrences of an entity associated with the case. Clicking on the count will open a window listing those entities within the Browse page.

#### Hierarchy

The hierarchy section is available for entities at any level (e.g., Clinical, Biospecimen, etc.), except for Case.

The hierarchy shows:

* The Case associated with the entity.
* The __direct__ parents of the entity.
* The __direct__ children of the entity.


[![GDC Submission Cases Details Hierarchy](images/GDC_Submission_Cases_Summary_Hierarchy_2.png)](images/GDC_Submission_Cases_Summary_Hierarchy_2.png "Click to see the full image.")

Using the hierarchy, the user can navigate through entities.
