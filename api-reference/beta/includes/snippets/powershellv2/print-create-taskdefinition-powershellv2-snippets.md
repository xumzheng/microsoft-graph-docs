---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Devices.CloudPrint

$params = @{
	displayName = "Test TaskDefinitionName"
	createdBy = @{
		displayName = "Requesting App Display Name"
	}
}

New-MgBetaPrintTaskDefinition -BodyParameter $params

```