---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Applications

$params = @{
	DisplayName = "New display name"
}

Update-MgBetaApplication -ApplicationId $applicationId -BodyParameter $params

```