---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Bookings

$params = @{
	"@odata.type" = "#microsoft.graph.businessScenario"
	displayName = "Contoso Order Tracking"
	uniqueName = "com.contoso.apps.ordertracking"
}

New-MgBetaBusinessScenario -BodyParameter $params

```