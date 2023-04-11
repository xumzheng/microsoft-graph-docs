---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Invitation()
request_body.invitedUserDisplayName = 'John Doe (Tailspin Toys)'

request_body.invitedUserEmailAddress = 'john@tailspintoys.com'

request_body.sendInvitationMessage = false

request_body.inviteRedirectUrl = 'https://myapps.microsoft.com'




result = await client.invitations.post(request_body = request_body)


```