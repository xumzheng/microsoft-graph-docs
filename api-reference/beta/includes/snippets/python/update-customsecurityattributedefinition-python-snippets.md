---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = CustomSecurityAttributeDefinition();
requestBody.setDescription('Target completion date (YYYY/MM/DD)');



result = awaitclient.directory().customSecurityAttributeDefinitionsById('customSecurityAttributeDefinition-id').patch(requestBody);


```