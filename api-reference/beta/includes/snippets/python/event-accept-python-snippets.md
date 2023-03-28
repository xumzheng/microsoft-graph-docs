---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new AcceptPostRequestBody();
$requestBody.setComment('comment-value');

$requestBody.setSendResponse(true);



$graphServiceClient.me().eventsById('event-id').accept().post($requestBody);


```