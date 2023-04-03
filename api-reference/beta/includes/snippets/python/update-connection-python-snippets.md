---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ExternalConnection();
requestBody.setName('Contoso HR Service Tickets');

requestBody.setDescription('Connection to index HR service tickets');



requestResult = graphServiceClient.external().connectionsById('externalConnection-id').patch(requestBody);


```