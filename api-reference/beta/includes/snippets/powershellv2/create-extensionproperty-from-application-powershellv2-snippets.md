---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Applications

$params = @{
	Name = "jobGroup"
	DataType = "String"
	TargetObjects = @(
		"User"
	)
}

New-MgBetaApplicationExtensionProperty -ApplicationId $applicationId -BodyParameter $params

```