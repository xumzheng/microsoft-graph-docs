---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Groups

$params = @{
	groupLifetimeInDays = 180
	managedGroupTypes = "Selected"
	alternateNotificationEmails = "admin@contoso.com"
}

Update-MgBetaGroupLifecyclePolicy -GroupLifecyclePolicyId $groupLifecyclePolicyId -BodyParameter $params

```