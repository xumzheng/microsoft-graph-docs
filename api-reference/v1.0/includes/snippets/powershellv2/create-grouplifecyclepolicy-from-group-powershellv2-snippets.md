---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Groups

$params = @{
	GroupLifetimeInDays = 100
	ManagedGroupTypes = "Selected"
	AlternateNotificationEmails = "admin@contoso.com"
}

New-MgGroupLifecyclePolicy -BodyParameter $params

```