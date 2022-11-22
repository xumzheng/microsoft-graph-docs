---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Groups

$params = @{
	Post = @{
		Body = @{
			ContentType = ""
			Content = "content-value"
		}
	}
}

Invoke-MgBetaReplyGroupThread -GroupId $groupId -ConversationThreadId $conversationThreadId -BodyParameter $params

```