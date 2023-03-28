---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new SetStatusMessagePostRequestBody();
$statusMessage = new PresenceStatusMessage();
$statusMessageMessage = new ItemBody();
$statusMessageMessage->setContent('Hey I am available now');

$statusMessageMessage->setContentType(new BodyType('text'));


$statusMessage->setMessage($statusMessageMessage);

$requestBody->setStatusMessage($statusMessage);


$graphServiceClient->usersById('user-id')->presence()->setStatusMessage()->post($requestBody);


```