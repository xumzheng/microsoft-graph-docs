---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = TokenLifetimePolicy();
requestBody.setDefinition(['{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"5:30:00\"}}', ]);

requestBody.setDisplayName('Contoso token lifetime policy');

requestBody.setIsOrganizationDefault(true);



result = await client.policies().tokenLifetimePoliciesById('tokenLifetimePolicy-id').patch(requestBody);


```