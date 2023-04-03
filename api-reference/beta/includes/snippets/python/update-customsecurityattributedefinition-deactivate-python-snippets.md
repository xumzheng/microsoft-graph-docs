---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = CustomSecurityAttributeDefinition();
requestBody.setStatus('Deprecated');



result = await client.directory().customSecurityAttributeDefinitionsById('customSecurityAttributeDefinition-id').patch(requestBody);


```