---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AddCopyFromContentTypeHubPostRequestBody();
requestBody.setContentTypeId('0x0101');



requestResult = graphServiceClient.sitesById('site-id').listsById('list-id').contentTypes().addCopyFromContentTypeHub().post(requestBody);


```