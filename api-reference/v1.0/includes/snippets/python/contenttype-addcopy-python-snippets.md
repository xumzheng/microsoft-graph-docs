---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AddCopyPostRequestBody();
requestBody.setContentType('https://graph.microsoft.com/v1.0/sites/{site-id}/contentTypes/0x0101');



result = awaitclient.sitesById('site-id').listsById('list-id').contentTypes().addCopy().post(requestBody);


```