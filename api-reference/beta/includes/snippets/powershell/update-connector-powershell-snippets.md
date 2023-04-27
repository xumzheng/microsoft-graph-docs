---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Beta.Devices.CloudPrint

$params = @{
	displayName = "ConnectorName"
	fullyQualifiedDomainName = "CONNECTOR-MACHINE"
	operatingSystem = "Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555"
	appVersion = "0.19.7338.23496"
	location = @{
		latitude = 1.1
		longitude = 2.2
		altitudeInMeters = 3
	}
}

Update-MgBetaPrintConnector -PrintConnectorId $printConnectorId -BodyParameter $params

```