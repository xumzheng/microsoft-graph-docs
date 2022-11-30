---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Devices.CloudPrint

$params = @{
	DisplayName = "Test Printer"
	Manufacturer = "Test Printer Manufacturer"
	Model = "Test Printer Model"
	PhysicalDeviceId = $null
	HasPhysicalDevice = $false
	CertificateSigningRequest = @{
		Content = "{content}"
		TransportKey = "{sampleTransportKey}"
	}
	ConnectorId = $null
}

New-MgBetaPrintPrinter -BodyParameter $params

```