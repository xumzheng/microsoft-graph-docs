---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users.Actions

$params = @{
	InputIds = @(
		"{rest-formatted-id-1}"
		"{rest-formatted-id-2}"
	)
	SourceIdType = "restId"
	TargetIdType = "restImmutableEntryId"
}

# A UPN can also be used as -UserId.
Invoke-MgBetaTranslateUserExchangeId -UserId $userId -BodyParameter $params

```