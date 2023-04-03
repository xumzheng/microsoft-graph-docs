---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Invitation();
requestBody.setInvitedUserEmailAddress('admin@fabrikam.com');

requestBody.setInviteRedirectUrl('https://myapp.contoso.com');



result = await client.invitations().post(requestBody);


```