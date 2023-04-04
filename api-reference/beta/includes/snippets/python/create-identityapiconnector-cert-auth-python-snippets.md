---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = IdentityApiConnector()
request_body.setDisplayName('Test API')

request_body.setTargetUrl('https://someotherapi.com/api')

authenticationConfiguration = ApiAuthenticationConfigurationBase()
authenticationConfiguration.set@odatatype('#microsoft.graph.pkcs12Certificate')

additionalData = [
'pkcs12Value' => 'eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA', 
'password' => '<password>', 
];
authenticationConfiguration.setAdditionalData(additionalData)



request_body.setAuthenticationConfiguration($authenticationConfiguration)


result = await client.identity.apiConnectors.post(request_body)


```