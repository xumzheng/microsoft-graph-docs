---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AuthenticationMethodConfiguration();
requestBody.set@odatatype('#microsoft.graph.fido2AuthenticationMethodConfiguration');

requestBody.setState(AuthenticationMethodState('enabled'));

additionalData = [
'isAttestationEnforced' => 'true', 
];
requestBody.setAdditionalData(additionalData);




requestResult = graphServiceClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurationsById('authenticationMethodConfiguration-id').patch(requestBody);


```