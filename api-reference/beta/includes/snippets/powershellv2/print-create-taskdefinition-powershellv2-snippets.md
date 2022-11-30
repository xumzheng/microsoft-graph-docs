---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Devices.CloudPrint

$params = @{
	DisplayName = "Test TaskDefinitionName"
	CreatedBy = @{
		DisplayName = "Requesting App Display Name"
	}
}

New-MgBetaPrintTaskDefinition -BodyParameter $params

```