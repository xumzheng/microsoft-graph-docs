---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = CopyPostRequestBody();
requestBody.setDestinationId('destinationId-value');



result = await client.me().mailFoldersById('mailFolder-id').copy().post(requestBody);


```