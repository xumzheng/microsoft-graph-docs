---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Devices.CloudPrint

$params = @{
	name = "PrinterName"
	location = @{
		latitude = 1.1
		longitude = 2.2
		altitudeInMeters = 3
	}
}

Update-MgPrintPrinter -PrinterId $printerId -BodyParameter $params

```