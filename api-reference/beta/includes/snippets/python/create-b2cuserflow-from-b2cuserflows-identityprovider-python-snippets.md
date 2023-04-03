---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = B2cIdentityUserFlow();
requestBody.setId('Customer');

requestBody.setUserFlowType(UserFlowType('signuporsignin'));

requestBody.setUserFlowTypeVersion(3);

identityProvidersIdentityProvider1 = IdentityProvider();
identityProvidersIdentityProvider1.setId('Facebook-OAuth');


identityProvidersArray []= identityProvidersIdentityProvider1;
requestBody.setIdentityProviders(identityProvidersArray);



requestConfiguration = B2cUserFlowsRequestBuilderPostRequestConfiguration();

headers = [
'Location' => 'https://graph.microsoft.com/beta/identity/b2cUserFlows(\'B2C_1_Customer\')',
];

requestConfiguration.headers = headers;


requestResult = graphServiceClient.identity().b2cUserFlows().post(requestBody, requestConfiguration);


```