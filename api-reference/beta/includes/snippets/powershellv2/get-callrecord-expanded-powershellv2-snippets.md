---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.CloudCommunications

Get-MgBetaCommunicationCallRecord -CallRecordId $callRecordId -ExpandProperty "sessions(`$expand=segments)" 

```