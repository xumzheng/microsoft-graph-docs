---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = AddCopyFromContentTypeHubPostRequestBody();
requestBody.setContentTypeId('0x0101');



result = await client.sitesById('site-id').listsById('list-id').contentTypes().addCopyFromContentTypeHub().post(requestBody);


```