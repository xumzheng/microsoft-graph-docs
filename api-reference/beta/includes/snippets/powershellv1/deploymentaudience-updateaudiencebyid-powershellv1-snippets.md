---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.WindowsUpdates

$params = @{
	MemberEntityType = "String"
	AddMembers = @(
		"String"
	)
	RemoveMembers = @(
		"String"
	)
	AddExclusions = @(
		"String"
	)
	RemoveExclusions = @(
		"String"
	)
}

Update-MgWindowsUpdatesDeploymentAudienceById -DeploymentId $deploymentId -BodyParameter $params

```