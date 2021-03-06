---
title: "Integration Services Transformations | Microsoft Docs"
ms.custom: ""
ms.date: "03/09/2017"
ms.prod: "sql-server-2014"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "integration-services"
ms.tgt_pltfrm: ""
ms.topic: conceptual
helpviewer_keywords: 
  - "transformations [Integration Services], listed"
  - "transformations [Integration Services], types"
  - "transformations [Integration Services]"
  - "data flow [Integration Services], transformations"
  - "business intelligence transformations [Integration Services]"
  - "join transformations"
  - "split transformations [Integration Services]"
  - "custom transformations [Integration Services]"
  - "row transformations [Integration Services]"
  - "rowset transformations [Integration Services]"
ms.assetid: c70c4f6e-82dd-4948-b923-fd5193f67f7e
caps.latest.revision: 55
author: "douglaslMS"
ms.author: "douglasl"
manager: craigg
---
# Integration Services Transformations
  [!INCLUDE[ssNoVersion](../../../includes/ssnoversion-md.md)] [!INCLUDE[ssISnoversion](../../../includes/ssisnoversion-md.md)] transformations are the components in the data flow of a package that aggregate, merge, distribute, and modify data. Transformations can also perform lookup operations and generate sample datasets. This section describes the transformations that [!INCLUDE[ssISnoversion](../../../includes/ssisnoversion-md.md)] includes and explains how they work.  
  
## Business Intelligence Transformations  
 The following transformations perform business intelligence operations such as cleaning data, mining text, and running data mining prediction queries.  
  
|Transformation|Description|  
|--------------------|-----------------|  
|[Slowly Changing Dimension Transformation](slowly-changing-dimension-transformation.md)|The transformation that configures the updating of a slowly changing dimension.|  
|[Fuzzy Grouping Transformation](fuzzy-grouping-transformation.md)|The transformation that standardizes values in column data.|  
|[Fuzzy Lookup Transformation](lookup-transformation.md)|The transformation that looks up values in a reference table using a fuzzy match.|  
|[Term Extraction Transformation](term-extraction-transformation.md)|The transformation that extracts terms from text.|  
|[Term Lookup Transformation](term-lookup-transformation.md)|The transformation that looks up terms in a reference table and counts terms extracted from text.|  
|[Data Mining Query Transformation](data-mining-query-transformation.md)|The transformation that runs data mining prediction queries.|  
|[DQS Cleansing Transformation](dqs-cleansing-transformation.md)|The transformation that corrects data from a connected data source by applying rules that were created for the data source.|  
  
## Row Transformations  
 The following transformations update column values and create new columns. The transformation is applied to each row in the transformation input.  
  
|Transformation|Description|  
|--------------------|-----------------|  
|[Character Map Transformation](character-map-transformation.md)|The transformation that applies string functions to character data.|  
|[Copy Column Transformation](copy-column-transformation.md)|The transformation that adds copies of input columns to the transformation output.|  
|[Data Conversion Transformation](data-conversion-transformation.md)|The transformation that converts the data type of a column to a different data type.|  
|[Derived Column Transformation](derived-column-transformation.md)|The transformation that populates columns with the results of expressions.|  
|[Export Column Transformation](export-column-transformation.md)|The transformation that inserts data from a data flow into a file.|  
|[Import Column Transformation](import-column-transformation.md)|The transformation that reads data from a file and adds it to a data flow.|  
|[Script Component](script-component.md)|The transformation that uses script to extract, transform, or load data.|  
|[OLE DB Command Transformation](ole-db-command-transformation.md)|The transformation that runs SQL commands for each row in a data flow.|  
  
## Rowset Transformations  
 The following transformations create new rowsets. The rowset can include aggregate and sorted values, sample rowsets, or pivoted and unpivoted rowsets.  
  
|Transformation|Description|  
|--------------------|-----------------|  
|[Aggregate Transformation](aggregate-transformation.md)|The transformation that performs aggregations such as AVERAGE, SUM, and COUNT.|  
|[Sort Transformation](sort-transformation.md)|The transformation that sorts data.|  
|[Percentage Sampling Transformation](percentage-sampling-transformation.md)|The transformation that creates a sample data set using a percentage to specify the sample size.|  
|[Row Sampling Transformation](row-sampling-transformation.md)|The transformation that creates a sample data set by specifying the number of rows in the sample.|  
|[Pivot Transformation](pivot-transformation.md)|The transformation that creates a less normalized version of a normalized table.|  
|[Unpivot Transformation](unpivot-transformation.md)|The transformation that creates a more normalized version of a nonnormalized table.|  
  
## Split and Join Transformations  
 The following transformations distribute rows to different outputs, create copies of the transformation inputs, join multiple inputs into one output, and perform lookup operations.  
  
|Transformation|Description|  
|--------------------|-----------------|  
|[Conditional Split Transformation](conditional-split-transformation.md)|The transformation that routes data rows to different outputs.|  
|[Multicast Transformation](multicast-transformation.md)|The transformation that distributes data sets to multiple outputs.|  
|[Union All Transformation](union-all-transformation.md)|The transformation that merges multiple data sets.|  
|[Merge Transformation](merge-transformation.md)|The transformation that merges two sorted data sets.|  
|[Merge Join Transformation](merge-join-transformation.md)|The transformation that joins two data sets using a FULL, LEFT, or INNER join.|  
|[Lookup Transformation](lookup-transformation.md)|The transformation that looks up values in a reference table using an exact match.|  
|[Cache Transform](cache-transform.md)|The transformation that writes data from a connected data source in the data flow to a Cache connection manager that saves the data to a cache file. The Lookup transformation performs lookups on the data in the cache file.|  
|[Balanced Data Distributor Transformation](balanced-data-distributor-transformation.md)|The transformation distributes buffers of incoming rows uniformly across outputs on separate threads to improve performance of SSIS packages running on multi-core and multi-processor servers.|  
  
## Auditing Transformations  
 [!INCLUDE[ssISnoversion](../../../includes/ssisnoversion-md.md)] includes the following transformations to add audit information and count rows.  
  
|Transformation|Description|  
|--------------------|-----------------|  
|[Audit Transformation](audit-transformation.md)|The transformation that makes information about the environment available to the data flow in a package.|  
|[Row Count Transformation](row-count-transformation.md)|The transformation that counts rows as they move through it and stores the final count in a variable.|  
  
## Custom Transformations  
 You can also write custom transformations. For more information, see [Developing a Custom Transformation Component with Synchronous Outputs](../../extending-packages-custom-objects-data-flow-types/developing-a-custom-transformation-component-with-synchronous-outputs.md) and [Developing a Custom Transformation Component with Asynchronous Outputs](../../extending-packages-custom-objects-data-flow-types/developing-a-custom-transformation-component-with-asynchronous-outputs.md).  
  
  