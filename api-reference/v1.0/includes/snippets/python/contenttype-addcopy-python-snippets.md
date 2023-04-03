---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AddCopyPostRequestBody();
requestBody.setContentType('https://graph.microsoft.com/v1.0/sites/{site-id}/contentTypes/0x0101');



requestResult = graphServiceClient.sitesById('site-id').listsById('list-id').contentTypes().addCopy().post(requestBody);


```