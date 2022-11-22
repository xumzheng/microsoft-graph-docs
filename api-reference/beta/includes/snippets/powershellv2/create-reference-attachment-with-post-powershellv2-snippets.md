---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Groups

$params = @{
	Post = @{
		Body = @{
			ContentType = "text"
			Content = "I attached a reference to a file on OneDrive."
		}
		Attachments = @(
			@{
				"@odata.type" = "#microsoft.graph.referenceAttachment"
				Name = "Personal pictures"
				SourceUrl = "https://contoso.com/personal/mario_contoso_net/Documents/Pics"
				ProviderType = "oneDriveConsumer"
				Permission = "Edit"
				IsFolder = "True"
			}
		)
	}
}

Invoke-MgBetaReplyGroupThread -GroupId $groupId -ConversationThreadId $conversationThreadId -BodyParameter $params

```