---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AddLargeGalleryViewPostRequestBody();
requestBody.setClientContext('785f4929-92ca-497b-863f-c778c77c9758');



result = awaitclient.communications().callsById('call-id').addLargeGalleryView().post(requestBody);


```