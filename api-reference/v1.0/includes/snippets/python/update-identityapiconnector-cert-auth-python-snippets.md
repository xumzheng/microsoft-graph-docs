---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = IdentityApiConnector()
authenticationConfiguration = ApiAuthenticationConfigurationBase()
authenticationConfiguration.@odatatype = '#microsoft.graph.pkcs12Certificate'

additionalData = [
'pkcs12Value' => 'eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA', 
'password' => 'secret', 
];
authenticationConfiguration.additionaldata(additionalData)



request_body.authenticationConfiguration = authenticationConfiguration



result = await client.identity.apiConnectors_by_id('identityApiConnector-id').patch(request_body = request_body)


```