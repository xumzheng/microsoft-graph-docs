---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	userIds = @(
		"04487ee0-f4f6-4e7f-8999-facc5a30e232"
		"13387ee0-f4f6-4e7f-8999-facc5120e345"
	)
}

Invoke-MgBetaDismissRiskyUser -BodyParameter $params

```