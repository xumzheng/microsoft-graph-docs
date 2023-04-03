---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = CopyToSectionPostRequestBody();
requestBody.setId('id-value');

requestBody.setGroupId('groupId-value');



result = await client.me().onenote().pagesById('onenotePage-id').copyToSection().post(requestBody);


```