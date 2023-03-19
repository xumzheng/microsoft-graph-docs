---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	Topic = "Group chat title update"
}

Update-MgBetaChat -ChatId $chatId -BodyParameter $params

```