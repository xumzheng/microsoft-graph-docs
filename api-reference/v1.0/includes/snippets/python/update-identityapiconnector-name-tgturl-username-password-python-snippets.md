---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = IdentityApiConnector();
requestBody.setDisplayName('New Test API');

requestBody.setTargetUrl('https://otherapi.com/api/endpoint');

authenticationConfiguration = ApiAuthenticationConfigurationBase();
authenticationConfiguration.set@odatatype('microsoft.graph.basicAuthentication');

additionalData = [
'username' => '<NEW_USERNAME>', 
'password' => '<NEW_PASSWORD>', 
];
authenticationConfiguration.setAdditionalData(additionalData);



requestBody.setAuthenticationConfiguration($authenticationConfiguration);


result = awaitclient.identity().apiConnectorsById('identityApiConnector-id').patch(requestBody);


```