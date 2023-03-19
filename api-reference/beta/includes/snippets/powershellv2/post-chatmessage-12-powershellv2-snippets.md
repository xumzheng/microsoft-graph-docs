---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	Body = @{
		ContentType = "html"
		Content = "<emoji alt="😶‍🌫️"></emoji>"
	}
}

New-MgBetaChatMessage -ChatId $chatId -BodyParameter $params

```