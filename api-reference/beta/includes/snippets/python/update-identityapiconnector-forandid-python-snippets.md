---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = IdentityApiConnector()
request_body.setDisplayName('New Test API')

request_body.setTargetUrl('https://otherapi.com/api/endpoint')

authenticationConfiguration = ApiAuthenticationConfigurationBase()
authenticationConfiguration.set@odatatype('microsoft.graph.basicAuthentication')

additionalData = [
'username' => '<NEW_USERNAME>', 
'password' => '<NEW_PASSWORD>', 
];
authenticationConfiguration.setAdditionalData(additionalData)



request_body.setAuthenticationConfiguration($authenticationConfiguration)


result = await client.identity.apiConnectorsById('identityApiConnector-id').patch(request_body)


```