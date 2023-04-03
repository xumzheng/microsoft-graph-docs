---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AuthenticationContextClassReference();
requestBody.setDisplayName('Contoso medium');

requestBody.setDescription('Medium protection level defined for Contoso policy');

requestBody.setIsAvailable(true);



result = awaitclient.identity().conditionalAccess().authenticationContextClassReferencesById('authenticationContextClassReference-id').patch(requestBody);


```