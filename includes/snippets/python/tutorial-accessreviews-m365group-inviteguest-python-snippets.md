---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Invitation();
requestBody.setInvitedUserDisplayName('John Doe (Tailspin Toys)');

requestBody.setInvitedUserEmailAddress('john@tailspintoys.com');

requestBody.setSendInvitationMessage(false);

requestBody.setInviteRedirectUrl('https://myapps.microsoft.com');



result = awaitclient.invitations().post(requestBody);


```