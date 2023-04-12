---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = IdentityApiConnector()
request_body.displayName = 'Test API'

request_body.targetUrl = 'https://someotherapi.com/api'

authenticationConfiguration = ApiAuthenticationConfigurationBase()
authenticationConfiguration.@odatatype = '#microsoft.graph.pkcs12Certificate'

additionalData = [
'pkcs12Value' => 'eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA', 
'password' => 'CertificatePassword', 
];
authenticationConfiguration.additionaldata(additionalData)



request_body.authenticationConfiguration = authenticationConfiguration



result = await client.identity.apiConnectors.post(request_body = request_body)


```