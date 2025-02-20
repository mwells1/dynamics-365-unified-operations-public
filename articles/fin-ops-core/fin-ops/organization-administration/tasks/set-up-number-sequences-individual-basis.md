--- 
# required metadata 
 
title: Set up number sequences on an individual basis
description: This topic explains how to set up number sequences on an individual basis.  
author: sericks007  
ms.date: 08/16/2019
ms.topic: business-process 
ms.prod:  
ms.technology:  
 
# optional metadata 
 
ms.search.form: NumberSequenceTableListPage, NumberSequenceDetails   
audience: Application User 
# ms.devlang:  
ms.reviewer: sericks
# ms.tgt_pltfrm:  
# ms.custom:  
ms.search.region: Global
# ms.search.industry: 
ms.author: sericks
ms.search.validFrom: 2016-06-30 
ms.dyn365.ops.version: Version 7.0.0 
---
# Set up number sequences on an individual basis

[!include [banner](../../includes/banner.md)]

This topic explains how to set up number sequences on an individual basis. Number sequences are used to generate readable, unique identifiers for master data records and transaction records that require them. A master data or transaction record that requires an identifier is referred to as a reference. Before you can create new records for a reference, you must set up a number sequence and associate it with the reference. You can set up all required number sequences at the same time by using the **Set up number sequences** wizard, or you can create or modify individual number sequences by using the **Number sequences** page.

1. Go to **Navigation pane > Modules > Organization administration > Number sequences > Number sequences**.
2. Select **Number sequence**.
3. In the **Number sequence code** field, type a value.
4. In the **Name** field, type a value.
5. On the **Scope parameters** FastTab, select a scope for the number sequence and select scope values from the drop-down list. The scope defines which organizations use the number sequence. In addition, number sequences that have a scope other than **Shared** can have segments that correspond to their scope. For example, a number sequence with a scope of **Legal entity** can have a legal entity segment. For more information about scopes, see [Number sequence overview](https://docs.microsoft.com/dynamics365/unified-operations/fin-and-ops/organization-administration/number-sequence-overview). 
6. Expand the **Segments** section.
    - Define the format for the number sequence by adding, removing, and rearranging segments.  
    - Number sequences of all scopes can contain *Constant segments* and *Alphanumeric segments*. Constant segments contain a set of alphanumeric characters that do not change. Use this segment type to add a hyphen or other separators between number sequence segments. Alphanumeric segments contain a combination of number signs (#) and ampersands (&). These characters represent letters and numbers that increment every time that a number from the sequence is used. Use a number sign (#) to indicate incrementing numbers and an ampersand (&) to indicate incrementing letters. For example, the format `#####_2014` creates the sequence `00001_2014`, `00002_2014`, and so on. At least one alphanumeric segment must be present. Scope segments, such as company or legal entity, are not required. However, if you do not include scope segments in the format, numbers for the selected reference are still generated per scope.  
7. Expand the **References** section. Select the document type or record to assign this number sequence to. This step is optional for sequences that are defined for special application usage patterns. In these scenarios, a new number is generated by using the value of a number sequence code or ID, without using a reference. An example of a special application usage pattern is a voucher series that is used for specific journal names. However, we do not recommend that you use such patterns.  
8. Expand the **General** section. On the General FastTab, specify whether the number sequence is manual, and continuous or non-continuous. In addition, enter the lowest and highest numbers that can be used in the number sequence. We do not recommend changing a non-continuous number sequence to a continuous number sequence. The number sequence will not be truly continuous. This change may also cause duplicate key violations in the database. In addition, continuous number sequences have a larger effect on performance.   
9. Click **Save**.



[!INCLUDE[footer-include](../../../../includes/footer-banner.md)]