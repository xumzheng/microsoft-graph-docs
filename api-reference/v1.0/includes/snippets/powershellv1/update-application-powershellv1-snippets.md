---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Applications

$params = @{
	DisplayName = "New display name"
}

Update-MgApplication -ApplicationId $applicationId -BodyParameter $params

```