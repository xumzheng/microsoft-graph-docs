---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = IdentityApiConnector();
requestBody.setDisplayName('Test API');

requestBody.setTargetUrl('https://someapi.com/api');

authenticationConfiguration = ApiAuthenticationConfigurationBase();
authenticationConfiguration.set@odatatype('#microsoft.graph.basicAuthentication');

additionalData = [
'username' => '<USERNAME>', 
'password' => '<PASSWORD>', 
];
authenticationConfiguration.setAdditionalData(additionalData);



requestBody.setAuthenticationConfiguration($authenticationConfiguration);


result = await client.identity().apiConnectors().post(requestBody);


```