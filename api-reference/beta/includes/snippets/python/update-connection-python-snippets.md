---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ExternalConnection();
requestBody.setName('Contoso HR Service Tickets');

requestBody.setDescription('Connection to index HR service tickets');



result = await client.external().connectionsById('externalConnection-id').patch(requestBody);


```