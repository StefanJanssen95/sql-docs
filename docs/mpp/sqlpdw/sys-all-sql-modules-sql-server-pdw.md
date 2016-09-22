---
title: "sys.all_sql_modules (SQL Server PDW)"
ms.custom: na
ms.date: 07/27/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 5155eb8d-2ae2-4171-816b-8ac98cb7cacc
caps.latest.revision: 12
author: BarbKess
---
# sys.all_sql_modules (SQL Server PDW)
Returns SQL Server modules, including user-defined and system objects.  
  
|Column Name|Data Type|Description|Range|  
|---------------|-------------|---------------|---------|  
|object_id|**int**|ID of the object of the containing object. Is unique within a database.||  
|definition|**nvarchar(max)**|SQL text that defines this module.||  
|uses_ansi_nulls|**bit**|Module was created with SET ANSI_NULLS ON.<br /><br />Will always be = 0 for rules and defaults.||  
|uses_quoted_identifier|**bit**|Module was created with SET QUOTED_IDENTIFIER ON.||  
|is_schema_bound|**bit**|Module was created with SCHEMABINDING option.||  
|uses_database_collation|**bit**||Always 0.|  
|is_recompiled|**bit**|Procedure was created WITH RECOMPILE option.|Always 0.|  
|null_on_null_input|**bit**|Module was declared to produce a NULL output on any NULL input.|Always 0.|  
|execute_as_principal_id|**int**||Always NULL.|  
  
## See Also  
[Common Metadata Query Examples &#40;SQL Server PDW&#41;](../../mpp/sqlpdw/common-metadata-query-examples-sql-server-pdw.md)  
[SQL Server Catalog Views &#40;SQL Server PDW&#41;](../../mpp/sqlpdw/sql-server-catalog-views-sql-server-pdw.md)  
[sys.sql_modules &#40;SQL Server PDW&#41;](../../mpp/sqlpdw/sys-sql-modules-sql-server-pdw.md)  
  