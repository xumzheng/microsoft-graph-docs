---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = CopyPostRequestBody();
requestBody.setDestinationId('destinationId-value');



result = awaitclient.me().mailFoldersById('mailFolder-id').copy().post(requestBody);


```