---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AddCopyFromContentTypeHubPostRequestBody();
requestBody.setContentTypeId('String');



requestResult = graphServiceClient.sitesById('site-id').listsById('list-id').contentTypes().addCopyFromContentTypeHub().post(requestBody);


```