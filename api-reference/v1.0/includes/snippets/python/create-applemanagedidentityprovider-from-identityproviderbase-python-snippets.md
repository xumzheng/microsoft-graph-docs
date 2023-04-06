---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = IdentityProviderBase()
request_body.set@odatatype('microsoft.graph.appleManagedIdentityProvider')

request_body.setDisplayName('Sign in with Apple')

additionalData = [
'developerId' => 'UBF8T346G9', 
'serviceId' => 'com.microsoft.rts.b2c.test.client', 
'keyId' => '99P6D879C4', 
'certificateData' => '******', 
];
request_body.setAdditionalData(additionalData)




result = await client.identity.identityProviders.post(request_body, headers=)


```