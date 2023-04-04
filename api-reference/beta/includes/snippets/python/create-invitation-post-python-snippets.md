---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Invitation();
request_body.setInvitedUserEmailAddress('admin@fabrikam.com');

request_body.setInviteRedirectUrl('https://myapp.contoso.com');



result = await client.invitations().post(request_body);


```