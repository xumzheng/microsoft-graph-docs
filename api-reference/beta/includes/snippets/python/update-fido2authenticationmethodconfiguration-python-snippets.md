---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AuthenticationMethodConfiguration();
requestBody.set@odatatype('#microsoft.graph.fido2AuthenticationMethodConfiguration');

requestBody.setState(AuthenticationMethodState('enabled'));

additionalData = [
'isAttestationEnforced' => 'true', 
];
requestBody.setAdditionalData(additionalData);




result = awaitclient.policies().authenticationMethodsPolicy().authenticationMethodConfigurationsById('authenticationMethodConfiguration-id').patch(requestBody);


```