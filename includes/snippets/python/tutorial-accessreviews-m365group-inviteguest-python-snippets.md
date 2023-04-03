---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Invitation();
requestBody.setInvitedUserDisplayName('John Doe (Tailspin Toys)');

requestBody.setInvitedUserEmailAddress('john@tailspintoys.com');

requestBody.setSendInvitationMessage(false);

requestBody.setInviteRedirectUrl('https://myapps.microsoft.com');



result = await client.invitations().post(requestBody);


```