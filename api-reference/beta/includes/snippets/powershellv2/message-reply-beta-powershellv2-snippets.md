---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Users.Actions

$params = @{
	Message = @{
		ToRecipients = @(
			@{
				EmailAddress = @{
					Address = "samanthab@contoso.onmicrosoft.com"
					Name = "Samantha Booth"
				}
			}
			@{
				EmailAddress = @{
					Address = "randiw@contoso.onmicrosoft.com"
					Name = "Randi Welch"
				}
			}
		)
	}
	Comment = "Samantha, Randi, would you name the group please?"
}

# A UPN can also be used as -UserId.
Invoke-MgBetaReplyUserMessage -UserId $userId -MessageId $messageId -BodyParameter $params

```