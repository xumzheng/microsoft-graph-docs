---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Teams

$params = @{
	body = @{
		content = "Hello world"
	}
}

New-MgChatMessage -ChatId $chatId -BodyParameter $params

```