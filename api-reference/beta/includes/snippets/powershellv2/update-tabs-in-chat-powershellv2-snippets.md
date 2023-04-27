---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	displayName = "My Contoso Tab - updated again"
}

Update-MgBetaChatTab -ChatId $chatId -TeamsTabId $teamsTabId -BodyParameter $params

```