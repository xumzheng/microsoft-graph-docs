---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = PrintTaskDefinition();
requestBody.setDisplayName('Test TaskDefinitionName');

createdBy = AppIdentity();
createdBy.setDisplayName('Requesting App Display Name');


requestBody.setCreatedBy($createdBy);


result = await client.print().taskDefinitionsById('printTaskDefinition-id').patch(requestBody);


```