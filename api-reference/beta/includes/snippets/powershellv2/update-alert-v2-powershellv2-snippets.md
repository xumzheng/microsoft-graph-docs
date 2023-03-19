---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Security

$params = @{
	AssignedTo = "secAdmin@contoso.onmicrosoft.com"
	Classification = "truePositive"
	Determination = "malware"
	Status = "inProgress"
}

Update-MgBetaSecurityAlertV2 -AlertId $alertId -BodyParameter $params

```