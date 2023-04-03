---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = CopyPostRequestBody();
requestBody.setDestinationId('destinationId-value');



requestResult = graphServiceClient.me().messagesById('message-id').copy().post(requestBody);


```