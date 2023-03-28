---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Invitation();
$requestBody.setInvitedUserEmailAddress('admin@fabrikam.com');

$requestBody.setInviteRedirectUrl('https://myapp.contoso.com');



$requestResult = $graphServiceClient.invitations().post($requestBody);


```