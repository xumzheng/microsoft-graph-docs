---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = AuthenticationContextClassReference();
requestBody.setId('c1');

requestBody.setDisplayName('Contoso medium');

requestBody.setDescription('Medium protection level defined for Contoso policy');

requestBody.setIsAvailable(true);



result = await client.identity().conditionalAccess().authenticationContextClassReferences().post(requestBody);


```