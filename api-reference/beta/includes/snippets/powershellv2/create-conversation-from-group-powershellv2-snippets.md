---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Groups

$params = @{
	topic = "New head count"
	threads = @(
		@{
			posts = @(
				@{
					body = @{
						contentType = "html"
						content = "The confirmation will come by the end of the week."
					}
					newParticipants = @(
						@{
							emailAddress = @{
								name = "Adele Vance"
								address = "AdeleV@contoso.onmicrosoft.com"
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