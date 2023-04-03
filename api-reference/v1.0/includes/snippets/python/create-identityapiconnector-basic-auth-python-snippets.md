---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = IdentityApiConnector();
requestBody.setDisplayName('Test API');

requestBody.setTargetUrl('https://someapi.com/api');

authenticationConfiguration = ApiAuthenticationConfigurationBase();
authenticationConfiguration.set@odatatype('#microsoft.graph.basicAuthentication');

additionalData = [
'username' => 'MyUsername', 
'password' => 'MyPassword', 
];
authenticationConfiguration.setAdditionalData(additionalData);



requestBody.setAuthenticationConfiguration($authenticationConfiguration);


result = awaitclient.identity().apiConnectors().post(requestBody);


```