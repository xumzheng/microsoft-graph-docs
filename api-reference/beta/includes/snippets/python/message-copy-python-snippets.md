---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = CopyPostRequestBody();
requestBody.setDestinationId('destinationId-value');



result = awaitclient.me().messagesById('message-id').copy().post(requestBody);


```