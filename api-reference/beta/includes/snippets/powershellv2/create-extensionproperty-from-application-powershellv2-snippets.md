---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Applications

$params = @{
	name = "jobGroup"
	dataType = "String"
	targetObjects = @(
		"User"
	)
}

New-MgBetaApplicationExtensionProperty -ApplicationId $applicationId -BodyParameter $params

```