---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ExternalGroup();
requestBody.setId('31bea3d537902000');

requestBody.setDisplayName('Contoso Marketing');

requestBody.setDescription('The product marketing team');



result = awaitclient.external().connectionsById('externalConnection-id').groups().post(requestBody);


```