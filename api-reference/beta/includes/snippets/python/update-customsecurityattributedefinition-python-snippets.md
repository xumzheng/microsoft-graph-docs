---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = CustomSecurityAttributeDefinition();
requestBody.setDescription('Target completion date (YYYY/MM/DD)');



requestResult = graphServiceClient.directory().customSecurityAttributeDefinitionsById('customSecurityAttributeDefinition-id').patch(requestBody);


```