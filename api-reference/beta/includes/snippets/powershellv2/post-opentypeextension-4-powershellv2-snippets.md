---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Groups

$params = @{
	Post = @{
		Body = @{
			ContentType = "html"
			Content = "<html><body><div><div><div><div>When and where? </div></div></div></div></body></html>"
		}
		Extensions = @(
			@{
				"@odata.type" = "microsoft.graph.openTypeExtension"
				ExtensionName = "Com.Contoso.HR"
				CompanyName = "Contoso"
				ExpirationDate = "2015-07-03T13:04:00.000Z"
				TopPicks = @(
					"Employees only"
					"Add spouse or guest"
					"Add family"
				)
			}
		)
	}
}

Invoke-MgBetaReplyGroupThreadPost -GroupId $groupId -ConversationThreadId $conversationThreadId -PostId $postId -BodyParameter $params

```