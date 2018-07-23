# **DEPUPLICATION OF RECORDS**

_API FieloPLT.MemberService.mergeMember (Map<Id,Id> mapMembersMerge, Boolean recalculateLevels, Boolean reparentOnline, String confJson)_

Fielo has developed API’s for the deduplication of records. The mergedMember method merges duplicate records of [Members](https://documentation.fielo.com/v10.2/docs/members) to provide an accurate loyalty point count and data set for each **Member**. A static resource (MembersMerge) specifies criteria for resolving field-level differences in duplicate Member records.

## Parameters

| Parameter |	Type |	Description |
| --------- | ---- | ------------ |
| _MapMembersMerge_ |	**Map<Id,Id>** |	Defines two **members** to be merged. |
| _recalculateLevels_ |	**Boolean** |	When true, recalculate count for two **members**. |
| _reparentOnline_ |	**Boolean** |	When true, merge two **members** online. |
| _ConfJson_ |	**String** |	Identifies data points to be merged. |

## Return Value

| Type |	Description |
| ---- |  ----------- |
| **Map<Id,String>** |	Map of errors from **Salesforce Contact** IDs. If operation is successful, value is an empty map. |
