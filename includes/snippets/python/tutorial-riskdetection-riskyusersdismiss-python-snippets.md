---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = DismissPostRequestBody();
requestBody.setUserIds(['4628e7df-dff3-407c-a08f-75f08c0806dc', ]);



await client.identityProtection().riskyUsers().dismiss().post(requestBody);


```