---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	"@odata.type" = "#microsoft.graph.continuousAccessEvaluationPolicy"
	Migrate = $true
}

Update-MgBetaIdentityContinuouAccessEvaluationPolicy -BodyParameter $params

```