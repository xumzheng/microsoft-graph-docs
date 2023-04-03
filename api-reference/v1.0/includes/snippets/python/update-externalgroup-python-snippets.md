---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ExternalGroup();
requestBody.setDisplayName('Contoso Marketing');

requestBody.setDescription('The product marketing team');



requestResult = graphServiceClient.external().connectionsById('externalConnection-id').groupsById('externalGroup-id').patch(requestBody);


```