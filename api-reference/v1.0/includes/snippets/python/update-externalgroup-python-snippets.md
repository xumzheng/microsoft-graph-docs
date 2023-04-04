---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = ExternalGroup();
request_body.setDisplayName('Contoso Marketing');

request_body.setDescription('The product marketing team');



result = await client.external().connectionsById('externalConnection-id').groupsById('externalGroup-id').patch(request_body);


```