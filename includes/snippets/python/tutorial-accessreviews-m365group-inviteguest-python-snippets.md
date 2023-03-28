---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Invitation();
$requestBody.setInvitedUserDisplayName('John Doe (Tailspin Toys)');

$requestBody.setInvitedUserEmailAddress('john@tailspintoys.com');

$requestBody.setSendInvitationMessage(false);

$requestBody.setInviteRedirectUrl('https://myapps.microsoft.com');



$requestResult = $graphServiceClient.invitations().post($requestBody);


```