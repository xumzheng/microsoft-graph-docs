---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Groups

$params = @{
	groupLifetimeInDays = 180
	managedGroupTypes = "Selected"
	alternateNotificationEmails = "admin@contoso.com"
}

Update-MgGroupLifecyclePolicy -GroupLifecyclePolicyId $groupLifecyclePolicyId -BodyParameter $params

```