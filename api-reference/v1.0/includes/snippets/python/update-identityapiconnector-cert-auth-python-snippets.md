---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = IdentityApiConnector();
authenticationConfiguration = ApiAuthenticationConfigurationBase();
authenticationConfiguration.set@odatatype('#microsoft.graph.pkcs12Certificate');

additionalData = [
'pkcs12Value' => 'eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA', 
'password' => 'secret', 
];
authenticationConfiguration.setAdditionalData(additionalData);



requestBody.setAuthenticationConfiguration($authenticationConfiguration);


requestResult = graphServiceClient.identity().apiConnectorsById('identityApiConnector-id').patch(requestBody);


```