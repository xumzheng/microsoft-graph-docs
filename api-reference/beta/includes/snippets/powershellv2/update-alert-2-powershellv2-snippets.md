---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Security

$params = @{
	AssignedTo = "String"
	ClosedDateTime = [System.DateTime]::Parse("String (timestamp)")
	Comments = @(
		"String"
	)
	Feedback = "@odata.type: microsoft.graph.alertFeedback"
	Status = "@odata.type: microsoft.graph.alertStatus"
	Tags = @(
		"String"
	)
	VendorInformation = @{
		Provider = "String"
		Vendor = "String"
	}
}

Update-MgBetaSecurityAlert -AlertId $alertId -BodyParameter $params

```