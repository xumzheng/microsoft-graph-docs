---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AllowedValue();
requestBody.setId('Alpine');

requestBody.setIsActive(true);



result = awaitclient.directory().customSecurityAttributeDefinitionsById('customSecurityAttributeDefinition-id').allowedValues().post(requestBody);


```