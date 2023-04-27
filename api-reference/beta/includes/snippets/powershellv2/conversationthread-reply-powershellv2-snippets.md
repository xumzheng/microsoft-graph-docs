---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Groups

$params = @{
	post = @{
		body = @{
			contentType = ""
			content = "content-value"
		}
	}
}

Invoke-MgBetaReplyGroupThread -GroupId $groupId -ConversationThreadId $conversationThreadId -BodyParameter $params

```