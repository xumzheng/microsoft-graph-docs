---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Invitation();
requestBody.setInvitedUserEmailAddress('admin@fabrikam.com');

requestBody.setInviteRedirectUrl('https://myapp.contoso.com');



result = awaitclient.invitations().post(requestBody);


```