---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = B2xIdentityUserFlow();
requestBody.setId('Partner');

requestBody.setUserFlowType(UserFlowType('signuporsignin'));

requestBody.setUserFlowTypeVersion(1);

identityProvidersIdentityProvider1 = IdentityProvider();
identityProvidersIdentityProvider1.setId('Facebook-OAuth');

identityProvidersIdentityProvider1.setType('Facebook');

identityProvidersIdentityProvider1.setName('Facebook');


identityProvidersArray []= identityProvidersIdentityProvider1;
requestBody.setIdentityProviders(identityProvidersArray);




result = awaitclient.identity().b2xUserFlows().post(requestBody);


```