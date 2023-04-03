---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = PrintTaskDefinition();
requestBody.setDisplayName('Test TaskDefinitionName');

createdBy = AppIdentity();
createdBy.setDisplayName('Requesting App Display Name');


requestBody.setCreatedBy($createdBy);


requestResult = graphServiceClient.print().taskDefinitions().post(requestBody);


```