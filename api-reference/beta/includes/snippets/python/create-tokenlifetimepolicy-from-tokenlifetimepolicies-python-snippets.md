---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = TokenLifetimePolicy();
requestBody.setDefinition(['{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}', ]);

requestBody.setDisplayName('Contoso token lifetime policy');

requestBody.setIsOrganizationDefault(true);



requestResult = graphServiceClient.policies().tokenLifetimePolicies().post(requestBody);


```