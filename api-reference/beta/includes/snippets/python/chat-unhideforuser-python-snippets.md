---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new UnhideForUserPostRequestBody();
$user = new TeamworkUserIdentity();
$user->setId('d864e79f-a516-4d0f-9fee-0eeb4d61fdc2');

$additionalData = [
'tenantId' => '2a690434-97d9-4eed-83a6-f5f13600199a', 
];
$user->setAdditionalData($additionalData);



$requestBody->setUser($user);


$graphServiceClient->chatsById('chat-id')->unhideForUser()->post($requestBody);


```