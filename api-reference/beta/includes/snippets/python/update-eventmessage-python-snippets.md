---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Message();
$requestBody.setIsRead(true);



$requestResult = $graphServiceClient.me().messagesById('message-id').patch($requestBody);


```