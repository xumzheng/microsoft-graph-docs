---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Security

$params = @{
	"@odata.type" = "#microsoft.graph.security.retentionEventType"
	DisplayName = "String"
	Description = "String"
	CreatedBy = @{
		"@odata.type" = "microsoft.graph.identitySet"
	}
}

New-MgBetaSecurityTriggerTypeRetentionEventType -BodyParameter $params

```