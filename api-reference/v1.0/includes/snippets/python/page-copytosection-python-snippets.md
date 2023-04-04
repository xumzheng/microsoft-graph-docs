---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = CopyToSectionPostRequestBody();
request_body.setId('id-value');

request_body.setGroupId('groupId-value');



result = await client.me.onenote.pagesById('onenotePage-id').copyToSection.post(request_body);


```