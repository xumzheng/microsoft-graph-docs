---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = IdentityApiConnector()
authenticationConfiguration = ApiAuthenticationConfigurationBase()
authenticationConfiguration.set@odatatype('#microsoft.graph.pkcs12Certificate')

additionalData = [
'pkcs12Value' => 'eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA', 
'password' => 'secret', 
];
authenticationConfiguration.setAdditionalData(additionalData)



request_body.setAuthenticationConfiguration($authenticationConfiguration)

request_config = IdentityApiConnectorRequestBuilderPatchRequestConfiguration(
request_config = IdentityApiConnectorRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.identity.apiConnectors_by_id('identityApiConnector-id').patch(request_body, headers=)


```