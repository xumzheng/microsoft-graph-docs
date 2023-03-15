---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Groups

$params = @{
	Topic = "New Conversation Thread Topic"
	Posts = @(
		@{
			Body = @{
				ContentType = "html"
				Content = "this is body content"
			}
			NewParticipants = @(
				@{
					EmailAddress = @{
						Name = "Alex Darrow"
						Address = "alexd@contoso.com"
					}
				}
			)
		}
	)
}

New-MgBetaGroupThread -GroupId $groupId -BodyParameter $params

```