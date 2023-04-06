---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = IdentityApiConnector()
request_body.setDisplayName('Test API')

request_body.setTargetUrl('https://someapi.com/api')

authenticationConfiguration = ApiAuthenticationConfigurationBase()
authenticationConfiguration.set@odatatype('#microsoft.graph.basicAuthentication')

additionalData = [
'username' => '<USERNAME>', 
'password' => '<PASSWORD>', 
];
authenticationConfiguration.setAdditionalData(additionalData)



request_body.setAuthenticationConfiguration($authenticationConfiguration)

request_config = ApiConnectorsRequestBuilderPostRequestConfiguration(
request_config = ApiConnectorsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.identity.apiConnectors.post(request_body, headers=)


```