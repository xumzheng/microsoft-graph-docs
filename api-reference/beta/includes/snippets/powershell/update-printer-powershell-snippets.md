---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Beta.Devices.CloudPrint

$params = @{
	name = "PrinterName"
	location = @{
		latitude = 1.1
		longitude = 2.2
		altitudeInMeters = 3
	}
}

Update-MgBetaPrintPrinter -PrinterId $printerId -BodyParameter $params

```