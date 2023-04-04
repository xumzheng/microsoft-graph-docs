---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Invitation();
request_body.setInvitedUserDisplayName('John Doe (Tailspin Toys)');

request_body.setInvitedUserEmailAddress('john@tailspintoys.com');

request_body.setSendInvitationMessage(false);

request_body.setInviteRedirectUrl('https://myapps.microsoft.com');



result = await client.invitations.post(request_body);


```