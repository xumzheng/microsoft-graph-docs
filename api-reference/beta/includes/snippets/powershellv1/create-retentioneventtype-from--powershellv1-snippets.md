---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Security

$params = @{
	"@odata.type" = "#microsoft.graph.security.retentionEventType"
	DisplayName = "String"
	Description = "String"
	CreatedBy = @{
		"@odata.type" = "microsoft.graph.identitySet"
	}
}

New-MgSecurityTriggerTypeRetentionEventType -BodyParameter $params

```