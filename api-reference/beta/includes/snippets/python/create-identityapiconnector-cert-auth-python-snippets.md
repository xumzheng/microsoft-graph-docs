---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = IdentityApiConnector();
requestBody.setDisplayName('Test API');

requestBody.setTargetUrl('https://someotherapi.com/api');

authenticationConfiguration = ApiAuthenticationConfigurationBase();
authenticationConfiguration.set@odatatype('#microsoft.graph.pkcs12Certificate');

additionalData = [
'pkcs12Value' => 'eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA', 
'password' => '<password>', 
];
authenticationConfiguration.setAdditionalData(additionalData);



requestBody.setAuthenticationConfiguration($authenticationConfiguration);


requestResult = graphServiceClient.identity().apiConnectors().post(requestBody);


```