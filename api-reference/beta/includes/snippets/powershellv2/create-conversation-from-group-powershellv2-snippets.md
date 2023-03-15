---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Groups

$params = @{
	Topic = "New head count"
	Threads = @(
		@{
			Posts = @(
				@{
					Body = @{
						ContentType = "html"
						Content = "The confirmation will come by the end of the week."
					}
					NewParticipants = @(
						@{
							EmailAddress = @{
								Name = "Adele Vance"
								Address = "AdeleV@contoso.onmicrosoft.com"
							}
						}
					)
				}
			)
		}
	)
}

New-MgBetaGroupConversation -GroupId $groupId -BodyParameter $params

```