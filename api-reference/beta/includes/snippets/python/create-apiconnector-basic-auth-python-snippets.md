---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = IdentityApiConnector()
request_body.displayName = 'Test API'

request_body.targetUrl = 'https://someapi.com/api'

authenticationConfiguration = ApiAuthenticationConfigurationBase()
authenticationConfiguration.@odatatype = '#microsoft.graph.basicAuthentication'

additionalData = [
'username' => '<USERNAME>', 
'password' => '<PASSWORD>', 
];
authenticationConfiguration.additionaldata(additionalData)



request_body.authenticationConfiguration = authenticationConfiguration



result = await client.identity.apiConnectors.post(request_body = request_body)


```