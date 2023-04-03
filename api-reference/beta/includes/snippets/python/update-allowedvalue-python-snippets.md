---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AllowedValue();
requestBody.setIsActive(false);



result = awaitclient.directory().customSecurityAttributeDefinitionsById('customSecurityAttributeDefinition-id').allowedValuesById('allowedValue-id').patch(requestBody);


```