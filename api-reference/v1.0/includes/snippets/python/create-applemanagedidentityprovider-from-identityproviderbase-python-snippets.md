---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = IdentityProviderBase();
requestBody.set@odatatype('microsoft.graph.appleManagedIdentityProvider');

requestBody.setDisplayName('Sign in with Apple');

additionalData = [
'developerId' => 'UBF8T346G9', 
'serviceId' => 'com.microsoft.rts.b2c.test.client', 
'keyId' => '99P6D879C4', 
'certificateData' => '******', 
];
requestBody.setAdditionalData(additionalData);




requestResult = graphServiceClient.identity().identityProviders().post(requestBody);


```