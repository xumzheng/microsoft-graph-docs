---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AllowedValue();
requestBody.setId('Alpine');

requestBody.setIsActive(true);



requestResult = graphServiceClient.directory().customSecurityAttributeDefinitionsById('customSecurityAttributeDefinition-id').allowedValues().post(requestBody);


```