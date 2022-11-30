---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Applications

$params = @{
	"@odata.id" = "https://graph.microsoft.com/beta/policies/appManagementPolicies/{id}"
}

New-MgApplicationAppManagementPolicyByRef -ApplicationId $applicationId -BodyParameter $params

```