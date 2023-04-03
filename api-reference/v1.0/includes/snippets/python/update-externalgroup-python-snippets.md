---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ExternalGroup();
requestBody.setDisplayName('Contoso Marketing');

requestBody.setDescription('The product marketing team');



result = await client.external().connectionsById('externalConnection-id').groupsById('externalGroup-id').patch(requestBody);


```