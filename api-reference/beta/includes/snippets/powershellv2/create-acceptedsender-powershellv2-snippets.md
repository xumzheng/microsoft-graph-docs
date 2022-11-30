---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Groups

$params = @{
	"@odata.id" = "https://graph.microsoft.com/beta/users/alexd@contoso.com"
}

New-MgBetaGroupAcceptedSenderByRef -GroupId $groupId -BodyParameter $params

```