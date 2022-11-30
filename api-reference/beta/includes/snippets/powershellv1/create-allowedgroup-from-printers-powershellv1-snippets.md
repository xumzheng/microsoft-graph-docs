---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Devices.CloudPrint

$params = @{
	"@odata.id" = "https://graph.microsoft.com/beta/groups/{id}"
}

New-MgPrintShareAllowedGroupByRef -PrinterShareId $printerShareId -BodyParameter $params

```