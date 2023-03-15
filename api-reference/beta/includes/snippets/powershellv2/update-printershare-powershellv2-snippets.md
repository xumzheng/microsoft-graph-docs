---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Devices.CloudPrint

$params = @{
	DisplayName = "ShareName"
	AllowAllUsers = $true
	"Printer@odata.bind" = "https://graph.microsoft.com/beta/print/printers/{id}"
}

Update-MgBetaPrintShare -PrinterShareId $printerShareId -BodyParameter $params

```