---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = IdentityApiConnector()
request_body.displayName = 'New Test API'

request_body.targetUrl = 'https://otherapi.com/api/endpoint'

authenticationConfiguration = ApiAuthenticationConfigurationBase()
authenticationConfiguration.@odatatype = 'microsoft.graph.basicAuthentication'

additionalData = [
'username' => '<NEW_USERNAME>', 
'password' => '<NEW_PASSWORD>', 
];
authenticationConfiguration.additionaldata(additionalData)



request_body.authenticationConfiguration = authenticationConfiguration



result = await client.identity.apiConnectors_by_id('identityApiConnector-id').patch(request_body = request_body)


```