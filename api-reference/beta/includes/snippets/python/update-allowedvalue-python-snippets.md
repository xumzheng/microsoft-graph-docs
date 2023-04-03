---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AllowedValue();
requestBody.setIsActive(false);



requestResult = graphServiceClient.directory().customSecurityAttributeDefinitionsById('customSecurityAttributeDefinition-id').allowedValuesById('allowedValue-id').patch(requestBody);


```